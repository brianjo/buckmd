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
# Rule Keys

::: overview
Buck works on top of build dependency graphs to decide what commands to
run and what order to execute them in. The picture in this page depicts
the last graph used by Buck during a build. This graph is called the
\"Action Graph\" and each node is referred to as a BuildRule.

![Example Action Graph](/static/action_graph.png){#action_graph
style="float: right; margin: 0px 0px 20px 20px;" width="300px"}

RuleKeys are used to encapsulate all of the factors which may contribute
to the output of a BuildRule into a single value - a hashcode. If any
RuleKey of a BuildRule has not changed, the output of that BuildRule
cannot have changed.

The goal of the RuleKeys is to help buck minimise the amount of
BuildRules that need to be built locally on each buck run. The artifacts
stored in the buck caches (both HTTP and dircache) are unsurprisingly
keyed off these RuleKeys as well.

## Common Rule Key Computations[\#](#common_computations){.inline-link} {#common_computations style="clear: right"}

There are different RuleKey types, each allowing for different
optimizations.

All RuleKeys are hashes of some information. The following base set of
information is included in all RuleKeys:

-   **Target type** (e.g. java_library) - this defines the actual
    computation that will produces the output of the BuildRule, such as
    what processes are executed.
-   **Buck version** - the internal implementation details of what a
    BuildRule means may change across Buck versions.
-   **Target name and package** (e.g. //example:foo) - this is used in
    things like generated output file names.
-   **The buck-out directory relative to the root of the Buck
    project** - this is used in input and output paths.

Certain other information is also recorded on a per-target-type basis,
e.g. environment variables which may affect the output, toolchain
versions, etc. Each different RuleKey type will then add extra
information to the hash. The RuleKey types Buck currently supports are:

## Rule Key Types[\#](#rule_key_types){.inline-link} {#rule_key_types style="clear: right"}

There are 4 types of Rule Keys in buck:

1.  [Input Based Rule Keys](#input_based_rule_keys)
2.  [Default Rule Keys](#default_rule_keys)
3.  [ABI Rule Keys](#abi_rule_keys)
4.  [Dependency File RuleKey (or \"Manifest
    RuleKey\")](#manifest_based_rule_keys)

### Input Based Rule Keys[\#](#input_based_rule_keys){.inline-link} {#input_based_rule_keys}

These are the simplest RuleKeys to reason about. They are always
applicable in all situations. Unfortunately, they require the
dependencies of the BuildRule to have already been built. This RuleKey
adds the following information to the hash:

-   The relative path to, and contents of, each direct input file to the
    BuildRule (typically, the value of the srcs attribute).
-   The relative path to, and contents of, each output file of each
    direct dependency of the BuildRule (typically, the output files of
    the values of the deps attribute).

**Example:** Let\'s say buck is building BuildRule #2 from the example
Action Graph. The input based rule key for this node will be generated
out of the combined hashes of all srcs defined in #2 with the hashes of
the outputs of BuildRules #4 and #5.

### Default Rule Keys[\#](#default_rule_keys){.inline-link} {#default_rule_keys}

These allow a RuleKey to be computed which is always applicable, without
needing to actually build the BuildRule\'s dependencies. This optimises
for builds which have high cache hit rates, as it allows Buck to
optimistically check caches from the top of our dependency graph,
iterating down until it gets a hit, and then only execute the BuildRules
which missed the cache, rather than needing to fetch cache hits (or
execute BuildRules) all the way from the bottom of the graph. This
RuleKey adds the following information to the hash:

-   The relative path to, and contents of, each direct input file to the
    BuildRule (typically, the value of the srcs attribute).
-   The default RuleKey value for each direct dependency of the
    BuildRule (typically, the default RuleKeys of the BuildRules which
    are the values of the deps attribute. Some rules may also have
    dependencies other than those listed in deps, such as on compiler
    toolchains).

**Example:** Once more taking as an example BuildRule #2, in order to
compute its rule key buck will compute the hash of its direct srcs
dependencies and combine that with the default rule keys of #4 and #5.
Notice recursive nature of this process, as the default rule key for #4
can only be calculated off the computation of the default rule key for
#7.

### ABI Rule Keys[\#](#abi_rule_keys){.inline-link} {#abi_rule_keys}

In some cases, only part of the output of a BuildRule is used by the
things which depend on it. For example, a java_library rule does not
need to be rebuilt in the case that one of its dependencies changes if
the public interface of the dependency didn\'t change. This knowledge
can be used to avoid spurious rebuilds, where it is known that the
output will be the same.

Note, though, that this RuleKey is not necessarily transitively
applicable - in the Java example, the java_binary which eventually
depends on the java_library *will* still need to be re-packaged to pick
up the changes which occurred in its transitive dependencies. It is
important to only apply ABI RuleKeys where they are applicable. This
RuleKey adds the following information to the hash:

-   The relative path to, and contents of, each direct input file to the
    BuildRule (typically, the value of the srcs attribute).
-   A representation of the ABI (e.g. Java public interface) of each
    direct dependency of the BuildRule (typically, of the values of the
    deps attribute).

Not all BuildRule types support ABI RuleKeys.

**Example:** Let\'s use again BuildRule #2 as an example. In order to
compute the ABI Rule Key, buck will compute the hashcode of #2\'s direct
source dependencies (srcs) and will combine that with the ABI
representation of the output of BuildRules #4 and #5.

### Dependency File RuleKey (or \"Manifest RuleKey\")[\#](#manifest_based_rule_keys){.inline-link} {#manifest_based_rule_keys}

In some cases, the listed input files to a BuildRule are an
over-approximation of the things which actually affect compilation.

For example, a cxx_library rule may list some header files which are not
actually used by all of the source files it compiles. In this case,
spurious recompiles of those source files can be avoided if they are not
affected by the changed header file. The knowledge about which headers
are depended on is only known after compilation has occurred, so there
is a bootstrapping build (or cache hit) which is required before this
RuleKey can be used. This over-approximation could be avoided, but for
the sake of usability we allow this, and introduce optimizations to
avoid re-executing BuildRules in this case.

To compute this RuleKey, two additional lists are required;

1.  A list of files which are conditional inputs (e.g. for a
    cxx_library, the list of header files)
2.  A list of the conditional input files which were actually used in
    the most recent BuildRule execution

Note that this RuleKey is only applicable where the conditionality of
the usage of any particular input could not have changed since these
lists were constructed (e.g. for a cxx_library, if no #include
statements were added, removed, modified, or re-ordered, and no header
files were added or removed to the target). This RuleKey adds the
following information to the hash:

-   The relative path to, and contents of, each direct input file to the
    BuildRule which is not in the conditional input files list (i.e.
    which is an unconditional input).
-   The relative path to, and contents of, each direct input file to the
    BuildRule which was in the list of conditional input files which
    were actually used.

Note that Dependency File RuleKeys are not currently implemented in such
a way as to take any other dependencies into account; all dependencies
are assumed to be expressed in the above information.

Not all BuildRule types support Dependency File RuleKeys.
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
