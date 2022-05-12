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
# kotlin_library()

::: overview
[This is liable to change in the future.]{.small}

A `kotlin_library()` rule is used to define a set of Kotlin files that
can be compiled together. The main output of a `kotlin_library()` rule
is a single JAR file containing all of the compiled class files, as well
as the static files specified in the `resources` argument.

## Arguments

-   ::: {#name}
    ### `name`{.argName} [(required)]{.argDefault} [\#](#name){.inline-link}

    The *short name* for this [build
    target](/concept/build_target.html).
    :::

-   ::: {#srcs}
    ### `srcs`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#srcs){.inline-link}

    The set of `.kt`, `.java` or `.kts` files to compile for this rule.
    If any of the files in this list end in `.src.zip`, then the entries
    in the ZIP file that end in `.java` or `.kt` will be included as
    ordinary inputs to compilation.
    :::

-   ::: {#resources}
    ### `resources`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#resources){.inline-link}

    Static files to include with the compiled `.class` files. These
    files can be loaded via
    [Class.getResource()](http://docs.oracle.com/javase/7/docs/api/java/lang/Class.html#getResource(java.lang.String)){target="_blank"}.

    **Note:** If `resources_root` isn\'t set, Buck uses the
    `[java].src_roots`property in
    [`.buckconfig`](/concept/buckconfig.html) to determine where
    resources should be placed within the generated JAR file.
    :::

-   ::: {#resources_root}
    ### `resources_root`{.argName} [(defaults to `None`)]{.argDefault} [\#](#resources_root){.inline-link}

    The path that resources are resolved against. For example, if
    `resources_root` is `"res"` and `resources` contains the file
    `"res/com/example/foo.txt"`, that file will end up as
    `"com/example/foo.txt"` in the output JAR. This parameter overrides
    the `[java].src_roots` property in
    [`.buckconfig`](/concept/buckconfig.html).
    :::

-   ::: {#deps}
    ### `deps`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#deps){.inline-link}

    Rules (usually other `kotlin_library` rules) that are used to
    generate the classpath required to compile this `kotlin_library`.
    :::

-   ::: {#kotlinc_plugins}
    ### `kotlinc_plugins`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#kotlinc_plugins){.inline-link}

    Use this to specify [Kotlin compiler
    plugins](https://kotlinlang.org/docs/reference/compiler-plugins.html)
    to use when compiling this library. This takes a list of source
    paths, each of which will be prefixed with `-Xplugin=` and passed as
    extra arguments to the compiler. Unlike `free_compiler_args`, these
    can be *source paths*, not just strings (though `free_compiler_args`
    should be used to specify plugin compiler options with `-P`).

    For example, if you want to use
    [kotlinx.serialization](https://github.com/Kotlin/kotlinx.serialization)
    with `kotlin_library()`, you need to specify
    `kotlinx-serialization-compiler-plugin.jar` under `kotlinc_plugins`
    and `kotlinx-serialization-runtime.jar` (which you may have to fetch
    from Maven) in your `deps`:

    ``` {.prettyprint .lang-py}
    kotlin_library(
        name = "example",
        srcs = glob(["*.kt"]),
        deps = [
            ":kotlinx-serialization-runtime",
        ],
        kotlinc_plugins = [
            # Likely copied from your $KOTLIN_HOME directory.
            "kotlinx-serialization-compiler-plugin.jar",
        ],
    )

    prebuilt_jar(
        name = "kotlinx-serialization-runtime",
        binary_jar = ":kotlinx-serialization-runtime-0.10.0",
    )

    # Note you probably want to set
    # maven_repo=http://jcenter.bintray.com/ in your .buckconfig until
    # https://github.com/Kotlin/kotlinx.serialization/issues/64
    # is closed.
    remote_file(
        name = "kotlinx-serialization-runtime-0.10.0",
        out = "kotlinx-serialization-runtime-0.10.0.jar",
        url = "mvn:org.jetbrains.kotlinx:kotlinx-serialization-runtime:jar:0.10.0",
        sha1 = "23d777a5282c1957c7ce35946374fff0adab114c"
    )
    ```
    :::

-   ::: {#free_compiler_args}
    ### `free_compiler_args`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#free_compiler_args){.inline-link}

    A list of additional compiler arguments.
    :::

-   ::: {#all_warnings_as_errors}
    ### `all_warnings_as_errors`{.argName} [(defaults to `false`)]{.argDefault} [\#](#all_warnings_as_errors){.inline-link}

    Report an error if there are any warnings.
    :::

-   ::: {#suppress_warnings}
    ### `suppress_warnings`{.argName} [(defaults to `false`)]{.argDefault} [\#](#suppress_warnings){.inline-link}

    Generate no warnings.
    :::

-   ::: {#verbose}
    ### `verbose`{.argName} [(defaults to `false`)]{.argDefault} [\#](#verbose){.inline-link}

    Enable verbose logging output.
    :::

-   ::: {#include_runtime}
    ### `include_runtime`{.argName} [(defaults to `false`)]{.argDefault} [\#](#include_runtime){.inline-link}

    Include Kotlin runtime in to resulting .jar
    :::

-   ::: {#jvm_target}
    ### `jvm_target`{.argName} [(defaults to `1.6`)]{.argDefault} [\#](#jvm_target){.inline-link}

    Target version of the generated JVM bytecode (1.6 or 1.8), default
    is 1.6 Possible values: \"1.6\", \"1.8\"
    :::

-   ::: {#jdk_home}
    ### `jdk_home`{.argName} [(defaults to `None`)]{.argDefault} [\#](#jdk_home){.inline-link}

    Path to JDK home directory to include into classpath, if differs
    from default JAVA_HOME
    :::

-   ::: {#no_jdk}
    ### `no_jdk`{.argName} [(defaults to `false`)]{.argDefault} [\#](#no_jdk){.inline-link}

    Don\'t include Java runtime into classpath.
    :::

-   ::: {#no_stdlib}
    ### `no_stdlib`{.argName} [(defaults to `true`)]{.argDefault} [\#](#no_stdlib){.inline-link}

    Don\'t include kotlin-stdlib.jar or kotlin-reflect.jar into
    classpath.
    :::

-   ::: {#no_reflect}
    ### `no_reflect`{.argName} [(defaults to `true`)]{.argDefault} [\#](#no_reflect){.inline-link}

    Don\'t include kotlin-reflect.jar into classpath.
    :::

-   ::: {#java_parameters}
    ### `java_parameters`{.argName} [(defaults to `false`)]{.argDefault} [\#](#java_parameters){.inline-link}

    Generate metadata for Java 1.8 reflection on method parameters.
    :::

-   ::: {#api_version}
    ### `api_version`{.argName} [(defaults to `None`)]{.argDefault} [\#](#api_version){.inline-link}

    Allow to use declarations only from the specified version of bundled
    libraries. Possible values: \"1.0\", \"1.1\", \"1.2\", \"1.3\",
    \"1.4 (EXPERIMENTAL)\".
    :::

-   ::: {#language_version}
    ### `language_version`{.argName} [(defaults to `None`)]{.argDefault} [\#](#language_version){.inline-link}

    Provide source compatibility with specified language version.
    Possible values: \"1.0\", \"1.1\", \"1.2\", \"1.3\", \"1.4
    (EXPERIMENTAL)\".
    :::

-   ::: {#friend_paths}
    ### `friend_paths`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#friend_paths){.inline-link}

    List of source paths to pass into the Kotlin compiler as
    friend-paths, that is, modules you can have access to internal
    methods.
    :::

-   ::: {#annotation_processing_tool}
    ### `annotation_processing_tool`{.argName} [(defaults to `kapt`)]{.argDefault} [\#](#annotation_processing_tool){.inline-link}

    Specifies the tool to use for annotation processing. Possible
    values: \"kapt\" or \"javac\". \"kapt\" allows running Java
    annotation processors against Kotlin sources while backporting it
    for Java sources too. \"javac\" works only against Java sources,
    Kotlin sources won\'t have access to generated classes at compile
    time.
    :::

-   ::: {#kapt_ap_options}
    ### `kapt_ap_options`{.argName} [(required)]{.argDefault} [\#](#kapt_ap_options){.inline-link}

    Map of annotation processor options to pass into kapt via the
    apoptions plugin option. Each entry should be a key value pair of
    the processor option and its value. Default is an empty map. E.g.
    kapt_ap_options = { \'someAnnotationOption\': \'someValue\' } More
    information here: https://kotlinlang.org/docs/reference/kapt.html
    :::

-   ::: {#remove_classes}
    ### `remove_classes`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#remove_classes){.inline-link}

    Specifies a list of `Patterns` that are used to exclude`classes`
    from the `JAR`. The pattern matching is based on the name of the
    class. This can be used to exclude a member class or delete a local
    view of a class that will be replaced during a later stage of the
    build.
    :::

-   ::: {#exported_deps}
    ### `exported_deps`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#exported_deps){.inline-link}

    Other `kotlin_library` rules that depend on this rule will also
    include its `exported_deps` in their classpaths. This is useful when
    the public API of a rule has return types or checked exceptions that
    are defined in another rule, which would otherwise require callers
    to add an extra dependency. It\'s also useful for exposing e.g. a
    collection of `prebuilt_jar` rules as a single target for callers to
    depend on. Targets in `exported_deps` are implicitly included in the
    `deps` of this rule, so they don\'t need to be repeated there.
    :::

-   ::: {#provided_deps}
    ### `provided_deps`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#provided_deps){.inline-link}

    These represent dependencies that are known to be provided at run
    time, but are required in order for the code to compile. Examples of
    `provided_deps` include the JEE servlet APIs. When this rule is
    included in a `kotlin_library`, the `provided_deps` will not be
    packaged into the output.
    :::

-   ::: {#exported_provided_deps}
    ### `exported_provided_deps`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#exported_provided_deps){.inline-link}

    This is a combination of `provided_deps` and `exported_deps`. Rules
    listed in this parameter will be added to classpath of rules that
    depend on this rule, but they will not be included in a binary if
    binary depends on a such target.
    :::

-   ::: {#labels}
    ### `labels`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#labels){.inline-link}

    Set of arbitrary strings which allow you to annotate a [build
    rule](/concept/build_rule.html) with tags that can be searched for
    over an entire dependency tree using
    [`buck query attrfilter()`](/command/query.html#attrfilter).
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

## Examples

``` {.prettyprint .lang-py}
# A rule that compiles a single .kt file.
kotlin_library(
  name = 'JsonUtil',
  srcs = ['JsonUtil.kt'],
  deps = [
    '//third_party/guava:guava',
    '//third_party/jackson:jackson',
  ],
)

# A rule that compiles all of the .kt files under the directory in
# which the rule is defined using glob(). It also excludes an
# individual file that may have additional dependencies, so it is
# compiled by a separate rule.
kotlin_library(
  name = 'messenger',
  srcs = glob(['**/*.kt'], excludes = ['MessengerModule.kt']),
  deps = [
    '//src/com/facebook/base:base',
    '//third_party/guava:guava',
  ],
)

kotlin_library(
  name = 'MessengerModule',
  srcs = ['MessengerModule.kt'],
  deps = [
    '//src/com/facebook/base:base',
    '//src/com/google/inject:inject',
    '//third_party/guava:guava',
    '//third_party/jsr-330:jsr-330',
  ],
)

# A rule that builds a library with both relative and
# fully-qualified deps.
kotlin_library(
  name = 'testutil',
  srcs = glob(['tests/**/*.kt'], excludes = 'tests/**/*Test.kt'),
  deps = [
    ':lib-fb4a',
    '//java/com/facebook/base:base',
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
