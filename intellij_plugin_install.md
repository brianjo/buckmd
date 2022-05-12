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
# Installing and using the IntelliJ Plugin

::: overview
To use the Buck Intellij Plugin you will have to install Buck, by
following the guide from [Downloading and Installing
Buck](/setup/install.html).

## Installing the plugin {#manual-install-buck}

You can download the plugin from
[here](https://plugins.jetbrains.com/plugin/7826-buck-for-idea) or
manually build it by following the guide from [Building the Buck
Intellij Plugin](/setup/intellij_plugin_build.html). After that, you can
install it by following the [Installing a Plugin from
Disk](https://www.jetbrains.com/help/idea/installing-a-plugin-from-disk.html)
guide.

## Using the plugin {#manual-use-intellij}

After you have installed it, you can view the Buck Plugin Tool Window by
accessing `View > Tool Windows > Buck`.

### Utility Functions {#buck-plugin-utility}

1.  Buck Code Completion

    Helps you complete the names of keywords and buck rule names within
    the visibility scope.

2.  Go to Buck File

    Jump to the BUCK file of current source file. To access it you can:

    -   `Tools > Buck > Go to Buck file`
    -   `Right click > Buck > Go to Buck file`
    -   `⇧ + ⌘ + P`

3.  Go to Buck Dependencies

    Quickly jump to other BUCK files with `⌘ + Click` or `⌘ + B`.

4.  Reformat BUCK files

    The Buck Plugin lets you reformat source code to meet the
    requirements of your code style. The plugin also supports customized
    spacing and indenting in the buck code style settings. You can
    access it by going to `Code > Reformat Code` or by pressing
    `⌥ + ⌘ + L`.

5.  Sort buck dependencies

    You can access it by going to `Code > Optimise Imports` or by
    pressing `^ + ⌥ + O`.

6.  Automatically Convert to Buck Dependencies after Paste in BUCK file

    For example:

    -   \"import com.example.activity.MyFirstActivity\" -\>
        \"//java/com/example/activity:activity\"
    -   \"package com.example.activity;\" -\>
        \"//java/com/example/activity:activity\"
    -   \"com.example.activity.MyFirstActivity\" -\>
        \"//java/com/example/activity:activity\"

7.  Error Annotation

    If a Buck dependency does not exist, it will be marked with red.

8.  Commenting and Uncommenting

    You can comment or uncomment selected lines of a BUCK file by
    accessing `Code > Comment with Line Comment` or by pressing `⌘ + /`.

### Executing Buck Commands {#buck-plugin-commands}

1.  Select target

    Before you start doing any of the below mentioned actions you will
    have to select a buck target.

    You can start selecting the buck target either by pressing the
    associated icon from the Buck Plugin tool window or by using
    `⇧ + ⌘ + J`.

    If you have an alias, you can just search for it. If you don\'t have
    an alias you have to write the whole path to the BUCK file. Once you
    are at the directory with the BUCK file, the plugin will search for
    all the available targets, which may take some time.

    You can use autocomplete by pressing → and navigate through the
    search by pressing ↑ and ↓.

2.  Build target

    Once you selected the target you can start a buck build either by
    pressing the associated icon from the Buck Plugin tool window or by
    using `⇧ + ⌘ + S`.

3.  Show Buck/compiler errors and easily go through them

    When building, you may receive compiler errors. You can easily
    navigate through them and on double click you will be sent to the
    appropriate column and line.

4.  Install target

    Once you selected the target you can start a buck install either by
    pressing the associated icon from the Buck Plugin tool window or by
    using `⇧ + ⌘ + X`.

5.  Uninstall target

    Once you selected the target you can start a buck uninstall either
    by pressing the associated icon from the Buck Plugin tool window or
    by using `⇧ + ⌘ + M`.

6.  Test target

    Once you selected the target you can start a buck test either by
    pressing the associated icon from the Buck Plugin tool window or by
    using `⇧ + ⌘ + Y`.

7.  Buck project target

    Once you selected the target you can start a buck project either by
    pressing the associated icon from the Buck Plugin tool window or by
    using `⇧ + ⌘ + B`.

8.  Buck kill

    Once you started one of the above mentioned actions you can stop it
    either by pressing the associated icon from the Buck Plugin tool
    window or by using `⇧ + ⌘ + L`.

### Settings {#buck-plugin-settings}

1.  Buck Settings

    You can set your buck executable path and other install settings by
    going to `Preferences > Tools > Buck`.

2.  Code Style Settings

    You can set code style settings by going to
    `Preferences > Editor > Code Style > Buck`.

3.  Colors & Font Settings

    You can set the syntax highlighting colors from
    `Preferences > Editor > Colors & Fonts > Buck`.
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
