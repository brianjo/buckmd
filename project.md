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
# buck project

::: overview
This command generates the configuration files for an IDE to work with
the project. This command creates files in-place in the repository,
which is unlike other Buck commands whose output is removed by
[`buck clean`](/command/clean.html). As a result, it is a good idea to
add these generated files to the list of ignored files by your choice of
source control. IDE-specific details are discussed in each section
below.

You can use this command by itself to generate a project for the entire
repository.

    buck project

You can also use this command to build a project slice (a project that
represents a subset of the repository). You can pass any number of
[build target](/concept/build_target.html)s or [build target
pattern](/concept/build_target_pattern.html)s to the command. The
constructed project slice will contain the specified targets and their
dependencies. This is useful for large repositories.

    buck project //java/...

## Common Parameters

-   `--ide` Specifies which IDE to create the project for. When using a
    project slice, Buck tries to determine what type of IDE to use
    automatically based on the [build
    target](/concept/build_target.html)s provided. Sometimes it is not
    possible to determine the type of IDE. You can specify the default
    ide in the `[project]` section of your `.buckconfig` file.
-   `--without-tests` Indicates that Buck should build a project slice
    without tests (the default is to include `tests` on `*_library` and
    `*_binary` rules).
-   `--without-dependencies-tests` Indicates that Buck should build a
    project slice with the tests of the specified targets only.
-   `--exclude-artifacts  ` Don\'t include references to the artifacts
    created by compiling a target in the module representing that
    target. This can improve indexing times, but will mean generated
    code does not show up in the ide. For example R files for Android.
-   `--remove-unused-ij-libraries ` After generating an IntelliJ project
    remove all IntelliJ libraries that are not used in the project.

## Supported IDEs

-   [IntelliJ](#intellij)
-   [Xcode](#xcode)
-   [gobuild (Go IDEs such as Visual Sudio Code,
    GoLand)]{hred="#gobuild"}

### IntelliJ

This command processes all of the [build
file](/concept/build_file.html)s whose targets were specified and uses
them to generate the configuration files for an IDE. The generated files
include:

-   `.idea/libraries/*.xml`, each of which defines a library in
    IntelliJ. A library always corresponds to a
    [`prebuilt_jar`](/rule/prebuilt_jar.html).
-   `.iml` files, each of which defines a module in IntelliJ. A module
    can depend on other modules, as well as libraries. It should be
    noted that although Buck allows multiple build targets per build
    file, IntelliJ\'s modules are only defined at the directory level.
    This means that you may find IntelliJ flagging compilation errors
    because of missing dependencies of classes outside of your project
    slice, but which happen to be in the same directory as classes
    within the slice.
-   `.idea/modules.xml`, which lists all of the IntelliJ modules in the
    project.

### Xcode

This command processes each [`apple_binary`](/rule/apple_binary.html),
[`apple_bundle`](/rule/apple_bundle.html), and
[`apple_library`](/rule/apple_library.html) specified, and uses them to
generate the files and directories that Xcode needs. The generated
folders include:

-   For each [build target](/concept/build_target.html), an
    `*.xcworkspace` directory that represents the
    [workspace](https://developer.apple.com/library/ios/featuredarticles/XcodeConcepts/Concept-Workspace.html)
    and contains one or more
    [schemes](https://developer.apple.com/library/ios/featuredarticles/XcodeConcepts/Concept-Schemes.html).
-   For each [build target](/concept/build_target.html) and its
    dependencies, an `*.xcodeproj` directory that represents the
    [project](https://developer.apple.com/library/ios/featuredarticles/XcodeConcepts/Concept-Projects.html).
    These generated projects are only buildable within the generated
    workspace.

#### Parameters

-   `--combined-project` Indicates that Buck should build a single
    monoproject for all [build target](/concept/build_target.html)s
    specified.
-   `--project-schemes` Enables the generation of separate schemes for
    all projects included in the generated workspace. Each project\'s
    scheme is constrained to the set of build and test targets that are
    members or deps of the associated project. You can specify the
    default value using by adding `project_schemes = true` to
    the`[project]` section of your `.buckconfig` file.

### Go IDEs {#gobuild}

Go IDEs, such as Visual Studio Code and GoLand, use the `go build`
command to build Go code. This command requires a proper layout of
source code under `GOPATH`. However, Buck puts generated code in
`buck-out`, which `go build` does not understand. The `project` command
copies generated Go packages from `buck-out` and arranges them in the
same layout as their import paths.

#### Parameters

-   `--project_path` The directory to copy the generated code to. If not
    specified, the `project` command copies it to `\/\/vendor`, or
    `\/\/src/vendor` if it exists.
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
