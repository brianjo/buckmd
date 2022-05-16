/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.tutorial} /\*\*\*/ {template .soyweb} {call buck.page} {param
title: \'Tutorials\' /} {param navid: \'learning_tutorial\' /} {param
prettify: true /} {param description} A more in-depth tutorial on using
Buck on a given platform. {/param} {param content}

::: {.{css .overview}}
This expanded tutorial shows extended concepts about using Buck to build
a project after you have installed Buck, including creating a project,
building a project, packaging a project, etc.

> **Currently this tutorial is Android specific for either Mac or Linux.
> We will be adding iOS, Java and Windows specific tutorial information
> in the near future.**

::: toggler
  --------------------- --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  **Platform:**         [Android](javascript:void(0);){.button-android onclick="display('platform', 'android')"} [MacOS](javascript:void(0);){.button-macos onclick="display('platform', 'macos')"} [Linux](javascript:void(0);){.button-linuxos onclick="display('platform', 'linuxos')"}
  **Development OS:**   [macOS](javascript:void(0);){.button-mac onclick="display('os', 'mac')"} [Linux](javascript:void(0);){.button-linux onclick="display('os', 'linux')"}
  **Language:**         [Java](javascript:void(0);){.button-java onclick="display('language', 'java')"} [Kotlin](javascript:void(0);){.button-kotlin onclick="display('language', 'kotlin')"} [Rust](javascript:void(0);){.button-rust onclick="display('language', 'rust')"}
  --------------------- --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
:::

## Path Setup

Add Buck to your `$PATH` and set up {call buck.buckd /}:

{literal}

    sudo ln -s ${PWD}/bin/buck /usr/bin/buck
    sudo ln -s ${PWD}/bin/buckd /usr/bin/buckd

{/literal}

## Create Project

We are going to build a sample application. We should start our project
in an empty directory, so create a new one and navigate to it:

{literal}

    mkdir -p ~/my-first-buck-project/
    cd ~/my-first-buck-project/

{/literal}

> **Note: the following instructions will now assume that all commands
> are run from your `~/my-first-buck-project` directory.**

## Compile Your Code

Android applications are typically written in Java and kotlin, so the
first thing we will do is to configure Buck to compile code against the
Android API. To do so, Buck needs to know where your Android SDK is.
Assuming that your Android SDK is installed in `~/android-sdk`, run the
following command to set a `ANDROID_SDK` environment variable that tells
Buck where to find your Android SDK:

{literal}

    export ANDROID_SDK=$HOME/android-sdk

{/literal}

Now that Buck can locate your Android SDK, it is time to compile some
Java code. First, we create a simple `Activity` at
`java/com/example/activity/MyFirstActivity.java`:

{literal}

    mkdir -p java/com/example/activity/
    echo "package com.example.activity;

    import android.app.Activity;
    import android.os.Bundle;

    public class MyFirstActivity extends Activity {

      @Override
      public void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
      }
    }" > java/com/example/activity/MyFirstActivity.java

{/literal}

Now we need a build file that defines a build rule to compile this Java
code, so we create an `android_library()` rule in
`java/com/example/activity/BUCK`:

{literal}

    echo "android_library(
      name = 'activity',
      srcs = glob(['*.java']),
      visibility = [ 'PUBLIC' ],
    )" > java/com/example/activity/BUCK

{/literal}

Now we can compile our Java code using Buck:

    buck build{sp}//java/com/example/activity:activity

> Buck generates its output in the `buck-out` directory, so this is a
> good time to specify `buck-out` as something that should be ignored by
> your version control system.

Now that Buck can locate your Android SDK, it is time to compile some
kotlin code. First, we create a simple `Activity` at
`kotlin/com/example/activity/MyFirstActivity.kt`:

{literal}

    mkdir -p kotlin/com/example/activity/
    echo "package com.example.activity

    import android.app.Activity
    import android.os.Bundle

    class MyFirstActivity : Activity() {

        override fun onCreate(savedInstanceState: Bundle?) {
            super.onCreate(savedInstanceState)
        }
    }" > kotlin/com/example/activity/MyFirstActivity.kt

{/literal}

Now we need a build file that defines a build rule to compile this
kotlin code, so we create an `android_library()` rule in
`kotlin/com/example/activity/BUCK`:

{literal}

    echo "android_library(
      name = 'activity',
      srcs = glob(['*.kt']),
      language = "KOTLIN",
      visibility = [ 'PUBLIC' ],
    )" > kotlin/com/example/activity/BUCK

{/literal}

Now we can compile our Java code using Buck:

    buck build{sp}//kotlin/com/example/activity:activity

> Buck generates its output in the `buck-out` directory, so this is a
> good time to specify `buck-out` as something that should be ignored by
> your version control system.

First, we create rust source files and directories:

