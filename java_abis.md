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
# Java ABIs

::: overview
This topic pertains to building Java code with Buck.

When compiling a Java rule, Buck creates an *Application Binary
Interface (ABI) JAR*, which contains only resources and class
interfaces, that is, the public interface for your module. Buck creates
this ABI JAR in addition to the *library JAR*, which contains all of the
compiled classes and resources for the rule. Since ABI JARs do not
contain method bodies or private members, they are smaller and change
less frequently than library JARs, which enables Buck to use ABI JARs in
two ways:

-   Use them in [ABI rule keys](/concept/rule_keys.html#abi_rule_keys)
    to more accurately determine which rules need to be rebuilt during
    an incremental build. In some cases, only part of the output of a
    BuildRule is used by the things which depend on it. For example, a
    java_library rule does not necessarily need to be rebuilt if one of
    its dependencies changes, *provided that the public interface of
    that dependency did not change.* This knowledge can be used to avoid
    extraneous rebuilds, where it is known that the output will be the
    same.
-   Use them on the compiler\'s classpath instead of library JARs to get
    a small but significant performance boost because the smaller size
    of ABI JARs enables the compiler to load them faster than library
    JARs.

## Three Kinds of ABI JARs

Depending on the
[`[java].abi_generation_mode`](/files-and-dirs/buckconfig.html#java.abi_generation_mode)
config setting, Buck can create an ABI JAR in three ways:

-   From classes, by building the library JAR first and then stripping
    out the unnecessary bits.
-   From source, by hooking in to the compiler while it is compiling the
    library JAR and emitting the ABI JAR partway through the compilation
    process. This helps to reduce bottlenecks due to slow rules or low
    parallelism in a build graph.
-   From source *only*, by examining only the text of the source code,
    and using heuristics to infer things that can normally be determined
    only by looking at dependencies. This dramatically increases
    parallelism in the rule graph and reduces the number of cache
    fetches required during incremental builds. The next section goes
    into the requirements for these *source-only ABI JARs* in greater
    detail.

## Requirements for Source-only ABI JARs

Buck generates source-only ABI JARs using only the text of the source
code for a rule, without first compiling (most of) the rule\'s
dependencies. Some details of an ABI JAR cannot be known for certain
from just the source, so Buck uses heuristics to infer those details.
Even when using source-only ABIs, Buck still uses a rule\'s dependencies
to compile the library JAR. At that time, Buck verifies whether the
heuristics used for the ABI JAR were correct, and if they were not, Buck
fails the build with an error.

Such build failures can generally be fixed with
[`buck fix`](/command/fix.html), although sometimes these fixes are
sub-optimal. In most cases, [`buck fix`](/command/fix.html) adds\--or
suggests that you add\--either `source_only_abi_deps=[<dependencies>]`
or `required_for_source_only_abi=True`. However, we recommend that, if
possible, you avoid using `source_only_abi_deps` and
`required_for_source_only_abi`.

Both `source_only_abi_deps` and `required_for_source_only_abi` have the
potential to negatively impact build times. The list of dependencies
specified by `source_only_abi_deps` must be built before Buck can build
a source-only ABI for the current module. In the case of
`required_for_source_only_abi`, the current module must be built first
before source ABIs that depend on it can be built. Whereas
`source_only_abi_deps` affects only the current module,
`required_for_source_only_abi` affects every module that depends on the
current module.

The following points describe the requirements for source-only ABI
generation, specifically how [`buck fix`](/command/fix.html) fixes
issues, and what options you have for more optimal fixes.

-   **Place annotations and constants in their own rules:** All
    annotations and compile-time constants (including enum values) used
    in the interface of a rule must be present during source-only ABI
    generation.

    The error will suggest adding `required_for_source_abi = True` to
    any rule that defines an annotation type or a compile-time constant
    that is used from another rule, and [`buck fix`](/command/fix.html)
    will make that change. For best results, such rules should be
    manually inspected to ensure they are as small as possible\--ideally
    containing only annotations, enums, and constants\--and have as few
    dependencies as possible. In general, put annotations, enums, and
    constants in their own packages. This keeps to a minimum the amount
    of code that needs to be built before ABI generation. And because
    constants, enums, and annotations don\'t change as frequently as
    other kinds of code, those packages won\'t need to be rebuilt as
    frequently.

-   **Name packages and classes according to Java conventions:** Any
    packages that will not be available during source-only ABI
    generation must have names that begin with a lowercase letter. Any
    top-level classes that will not be available must have names that
    begin with an uppercase letter. These naming conventions are
    extremely common in Java.

    The error will suggest renaming the package or class, but *you will
    have to make this change manually*; [`buck fix`](/command/fix.html)
    will not do it for you. If the package or class name in question
    cannot be changed, add `required_for_source_abi = True` to the build
    rule that defines it.

-   **Reference member types canonically:** Any references to member
    types that will not be available during source-only ABI generation
    must be canonical. That is, although member types are inherited by
    subclasses, a canonical reference refers to the member type as a
    member of the class in which it is defined, not one that inherits
    it.

    If the defining class is accessible, the error will suggest using
    the canonical name. Otherwise, it will suggest adding
    `source_only_abi_deps` and [`buck fix`](/command/fix.html) will make
    whichever change is suggested by the error. For best results,
    consider making the defining class accessible so that the extra
    dependencies are not needed.

-   **Reference superclass member types unambiguously:** Any references
    to member types that are inherited by the current class and will not
    be available during source-only ABI generation must be at least
    partially qualified.

    The error will suggest adding an import and partially qualifying the
    name, and [`buck fix`](/command/fix.html) will make this change.

-   **Provide enough deps for the compiler to run:** Source-only ABI
    generation involves running the Java compiler front-end over a
    rule\'s code without providing most of that rule\'s dependencies,
    then working with the compiler\'s data model to generate the ABI.
    The compiler is remarkably resilient to missing dependencies, but in
    some cases a missing dependency will prevent it from getting far
    enough for Buck to generate the source-only ABI. These cases
    typically involve inheritance, where a type is available during
    source-only ABI generation, but one of its superclasses is defined
    in another rule that is not available.

    The error will suggest adding `source_only_abi_deps` to the rule so
    that the necessary dependencies will be available, and
    [`buck fix`](/command/fix.html) will make this change. For best
    results, limit the depth of class hierarchies\--which is a best
    practice for Java design in many cases\--and avoid splitting the
    class hierarchies across modules.

-   **Only single-type imports:** On-demand imports (star imports) and
    `static` imports of types cannot be resolved at source-ABI
    generation time unless the rule containing the type in question is
    available.

    The error will suggest either adding a single-type import (in the
    case of star imports) or adding `source_only_abi_deps` in the case
    of `static` imports, and [`buck fix`](/command/fix.html) will make
    that change. For best results, consider changing `static` imports of
    types to non-static imports to avoid needing to add the extra
    dependencies.
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
