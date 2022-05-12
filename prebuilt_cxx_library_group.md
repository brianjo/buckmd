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
# prebuilt_cxx_library_group()

::: overview
[This is liable to change in the future.]{.small}

A `prebuilt_cxx_library_group()` rule represents a group of native
libraries which should be handled together in a single rule, perhaps
using special link-line construction.

## Arguments

-   ::: {#name}
    ### `name`{.argName} [(required)]{.argDefault} [\#](#name){.inline-link}

    The *short name* for this [build
    target](/concept/build_target.html).
    :::

-   ::: {#exported_preprocessor_flags}
    ### `exported_preprocessor_flags`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#exported_preprocessor_flags){.inline-link}

    Just as `preprocessor_flags`, flags to use when preprocessing any of
    the above sources (which require preprocessing). However, unlike
    `preprocessor_flags`, these preprocessor flags are also used by
    rules that transitively depend on this rule when preprocessing their
    own sources.
    :::

-   ::: {#static_link}
    ### `static_link`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#static_link){.inline-link}

    The arguments to use when linking this library group using the
    static link style. The actual paths to libraries should be listed in
    the `static_libs` parameter, and referenced via the the
    `$(lib [index])` macro in these args.
    :::

-   ::: {#static_libs}
    ### `static_libs`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#static_libs){.inline-link}

    The paths to the libraries used when using the static link style.
    The `static_link` parameter should refer to these libs using their
    index number.
    :::

-   ::: {#static_pic_link}
    ### `static_pic_link`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#static_pic_link){.inline-link}

    The arguments to use when linking this library group using the
    static-pic link style. The actual paths to libraries should be
    listed in the `static_pic_libs`parameter, and referenced via the the
    `$(lib [index])` macro in these args.
    :::

-   ::: {#static_pic_libs}
    ### `static_pic_libs`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#static_pic_libs){.inline-link}

    The paths to the libraries used when using the static link style.
    The `static_pic_link` parameter should refer to these libs using
    their index number.
    :::

-   ::: {#shared_link}
    ### `shared_link`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#shared_link){.inline-link}

    The arguments to use when linking this library group using the
    shared link style. The actual paths to libraries should be listed in
    the `shared_libs`parameter, and referenced via the the
    `$(lib [name])` macro (or the`$(rel-lib [name])` macro, when the
    shared library should be linked using the `-L[dir] -l[name]` style)
    in these args.
    :::

-   ::: {#shared_libs}
    ### `shared_libs`{.argName} [(defaults to `{}`)]{.argDefault} [\#](#shared_libs){.inline-link}

    The map of shared library names to paths used when using the shared
    link style. The `shared_link` parameter should refer to these libs
    using their library name.
    :::

-   ::: {#provided_shared_libs}
    ### `provided_shared_libs`{.argName} [(defaults to `{}`)]{.argDefault} [\#](#provided_shared_libs){.inline-link}

    The map of system-provided shared library names to paths used when
    using the shared link style. The `shared_link` parameter should
    refer to these libs using their library name.
    :::

-   ::: {#exported_deps}
    ### `exported_deps`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#exported_deps){.inline-link}

    Dependencies that will also appear to belong to any rules that
    depend on this one. This has two effects:

    -   Exported dependencies will also be included in the link line of
        dependents of this rules, but normal dependencies will not.
    -   When `reexport_all_header_dependencies = False`, only exported
        headers of the rules specified here are re-exported.
    :::

-   ::: {#exported_platform_deps}
    ### `exported_platform_deps`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#exported_platform_deps){.inline-link}

    Platform specific dependencies that will also appear to belong to
    any rules that depend on this one. These should be specified as a
    list of pairs where the first element is an un-anchored regex (in
    java.util.regex.Pattern syntax) against which the platform name is
    matched, and the second element is a list of external dependencies
    (same format as `exported_deps`) that are exported if the platform
    matches the regex. See `exported_deps` for more information.
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

A prebuilt library group wrapping two libraries that must be linked
together.

``` {.prettyprint .lang-py}
prebuilt_cxx_library_group(
  name = 'util',
  static_link = [
    '-Wl,--start-group',
    '$(lib 0)',
    '$(lib 1)',
    '-Wl,--end-group',
  ],
  static_libs = [
    'lib/liba.a',
    'lib/libb.a',
  ],
  static_pic_link = [
    '-Wl,--start-group',
    '$(lib 0)',
    '$(lib 1)',
    '-Wl,--end-group',
  ],
  static_libs = [
    'lib/liba_pic.a',
    'lib/libb_pic.a',
  ],
  shared_link = [
    '$(rel-lib liba.so)',
    '$(rel-lib libb.so)',
  ],
  shared_libs = {
    'liba.so': 'lib/liba.so',
  },
  provided_shared_libs = {
    'libb.so': 'lib/libb.so',
  },
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