{literal}

    mkdir -p src/front_of_house
    echo "mod front_of_house;

    pub use crate::front_of_house::hosting;
    pub use crate::front_of_house::serving;

    fn main() {
        hosting::add_to_waitlist();
        hosting::seat_at_table();
        serving::take_order();
        serving::serve_order();
        serving::take_payment();
    }" > src/main.rs

    echo "pub mod hosting;
    pub mod serving;" > src/front_of_house.rs

    echo "pub fn add_to_waitlist() {
        println!(\"Added to watinglist.\");
    }

    pub fn seat_at_table() {
        println!(\"Seated at table.\");
    }" > src/front_of_house/hosting.rs

    echo "pub fn take_order() {
        println!(\"Ordered.\");
    }

    pub fn serve_order() {
        println!(\"Order served.\");
    }

    pub fn take_payment() {
        println!(\"Payment done.\");
    }" > src/front_of_house/serving.rs

{/literal}

Now we need a build file that defines a build rule to compile this rust
code, so we create an `rust_binary()` rule in `BUCK`: {literal}

    echo "rust_binary(
        name = 'restaurant',
        srcs = glob(
            ['src/**/*.rs'],
        ),
    )" >BUCK

{/literal}

Now we can build our rust code using Buck:

    buck build{sp}:restaurant

And run the sample:

    buck run{sp}:restaurant

> Buck generates its output in the `buck-out` directory, so this is a
> good time to specify `buck-out` as something that should be ignored by
> your version control system.

## Package Resources

Android applications frequently contain resources, such as strings and
images. For this example, we will create a trivial Android resource
bundle that contains a single string:

{literal}

    mkdir -p res/com/example/activity/res/values/
    echo "<?xml version='1.0' encoding='utf-8' ?>
    <resources>
      <string name='app_name'>Hello World</string>
    </resources>" > res/com/example/activity/res/values/strings.xml

{/literal}

Buck needs a way to reference this collection of resources, so we need
to create a build file that defines an {call buck.android_resource /}
rule:

{literal}

    echo "android_resource(
      name = 'res',
      res = subdir_glob([('res', '**')]),
      package = 'com.example',
      visibility = [
        '//apps/myapp:',
      ],
    )" > res/com/example/activity/BUCK

{/literal}

## Create a Keystore

In practice, you will want to be able to test your Android app on a
physical Android device, which means that it needs to be signed. We will
create app-specific information, such as the key and manifest, in its
own directory to keep things tidy:

    mkdir -p apps/myapp/

To keep things simple, we will create a self-signed certificate for
debugging.

> Unfortunately, this is not a one-liner because there is a number of
> prompts from the `keytool` command.

{literal}

    keytool -genkey -keystore apps/myapp/debug.keystore -alias my_alias \
        -keyalg RSA -keysize 2048 -validity 10000

{/literal}

When prompted for a keystore password, just use `android` (and then type
it again to confirm it), and hit `Enter` to accept the default values
for name, organizational unit, etc.

Then create a `.properties` file that stores all of this information:

{literal}

    echo "key.alias=my_alias
    key.store.password=android
    key.alias.password=android" > apps/myapp/debug.keystore.properties

{/literal}

## Build an APK

An Android application needs a manifest named `AndroidManifest.xml`, so
we must create such a file:

{literal}

    echo "<?xml version='1.0' encoding='utf-8'?>
    <manifest xmlns:android='http://schemas.android.com/apk/res/android'
              package='com.example'
              >

      <application
          android:label='@string/app_name'
          android:hardwareAccelerated='true'>
        <activity android:name='.activity.MyFirstActivity'>
          <intent-filter>
            <action android:name='android.intent.action.MAIN' />
            <category android:name='android.intent.category.LAUNCHER' />
          </intent-filter>
        </activity>
      </application>

    </manifest>" > apps/myapp/AndroidManifest.xml

{/literal}

Now we define an {call buck.android_binary /} and {call buck.keystore /}
rule in our build file:

{literal}

    echo "android_binary(
      name = 'app',
      manifest = 'AndroidManifest.xml',
      manifest_entries = {
        'version_code': 1,
        'version_name': '1.0',
        'min_sdk_version': 26,
        'target_sdk_version': 29
      },
      keystore = ':debug_keystore',
      deps = [
        '//java/com/example/activity:activity',
        '//res/com/example/activity:res',
      ],
    )

    keystore(
      name = 'debug_keystore',
      store = 'debug.keystore',
      properties = 'debug.keystore.properties',
    )" > apps/myapp/BUCK

{/literal}

Building an {call buck.android_binary /} rule will produce an APK:

    buck build{sp}//apps/myapp:app

Alternatively, if you have an Android device connected to your computer,
you can build and install the APK in one step with {call
buck.cmd_install /}:

    buck install{sp}//apps/myapp:app

## Create an Alias

Typing `buck build{sp}//apps/myapp:app` every time you want to rebuild
your APK can be tedious. Fortunately, Buck makes it possible to define
an *alias* for a build target. An alias can always be used in place of a
build target when using Buck\'s command-line interface.

Aliases must be defined in the {call buckconfig.alias /} a config file
in the root of the project:

{literal}

    echo "[alias]
        app = //apps/myapp:app" > .buckconfig

{/literal}

With this alias in place, the command to build and install the APK is
much shorter and easier to remember:

    buck install app

## Create an IntelliJ Project

You likely want to develop your Android app using an IDE. Fortunately,
Buck can generate an IntelliJ project from the build rules you defined
in your build files.

In order to ensure that IntelliJ recognizes where your Java folders are,
you need to specify the {call buckconfig.java_src_roots /} in your {call
buck.buckconfig_link /} file:

{literal}

    echo "[java]
        src_roots = /java/" >> .buckconfig

{/literal}

Now you can create the IntelliJ project by running {call
buck.cmd_project /}:

    buck project --ide intellij

Note that you will likely want to exclude these generated files from
version control, so add the following to your `.gitignore` file (or
`.hgignore` if you are using Mercurial) along with the files generated
by {call buck.buckd /}:

{literal}

    echo "/.buckd
    /buck-out
    *.iml
    /.idea/compiler.xml
    /.idea/libraries/*.xml
    /.idea/modules.xml
    /.idea/runConfigurations/Debug_Buck_test.xml" > .gitignore

{/literal}

Now you can build your Android application from either IntelliJ or the
command line.
:::

// close overview {/param} {/call} {literal}

{/literal} {/template}
