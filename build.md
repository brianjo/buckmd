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
# buck build

::: overview
Builds one or more rules specified by a set of [build
target](/concept/build_target.html)s and [build target
pattern](/concept/build_target_pattern.html)s. This is the most commonly
used command in Buck.

Syntax:

    buck build { <build target> | <build target pattern> } . . .

Example:

    buck build //java/com/example/app:amazing

Note that any [`remote_file`](/rule/remote_file.html) rules referenced
by your build rules must be downloaded with
[`buck fetch`](/command/fetch.html) prior to calling this command unless
you set `in_build = true` in the `[download]` section of your
[`.buckconfig`](/files-and-dirs/buckconfig.html).

## Parameters

-   `--build-report` Specifies a file where a JSON summary of the build
    output should be written. Note that `--build-report` can be used
    without `--keep-going`, though if `--keep-going` is not specified,
    the generated report may be partial and not include information
    about the targets that buck haven\'t had a chance to try to build.
    Here is a sample build report:

    ``` {.prettyprint .lang-js}
    {
      "success": false,
      "results": {
        "//fake:rule1": {
          "success": true,
          "type": "BUILT_LOCALLY",
          "output": "buck-out/gen/fake/rule1.txt"
        },
        "//fake:rule2": {
          "success": false
        },
        "//fake:rule3": {
          "success": true,
          "type": "FETCHED_FROM_CACHE"
        }
      }
    }
    ```

    In this example, both `//fake:rule1` and `//fake:rule3` were built
    successfully, but only `//fake:rule1` had an output file associated
    with the rule.

    Note that this contains the same information that `--keep-going`
    prints to the console, but is easier to parse programmatically. This
    report may contain more fields in the future.

-   `--keep-going` When specified, Buck will attempt to build all
    targets specified on the command line, even if some of the targets
    fail. (Buck\'s default behavior is to exit immediately when any of
    the specified targets fail.)

    When `--keep-going` is specified, a report of the build will be
    printed to stderr, detailing the build status of each target. Each
    line of the report represents the status of one build target, which
    has up to four columns:

    1.  `OK` or `FAIL`, as per the success of the build rule.
    2.  The build target of the rule.
    3.  If successful, the type of the success as defined by the
        [`com.facebook.buck.core.build.engine.BuildRuleSuccessType`](https://buckbuild.com/javadoc/com/facebook/buck/core/build/engine/BuildRuleSuccessType.html)
        enum.
    4.  If successful, the path to the output file of the rule, if it
        exists.

    For example, if Buck were run with the following arguments:

        buck build --keep-going //fake:rule1 //fake:rule2 //fake:rule3

    Then the report printed to stderr might look like:

        OK   //fake:rule1 BUILT_LOCALLY buck-out/gen/fake/rule1.txt
        FAIL //fake:rule2
        OK   //fake:rule3 FETCHED_FROM_CACHE

    In this example, both `//fake:rule1` and `//fake:rule3` were built
    successfully, but only `//fake:rule1` had an output file associated
    with the rule. Admittedly, the state of column 1 could be derived
    from the presence of column 3, but the encoding of column 1 makes it
    easier to filter out successful rules from failed ones.

    Note that when `--keep-going` is specified, the exit code will be 0
    only if all targets were built successfully.

    This option is analogous to `-k/--keep-going` in Make.

-   `--out` Takes the output of the build target and copies it to the
    specified path. Only works with a single build target, and the
    corresponding build rule must support this option.

-   `--populate-cache` Performs a cache population, which makes the
    output of all unchanged transitive dependencies available (if these
    outputs are available in the remote cache). Does not build changed
    or unavailable dependencies locally.

-   `--show-output`

    Print the relative paths to the output for each target after the
    target name. Note that some rules---such as
    [`genrule`](/rule/genrule.html)---generate sources instead of build
    artifacts.

    #### Additional Parameters

    For additional parameters that are available with this command, see
    the [Common Parameters](/command/common_parameters.html) topic.

## Examples

### View compiler flags using the compilation database

For C++ builds, to view the compiler flags that Buck is passing to the
C++ compiler, tell Buck to generate a *compilation database* for the
target. The compilation database is a JSON file that contains
information about how Buck compiled the target. The syntax is:

``` {.prettyprint .lang-bash}
buck build path/to/target#compilation-database
```

You can then get the path to the compilation-database file itself using:

``` {.prettyprint .lang-bash}
buck targets --show-output path/to/target#compilation-database
```

For example:

``` {.prettyprint .lang-bash}
$ buck clean
Parsing buck files: finished in 1.7 sec (100%)
Building: finished in 1.5 sec (100%) 3/3 jobs, 3 updated, 0.0% cache miss
  Total time: 3.7 sec

$ buck build :main#compilation-database
Building: finished in 1.5 sec (100%) 3/3 jobs, 3 updated, 0.0% cache miss
  Total time: 3.7 sec

$ buck targets --show-output :main#compilation-database
//:main#compilation-database buck-out/gen/__main#compilation-database/compile_commands.json

$ jq . buck-out/gen/__main#compilation-database/compile_commands.json 
[
  {
    "directory": "/Users/devuser/git/gtDev/C++/oop/simple-classes",
    "file": "/Users/devuser/git/gtDev/C++/oop/simple-classes/main.cpp",
    "arguments": [
      "/usr/bin/clang++",
      "-x",
      "c++",
      "-I",
      "buck-out/gen/main#default,private-headers.hmap",
      "-I",
      "buck-out",
      "-Xclang",
      "-fdebug-compilation-dir",
      "-Xclang",
      ".",
      "-fdebug-prefix-map=/Users/devuser/git/gtDev/C++/oop/simple-classes=.",
      "-c",
      "-MD",
      "-MF",
      "buck-out/gen/main#compile-main.cpp.oa5b6a1ba,default/main.cpp.o.dep",
      "main.cpp",
      "-o",
      "buck-out/gen/main#compile-main.cpp.oa5b6a1ba,default/main.cpp.o"
    ]
  }
]
```

In the preceding example `:main` specifies a *relative* build target
that is defined in the build file located in the current directory. The
`jq` tool---available through package managers such as
Homebrew---enables you to pretty-print JSON files.
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
