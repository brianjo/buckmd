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
# Build Rule

::: overview
A *build rule* is a procedure for producing output files from a set of
input files in the context of a specified build configuration. Build
rules are specified in [build
file](/concept/build_file.html)s---typically named BUCK.

**Note:** A build rule must explicitly specify, in its arguments, all of
its required inputs in order for Buck to be able to build the rule\'s
output in a way that is deterministic and reproducible.

## Buck\'s collection of build rules

Buck comes with a collection of built-in build rules for many common
build procedures. For example, compiling Java code against the Android
SDK is a common procedure, so Buck provides the build rule
[`android_library`](/rule/android_library.html) to do that. Similarly,
the final product of most Android development is an APK, so you can use
the build rule [`android_binary`](/rule/android_binary.html) to create
an APK.

This documentation organizes Buck\'s build rules by development language
and by target platform. Examples are: **C++**, **Java**, **Python**
(development languages) and **Android**, **iOS**, **.NET** (target
platforms). Consult the table of contents to locate the build rules that
are appropriate for your development project.

You can view a list of Buck\'s build rules from the command line with
the command:

    buck audit ruletypes

You can view the arguments supported by a particular rule with the
command:

    buck audit ruletype <rule>

Note that the first of these commands uses the *plural* `ruletypes`, and
the second uses the *singular* `ruletype`. For more information, see the
[`buck audit`](/command/audit.html) documentation.

## Source files as inputs to build rules

Most build rules specify source files as inputs. For example, a
[`cxx_library`](/rule/cxx_library.html) rule would specify `.cpp` files
as inputs. To support specifying these files, a `cxx_library` rule
provides the `srcs` argument. Some languages, such as C++, use header
files as well. To specify these, `cxx_library` provides a `headers`
argument.

In addition to `srcs` and `headers`, some rules provide variants of
these arguments, such as `platform_srcs` and `platform_headers`. These
arguments support groups of source files that should be used as inputs
only when building for specific platforms. For more information, see the
descriptions for `platform_srcs` and `platform_headers` in, for example,
the [`cxx_library`](/rule/cxx_library.html) topic.

### Package boundaries and access to source files

In Buck, a BUCK file defines a *package*, which corresponds *roughly* to
the directory that contains the BUCK file and those subdirectories that
do not themselves contain BUCK files. (To learn more, see the [Key
Concepts](/about/overview.html) topic.)

A rule in a BUCK file cannot specify a source file as an input unless
that source file is in that BUCK file\'s package. An exception to this
restriction exists for header files, but only if a rule in the package
that contains the header file *exports* that header file using the
`exported_headers` argument. For more details, see the description for
`exported_headers` in, for example, the
[`cxx_library`](/rule/cxx_library.html) topic.

More commonly though, the package for a BUCK file contains all the
source files required for the rules defined in that BUCK file.
Functionality in source files from other packages is made available
through the artifacts produced by the rules in the BUCK files for those
packages. For example, a [`cxx_binary`](/rule/cxx_binary.html) might use
the functionality in a `cxx_library` that is defined in another package.
To access that functionality, the `cxx_binary` would take that
`cxx_library` as a *dependency*.

##### Symlinks: Use with caution if at all

We recommend that you do *not* use symlinks---either absolute or
relative---to specify input files to build rules. Although using
symlinks in this context does sometimes work, it can lead to unexpected
behavior and errors.

## Dependencies: Output from one rule as input to another rule

A build rule can use the output from another build rule as one of its
inputs by specifying that rule as a *dependency*. Typically, a build
rule specifies its dependencies as a list of [build
target](/concept/build_target.html)s in its `deps` argument. However,
the rule can also specify dependencies---as build targets---in other
arguments, such as `srcs`.

**Example:** The output of a [`java_library`](/rule/java_library.html)
rule is a JAR file. If a `java_library` rule specifies another
`java_library` rule as a dependency, the JAR file produced by the
specified rule is added to the classpath for the `java_library` that
depends on it.

**Example:** If a [`java_binary`](/rule/java_binary.html) rule specifies
a `java_library` rule as a dependency, the JAR file for the specified
`java_library` is available on the classpath for the `java_binary`. In
addition, in the case of `java_binary`, the JAR files for any
dependencies of the `java_library` rule *are also* made available to the
`java_binary` rule---and if those dependencies have dependencies of
their own, they are added as well. This exhaustive cascade of
dependencies is referred to as the rule\'s *transitive closure*.

### Required dependencies are always built first

Buck guarantees that any dependencies that a rule lists that are
required in order to build that rule are built successfully *before*
Buck builds the rule itself. Note though that there can be special
cases---such as [`apple_bundle`](/rule/apple_bundle.html)---where a
rule\'s listed dependencies do not actually need to be built before the
rule.

### Visibility

In order for a build rule to take a dependency on another build rule,
the build rule on which the dependency is taken must be *visible* to the
build rule taking the dependency. A build rule\'s `visibility` argument
is a list of [build target pattern](/concept/build_target_pattern.html)s
that specify the rules that can take that rule as a dependency. For more
information about the concept of visibility in Buck, see the
[Visibility](/concept/Visibility.html) topic.

### Dependencies define a graph

Build rules and their dependencies define a directed acyclic graph
(DAG). Buck requires this graph to be acyclic to make it possible to
build independent subgraphs in parallel.

## How to handle special cases: genrules and macros

Although Buck provides a rich set of built-in build rules for
developers, it is not able to address all possible needs. As an \"escape
hatch,\" Buck provides a category of generic build rules called
*genrules*. With genrules, you can perform arbitrary operations using
shell scripts. The genrules supported by Buck are:

-   [`genrule`](/rule/genrule.html)
-   [`apk_genrule`](/rule/apk_genrule.html)
-   [`cxx_genrule`](/rule/cxx_genrule.html)

### Multiple output files with genrules

In most cases, a build rule produces exactly one output file. However,
with genrules, you can specify an output *directory* and write arbitrary
files to that directory.

### Macros

Finally, note that you can define functions that generate build rules.
In general, this should not be something that you need to do, but taking
advantage of this option might help you add needed functionality to
Buck\'s without editing its source code. For more details, see the
[Custom Macros](/extending/macros.html) topic.
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
