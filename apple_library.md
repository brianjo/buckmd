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
# apple_library()

::: overview
[This is liable to change in the future.]{.small}

An `apple_library()` rule represents a set of Objective-C/C++/Swift
source files and is similar to a [`cxx_library()`
rule](/rule/cxx_library.html) with which it shares many attributes. In
addition to those common attributes, `apple_library()` has a some
additional attributes that are specific to binaries intended to be built
using the Apple toolchain. Note, however, that `apple_library()` and
`cxx_library()` differ in the way that they import header files, in
order to better accommodate existing conventions. See the sections for
the `headers` and `exported_headers` attributes for more details.

Buck enables you to override components of the Apple toolchain with
alternate tools, either from the Xcode search paths or from directories
that you specify. See
[`[apple].replacement`](/files-and-dirs/buckconfig.html#apple.replacement)
and
[`[apple].xcode_tool_name_override`](/files-and-dirs/buckconfig.html#apple.xcode_tool_name_override)
for more information.

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
    can be either a string specifying a source file (e.g. `'foo/bar.m'`)
    or a tuple of a string specifying a source file and a list of
    compilation flags (e.g. `('foo/bar.m', ['-Wall', '-Werror'])`). In
    the latter case the specified flags will be used in addition to the
    rule\'s other flags when preprocessing and compiling that file (if
    applicable).
    :::

-   ::: {#platform_srcs}
    ### `platform_srcs`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#platform_srcs){.inline-link}

    Platform specific source files. These should be specified as a list
    of pairs where the first element is an un-anchored regex (in
    java.util.regex.Pattern syntax) against which the platform name is
    matched, and the second element is either a list of source files or
    a list of tuples of source files and a list of compilation flags to
    be preprocessed, compiled and assembled if the platform matches the
    regex. See `srcs` for more information.
    :::

-   ::: {#headers}
    ### `headers`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#headers){.inline-link}

    The set of header files that are made available for inclusion to the
    source files in this target. These should be specified as either a
    list of header files or a dictionary of header names to header
    files. The header names can contain forward slashes (`/`). If a list
    of header files is specified, the headers can be imported with
    `#import "$HEADER_PATH_PREFIX/$HEADER_NAME"` or
    `#import "$HEADER_NAME"`, where `$HEADER_PATH_PREFIX` is the value
    of the target\'s `header_path_prefix` attribute, and `$HEADER_NAME`
    is the filename of the header file. If a dictionary is specified,
    each header can be imported with `#import "$HEADER_NAME"`, where
    `$HEADER_NAME` is the key corresponding to this file. In this case,
    the `header_path_prefix` attribute is ignored. In either case,
    quotes in the import statements can be replaced with angle brackets.
    :::

-   ::: {#exported_headers}
    ### `exported_headers`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#exported_headers){.inline-link}

    The set of header files that are made available for inclusion to the
    source files in this target and all targets that transitively depend
    on this one. These should be specified as either a list of header
    files or a dictionary of header names to header files. The header
    names can contain forward slashes (`/`). If a list of header files
    is specified, the headers can be imported with
    `#import "$HEADER_PATH_PREFIX/$HEADER_NAME"` or, if a header file
    that belongs to the same rule is being imported, with
    `#import "$HEADER_NAME"`, where `$HEADER_PATH_PREFIX` is the value
    of the target\'s `header_path_prefix` attribute, and `$HEADER_NAME`
    is the filename of the header file. If a dictionary is specified,
    each header can be imported with `#import "$HEADER_NAME"`, where
    `$HEADER_NAME` is the key corresponding to this file. In this case,
    the `header_path_prefix` attribute is ignored. In either case,
    quotes in the import statements can be replaced with angle brackets.
    :::

-   ::: {#header_path_prefix}
    ### `header_path_prefix`{.argName} [(defaults to `name`)]{.argDefault} [\#](#header_path_prefix){.inline-link}

    A path prefix when including headers of this target. For example,
    headers from a library defined using

    ``` {.prettyprint .lang-py}
    apple_library(
        name = "Library",
        headers = glob(["**/*.h"]),
        header_path_prefix = "Lib",
    )
    ```

    can be imported using following mapping
        Library/SubDir/Header1.h -> Lib/Header1.h
        Library/Header2.h -> Lib/Header2.h
          

    Defaults to the short name of the target. Can contain forward
    slashes (`/`), but cannot start with one. See `headers` for more
    information.
    :::

-   ::: {#header_namespace}
    ### `header_namespace`{.argName} [(defaults to `name`)]{.argDefault} [\#](#header_namespace){.inline-link}

    A path prefix when including headers of this target. Defaults to the
    path from the root of the repository to the directory where this
    target is defined. Can contain forward slashes (`/`), but cannot
    start with one. See `headers` for more information.
    :::

-   ::: {#frameworks}
    ### `frameworks`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#frameworks){.inline-link}

    A list of system frameworks that the code in this target uses. Each
    entry should be a path starting with `$SDKROOT` or `$PLATFORM_DIR`
    to denote that the rest of the path is relative to the root of the
    SDK used for the build or to the platform toolchain directory.
    :::

-   ::: {#preprocessor_flags}
    ### `preprocessor_flags`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#preprocessor_flags){.inline-link}

    Flags to use when preprocessing any of the above sources (which
    require preprocessing).
    :::

-   ::: {#exported_preprocessor_flags}
    ### `exported_preprocessor_flags`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#exported_preprocessor_flags){.inline-link}

    Just as `preprocessor_flags`, flags to use when preprocessing any of
    the above sources (which require preprocessing). However, unlike
    `preprocessor_flags`, these preprocessor flags are also used by
    rules that transitively depend on this rule when preprocessing their
    own sources.
    :::

-   ::: {#compiler_flags}
    ### `compiler_flags`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#compiler_flags){.inline-link}

    Flags to use when compiling any of the above sources (which require
    compilation).
    :::

-   ::: {#platform_compiler_flags}
    ### `platform_compiler_flags`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#platform_compiler_flags){.inline-link}

    Platform specific compiler flags. These should be specified as a
    list of pairs where the first element is an un-anchored regex (in
    java.util.regex.Pattern syntax) against which the platform name is
    matched, and the second element is a list of flags to use when
    compiling the target\'s sources. See `compiler_flags` for more
    information.
    :::

-   ::: {#linker_extra_outputs}
    ### `linker_extra_outputs`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#linker_extra_outputs){.inline-link}

    Declares extra outputs that the linker emits. These identifiers can
    be used in `$(output ...)` macros in `linker_flags` to interpolate
    the output path into the linker command line. Useful for custom
    linkers that emit extra output files.
    :::

-   ::: {#linker_flags}
    ### `linker_flags`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#linker_flags){.inline-link}

    Flags to add to the linker command line whenever the output from
    this rule is used in a link operation, such as linked into an
    executable or a shared library.
    :::

-   ::: {#exported_linker_flags}
    ### `exported_linker_flags`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#exported_linker_flags){.inline-link}

    Flags to add to the linker command line when the output from this
    rule, or the output from any rule that transitively depends on this
    rule, is used in a link operation.
    :::

-   ::: {#exported_platform_linker_flags}
    ### `exported_platform_linker_flags`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#exported_platform_linker_flags){.inline-link}

    Platform-specific linker flags for this rule and for all rules that
    transitively depend on this rule. This argument is specified as a
    list of pairs where the first element in each pair is an un-anchored
    regex against which the platform name is matched. The regex should
    use `java.util.regex.Pattern` syntax. The second element in each
    pair is a list of linker flags. If the regex matches the platform,
    these flags are added to the linker command line when the output
    from this rule, or the output from any rule that transitively
    depends on this rule, is used in a link operation.
    :::

-   ::: {#target_sdk_version}
    ### `target_sdk_version`{.argName} [(defaults to `None`)]{.argDefault} [\#](#target_sdk_version){.inline-link}

    The minimum OS version that the library target should support,
    overriding the minimum set in`.buckconfig`. When set, Buck will
    automatically add flags to both Objective-C and Swift compilation
    that will allow the use of the new APIs without guarding code inside
    availability checks.
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

-   ::: {#link_style}
    ### `link_style`{.argName} [(defaults to `static`)]{.argDefault} [\#](#link_style){.inline-link}

    Determines whether to build and link this rule\'s dependencies
    statically or dynamically. Can be either `static`, `static_pic` or
    `shared`.
    :::

-   ::: {#link_whole}
    ### `link_whole`{.argName} [(defaults to `False`)]{.argDefault} [\#](#link_whole){.inline-link}

    On some platforms, the linker may choose to drop objects from
    libraries if it determines they may be unused. This parameter causes
    the linker to always include the entire library in top-level
    executables or shared libraries.
    :::

-   ::: {#reexport_all_header_dependencies}
    ### `reexport_all_header_dependencies`{.argName} [(defaults to `True`)]{.argDefault} [\#](#reexport_all_header_dependencies){.inline-link}

    Whether to automatically re-export the exported headers of all
    dependencies.

    When this is set to false, only exported headers from
    `exported_deps` are re-exported.
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

-   ::: {#tests}
    ### `tests`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#tests){.inline-link}

    List of [build targets](/concept/build_target.html) that identify
    the test rules that exercise this target. Note that non
    [`apple_test`](/rule/apple_test.html) targets will not be included
    in generated projects due to Xcode\'s limitations but will still
    work with [`buck test`](/command/test.html).
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
apple_library(
  name = 'MyLibrary',
  deps = [
    ':OtherLibrary',
    '//Libraries:YetAnotherLibrary',
  ],
  preprocessor_flags = ['-fobjc-arc'],
  headers = [
    'MyHeader.h',
  ],
  srcs = [
    'MySource.m',
    'MySource.swift',
  ],
  frameworks = [
    '$SDKROOT/System/Library/Frameworks/UIKit.framework',
    '$SDKROOT/System/Library/Frameworks/Foundation.framework',
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