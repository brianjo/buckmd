::: {#fb-root}
:::

::: topbar
[](http://buck.build/)

# Buck

-   
-   [Docs](/setup/getting_started.html)
-   [Issues](https://github.com/facebook/buck/issues)
-   [GitHub](https://github.com/facebook/buck)
:::

::: socialBanner
Support Ukraine. [Help Provide Humanitarian Aid to
Ukraine](https://opensource.fb.com/support-ukraine).
:::

::: {.section .content}
::: width
# Tutorials

::: overview
::: overview
This expanded tutorial shows extended concepts about using Buck to build
a project after you have installed Buck, including creating a project,
building a project, packaging a project, etc.

> **Currently this tutorial is Android specific for either Mac or Linux.
> We will be adding iOS, Java and Windows specific tutorial information
> in the near future.**

::: toggler
  --------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  **Platform:**         [Android](javascript:void(0);){.button-android onclick="display('platform', 'android')"}[MacOS](javascript:void(0);){.button-macos onclick="display('platform', 'macos')"}[Linux](javascript:void(0);){.button-linuxos onclick="display('platform', 'linuxos')"}
  **Development OS:**   [macOS](javascript:void(0);){.button-mac onclick="display('os', 'mac')"}[Linux](javascript:void(0);){.button-linux onclick="display('os', 'linux')"}
  **Language:**         [Java](javascript:void(0);){.button-java onclick="display('language', 'java')"}[Kotlin](javascript:void(0);){.button-kotlin onclick="display('language', 'kotlin')"}[Rust](javascript:void(0);){.button-rust onclick="display('language', 'rust')"}
  --------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
:::

## Path Setup

Add Buck to your `$PATH` and set up [`buckd`](/concept/buckd.html):

    sudo ln -s ${PWD}/bin/buck /usr/bin/buck
    sudo ln -s ${PWD}/bin/buckd /usr/bin/buckd

## Create Project

We are going to build a sample application. We should start our project
in an empty directory, so create a new one and navigate to it:

    mkdir -p ~/my-first-buck-project/
    cd ~/my-first-buck-project/

> **Note: the following instructions will now assume that all commands
> are run from your `~/my-first-buck-project` directory.**

## Compile Your Code

Android applications are typically written in Java and kotlin, so the
first thing we will do is to configure Buck to compile code against the
Android API. To do so, Buck needs to know where your Android SDK is.
Assuming that your Android SDK is installed in `~/android-sdk`, run the
following command to set a `ANDROID_SDK` environment variable that tells
Buck where to find your Android SDK:

    export ANDROID_SDK=$HOME/android-sdk

Now that Buck can locate your Android SDK, it is time to compile some
Java code. First, we create a simple `Activity` at
`java/com/example/activity/MyFirstActivity.java`:

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

Now we need a build file that defines a build rule to compile this Java
code, so we create an `android_library()` rule in
`java/com/example/activity/BUCK`:

    echo "android_library(
      name = 'activity',
      srcs = glob(['*.java']),
      visibility = [ 'PUBLIC' ],
    )" > java/com/example/activity/BUCK

Now we can compile our Java code using Buck:

    buck build //java/com/example/activity:activity

> Buck generates its output in the `buck-out` directory, so this is a
> good time to specify `buck-out` as something that should be ignored by
> your version control system.

Now that Buck can locate your Android SDK, it is time to compile some
kotlin code. First, we create a simple `Activity` at
`kotlin/com/example/activity/MyFirstActivity.kt`:

    mkdir -p kotlin/com/example/activity/
    echo "package com.example.activity

    import android.app.Activity
    import android.os.Bundle

    class MyFirstActivity : Activity() {

        override fun onCreate(savedInstanceState: Bundle?) {
            super.onCreate(savedInstanceState)
        }
    }" > kotlin/com/example/activity/MyFirstActivity.kt

Now we need a build file that defines a build rule to compile this
kotlin code, so we create an `android_library()` rule in
`kotlin/com/example/activity/BUCK`:

    echo "android_library(
      name = 'activity',
      srcs = glob(['*.kt']),
      language = "KOTLIN",
      visibility = [ 'PUBLIC' ],
    )" > kotlin/com/example/activity/BUCK

Now we can compile our Java code using Buck:

    buck build //kotlin/com/example/activity:activity

> Buck generates its output in the `buck-out` directory, so this is a
> good time to specify `buck-out` as something that should be ignored by
> your version control system.

First, we create rust source files and directories:

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

Now we need a build file that defines a build rule to compile this rust
code, so we create an `rust_binary()` rule in `BUCK`:

    echo "rust_binary(
        name = 'restaurant',
        srcs = glob(
            ['src/**/*.rs'],
        ),
    )" >BUCK

Now we can build our rust code using Buck:

    buck build :restaurant

And run the sample:

    buck run :restaurant

> Buck generates its output in the `buck-out` directory, so this is a
> good time to specify `buck-out` as something that should be ignored by
> your version control system.

## Package Resources

Android applications frequently contain resources, such as strings and
images. For this example, we will create a trivial Android resource
bundle that contains a single string:

    mkdir -p res/com/example/activity/res/values/
    echo "<?xml version='1.0' encoding='utf-8' ?>
    <resources>
      <string name='app_name'>Hello World</string>
    </resources>" > res/com/example/activity/res/values/strings.xml

Buck needs a way to reference this collection of resources, so we need
to create a build file that defines an
[`android_resource`](/rule/android_resource.html) rule:

    echo "android_resource(
      name = 'res',
      res = subdir_glob([('res', '**')]),
      package = 'com.example',
      visibility = [
        '//apps/myapp:',
      ],
    )" > res/com/example/activity/BUCK

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

    keytool -genkey -keystore apps/myapp/debug.keystore -alias my_alias \
        -keyalg RSA -keysize 2048 -validity 10000

When prompted for a keystore password, just use `android` (and then type
it again to confirm it), and hit `Enter` to accept the default values
for name, organizational unit, etc.

Then create a `.properties` file that stores all of this information:

    echo "key.alias=my_alias
    key.store.password=android
    key.alias.password=android" > apps/myapp/debug.keystore.properties

## Build an APK

An Android application needs a manifest named `AndroidManifest.xml`, so
we must create such a file:

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

Now we define an [`android_binary`](/rule/android_binary.html) and
[`keystore`](/rule/keystore.html) rule in our build file:

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

Building an [`android_binary`](/rule/android_binary.html) rule will
produce an APK:

    buck build //apps/myapp:app

Alternatively, if you have an Android device connected to your computer,
you can build and install the APK in one step with
[`buck install`](/command/install.html):

    buck install //apps/myapp:app

## Create an Alias

Typing `buck build //apps/myapp:app` every time you want to rebuild your
APK can be tedious. Fortunately, Buck makes it possible to define an
*alias* for a build target. An alias can always be used in place of a
build target when using Buck\'s command-line interface.

Aliases must be defined in the
[`[alias]`](/files-and-dirs/buckconfig.html#alias) a config file in the
root of the project:

    echo "[alias]
        app = //apps/myapp:app" > .buckconfig

With this alias in place, the command to build and install the APK is
much shorter and easier to remember:

    buck install app

## Create an IntelliJ Project

You likely want to develop your Android app using an IDE. Fortunately,
Buck can generate an IntelliJ project from the build rules you defined
in your build files.

In order to ensure that IntelliJ recognizes where your Java folders are,
you need to specify the
[`[java].src_roots`](/files-and-dirs/buckconfig.html#java.src_roots) in
your [`.buckconfig`](/files-and-dirs/buckconfig.html) file:

    echo "[java]
        src_roots = /java/" >> .buckconfig

Now you can create the IntelliJ project by running
[`buck project`](/command/project.html):

    buck project --ide intellij

Note that you will likely want to exclude these generated files from
version control, so add the following to your `.gitignore` file (or
`.hgignore` if you are using Mercurial) along with the files generated
by [`buckd`](/concept/buckd.html):

    echo "/.buckd
    /buck-out
    *.iml
    /.idea/compiler.xml
    /.idea/libraries/*.xml
    /.idea/modules.xml
    /.idea/runConfigurations/Debug_Buck_test.xml" > .gitignore

Now you can build your Android application from either IntelliJ or the
command line.
:::
:::

### The Basics

-   [Getting Started](/setup/getting_started.html)
-   [Key Concepts](/about/overview.html)
-   [Tutorial](/learning/tutorial.html)
-   [Installing the IntelliJ
    Plugin](/setup/intellij_plugin_install.html)
-   [Exopackage](/article/exopackage.html)
-   [Buck Cheat Sheet](/article/query_cheat_sheet.html)

### About

-   [What Makes Buck so Fast?](/concept/what_makes_buck_so_fast.html)
-   [Showcase](/about/showcase.html)
-   [Troubleshooting](/concept/troubleshooting.html)
-   [Performance Tuning](/about/performance_tuning.html)
-   [FAQ](/concept/faq.html)
-   [Learn More (Buck Presentations)](/presentations/index.html)

### Concepts

-   [Build Rule](/concept/build_rule.html)
-   [Build File](/concept/build_file.html)
-   [Build Target](/concept/build_target.html)
-   [Build Target Pattern](/concept/build_target_pattern.html)
-   [Buck Daemon (buckd)](/concept/buckd.html)
-   [Visibility](/concept/visibility.html)
-   [Flavors](/concept/flavors.html)
-   [HTTP Cache API](/concept/http_cache_api.html)
-   [Rule Keys](/concept/rule_keys.html)
-   [Java ABIs](/concept/java_abis.html)
-   [Skylark](/concept/skylark.html)

### Files and Directories

-   [.buckconfig](/files-and-dirs/buckconfig.html)
-   [.buckjavaargs](/files-and-dirs/buckjavaargs.html)
-   [buck-out](/files-and-dirs/buck-out.html)

### Commands

-   [Common Parameters](/command/common_parameters.html)
-   [buck audit](/command/audit.html)
-   [buck build](/command/build.html)
-   [buck clean](/command/clean.html)
-   [buck doctor](/command/doctor.html)
-   [buck fetch](/command/fetch.html)
-   [buck fix](/command/fix.html)
-   [buck install](/command/install.html)
-   [buck kill](/command/kill.html)
-   [buck killall](/command/killall.html)
-   [buck project](/command/project.html)
-   [buck publish](/command/publish.html)
-   [buck query](/command/query.html)
-   [buck run](/command/run.html)
-   [buck root](/command/root.html)
-   [buck server](/command/server.html)
-   [buck targets](/command/targets.html)
-   [buck test](/command/test.html)
-   [buck uninstall](/command/uninstall.html)
-   [Exit Codes](/command/exit_codes.html)

### Build Rules

-   **Core**
-   [command_alias()](/rule/command_alias.html)
-   [export_file()](/rule/export_file.html)
-   [filegroup()](/rule/filegroup.html)
-   [genrule()](/rule/genrule.html)
-   [http_archive()](/rule/http_archive.html)
-   [http_file()](/rule/http_file.html)
-   [remote_file()](/rule/remote_file.html)
-   [test_suite()](/rule/test_suite.html)
-   [worker_tool()](/rule/worker_tool.html)
-   [zip_file()](/rule/zip_file.html)
-   **Android**
-   [android_aar()](/rule/android_aar.html)
-   [android_binary()](/rule/android_binary.html)
-   [android_build_config()](/rule/android_build_config.html)
-   [android_instrumentation_apk()](/rule/android_instrumentation_apk.html)
-   [android_instrumentation_test()](/rule/android_instrumentation_test.html)
-   [android_library()](/rule/android_library.html)
-   [android_manifest()](/rule/android_manifest.html)
-   [android_prebuilt_aar()](/rule/android_prebuilt_aar.html)
-   [android_resource()](/rule/android_resource.html)
-   [apk_genrule()](/rule/apk_genrule.html)
-   [gen_aidl()](/rule/gen_aidl.html)
-   [keystore()](/rule/keystore.html)
-   [ndk_library()](/rule/ndk_library.html)
-   [prebuilt_jar()](/rule/prebuilt_jar.html)
-   [prebuilt_native_library()](/rule/prebuilt_native_library.html)
-   [robolectric_test()](/rule/robolectric_test.html)
-   **CXX**
-   [cxx_binary()](/rule/cxx_binary.html)
-   [cxx_library()](/rule/cxx_library.html)
-   [cxx_genrule()](/rule/cxx_genrule.html)
-   [cxx_precompiled_header()](/rule/cxx_precompiled_header.html)
-   [cxx_test()](/rule/cxx_test.html)
-   [prebuilt_cxx_library()](/rule/prebuilt_cxx_library.html)
-   [prebuilt_cxx_library_group()](/rule/prebuilt_cxx_library_group.html)
-   **D**
-   [d_binary()](/rule/d_binary.html)
-   [d_library()](/rule/d_library.html)
-   [d_test()](/rule/d_test.html)
-   **Go**
-   [go_binary()](/rule/go_binary.html)
-   [go_library()](/rule/go_library.html)
-   [go_test()](/rule/go_test.html)
-   [cgo_library()](/rule/cgo_library.html)
-   **Groovy**
-   [groovy_library()](/rule/groovy_library.html)
-   **Halide**
-   [halide_library()](/rule/halide_library.html)
-   **Haskell**
-   [haskell_binary()](/rule/haskell_binary.html)
-   [haskell_library()](/rule/haskell_library.html)
-   [prebuilt_haskell_library()](/rule/prebuilt_haskell_library.html)
-   **iOS**
-   [apple_asset_catalog()](/rule/apple_asset_catalog.html)
-   [apple_binary()](/rule/apple_binary.html)
-   [apple_bundle()](/rule/apple_bundle.html)
-   [apple_library()](/rule/apple_library.html)
-   [apple_package()](/rule/apple_package.html)
-   [apple_resource()](/rule/apple_resource.html)
-   [apple_test()](/rule/apple_test.html)
-   [core_data_model()](/rule/core_data_model.html)
-   [prebuilt_apple_framework()](/rule/prebuilt_apple_framework.html)
-   **Java**
-   [java_binary()](/rule/java_binary.html)
-   [java_library()](/rule/java_library.html)
-   [java_test()](/rule/java_test.html)
-   [prebuilt_jar()](/rule/prebuilt_jar.html)
-   [prebuilt_native_library()](/rule/prebuilt_native_library.html)
-   **Kotlin**
-   [kotlin_library()](/rule/kotlin_library.html)
-   [kotlin_test()](/rule/kotlin_test.html)
-   **Lua**
-   [cxx_lua_extension()](/rule/cxx_lua_extension.html)
-   [lua_binary()](/rule/lua_binary.html)
-   [lua_library()](/rule/lua_library.html)
-   **OCaml**
-   [ocaml_binary()](/rule/ocaml_binary.html)
-   [ocaml_library()](/rule/ocaml_library.html)
-   **Python**
-   [prebuilt_python_library()](/rule/prebuilt_python_library.html)
-   [python_binary()](/rule/python_binary.html)
-   [python_library()](/rule/python_library.html)
-   [python_test()](/rule/python_test.html)
-   **Rust**
-   [rust_binary()](/rule/rust_binary.html)
-   [rust_library()](/rule/rust_library.html)
-   [rust_test()](/rule/rust_test.html)
-   [prebuilt_rust_library()](/rule/prebuilt_rust_library.html)
-   **Shell**
-   [sh_binary()](/rule/sh_binary.html)
-   [sh_test()](/rule/sh_test.html)
-   **.NET**
-   [csharp_library()](/rule/csharp_library.html)
-   [prebuilt_dotnet_library()](/rule/prebuilt_dotnet_library.html)

### Functions

-   **Python DSL**
-   [add_build_file_dep()](/function/add_build_file_dep.html)
-   [allow_unsafe_import()](/function/allow_unsafe_import.html)
-   [flatten_dicts()](/function/flatten_dicts.html)
-   [glob()](/function/glob.html)
-   [get_base_path()](/function/get_base_path.html)
-   [get_cell_name()](/function/get_cell_name.html)
-   [host_info()](/function/host_info.html)
-   [include_defs()](/function/include_defs.html)
-   [load()](/function/load.html)
-   [read_config()](/function/read_config.html)
-   [subdir_glob()](/function/subdir_glob.html)
-   [String Parameter Macros](/function/string_parameter_macros.html)

```{=html}
<!-- -->
```
-   **Skylark**
-   [glob()](/skylark/generated/glob.html)
-   [host_info()](/skylark/generated/host_info.html)
-   [package_name()](/skylark/generated/package_name.html)
-   [provider()](/skylark/generated/provider.html)
-   [read_config()](/skylark/generated/read_config.html)
-   [repository_name()](/skylark/generated/repository_name.html)
-   [rule_exists()](/skylark/generated/rule_exists.html)

### Extending Buck

-   [Custom Macros](/extending/macros.html)
-   [Custom Rules](/extending/rules.html)
-   [Building E2E Tests for Buck](/extending/e2e_tests.html)
:::
:::

::: width
© Copyright Facebook, 2013 - 2020
:::
