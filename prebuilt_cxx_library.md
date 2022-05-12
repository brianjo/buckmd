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
# prebuilt_cxx_library()

::: overview
[This is liable to change in the future.]{.small}

A `prebuilt_cxx_library()` rule represents a set of native libraries and
C/C++ header files and provides various flags to control how they are
linked and exported.

## Arguments

-   ::: {#name}
    ### `name`{.argName} [(required)]{.argDefault} [\#](#name){.inline-link}

    The *short name* for this [build
    target](/concept/build_target.html).
    :::

-   ::: {#header_only}
    ### `header_only`{.argName} [(defaults to `False`)]{.argDefault} [\#](#header_only){.inline-link}

    Indicates if this library only consists of headers or not. If this
    is set to `True`, Buck will not link this library into any library
    that depends on it.
    :::

-   ::: {#header_dirs}
    ### `header_dirs`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#header_dirs){.inline-link}

    A directory that headers can be included from. These directories are
    added to the include path using `-isystem`.
    :::

-   ::: {#platform_header_dirs}
    ### `platform_header_dirs`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#platform_header_dirs){.inline-link}

    Platform specific header directories. These should be specified as a
    list of pairs where the first element is an un-anchored regex (in
    java.util.regex.Pattern syntax) against which the platform name is
    matched, and the second element is either a list of header
    directories. See `header_dirs` for more information.
    :::

-   ::: {#static_lib}
    ### `static_lib`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#static_lib){.inline-link}

    The path to the library to use when performing static linking.
    :::

-   ::: {#platform_static_lib}
    ### `platform_static_lib`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#platform_static_lib){.inline-link}

    Platform specific static library. These should be specified as a
    list of pairs where the first element is an un-anchored regex (in
    java.util.regex.Pattern syntax) against which the platform name is
    matched, and the second element the path to the library. See
    `static_lib` for more information.
    :::

-   ::: {#static_pic_lib}
    ### `static_pic_lib`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#static_pic_lib){.inline-link}

    The path to the library to use when performing static PIC linking.
    :::

-   ::: {#platform_static_pic_lib}
    ### `platform_static_pic_lib`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#platform_static_pic_lib){.inline-link}

    Platform specific static PIC library. These should be specified as a
    list of pairs where the first element is an un-anchored regex (in
    java.util.regex.Pattern syntax) against which the platform name is
    matched, and the second element the path to the library. See
    `static_pic_lib` for more information.
    :::

-   ::: {#shared_lib}
    ### `shared_lib`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#shared_lib){.inline-link}

    The path to the library to use when performing shared linking.
    :::

-   ::: {#platform_shared_lib}
    ### `platform_shared_lib`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#platform_shared_lib){.inline-link}

    Platform specific shared library. These should be specified as a
    list of pairs where the first element is an un-anchored regex (in
    java.util.regex.Pattern syntax) against which the platform name is
    matched, and the second element the path to the library. See
    `shared_lib` for more information.
    :::

-   ::: {#supported_platforms_regex}
    ### `supported_platforms_regex`{.argName} [(defaults to `None`)]{.argDefault} [\#](#supported_platforms_regex){.inline-link}

    If present, an un-anchored regex (in java.util.regex.Pattern syntax)
    that matches all platforms that this library supports. It will not
    be built for other platforms.
    :::

-   ::: {#exported_headers}
    ### `exported_headers`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#exported_headers){.inline-link}

    The set of header files that are made available for inclusion to the
    source files in the target and all targets that transitively depend
    on it. These should be specified as either a list of header files or
    a dictionary of header names to header files. The headers can be
    included with `#include "$HEADER_NAMESPACE/$HEADER_NAME"` or
    `#include <$HEADER_NAMESPACE/$HEADER_NAME>`, where
    `$HEADER_NAMESPACE` is the value of the target\'s `header_namespace`
    attribute, and `$HEADER_NAME` is the header name if specified, and
    the filename of the header file otherwise. Note that the header name
    can contain forward slashes (`/`). See `header_namespace` for more
    information.
    :::

-   ::: {#exported_platform_headers}
    ### `exported_platform_headers`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#exported_platform_headers){.inline-link}

    Platform specific header files. These should be specified as a list
    of pairs where the first element is an un-anchored regex (in
    java.util.regex.Pattern syntax) against which the platform name is
    matched, and the second element is either a list of header files or
    a dictionary of header names to header files that will be made
    available for inclusion to the source files in the target and all
    targets that transitively depend on it if the platform matches the
    regex. See `headers` for more information.
    :::

-   ::: {#header_namespace}
    ### `header_namespace`{.argName} [(defaults to `name`)]{.argDefault} [\#](#header_namespace){.inline-link}

    A path prefix when including headers of this target. Defaults to the
    path from the root of the repository to the directory where this
    target is defined. Can contain forward slashes (`/`), but cannot
    start with one. See `headers` for more information.
    :::

-   ::: {#exported_preprocessor_flags}
    ### `exported_preprocessor_flags`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#exported_preprocessor_flags){.inline-link}

    Just as `preprocessor_flags`, flags to use when preprocessing any of
    the above sources (which require preprocessing). However, unlike
    `preprocessor_flags`, these preprocessor flags are also used by
    rules that transitively depend on this rule when preprocessing their
    own sources.
    :::

-   ::: {#exported_platform_preprocessor_flags}
    ### `exported_platform_preprocessor_flags`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#exported_platform_preprocessor_flags){.inline-link}

    Platform specific exported preprocessor flags. These should be
    specified as a list of pairs where the first element is an
    un-anchored regex (in java.util.regex.Pattern syntax) against which
    the platform name is matched, and the second element is a list of
    flags to use when preprocessing the source files in the target and
    all targets that transitively depend on it if the platform matches
    the regex. See `exported_preprocessor_flags` for more information.
    :::

-   ::: {#exported_linker_flags}
    ### `exported_linker_flags`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#exported_linker_flags){.inline-link}

    Flags to add to the linker command line when the output from this
    rule, or the output from any rule that transitively depends on this
    rule, is used in a link operation.
    :::

-   ::: {#force_static}
    ### `force_static`{.argName} [(defaults to `False`)]{.argDefault} [\#](#force_static){.inline-link}

    DEPRECATED: `See preferred_linkage`. If `true`, the library will
    always be linked statically, even if the target that depends on it
    specifies `link_style` to be something other than `static`. Note
    that this may still cause the library to be linked into its own
    shared library, if it happens to be the root of the linkable
    dependency tree (e.g. if a Python library directly depends on the
    library with `force_static=True`). Also note this will cause
    duplicate symbols if multiple targets that depend on the library are
    linked together.
    :::

-   ::: {#preferred_linkage}
    ### `preferred_linkage`{.argName} [(defaults to `any`)]{.argDefault} [\#](#preferred_linkage){.inline-link}

    Controls how a library should be linked.

    `any`
    :   The library will be linked based on its dependents `link_style`.

    `shared`
    :   The library will be always be linked as a shared library.

    `static`
    :   The library will be linked as a static library.

    Note: since shared libraries re-export its dependencies, depending
    on multiple shared libraries which themselves have overlapping
    static dependencies will cause duplicate symbols.
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

-   ::: {#supports_merged_linking}
    ### `supports_merged_linking`{.argName} [(defaults to `True`)]{.argDefault} [\#](#supports_merged_linking){.inline-link}

    Whether this rule supports building with the merged linking strategy
    when building for non-native binaries (e.g. when using
    [`[python].native_link_strategy`](/files-and-dirs/buckconfig.html#python.native_link_strategy)s
    `merged` setting).
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

A prebuilt library containing only headers that other libraries may
need.

``` {.prettyprint .lang-py}
prebuilt_cxx_library(
  name = 'stdutil',
  header_only = True,
  header_dirs = [
    'include',
  ],
)
```

A prebuilt library with static and shared libs.

``` {.prettyprint .lang-py}
prebuilt_cxx_library(
  name = 'mylib',
  soname = 'libmylib.so',
  static_lib = 'libmylib.a',
  static_pic_lib = 'libmylib_pic.a',
  shared_lib = 'libmylib.so',
  exported_headers = [
    'mylib.h',
  ],
)
```

A prebuilt library with multiple builds for multiple platforms.

``` {.prettyprint .lang-py}
prebuilt_cxx_library(
  name = 'mylib',
  soname = 'libmylib.so',
  platform_shared_lib = [
    ('android-arm', 'android-arm/libmylib.so'),
    ('android-x86', 'android-x86/libmylib.so'),
    ('iphonesimulator-x86_64', 'iphonesimulator-x86_64/libmylib.so'),
  ],
  platform_static_lib = [
    ('android-arm', 'android-arm/libmylib.a'),
    ('android-x86', 'android-x86/libmylib.a'),
    ('iphonesimulator-x86_64', 'iphonesimulator-x86_64/libmylib.a'),
  ],
  exported_headers = [
    'mylib.h',
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
