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
# go_test()

::: overview
[This is liable to change in the future.]{.small}

A `go_test()` rule builds a native binary from the specified Go source
and resource files---and a generated main file. It\'s similar to the
`go test` command.

If your test requires static files you should specify these in the
**resources** argument. If you do not specify these files, they won\'t
be available when your test runs.

Buck currently supports Go version 1.10.

## Arguments

-   ::: {#name}
    ### `name`{.argName} [(required)]{.argDefault} [\#](#name){.inline-link}

    The *short name* for this [build
    target](/concept/build_target.html).
    :::

-   ::: {#srcs}
    ### `srcs`{.argName} [(required)]{.argDefault} [\#](#srcs){.inline-link}

    The set of source files to be compiled by this rule. .go files will
    be compiled with the Go compiler, .s files will be compiled with the
    assembler, and everything else is assumed to be files that may be
    `#include`d by the assembler.
    :::

-   ::: {#library}
    ### `library`{.argName} [(defaults to `None`)]{.argDefault} [\#](#library){.inline-link}

    Specify the library that this internal test is testing. This will
    copy the `srcs`, `package_name` and `deps` from the target specified
    so you don\'t have to duplicate them.
    :::

-   ::: {#package_name}
    ### `package_name`{.argName} [(defaults to `go.prefix + path relative to the buck root + "_test"`)]{.argDefault} [\#](#package_name){.inline-link}

    Sets the full name of the test package being compiled. This defaults
    to the path from the buck root with \"\_test\" appended. (e.g. given
    a ./.buckconfig, a rule in ./a/b/BUCK defaults to package
    \"a/b_test\")

    Note: if you want to test packages internally (i.e. same package
    name), use the `library` parameter instead of setting `package_name`
    to include the tested source files.
    :::

-   ::: {#coverage_mode}
    ### `coverage_mode`{.argName} [(defaults to `None`)]{.argDefault} [\#](#coverage_mode){.inline-link}

    Test coverage functionality will be included in the executable.
    Modes: set, count, atomic
    :::

-   ::: {#deps}
    ### `deps`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#deps){.inline-link}

    The set of dependencies of this rule. Currently, this only supports
    go_library rules.
    :::

-   ::: {#link_style}
    ### `link_style`{.argName} [(defaults to `static_pic`)]{.argDefault} [\#](#link_style){.inline-link}

    Determines whether to build and link this rule\'s dependencies
    statically or dynamically. Can be one of the following values:
    `static`, `static_pic` or `shared`. This argument is relevant only
    if the cgo extension is enabled. Otherwise, Buck ignores this
    argument.
    :::

-   ::: {#link_mode}
    ### `link_mode`{.argName} [(defaults to ``)]{.argDefault} [\#](#link_mode){.inline-link}

    Determines the link mode (equivalent of `-mode`). Can be one of the
    following values: `internal`, `external`. If no value is provided,
    the mode is set automatically depending on the other args.
    :::

-   ::: {#compiler_flags}
    ### `compiler_flags`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#compiler_flags){.inline-link}

    The set of additional compiler flags to pass to `go tool compile`.
    :::

-   ::: {#assembler_flags}
    ### `assembler_flags`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#assembler_flags){.inline-link}

    The set of additional assembler flags to pass to `go tool asm`.
    :::

-   ::: {#linker_flags}
    ### `linker_flags`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#linker_flags){.inline-link}

    Extra linker flags passed to go link
    :::

-   ::: {#external_linker_flags}
    ### `external_linker_flags`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#external_linker_flags){.inline-link}

    Extra external linker flags passed to go link via `-extld` argument.
    If argument is non-empty or `cgo_library` is used, the link mode
    will switch to `external`.
    :::

-   ::: {#resources}
    ### `resources`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#resources){.inline-link}

    Static files that are symlinked into the working directory of the
    test. You can access these files in your test by opening them using
    relative paths, such as `ioutil.ReadFile("testdata/input")`.
    :::

-   ::: {#labels}
    ### `labels`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#labels){.inline-link}

    A list of labels to be applied to these tests. These labels are
    arbitrary text strings and have no meaning within buck itself. They
    can, however, have meaning for you as a test author (e.g., `smoke`
    or `fast`). A label can be used to filter or include a specific test
    rule when executing [`buck test`](/command/test.html).
    :::

-   ::: {#test_rule_timeout_ms}
    ### `test_rule_timeout_ms`{.argName} [(defaults to `None`)]{.argDefault} [\#](#test_rule_timeout_ms){.inline-link}

    If set specifies the maximum amount of time (in milliseconds) in
    which all of the tests in this rule should complete. This overrides
    the default `rule_timeout` if any has been specified in
    [`[test].rule_timeout`](/files-and-dirs/buckconfig.html#test.rule_timeout).
    :::

-   ::: {#env}
    ### `env`{.argName} [(defaults to `{}`)]{.argDefault} [\#](#env){.inline-link}

    A map of environment variables and values to set when running the
    test.
    :::

-   ::: {#run_test_separately}
    ### `run_test_separately`{.argName} [(defaults to `False`)]{.argDefault} [\#](#run_test_separately){.inline-link}

    If set to `True`, the test(s) in this rule are run separately from
    all other tests. (This is useful for integration tests which access
    a physical device or other limited resource.)

    If unset, the test(s) in this rule in parallel with all other tests.
    :::

-   ::: {#contacts}
    ### `contacts`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#contacts){.inline-link}

    A list of organizational contacts for this test. These could be
    individuals who you would contact in the event of a test failure or
    other issue with the test.

        contacts = [ 'Joe Sixpack', 'Erika Mustermann' ]
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

For more examples, check out our [integration
tests](https://github.com/facebook/buck/tree/master/test/com/facebook/buck/features/go/testdata).

``` {.prettyprint .lang-py}
go_library(
  name='greeting',
  srcs=[
    'greeting.go',
  ],
  deps=[
    ':join',
  ],
)

go_test(
  name='greeting-test',
  srcs=[
    'greeting_ext_test.go',
  ],
  deps=[
    ':greeting'
  ],
)

go_test(
  name='greeting-internal-test',
  package_name='greeting',
  srcs=[
    'greeting.go',
    'greeting_test.go',
  ],
  deps=[
    ':join',
  ],
)

# Or

go_test(
  name='greeting-better-internal-test',
  srcs=['greeting_test.go'],
  library=':greeting',
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
