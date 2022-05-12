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
# Common Parameters

::: overview
This topic describes command-line parameters that affect the operation
of Buck itself and that are available irrespective of which subcommand
(`build`, `run`,`test`, etc) you invoke.

## Parameters

-   `--verbose`

    Set the verbosity level of the console output. The verbosity level
    is a single numeric value between `1` and `8` inclusive. For
    example:

        buck targets --verbose 8

    Higher verbosity levels include all the output of lower levels.

    The output that Buck produces is affected by factors in addition to
    the verbosity level. Such factors include the subcommand (`build`,
    `install`, `test`, etc), the types of rules being built, and the
    degree to which artifacts from previous builds have been cached.

    Buck has not yet implemented differences between all levels. For
    example, there are currently no differences in verbosity between
    levels `5` and `7` inclusive.

      Numeric level          Boolean function                                     Description
      ---------------------- ---------------------------------------------------- --------------------------------------------------------------------
      `1`{.not-inline}       `shouldPrintStandardInformation()`{.not-inline}      Print warnings from build steps and summary information for tests.
      `2`{.not-inline}       `shouldPrintBinaryRunInformation()`{.not-inline}     Print additional output for generated binaries or tests.
      `3`{.not-inline}       `shouldPrintCommand()`{.not-inline}                  Print commands that Buck runs during the build process.
      `4`{.not-inline}       `shouldPrintSelectCommandOutput()`{.not-inline}      Print output for selected commands that Buck runs.
      `5 - 7`{.not-inline}   `shouldPrintOutput()`{.not-inline}                   Print output for all commands that Buck runs.
      `8`{.not-inline}       `shouldUseVerbosityFlagIfAvailable()`{.not-inline}   Print all available diagnostic/logging information.

    For more precise information about how a particular verbosity level
    affects output, you can search the Buck source code for the
    corresponding boolean function. For example:

        grep --recursive "getVerbosity().shouldPrintOutput()" ~/local/buck/src

-   `--no-cache`

    Disable the build artifact caches. If this parameter is specified,
    Buck ignores any artifacts in any of the caches specified in the
    [`[cache]`](/files-and-dirs/buckconfig.html#cache) section of
    `.buckconfig`. These include the filesystem cache (`dir`), remote
    cache (`http`), and SQLite cache (`sqlite`).

    The contents of the caches are unaffected, but Buck does not use
    them for the specified command.

    Note that if there is an output file in the `buck-out` directory for
    a previously-built and unchanged rule, Buck still uses that output
    file in your build---even if `--no-cache` is specified. If you
    don\'t want Buck to use these (valid) build artifacts, run the
    [`buck clean`](/command/clean.html) command before your build to
    delete them from `buck-out`.

-   `--config`

    Specify configuration settings or override existing settings in
    [`.buckconfig`](/files-and-dirs/buckconfig.html). For example:

        buck build --config cache.mode=dir //java/com/example/app:amazing

    The `--config` parameter can be abbreviated as `-c`.

    You can specify the `--config` parameter multiple times on the same
    command line. Note, however, that if the same configuration option
    is specified more than once, Buck uses the last value specified
    (\"last write wins\"). For example, the following invocation of
    `buck build` builds the `//:prod` target, rather than the `//:dev`
    target, which was specified earlier on the command line. (The
    example uses the abbreviated, `-c`, version of the parameter.)

        #
        # Build for development? 
        #
        # No, build for production.
        #
        buck build -c 'alias.main=//:dev' -c 'alias.main=//:prod' main

    The preferred method of overriding values in `.buckconfig` is by
    using a `.buckconfig.local` file. Overriding values of `.buckconfig`
    from the command line can make it difficult to reproduce builds.

-   `--config-file`

    Specify build-configuration settings in a file that uses the same
    syntax as [`.buckconfig`](/files-and-dirs/buckconfig.html). For
    example:

        buck build --config-file debug.buckconfig

    The `--config-file` parameter provides functionality similar to
    `--flagfile` (see below), but with `.buckconfig` syntax rather than
    command-line parameter syntax.

    Any values specified using `--config-file` override values specified
    in `.buckconfig` and `.buckconfig.local`.

    You can specify the path to the configuration file in one of three
    ways.

    ##### Use a path that is relative to the directory that contains the current cell\'s `.buckconfig`.

        --config-file relative/path/to/file.buckconfig

    ##### Use a path that is relative to the directory that contains a *specified* cell\'s `.buckconfig`.

        --config-file <cell name>//path/to/file.buckconfig

    ##### Use an absolute path from the root of your file system.

        --config-file /absolute/path/to/file.buckconfig

    You can also specify a particular cell to which to apply the
    configuration. By default, the settings in the configuration file
    apply to *all* cells in the current build.

    ##### Apply the configuration only to the *current* cell.

        --config-file //=<path-to-config-file>

    ##### Apply the configuration only to a *specified* cell.

        --config-file <target-cell>=<path-to-config-file>

    If you specify `*` as the target cell, the configuration is applied
    to *all* the cells in the build. This is the default, but this
    syntax enables you to be explicit.

    To learn more about Buck\'s concept of cells, see the [Key
    Concepts](/about/overview.html) topic.

-   `--num-threads`

    Specify the number of threads that buck uses when executing jobs.
    The default value is 1.25 times the number of *logical* cores in the
    system; on systems with hyperthreading, this means that each
    physical core is counted as two logical cores. You can also set the
    number of threads to use for building by adding a `threads` key to
    the `[build]` section of the `.buckconfig` file.

    The order of precedence for setting the number of build threads
    (from highest to lowest) is:

    1.  The `--num-threads` command-line parameter.
    2.  The `.buckconfig` setting.
    3.  The default value (see above).

    The number of *active* threads might not always be equal to this
    argument.

-   `--flagfile /path/to/commandline-args or @/path/to/commandline-args`

    Specify additional command-line arguments in external files (*flag
    files*), one argument per line. The arguments in these files can
    themselves be `--flagfile` or `@` arguments, which would then
    include the additional specified file\'s contents as arguments.

    ``` {.prettyprint .lang-ini}
    # File config/common
    --verbose
    ```

    ``` {.prettyprint .lang-ini}
    # File config/gcc
    @config/common
    --config
    cxx.cxx=/usr/bin/g++
    ...
    ```

    ``` {.prettyprint .lang-ini}
    # File config/clang
    @config/common
    --config
    cxx.cxx=/usr/bin/clang++
    ...
    ```

    ``` {.prettyprint .lang-ini}
    buck build @config/gcc foo/bar:
    buck build @config/clang foo/bar:
    ```

    Lines in flag files must not have any leading or trailing white
    space.

    The equals sign (`=`) separates the specified property and value.
    There should be no white space between the property and the equals
    sign, nor between the equals sign and the value.

    We recommend that you use `--flagfile` rather than the `@` symbol as
    `--flagfile` is more self-describing.

    This `--config-file` parameter (described earlier) provides
    functionality similar to `--flagfile`, but with `.buckconfig` syntax
    rather than command-line parameter syntax.

    If Buck is regularly invoked with different sets of arguments, we
    recommend that you use flag files or config files, as they can be
    stored in source control, which makes builds more reproducible.
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
