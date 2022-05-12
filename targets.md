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
# buck targets

::: overview
List information about the build targets in the current project.

    buck targets <build target> | <build target pattern> ...

The `buck targets` command must take at least one parameter: a [build
target](/concept/build_target.html) or [build target
pattern](/concept/build_target_pattern.html) or a combination of these.

The following prints all build targets in the project (sorted
alphabetically) to standard out:

    buck targets //...

You can pass a list of targets to `buck targets`, and Buck prints
information only for those targets. For example, the following command
line prints the target `main` from the `BUCK` file in the root of the
Buck project and all the targets from the `BUCK` file in the
subdirectory `myclass`.

    buck targets //:main //myclass:

The `buck targets` command is commonly used with the `--show-output`
option to obtain the output paths for the build artifacts for Buck
targets.

    buck targets --show-output //java/com/myproject:binary
    > //java/com/myproject:binary buck-out/gen/java/com/myproject/binary.apk

## Parameters

-   `--type`

    The types of target by which to filter. For example:

        buck targets //java/com/myproject/... --type java_test java_binary

    Note that the `--type` parameter comes *after* the specified
    targets.

    This parameter can be handy in programmatic tasks, such as running
    all of the Java tests under `//java/com/myproject`:

        buck targets //java/com/myproject/... --type java_test | xargs buck test

-   `--referenced-file`

    Filters targets by the list of rules that include the specified file
    in their transitive closure.

    For example, to run all tests that could be affected by a particular
    file, you could use:

        buck targets //java/com/myproject/... --type java_test \
          --referenced-file java/com/example/Foo.java |
          xargs buck test

-   `--json`

    Print a JSON representation of each target.

    In addition, the JSON includes a list of `direct_dependencies` for
    each target, which may include additional dependencies for targets
    whose descriptions implement `ImplicitDepsInferringDescription`. The
    fully qualified names of targets are given.

    For example, when resolving a genrule, the direct dependencies
    includes both the build targets in `deps` as well as any build
    targets in a script associated with the genrule.

-   `--output-attributes`

    Specify the attributes used in the JSON representation.

    If you omit this option, Buck shows all attributes.

-   `--print0`

    Delimit targets using the ASCII NUL character if `--json` is not
    specified. This facilitates use with `xargs`:

        buck targets --print0 | xargs -0 buck build

-   `--resolve-alias`

    Print the fully-qualified build target for the specified
    alias\[es\]. This command also accepts build targets. For more
    information, see [`[alias]`](/files-and-dirs/buckconfig.html#alias)
    in the `.buckconfig` documentation.

-   `--show-output`

    Print the relative paths to the output for each target after the
    target name. Note that some rules---such as
    [`genrule`](/rule/genrule.html)---generate sources instead of build
    artifacts.

-   `--show-rulekey`

    Print the [rule keys](/concept/rule_keys.html), for the specified
    targets.

    For example, if you have a rule named `main` defined in the build
    file in your current directory, the following command prints its
    rule key.

        buck targets --show-rulekey ':main'

    Note that the rule key for a target is different from the *target
    hash* for that target. (See `show-target-hash` below.) Further, the
    inputs for the computation of the rule key are *not* a superset of
    the inputs for the target hash. For example, the value of the
    [visibility](/concept/Visibility.html) argument *is not* an input
    for the rule key but *is* an input for the target hash.

-   `--show-transitive-rulekeys`

    When specified in conjunction with `--show-rulekey`, prints the
    [rule keys](/concept/rule_keys.html) for the specified targets *and
    their transitive closure*.

    For example, if you have a rule named `main` defined in the build
    file in your current directory, the following command prints the
    rule key for that rule and the rule keys for all of the rules that
    are in its transitive closure.

        buck targets --show-rulekey --show-transitive-rulekeys ':main'

-   `--show-target-hash`

    Print each rule\'s target hash after the rule\'s name. Target hashes
    can be used to detect which targets are affected when source files
    in BUCK files change: if a target is affected, its target hash will
    be different after the change from what it was before.

    A target hash is created by finding all the transitive dependencies
    of the given target and hashing all their attributes and the files
    they reference. For more details about how the referenced files are
    hashed see the `--target-hash-file-mode` flag. *The format of the
    data that is hashed is undocumented and can change between Buck
    versions.*

-   `--target-hash-file-mode`

    Modify how target hashes are computed.

    Can be set to either `PATHS_AND_CONTENTS` or `PATHS_ONLY`.

    If set to `PATHS_AND_CONTENTS` (the default), the contents of all
    files referenced from the targets will be used to compute the target
    hash.

    If set to `PATHS_ONLY`, only files\' paths contribute to the hash.
    `PATHS_ONLY` will generally be faster because it does not need to
    read all of the referenced files, but it will not detect file
    changes automatically. See `--target-hash-modified-paths` for
    another way to handle changes to referenced files without losing the
    performance benefits.

-   `--target-hash-modified-paths`

    Modify how target hashes are computed.

    If a target or its dependencies reference a file from the specified
    set of paths, the target\'s hash will be different than if this
    option had been omitted. Otherwise, the target\'s hash will be the
    same as if this option was omitted.

    This option can be used to detect changes in referenced files if the
    list of modified files is available from an external source, such as
    a source control system.

    This option is effective only when `--target-hash-file-mode` is set
    to `PATHS_ONLY`. Otherwise, the actual contents of the files are
    used to detect modifications and this option is ignored.
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
