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
# Build Target

::: overview
A *build target* is a string that identifies a build rule in your
project. Build targets are used as arguments to Buck commands, such as
[`buck build`](/command/build.html) and [`buck run`](/command/run.html).
Build targets are also used as arguments to [build
rules](/concept/build_rule.html) to enable one build rule to reference
another. For example, a build rule might use a build target to reference
another rule in order to specify that rule as a *dependency*.

#### Fully-qualified build targets

Here is an example of a *fully-qualified* build target:

    //java/com/facebook/share:ui

A fully-qualified build target has three components:

1.  The `//` prefix indicates that the subsequent path is from the
    *root* of your project. You can use the
    [`buck root`](/command/root.html) command to identify the root of
    your project.
2.  The `java/com/facebook/share` between the `//` prefix and the colon
    (`:`) indicates that the [build file](/concept/build_file.html)
    (usually named `BUCK`) is located in the directory
    `java/com/facebook/share`.
3.  The `ui` after the colon (`:`) indicates the name of the build rule
    within the build file. Build rule names must be unique within a
    build file. By *name* we mean, more formally, the value of the
    `name` argument to the build rule.

Note that the name of the build file itself---usually BUCK---does *not*
occur in the build target. All build files within a given Buck project
must have the same name---defined in the
[`[buildfile].name`](/files-and-dirs/buckconfig.html#buildfile.name)
entry of `.buckconfig`. Therefore, it is unnecessary to include the name
in the target.

The full regular expression for a fully-qualified build target is as
follows:

    [A-Za-z0-9._-]*//[A-Za-z0-9/._-]*:[A-Za-z0-9_/.=,@~+-]+
    |- cell name -|  | package path | |--- rule name ----|

In Buck, a *cell* defines a directory tree of one or more Buck packages.
For more information about Buck cells and their relationship to packages
and projects, see the [Key Concepts](/about/overview.html) topic.

**NOTE:** All target paths are assumed to start from the root of the
Buck project. Buck does not support specifying a target path that starts
from a directory below the root. Although the double forward slash
(`//`) that prefixes target paths can be ommitted when specifying a
target from the command line (see **Pro Tips** below), Buck still
assumes that the path is from the root. Buck does support *relative*
build paths, but in Buck, that concept refers to specifying build
targets *from within* a build file. See **Relative build targets** below
for more details.

#### Relative build targets

A *relative* build target can be used to reference a [build
rule](/concept/build_rule.html) *within the same [build
file](/concept/build_file.html)*. A relative build target starts with a
colon (`:`) and is followed by only the third component (or *short
name*) of the fully-qualified build target.

The following snippet from a build file shows an example of using a
relative path.

``` {.prettyprint .lang-py}
#
# Assume this rule is in //java/com/facebook/share/BUCK
#
java_binary(
  name = 'ui_jar',
  deps = [
    #
    # The following target path
    #
    #   //java/com/facebook/share:ui
    #
    # is the same as using the following relative path.
    #
    ':ui',
  ],
)
```

## Command-line Pro Tips

Here are some ways that you can reduce your typing when you specify
build targets as command-line arguments to the
[`buck build`](/command/build.html) or [`buck run`](/command/run.html)
commands.

Consider the following example of a fully-qualified build target used
with the `buck build` command:

    buck build //java/com/facebook/share:share

Although Buck is always strict when parsing build targets in build
files, Buck is flexible when parsing build targets on the command-line.
Specifically, the leading `//` is optional on the command line, so the
above could be:

    buck build java/com/facebook/share:share

Also, if there is a forward slash before the colon, it is ignored, so
this could also be written as:

    buck build java/com/facebook/share/:share

which enables you to produce the red text shown below using
tab-completion, which dramatically reduces how much you need to type:

    buck build java/com/facebook/share/:share

Finally, if the final path element matches the value specified after the
colon, it can be omitted:

    # This is treated as //java/com/facebook/share:share.
    buck build java/com/facebook/share/

which makes the build target even easier to tab-complete. For this
reason, the name of the build rule for the primary deliverable in a
build file is often named the same as the parent directory. That way, it
can be built from the command-line with less typing.

## See also

Buck supports the ability to define ***aliases* for build targets**;
using aliases can improve brevity when specifying targets on the Buck
command line. For more information, see the
[`[alias]`](/files-and-dirs/buckconfig.html#alias) section in the
documentation for [`.buckconfig`](/files-and-dirs/buckconfig.html).

A **[build target pattern](/concept/build_target_pattern.html)** is a
string that describes a set of one or more build targets. For example,
the pattern `//...` is used to build an entire project. For more
information, see the **Build Target Pattern** topic.
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
