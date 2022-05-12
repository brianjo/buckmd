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
# cxx_test()

::: overview
[This is liable to change in the future.]{.small}

A cxx_test() rule builds a C/C++ binary against a C/C++ testing
framework and runs it as part of [`buck test`](/command/test.html).

## Arguments

-   ::: {#name}
    ### `name`{.argName} [(required)]{.argDefault} [\#](#name){.inline-link}

    The *short name* for this [build
    target](/concept/build_target.html).
    :::

-   ::: {#srcs}
    ### `srcs`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#srcs){.inline-link}

    The set of C, C++, Objective-C, Objective-C++, or assembly source
    files to be preprocessed, compiled, and assembled by this rule. We
    determine which stages to run on each input source based on its file
    extension. See the [GCC
    documentation](https://gcc.gnu.org/onlinedocs/gcc/Overall-Options.html)
    for more detail on how file extensions are interpreted. Each element
    can be either a string specifying a source file (e.g. `'foo/bar.c'`)
    or a tuple of a string specifying a source file and a list of
    compilation flags (e.g. `('foo/bar.c', ['-Wall', '-Werror'])`). In
    the latter case the specified flags will be used in addition to the
    rule\'s other flags when preprocessing and compiling that file (if
    applicable).
    :::

-   ::: {#headers}
    ### `headers`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#headers){.inline-link}

    The set of header files that are made available for inclusion to the
    source files in this target. These should be specified as either a
    list of header files or a dictionary of header names to header
    files. The header name can contain forward slashes (`/`). The
    headers can be included with
    `#include "$HEADER_NAMESPACE/$HEADER_NAME"` or
    `#include <$HEADER_NAMESPACE/$HEADER_NAME>`, where
    `$HEADER_NAMESPACE` is the value of the target\'s `header_namespace`
    attribute, and `$HEADER_NAME` is the header name if specified, and
    the filename of the header file otherwise. See `header_namespace`
    for more information.
    :::

-   ::: {#preprocessor_flags}
    ### `preprocessor_flags`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#preprocessor_flags){.inline-link}

    Flags to use when preprocessing any of the above sources (which
    require preprocessing).
    :::

-   ::: {#compiler_flags}
    ### `compiler_flags`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#compiler_flags){.inline-link}

    Flags to use when compiling any of the above sources (which require
    compilation).
    :::

-   ::: {#linker_flags}
    ### `linker_flags`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#linker_flags){.inline-link}

    Flags to add to the linker command line whenever the output from
    this rule is used in a link operation, such as linked into an
    executable or a shared library.
    :::

-   ::: {#precompiled_header}
    ### `precompiled_header`{.argName} [(defaults to `None`)]{.argDefault} [\#](#precompiled_header){.inline-link}

    Path to a
    [`cxx_precompiled_header`](/rule/cxx_precompiled_header.html) to use
    when compiling this rule\'s sources. The precompiled header (PCH) is
    built on-demand, using compiler flags matching those used in this
    rule\'s compile jobs. This is to ensure compatibility between this
    rule and the PCH. Also, this rule will inherit additional `deps`
    from the PCH rule, and as a result, additional include paths as well
    (e.g. `-I`, `-isystem`, `-iquote` path lists, and framework paths
    specified with `-F`).
    :::

-   ::: {#deps_query}
    ### `deps_query`{.argName} [(defaults to `None`)]{.argDefault} [\#](#deps_query){.inline-link}

    Status: **experimental/unstable**. The deps query takes a query
    string that accepts the following query functions, and appends the
    output of the query to the declared deps:

    -   `attrfilter`
    -   `deps`
    -   `except`
    -   `intersect`
    -   `filter`
    -   `kind`
    -   `set`
    -   `union`

    The macro `$declared_deps` may be used anywhere a target literal
    pattern is expected in order to refer to the explicit deps of this
    rule as they appear in the rule\'s definition. For example, if your
    build rule declares
    ``` {.prettyprint .lang-py}
      android_library(
        name = 'lib',
        deps = ['//foo:foo'],
        deps_query = '$declared_deps',
      )
    ```

    then the macro `$declared_deps` would be expanded to a literal
    `set(//foo:foo)`. Some example queries:
          "filter({name_regex}, $declared_deps)".format(name_regex='//.*')
          "attrfilter(annotation_processors, com.foo.Processor, $declared_deps)"
    :::

-   ::: {#resources}
    ### `resources`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#resources){.inline-link}

    This attribute is currently not implemented, and just causes buck to
    rebuild the test file if any of the resources change. This will
    change in the future to provide a more reliable interface for
    resource files.

    Additional data or source files which this test uses.
    :::

-   ::: {#raw_headers}
    ### `raw_headers`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#raw_headers){.inline-link}

    The set of header files that can be used for inclusion to the source
    files in the target and all targets that transitively depend on it.
    Buck doesn\'t add raw headers to the search path of a
    compiler/preprocessor automatically.`include_directories` and
    `public_include_directories` are the recommended way to add raw
    headers to the search path (they will be added via
    `-I`).`compiler_flags`, `preprocessor_flags` and
    `exported_preprocessor_flags`can also be used to add such raw
    headers to the search path if inclusion via `-isystem` or`-iquote`
    is needed.`raw_headers` cannot be used together with `headers` or
    `exported_headers` in the same target.
    :::

-   ::: {#include_directories}
    ### `include_directories`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#include_directories){.inline-link}

    A list of include directories (with `raw_headers`) to be added to
    the compile command for compiling this target (via `-I`). An include
    directory is relative to the current package.
    :::

-   ::: {#framework}
    ### `framework`{.argName} [(defaults to `"gtest"`)]{.argDefault} [\#](#framework){.inline-link}

    The testing framework to build against and run with. We currently
    support [`gtest`](https://github.com/google/googletest) and
    [`boost`](http://www.boost.org/doc/libs/1_57_0/libs/test/doc/html/index.html).

    When set to `gtest`, you must also set
    [`[cxx].gtest_dep`](/files-and-dirs/buckconfig.html#cxx.gtest_dep).
    :::

-   ::: {#env}
    ### `env`{.argName} [(defaults to `{}`)]{.argDefault} [\#](#env){.inline-link}

    A map of environment names and values to set when running the test.\
    \
    It is also possible to expand references to other rules within the
    **values** of these environment variables, using builtin [string
    parameter macros](/function/string_parameter_macros.html):

    `$(location //path/to:target)`
    :   Expands to the location of the output of the build rule. This
        means that you can refer to these without needing to be aware of
        how Buck is storing data on the disk mid-build.
    :::

-   ::: {#args}
    ### `args`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#args){.inline-link}

    A list of additional arguments to pass to the test when it\'s run.\
    \
    It is also possible to expand references to other rules within these
    arguments, using builtin [string parameter
    macros](/function/string_parameter_macros.html):

    `$(location //path/to:target)`
    :   Expands to the location of the output of the build rule. This
        means that you can refer to these without needing to be aware of
        how Buck is storing data on the disk mid-build.
    :::

-   ::: {#contacts}
    ### `contacts`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#contacts){.inline-link}

    A list of organizational contacts for this test. These could be
    individuals who you would contact in the event of a test failure or
    other issue with the test.

        contacts = [ 'Joe Sixpack', 'Erika Mustermann' ]
    :::

-   ::: {#run_test_separately}
    ### `run_test_separately`{.argName} [(defaults to `False`)]{.argDefault} [\#](#run_test_separately){.inline-link}

    If set to `True`, the test(s) in this rule are run separately from
    all other tests. (This is useful for integration tests which access
    a physical device or other limited resource.)

    If unset, the test(s) in this rule in parallel with all other tests.
    :::

-   ::: {#test_rule_timeout_ms}
    ### `test_rule_timeout_ms`{.argName} [(defaults to `None`)]{.argDefault} [\#](#test_rule_timeout_ms){.inline-link}

    If set specifies the maximum amount of time (in milliseconds) in
    which all of the tests in this rule should complete. This overrides
    the default `rule_timeout` if any has been specified in
    [`[test].rule_timeout`](/files-and-dirs/buckconfig.html#test.rule_timeout).
    :::

-   ::: {#extra_xcode_sources}
    ### `extra_xcode_sources`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#extra_xcode_sources){.inline-link}

    When the project is generated, this is the list of files that will
    added to the build phase \"Compile Sources\" of the given target.
    :::

-   ::: {#extra_xcode_files}
    ### `extra_xcode_files`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#extra_xcode_files){.inline-link}

    When the project is generated, this is the list of files that will
    added to the project. Those files won\'t be added to the build phase
    \"Compile Sources\".
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

## Examples

``` {.prettyprint .lang-py}
# A rule that builds and runs C/C++ test using gtest.
cxx_test(
  name = 'echo_test',
  srcs = [
    'echo_test.cpp',
  ],
)
```
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
