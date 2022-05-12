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
# Adding Custom Rules to Buck

::: overview
As of the writing of this document, the only official way to add rules
to Buck is to fork the project and modify the source. We will, at some
point, construct a beautiful and elegant extensions API. Until then,
you\'ll want to have the documentation of our internal [API](/javadoc/)
handy, and then\...

Start by editing `KnownBuildRuleTypes`. You\'ll need to edit
`createBuilder()` and find the block where there are a large number of
calls to `builder.register()`.

``` {.prettyprint .lang-java}
builder.register(new YourDescription());
```

What is `YourDescription`? It\'s an implementation of the
[`Description`](https://buck.build/javadoc/com/facebook/buck/core/description/Description.html)
interface. This interface serves three roles in Buck:

1.  It provides the name for the rule type, eg. `java_library`
2.  It makes clear the parameters which are accepted by a rule
3.  It acts as a factory of
    [`BuildRule`](https://buck.build/javadoc/com/facebook/buck/rules/BuildRule.html)
    instances.

### Defining Rule Parameters

This is done by implementing
`Description.createUnpopulatedConstructorArg()`. This should return a
java object, the public fields of which are the camelCased names of the
parameters used by the rule in BUCK files. When referenced in BUCK
files, the field name is snake_cased. That is \"someParam\" would become
\"some_param\".

You may use primitives, enums, generic types, collections (including
generic collections), and custom types for the fields of the constructor
arg. If you are using a custom type which Buck does not know how to
marshal from JSON, then you must implement a
[`TypeCoercer`](https://buck.build/javadoc/com/facebook/buck/rules/coercer/TypeCoercer.html).
How to do this is beyond the scope of this doc.

Note: if a parameter might either be a local file or an output of a
`BuildRule`, then you can use a
[`SourcePath`](https://buck.build/javadoc/com/facebook/buck/rules/SourcePath.html)to
represent that parameter.

If a parmater is considered to be optional, then the field should be
declared using Guava\'s `Optional` class (eg.
`public Optional<String> name;`)

### Constructing new BuildRule instances

When Buck needs to construct a `BuildRule` it will call
`Description.createBuildRule()`, passing in a populated constructor arg.
Collection types on that arg will have been instantiated with an empty
collection, even if they are declared as being optional.

The `createBuildRule` method is responsible for returning an
instantiated `BuildRule` that can be used to construct whatever it is
that we\'re adding this build rule for. The current instances typically
inherit from
[`AbstractBuildRule`](https://buck.build/javadoc/com/facebook/buck/rules/AbstractBuildRule.html),
and we suggest you do so too.

The created `BuildRule` will be registered with the `BuildRuleResolver`
automatically. There are, however, plenty of cases where a `BuildRule`
will want to depend on existing functionality that\'s already expressed
as a `BuildRule`. In this case, it\'s fine to create that intermediate
rule in the `createBuildRule()` method, add it to the resolver, and then
add that newly created rule as a dependency of the one ultimately
returned from the method. The only caveat: each rule must have its own,
unique, `BuildTarget`, which is the name by which it\'s referred to in
the action graph.

You are strongly encouraged to delay doing any work in your `BuildRule`
until the `getBuildSteps()` method. In particular, don\'t do any work
other than assigning fields in the constructor! The exception to this is
working out the path to the output of your rule.

You can think of a `Description` as a factory of `BuildRule` instances.
Similarly, you can think of a `BuildRule` as a factory of
[`Step`s](https://buck.build/javadoc/com/facebook/buck/step/Step.html)
that must be executed in order to create a specific output. Unlike
rules, steps are executed sequentially in the order in which they are
returned.

### Ensuring Your Rule Is Rebuilt Correctly

If your rule extends `AbstractBuildRule`, then it\'s enough to simply
annotate any field on that rule that contributes to its uniqueness with
[`@AddToRuleKey`](https://buck.build/javadoc/com/facebook/buck/rules/AddToRuleKey.html).
This is used by Buck to calculate the rule key, which, if the value
changes between builds, will cause Buck to re-execute your `BuildRule`.

Another tip for ensuring your rule rebuilds correctly between builds is
to ensure that the output directory is cleaned each time. Commonly,
you\'ll see the first steps of a rule are something like:

``` {.prettyprint .lang-java}
Path outputDir = BuildTargets.getGenPath(target, "%s-output"); steps.add(new MakeCleanDirectoryStep(outputDir));
```

In your IDE, take a look at the key interfaces and classes to discover
more about what you can do within Buck:

-   [`Description`](https://buck.build/javadoc/com/facebook/buck/rules/Description.html)
-   [`AbstractBuildRule`](https://buck.build/javadoc/com/facebook/buck/rules/AbstractBuildRule.html)
-   [`Step`](https://buck.build/javadoc/com/facebook/buck/step/Step.html)
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
