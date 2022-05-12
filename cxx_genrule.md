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
# cxx_genrule()

::: overview
A `cxx_genrule()` enables you to run shell commands as part of the Buck
build process. A `cxx_genrule()` exposes---through a set of string
parameter macros and variables---information about the tools and
configuration options used by the Buck environment, specifically those
related to the C/C++ toolchain.

The information exposed through these tools and configuration options is
a reflection of: Buck\'s built-in settings, the settings in
[`.buckconfig`](/files-and-dirs/buckconfig.html) and
`.buckconfig.local`, and the result of various command-line overrides
specified through the [`--config`](/command/common_parameters.html)
command-line option.

This information is available only to the shell commands specified in
the `cxx_genrule`. The information is not available to other arguments
of the rule.

A `cxx_genrule()` can be an input to another `cxx_genrule()`.

Note that if you specify the `cxx_genrule` as a command-line target to
`buck build`, you must include a platform flavor. For example:

    buck build :cxx_gr_name#iphonesimulator-x86_64

You could also just specify the default platform flavor explicitly:

    buck build :cxx_gr_name#default

## Arguments

-   ::: {#name}
    ### `name`{.argName} [(required)]{.argDefault} [\#](#name){.inline-link}

    The *short name* for this [build
    target](/concept/build_target.html).
    :::

-   ::: {#srcs}
    ### `srcs`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#srcs){.inline-link}

    Either a list or a map of the source files which Buck makes
    available to the shell command at the path in the `SRCDIR`
    environment variable. If you specify a list, the source files are
    the names in the list. If you specify a map, the source files are
    made available as the names in the keys of the map, where the values
    of the map are the original source file names.
    :::

-   ::: {#cmd}
    ### `cmd`{.argName} [(defaults to `None`)]{.argDefault} [\#](#cmd){.inline-link}

    The shell command to run to generate the output file. It is the
    fallback of `bash` and `cmd_exe`. The shell command can access
    information about the buck build environment through a set of
    *macros*, *parameterized macros*, and *variables*.

    #### Macros

    The following macros are available to the shell command and are
    accessed using the following syntax.

        $(<macro>)

    Example:

        $(cc)

    `$(cc)`
    :   Path to the C compiler.

    `$(cxx)`
    :   Path to the C++ compiler.

    `$(cflags)`
    :   Flags passed to the C compiler.

    `$(cppflags)`
    :   Flags passed to the C preprocessor.

    `$(cxxflags)`
    :   Flags passed to the C++ compiler.

    `$(ld)`
    :   Path to the linker.

    `$(ldflags-pic)`
    :   Flags passed to the linker for binaries that use
        position-independent code (PIC).

    `$(ldflags-pic-filter <pattern>)`
    :   Flags passed to the linker for binaries that use
        position-independent code (PIC). Use the *pattern* parameter to
        specify a regular expression that matches the build targets that
        use these flags.

    `$(ldflags-shared)`
    :   Flags passed to the linker for shared libraries, such as
        dynamic-link libraries (DLLs).

    `$(ldflags-shared-filter <pattern>)`
    :   Flags passed to the linker for shared libraries, such as
        dynamic-link libraries (DLLs). Use the *pattern* parameter to
        specify a regular expression that matches the build targets that
        use these flags.

    `$(ldflags-static)`
    :   Flags passed to the linker for statically-linked libraries.

    `$(ldflags-static-filter <pattern>)`
    :   Flags passed to the linker for statically-linked libraries. Use
        the *pattern* parameter to specify a regular expression that
        matches the build targets that use these flags.

    `$(platform-name)`
    :   The platform flavor with which this `cxx_genrule` was specified.

    #### Parameterized Macros

    It is also possible to expand references to other rules within the
    shell command, using the following subset of the builtin [string
    parameter macros](/function/string_parameter_macros.html). Note that
    all build rules expanded in the command are automatically considered
    to be dependencies of the `genrule()`.

    Note that the paths returned by these macros are *absolute* paths.
    You should convert these paths to be relative paths before embedding
    them in, for example, a shell script or batch file. Using relative
    paths ensures that your builds are *hermetic*, that is, they are
    reproducible across different machine environments.

    Additionally, if you embed these paths in a shell script, you should
    execute that script using the [`sh_binary`](/rule/sh_binary.html)
    rule and include the targets for these paths in the `resources`
    argument of that `sh_binary` rule. These are the same targets that
    you pass to the string parameter macros.

    `$(exe //path/to:target)`
    :   Expands to the commands necessary to run the executable
        generated by the specified build rule. For a C++ executable,
        this will typically just be the name of the output executable
        itself, such as `main`. If the specified build rule does not
        generate an executable output, an exception will be thrown and
        the build will fail.

    `$(location //path/to:target)`
    :   Expands to the path of the output of the build rule. This means
        that you can refer to these without needing to be aware of how
        Buck is storing data on the disk mid-build.

    #### Variables

    Finally, Buck adds the following variables to the environment in
    which the shell command runs. They are accessed using the following
    syntax. Note the use of braces rather than parentheses.

        ${<variable>}

    Example:

        ${SRCS}

    `${SRCS}`\
    :   A string expansion of the `srcs` argument delimited by the
        `environment_expansion_separator` argument where each element of
        `srcs` will be translated into an absolute path.

    `${SRCDIR}`\
    :   The absolute path to the to which sources are copied prior to
        running the command.

    `${OUT}`
    :   The output file for the `genrule()`. The file specified by this
        variable must always be written by this command. If not, the
        execution of this rule will be considered a failure, halting the
        build process.

    `${TMP}`
    :   A temporary directory which can be used for intermediate results
        and will not be bundled into the output.
    :::

-   ::: {#bash}
    ### `bash`{.argName} [(defaults to `None`)]{.argDefault} [\#](#bash){.inline-link}

    A platform-specific version of the shell command parameter `cmd`. It
    runs on Linux and UNIX systems---including OSX---on which `bash` is
    installed. It has a higher priority than `cmd`. The `bash` argument
    is run with `/bin/bash -c`. It has access to the same set of macros
    and variables as the `cmd` argument.
    :::

-   ::: {#cmd_exe}
    ### `cmd_exe`{.argName} [(defaults to `None`)]{.argDefault} [\#](#cmd_exe){.inline-link}

    A platform-specific version of the shell command parameter `cmd`. It
    runs on Windows and has a higher priority than `cmd`. The `cmd_exe`
    argument is run with `cmd.exe /c`. It has access to the same set of
    macros and variables as the `cmd` argument.
    :::

-   ::: {#type}
    ### `type`{.argName} [(defaults to `None`)]{.argDefault} [\#](#type){.inline-link}

    Specifies the *type* of this genrule. This is used for logging and
    is particularly useful for grouping genrules that share an
    underlying logical \"type\".

    For example, if you have the following `cxx_genrule` defined in the
    root directory of your Buck project

        cxx_genrule(
          name = 'cxx_gen',
          type = 'epilog',
          cmd  = 'touch finish.txt; cp finish.txt $OUT',
          out  = 'finish.txt'
        )

    then the following `buck query` command

        buck query "attrfilter( type, 'epilog', '//...' )"

    returns

        //:cxx_gen
    :::

-   ::: {#out}
    ### `out`{.argName} [(required)]{.argDefault} [\#](#out){.inline-link}

    The name of the output file or directory. The complete path to this
    argument is provided to the shell command through the `OUT`
    environment variable.
    :::

-   ::: {#environment_expansion_separator}
    ### `environment_expansion_separator`{.argName} [(defaults to `" "`)]{.argDefault} [\#](#environment_expansion_separator){.inline-link}

    The delimiter between paths in environment variables, such as SRCS,
    that can contain multiple paths. It can be useful to specify this
    parameter if the paths could contain spaces.
    :::

-   ::: {#enable_sandbox}
    ### `enable_sandbox`{.argName} [(defaults to `False`)]{.argDefault} [\#](#enable_sandbox){.inline-link}

    Whether this target should be executed in a sandbox or not.
    :::

-   ::: {#executable}
    ### `executable`{.argName} [(defaults to `False`)]{.argDefault} [\#](#executable){.inline-link}

    Whether the output of the genrule is itself executable. Marking an
    output as executable makes `buck run` and `$(exe ...)` macro
    expansion work with this target.
    :::

-   ::: {#tests}
    ### `tests`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#tests){.inline-link}

    List of [build targets](/concept/build_target.html) that identify
    tests that exercise this target.
    :::

-   ::: {#visibility}
    ### `visibility`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#visibility){.inline-link}

    List of [build target patterns](/concept/build_target_pattern.html)
    that identify the build rules that can include this rule as a
    dependency, for example, by listing it in their `deps` or
    `exported_deps` attributes. For more information, see
    [visibility](/concept/visibility.html).
    :::

-   ::: {#licenses}
    ### `licenses`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#licenses){.inline-link}

    Set of license files for this library. To get the list of license
    files for a given [build rule](/concept/build_rule.html) and all of
    its dependencies, you can use [`buck query`](/command/query.html).
    :::

-   ::: {#labels}
    ### `labels`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#labels){.inline-link}

    Set of arbitrary strings which allow you to annotate a [build
    rule](/concept/build_rule.html) with tags that can be searched for
    over an entire dependency tree using
    [`buck query attrfilter()`](/command/query.html#attrfilter).
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
