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
# android_library()

::: overview
An `android_library()` rule is used to define a set of Java files that
can be compiled together against the Android SDK. The main output of an
`android_library()` rule is a single JAR file containing all of the
compiled class files and resources.

## Arguments

-   ::: {#name}
    ### `name`{.argName} [(required)]{.argDefault} [\#](#name){.inline-link}

    The *short name* for this [build
    target](/concept/build_target.html).
    :::

-   ::: {#srcs}
    ### `srcs`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#srcs){.inline-link}

    The set of `.java` files to compile for this rule.
    :::

-   ::: {#resources}
    ### `resources`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#resources){.inline-link}

    Static files to include among the compiled `.class` files. These
    files can be loaded via
    [Class.getResource()](http://docs.oracle.com/javase/7/docs/api/java/lang/Class.html#getResource(java.lang.String)){target="_blank"}.

    **Note:** Buck uses the `src_roots` property in
    [`.buckconfig`](/concept/buckconfig.html) to help determine where
    resources should be placed within the generated JAR file.
    :::

-   ::: {#manifest}
    ### `manifest`{.argName} [(defaults to `None`)]{.argDefault} [\#](#manifest){.inline-link}

    An optional [Android
    Manifest](http://developer.android.com/guide/topics/manifest/manifest-intro.html)
    for the library to declare any permissions or intents it may need or
    want to handle. May either be a file or a
    [`android_manifest`](/rule/android_manifest.html) target.
    :::

-   ::: {#final_r_name}
    ### `final_r_name`{.argName} [(defaults to `None`)]{.argDefault} [\#](#final_r_name){.inline-link}

    An optional name for a class like R.java with final values that is
    generated to be used for annotation processors. The values will be
    wrong i.e they will not match the real values in the final android
    binary, so they should only be used by carefully crafted annotation
    processors.
    :::

-   ::: {#skip_non_union_r_dot_java}
    ### `skip_non_union_r_dot_java`{.argName} [(defaults to `false`)]{.argDefault} [\#](#skip_non_union_r_dot_java){.inline-link}

    When using `resource_union_package` setting
    `skip_non_union_r_dot_java` will skip generating dummy R.java for
    other packages which are unnecessary. Reducing the number of R.java
    helps in improving the overall compile time especially in libraries
    with large number of dependent prebuilt targets.
    :::

-   ::: {#deps}
    ### `deps`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#deps){.inline-link}

    Rules (usually other `android_library` rules) that are used to
    generate the classpath required to compile this `android_library`.
    :::

-   ::: {#source}
    ### `source`{.argName} [(defaults to `<global value>`)]{.argDefault} [\#](#source){.inline-link}

    Specifies the version of Java (as a string) to interpret source
    files as. Overrides the value in \"source_level\" in the \"java\"
    section of [`.buckconfig`](/concept/buckconfig.html).
    :::

-   ::: {#target}
    ### `target`{.argName} [(defaults to `<global value>`)]{.argDefault} [\#](#target){.inline-link}

    Specifies the version of Java (as a string) for which to generate
    code. Overrides the value in \"target_level\" in the \"java\"
    section of [`.buckconfig`](/concept/buckconfig.html).
    :::

-   ::: {#javac}
    ### `javac`{.argName} [(defaults to `<global value>`)]{.argDefault} [\#](#javac){.inline-link}

    Specifies the Java compiler program to use for this rule. The value
    is a source path (e.g., Only one of \"javac\" and \"javac_jar\" may
    be set for a given rule. Overrides the value in \"javac\" in the
    \"tools\" section of [`.buckconfig`](/concept/buckconfig.html).
    :::

-   ::: {#javac_jar}
    ### `javac_jar`{.argName} [(defaults to `<global value>`)]{.argDefault} [\#](#javac_jar){.inline-link}

    Specifies the Java compiler program to use for this rule. The value
    is a source path (e.g., Only one of \"javac_jar\" and \"javac\" may
    be set for a given rule. Overrides the value in \"javac_jar\" in the
    \"tools\" section of [`.buckconfig`](/concept/buckconfig.html).
    :::

-   ::: {#compiler_class_name}
    ### `compiler_class_name`{.argName} [(defaults to `<global value>`)]{.argDefault} [\#](#compiler_class_name){.inline-link}

    Specifies the Java compiler class name to use in tandem with
    javac_jar. Overrides the value in
    [`.buckconfig`](/concept/buckconfig.html#tools.compiler_class_name).
    :::

-   ::: {#extra_arguments}
    ### `extra_arguments`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#extra_arguments){.inline-link}

    List of additional arguments to pass into the Java compiler. These
    arguments follow the ones specified in
    [`.buckconfig`](/concept/buckconfig.html).
    :::

-   ::: {#free_compiler_args}
    ### `free_compiler_args`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#free_compiler_args){.inline-link}

    List of additional arguments to pass into the Kotlin compiler.
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

-   ::: {#exported_deps}
    ### `exported_deps`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#exported_deps){.inline-link}

    Other `android_library` rules that depend on this rule will also
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
    included in a `android_binary`, the `provided_deps` will not be
    packaged into the output.
    :::

-   ::: {#exported_provided_deps}
    ### `exported_provided_deps`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#exported_provided_deps){.inline-link}

    This is a combination of `provided_deps` and `exported_deps`. Rules
    listed in this parameter will be added to classpath of rules that
    depend on this rule, but they will not be included in a binary if
    binary depends on a such target.
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

-   ::: {#provided_deps_query}
    ### `provided_deps_query`{.argName} [(defaults to `None`)]{.argDefault} [\#](#provided_deps_query){.inline-link}

    Status: **experimental/unstable**. The provided deps query functions
    in the same way as the deps query, but the referenced deps using
    `$declared` are the provided deps of the target, and the results of
    the query are appended to the declared provided deps.
    :::

-   ::: {#abi_generation_mode}
    ### `abi_generation_mode`{.argName} [(defaults to `None`)]{.argDefault} [\#](#abi_generation_mode){.inline-link}

    Overrides
    [`[java].abi_generation_mode`](/files-and-dirs/buckconfig.html#java.abi_generation_mode)
    for this rule.
    :::

-   ::: {#source_only_abi_deps}
    ### `source_only_abi_deps`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#source_only_abi_deps){.inline-link}

    These are dependencies that must be present during [source-only ABI
    generation](/concept/java_abis.html). Typically such dependencies
    are added when some property of the code in this rule prevents
    source-only ABI generation from being correct without these
    dependencies being present.

    Having `source_only_abi_deps` prevents Buck from completely
    flattening the build graph, thus reducing the performance win from
    source-only ABI generation. They should be avoided when possible.
    Often only a small code change is needed to avoid them. For more
    information on such code changes, read about [source-only ABI
    generation](/concept/java_abis.html).
    :::

-   ::: {#required_for_source_only_abi}
    ### `required_for_source_only_abi`{.argName} [(defaults to `False`)]{.argDefault} [\#](#required_for_source_only_abi){.inline-link}

    Indicates that this rule must be present on the classpath
    during [source-only ABI generation](/concept/java_abis.html)  of any
    rule that depends on it. Typically this is done when a rule contains
    annotations, enums, constants, or interfaces.

    Having rules present on the classpath during source-only ABI
    generation prevents Buck from completely flattening the build graph,
    thus reducing the performance win from source-only ABI generation.
    These rules should be kept small (ideally just containing
    annotations, constants, enums, and interfaces) and with minimal
    dependencies of their own.
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

An `android_library` rule used in concert with an
[`android_resource`](/rule/android_resource.html) rule. This would be a
common arrangement for a standard Android Library project as defined by
<http://developer.android.com/tools/projects/index.html>

``` {.prettyprint .lang-py}
android_resource(
  name = 'res',
  res = 'res',
  package = 'com.example',
)

android_library(
  name = 'my_library',
  srcs = glob(['src/**/*.java']),
  deps = [
    ':res',
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
