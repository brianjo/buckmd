/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.exopackage} /\*\*\*/ {template .soyweb} {call buck.page} {param
title: \'Exopackage\' /} {param navid: \'article_exopackage\' /} {param
subtitle: \'A technique for fast, iterative Android development.\' /}
{param prettify: true /} {param description} Buck has an advanced
feature to speed up iterative Android development called exopackage. An
exopackage is a small shell of an Android app that contains the minimal
code and resources needed to bootstrap loading the code for a
full-fledged Android application. {/param} {param content} {let
\$step2sha1: \'6c809273e70428f2f465cdeef568e1f35c30b439\' /} {let
\$step3sha1: \'5f7ce4934e9e8ea9a391a09d2093c79b64b7d207\' /} {let
\$step4sha1: \'d4553a92eb8969e05d7cd9c2e73b4309fee72966\' /} {let
\$step5sha1: \'1f1b375624664ac1cdc82668a4b952c6f332bdb0\' /} {let
\$step6sha1: \'4250292b4d4742d40a9b06ce638741b2873210f1\' /}

Buck has an advanced feature to speed up iterative Android development
called exopackage. An *exopackage* is a small shell of an Android app
that contains the minimal code and resources needed to bootstrap loading
the code for a full-fledged Android application. Loading the application
code at runtime avoids a full reinstall of the app when testing a Java
change, which dramatically reduces the length of edit/refresh cycles.
Here are the performance improvements in build times for Buck vs. Gradle
in a real world Android application,{sp}
[AntennaPod](https://github.com/danieloeh/AntennaPod):

  --------------------- -------- ------ ----------
                        Gradle   Buck   Speed Up
  clean build           31s      6s     5x
  incremental build     13s      1.7s   7.5x
  no-op build           3s       0.2s   15x
  clean install         7.2s     7.2s   1x
  incremental install   7.2s     1.5s   4.8x
  --------------------- -------- ------ ----------

(Note: These measurements were done on a MacBook Pro with a i7-3740QM
CPU, with HyperThreading enabled, using Oracle Java 1.7.0_45 for Linux.
We used 8 threads by running \"./gradlew \--parallel-threads 8\".
Gradle\'s daemon, parallel, and configureondemand options were enabled,
as was Buck\'s daemon (which is enabled by default). In all cases, the
builds were run multiple times to allow Java\'s JIT to warm up fully.
The incremental build was adding a single blank line to a Java file.)

As you might expect, using exopackage requires you to make some code
changes to your application. This article serves two purposes: it is
both a **tutorial** that shows how to migrate an Android app that builds
with Gradle over to Buck with exopackage, as well as a **technical
explanation** of how exopackage works.

For this tutorial, we will demonstrate how to use exopackage by adding
Buck support to [AntennaPod](https://github.com/danieloeh/AntennaPod),
an open source podcast management app for Android. Each step in the
process is documented as a separate commit in{sp} [our fork of
AntennaPod](https://github.com/facebookarchive/AntennaPod). Note that
most of the work in this tutorial is in adding Buck support to
AntennaPod. If your Android project already uses Buck, then you can jump
straight to [Step 5](#build-buck-support-library), which will require
minimal changes to your existing project.

**Table of Contents**

-   [Step 1: Check out AntennaPod](#check-out)
-   [Step 2: Import JARs for third party
    dependencies](#import-dependencies)
-   [Step 3: Ensure R.\* constants are not assumed to be
    final](#refactor-r-constants)
-   [Step 4: Create BUCK files that define build rules to build
    AntennaPod with Buck](#build-rules)
-   [Step 5: Build Buck\'s Android support
    library](#build-buck-support-library)
-   [Step 6: Modify AntennaPod to use exopackage](#use-exopackage)
-   [Step 7: Profit!](#profit)
-   [Caveats](#caveats)
-   [Incompatible Devices](#incompatible-devices)

## Step 1: Check out AntennaPod {#check-out}

If you want to walk through this tutorial and make all of the changes
yourself, then the first step is to clone the AntennaPod application at
the same revision used to create this tutorial:

    {literal}
    git clone --recursive git@github.com:facebookarchive/AntennaPod.git
    cd AntennaPod
    git checkout c2080b1dfd17fc371e04ce1e7b39ebadaf3cb7a7
    {/literal}

If you just want to play with the final version of the tutorial after
all of the Buck/exopackage support has been added, then checkout to the
appropriate revision so you can build and run AntennaPod using Buck.
Note that you must add your own keystore before you can do a build. (We
do not check in `debug.keystore` for security reasons.)

    {literal}
    git checkout {/literal}{$step6sha1}{literal}
    cp ~/.android/debug.keystore keystore/debug.keystore
    buck install --run antennapod
    {/literal}

## Step 2: Import JARs for third party dependencies {#import-dependencies}

{call .gitHubCommit} {param sha1 : \$step2sha1 /} {/call}

Unlike Gradle, Buck requires that all files that contribute to the
project live under the project root (which is defined by the presence of
a `.buckconfig` file). Instead of downloading third party JARs from the
Maven Central Repository as part of the build process (like Gradle),
Buck expects such dependencies to live in version control, just like
application code. This ensures that builds are *reproducible* and
*hermetic*.

For AntennaPod, we ran `./gradlew --debug assembleDebug` and inspected
the output to figure out which third party JAR files Gradle was using to
build the app. As a result, we ended up adding the following files to
the `libs` directory, which also includes an
[AAR](https://developer.android.com/studio/projects/android-library#aar-contents){sp}
file for the Android support library for v7 compatibility.

    {literal}
    libs/appcompat-v7-19.1.0.aar
    libs/commons-io-2.4.jar
    libs/commons-lang3-3.3.2.jar
    libs/flattr4j-core-2.10.jar
    libs/library-2.4.0.jar
    libs/support-v4-19.1.0.jar
    {/literal}

Note that we also removed the `libs` directory from `.gitignore` as part
of this change.

## Step 3: Ensure R.\* constants are not assumed to be final {#refactor-r-constants}

{call .gitHubCommit} {param sha1 : \$step3sha1 /} {/call}

If you have any code like the following:

``` {.prettyprint .lang-java}
{literal}
  int id = view.getId();
  switch (id) {
    case R.id.button1:
      action1();
      break;
    case R.id.button2:
      action2();
      break;
    case R.id.button3:
      action3();
      break;
  }
{/literal}
```

You must convert it to use `if`/`else` blocks as follows:

``` {.prettyprint .lang-java}
{literal}
  int id = view.getId();
  if (id == R.id.button1) {
    action1();
  } else if (id == R.id.button2) {
    action2();
  } else if (id == R.id.button3) {
    action3();
  }
{/literal}
```

As explained in the article [Non-constant Fields in Case
Labels](http://tools.android.com/tips/non-constant-fields), the
constants in the `R` class for an Android library projects are not
`final`, which means they cannot be used as constant expressions in
`case` statements. Because Buck treats the code for an {call
buck.android_library /} as if it were part of an Android library
project, this applies to all Android code built by Buck. The article
explains how you can leverage your IDE to automate this refactoring.

## Step 4: Create BUCK files that define build rules to build AntennaPod with Buck {#build-rules}

{call .gitHubCommit} {param sha1 : \$step4sha1 /} {/call}

In Buck, build rules are defined in build files named `BUCK`. In this
step, we create a `BUCK` file and add the build rules necessary to build
the AntennaPod APK using Buck without touching any other files in the
AntennaPod repository.

We start by creating a `BUCK` file and defining an {call
buck.android_library /} rule that exposes all of the JARs in the `libs`
directory as a single dependency, `:all-jars`:

``` {.prettyprint .lang-py}
{literal}
  import re

  jar_deps = []
  for jarfile in glob(['libs/*.jar']):
    name = 'jars__' + re.sub(r'^.*/([^/]+)\.jar$', r'\1', jarfile)
    jar_deps.append(':' + name)
    prebuilt_jar(
      name = name,
      binary_jar = jarfile,
    )

  android_library(
    name = 'all-jars',
    exported_deps = jar_deps,
  )
{/literal}
```

We also wrap the AAR file for the Android support library with an {call
buck.android_prebuilt_aar /} rule:

``` {.prettyprint .lang-py}
{literal}
  android_prebuilt_aar(
    name = 'appcompat',
    aar = 'libs/appcompat-v7-19.1.0.aar',
  )
{/literal}
```

Next, we define some rules to generate `.java` files from `.aidl` files
and package them as an {call buck.android_library /}, as well:

``` {.prettyprint .lang-py}
{literal}
  presto_gen_aidls = []
  for aidlfile in glob(['src/com/aocate/presto/service/*.aidl']):
    name = 'presto_aidls__' + re.sub(r'^.*/([^/]+)\.aidl$', r'\1', aidlfile)
    presto_gen_aidls.append(':' + name)
    gen_aidl(
      name = name,
      aidl = aidlfile,
      import_path = 'src',
    )

  android_library(
    name = 'presto-aidls',
    srcs = presto_gen_aidls,
  )
{/literal}
```

Then we define an {call buck.android_build_config /}, which will
generate {sp}`de.danoeh.antennapod.BuildConfig` for us, compile it, and
expose it as a {call buck.java_library /}. As we will see, this class
plays an important role in creating an exopackage:

``` {.prettyprint .lang-py}
{literal}
  android_build_config(
    name = 'build-config',
    package = 'de.danoeh.antennapod',
  )
{/literal}
```

Before we can define an {call buck.android_library /} rule to compile
the primary sources for AntennaPod, we must define some rules to bundle
the resources and code for its dependent Android library projects:

``` {.prettyprint .lang-py}
{literal}
  android_resource(
    name = 'dslv-res',
    package = 'com.mobeta.android.dslv',
    res = 'submodules/dslv/library/res',
  )

  android_library(
    name = 'dslv-lib',
    srcs = glob(['submodules/dslv/library/src/**/*.java']),
    deps = [
      ':all-jars',
      ':dslv-res',
    ],
  )

  android_library(
    name = 'presto-lib',
    srcs = glob(['src/com/aocate/**/*.java']),
    deps = [
      ':all-jars',
      ':presto-aidls',
    ],
  )
{/literal}
```

Now that the dependent Android library projects can be expressed as
dependencies in Buck, we define {call buck.android_resource /} and {call
buck.android_library /} rules that build the main AntennaPod code:

``` {.prettyprint .lang-py}
{literal}
  android_resource(
    name = 'res',
    package = 'de.danoeh.antennapod',
    res = 'res',
    assets = 'assets',
    deps = [
      ':appcompat',
      ':dslv-res',
    ]
  )

  android_library(
    name = 'main-lib',
    srcs = glob(['src/de/**/*.java']),
    deps = [
      ':all-jars',
      ':appcompat',
      ':build-config',
      ':dslv-lib',
      ':presto-lib',
      ':res',
    ],
  )
{/literal}
```

To package the Android code into an APK, we need a keystore with which
it should be signed, a manifest that defines the app, and a rule to
package everything toegether. Let\'s start with the keystore, as
defining this rule requires an extra step from the command line:

``` {.prettyprint .lang-py}
{literal}
keystore(
  name = 'debug_keystore',
  store = 'keystore/debug.keystore',
  properties = 'keystore/debug.keystore.properties',
)
{/literal}
```

Note that a clean checkout of the AntennaPod repository includes a
`keystore/debug.keystore.properties` file, but no
`keystore/debug.keystore` file. This is because the Android Developer
Tools creates a keystore with a common set of credentials under
`~/.android/debug.keystore` on your machine. Assuming you have not
changed this default, the values in `keystore/debug.keystore.properties`
will be appropriate for your `~/.android/debug.keystore`. Recall that
Buck requires all files it must know about to live under the project
root, so **you must copy the keystore to your project where Buck expects
it**:

    cp ~/.android/debug.keystore keystore/debug.keystore

With the {call buck.keystore /} defined, now we can define the {call
buck.android_binary /} rule whose output will be the AntennaPod APK.
Note that the only item listed in its `deps` is {sp}`:main-lib`, as
{call buck.android_binary /} will package {sp}`:main-lib` and its
transitive dependencies into the APK.

``` {.prettyprint .lang-py}
{literal}
android_binary(
  name = 'antennapod',
  manifest = 'AndroidManifest.xml',
  keystore = ':debug_keystore',
  deps = [
    ':main-lib',
  ],
)
{/literal}
```

To facilitate building from the command line (and to leverage the build
cache), create a file named `.buckconfig` in the root of the repo with
the following contents:

    {literal}
    [alias]
      antennapod = //:antennapod
    [cache]
      mode = dir
      dir_max_size = 1GB
    [android]
      target = Google Inc.:Google APIs:19
    {/literal}

Now you should be able to run `{call buck.cmd_build /} antennapod` to
build the app, or `{call buck.cmd_install /} antennapod` to install it
if `adb devices` is not empty.

## Step 5: Build Buck\'s Android support library {#build-buck-support-library}

{call .gitHubCommit} {param sha1 : \$step5sha1 /} {/call}

In order for your app to use exopackage, it needs to use Buck\'s Java
library that provides support for it. You can easily build this library
from source from your checkout of Buck as follows:

    {literal}
    # Run this from the root of your checkout of Buck, not from AntennaPod.
    buck build --out buck-android-support.jar buck-android-support
    {/literal}

Once you have built it, move it over to AntennaPod\'s `libs` directory,
just like the other third party JAR files:

    {literal}
    mv buck-android-support.jar path/to/AntennaPod/libs
    {/literal}

## Step 6: Modify AntennaPod to use exopackage {#use-exopackage}

{call .gitHubCommit} {param sha1 : \$step6sha1 /} {/call}

On a high level, the main thing that you need to do to leverage
exopackage is change the insertion point of your app from the existing
`android.app.Application` that your app uses to an {call
.ExopackageApplication /} that delegates to your original `Application`.
This level of indirection is what makes it possible for exopackage to
dynamically load the code for your application in debug mode. In release
mode, {call .ExopackageApplication /} {sp}expects all of the code for
your app to be present in the APK, so it skips the step where it tries
to dynamically load code.

If your app has a class that subclasses `android.app.Application` that
is listed as the main app in `AndroidManifest.xml` via the{sp}
`<application name>` attribute, then the first thing that you need to do
is modify that class so it extends {call .DefaultApplicationLike /}{sp}
rather than `Application`:

    {literal}
    -public class PodcastApp extends Application {
    +public class PodcastApp extends DefaultApplicationLike {
    {/literal}

Further, your {call .DefaultApplicationLike /} must declare a
constructor that takes an `Application` as its only parameter. You most
likely want to store it as a field:

``` {.prettyprint .lang-java}
{literal}
  private final Application appContext;

  public PodcastApp(Application appContext) {
    this.appContext = appContext;
  }
{/literal}
```

Now all methods that previously accessed the API of `Application` via
inheritance can delegate to the `appContext` instance instead:

    {literal}
    -LOGICAL_DENSITY = getResources().getDisplayMetrics().density;
    +LOGICAL_DENSITY = appContext.getResources().getDisplayMetrics().density;
    {/literal}

Now you must create your new `Application` class, which will be a
subclass of {call .ExopackageApplication /}. As you can see from its
API, it is an `abstract` class that does not have a default constructor,
so you must define a no-arg constructor as follows:

``` {.prettyprint .lang-java}
{literal}
  package de.danoeh.antennapod;

  import com.facebook.buck.android.support.exopackage.ExopackageApplication;

  public class AppShell extends ExopackageApplication {

    public AppShell() {
      super(
        // This is passed as a string so the shell application does not
        // have a binary dependency on your ApplicationLike class.
        /* applicationLikeClassName */ "de.danoeh.antennapod.PodcastApp",

        // The package for this BuildConfig class must match the package
        // from the android_build_config() rule. The value of the flags
        // will be set based on the "exopackage_modes" argument to
        // android_binary().
        de.danoeh.antennapod.BuildConfig.EXOPACKAGE_FLAGS);
    }
  }
{/literal}
```

Alternatively, if your original app did not have a custom subclass of
`android.app.Application`, then you do not have to create an
implementation of `ApplicationLike`. You must still create a subclass of
`ExopackageApplication`, but now your implementation can be simpler:

``` {.prettyprint .lang-java}
{literal}
  package de.danoeh.antennapod;

  import com.facebook.buck.android.support.exopackage.ExopackageApplication;

  public class AppShell extends ExopackageApplication {

    public AppShell() {
      super(de.danoeh.antennapod.BuildConfig.EXOPACKAGE_FLAGS);
    }
  }
{/literal}
```

Now the more sophisticated changes will be in the `BUCK` file where you
defined your {call buck.android_binary /} rule. First, you will need to
create an {call buck.android_library /} that builds your {call
.ExopackageApplication /}:

``` {.prettyprint .lang-py}
{literal}
  APP_CLASS_SOURCE = 'src/de/danoeh/antennapod/AppShell.java'

  android_library(
    name = 'application-lib',
    srcs = [APP_CLASS_SOURCE],
    deps = [
      # This is the android_build_config() rule that you created in Step 4.
      # If you jumped straight to Step 5 because your Android app was already
      # configured to build with Buck, then go back to Step 4 and add this rule
      # if you aren't already using an android_build_config().
      ':build-config',

      # This is the prebuilt_jar() rule that wraps buck-android-support.jar.
      ':jars__buck-android-support',
    ],
  )
{/literal}
```

If you have an existing {call buck.android_library /} rule that {call
buck.fn_glob /}s your {call .ExopackageApplication /}\'s source file,
then make sure to exclude it:

    {literal}
    -  srcs = glob(['src/de/**/*.java']),
    +  srcs = glob(['src/de/**/*.java'], excludes = [APP_CLASS_SOURCE]),
    {/literal}

The biggest change to your `BUCK` file will be the new arguments to your
{call buck.android_binary /} rule (new lines are highlighted in
[green]{style="color:green"}):

    {literal}
    android_binary(
      name = 'antennapod',
      manifest = 'AndroidManifest.xml',
      keystore = ':debug_keystore',
      use_split_dex = True,
      exopackage_modes = ['secondary_dex'],
      primary_dex_patterns = [
        '^de/danoeh/antennapod/AppShell^',
        '^de/danoeh/antennapod/BuildConfig^',
        '^com/facebook/buck/android/support/exopackage/',
      ],  
      deps = [
        ':application-lib',
        ':main-lib',
      ],
    )
    {/literal}

As you might have guessed, `primary_dex_patterns` is a pattern that
identifies which `.class` files from the transitive `deps` that must be
included in the shell app that bootstraps the rest of the app. As such,
these patterns match the transitive deps of `:application-lib`.

Setting `exopackage_modes = ['secondary_dex']` is what ensures that
{sp}`BuildConfig.EXOPACKAGE_FLAGS` will be set correctly, in addition to
the other packaging changes that Buck makes to support exopackage. This
must used with `use_split_dex = True` because using exopackage requires
dividing the app into multiple dex files.

Finally, you must update your `AndroidManifest.xml` to refer to the
`ExopackageApplication` as the new entry point into your app:

    {literal}
    -android:name="de.danoeh.antennapod.PodcastApp"
    +android:name="de.danoeh.antennapod.AppShell"
    {/literal}

## Step 7: Profit! {#profit}

Now your development cycle should be as follows:

    {literal}
    buck install --run antennapod
    # Edit your application's Java code.
    buck install --run antennapod
    # Watch in amazement as your changes are loaded faster than ever before!
    {/literal}

## Caveats

Currently, exopackage speeds up incremental install times for Java
changes, but changes to Android resources or native libraries require a
full reinstall. This is something we hope to improve in the future.

Be aware of the following limitations when using Buck and exopackage:

-   You cannot use `adb install` for exopackages. You must use {call
    buck.cmd_install /}.
-   You should use {call buck.cmd_uninstall /} instead of
    `adb uninstall` to uninstall the app. Otherwise, unnecessary files
    will be left in `/data/local/tmp`. You can remove them with
    `adb shell rm -r /data/local/tmp/exopackage/$PACKAGE_NAME`.
-   Some devices are not compatible with the exopackage installer.
    {sp}[See below](#incompatible-devices).
-   Install to SD card does not work right now.
-   Exopackages will not start up for non-primary users on a multi-user
    android device. // (TODO: This might not be true any more.)
-   When you do an install, system notifications and alarms will **not**
    be cleared, so you might get an intent back from them with the old
    version of your `Parcelable`, which could cause a crash or other
    confusing behavior.
-   When you do an install on pre-ICS devices, the app will not be
    stopped.

## Incompatible Devices

Empirically, we have determined that the following devices do not work
with exopackage:

-   Some AOSP builds between the KitKat release and L Preview.

You might want to keep two versions of your {call buck.android_binary /}
rule in your `BUCK` files: one that uses exopackage and one that does
not. That way, you will always have a way to test on devices that do not
support exopackage. {/param} {/call} {/template} /\*\*\*/ {template
.ExopackageApplication}
[`ExopackageApplication`](http://buck.build/javadoc/com/facebook/buck/android/support/exopackage/ExopackageApplication.html)
{/template} /\*\*\*/ {template .DefaultApplicationLike}
[`DefaultApplicationLike`](http://buck.build/javadoc/com/facebook/buck/android/support/exopackage/DefaultApplicationLike.html)
{/template} /\*\* \* \@param sha1 \*/ {template .gitHubCommit} [ View on
GitHub:
[{\$sha1}](https://github.com/facebookarchive/AntennaPod/commit/%7B$sha1%7D)
]{style="font-size: 80%"} {/template}
