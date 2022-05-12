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
# buck audit

::: overview
Provide information about build configuration parameters, targets, and
rules.

Syntax:

    buck audit <command> [ <parameter> . . . ] <target>  . . .

Example:

    buck audit input //java/com/example/app:amazing

For more examples, see the command descriptions and **Examples** section
below.

## Commands

-   `alias --list`

    List the aliases declared in
    [`.buckconfig`](/files-and-dirs/buckconfig.html) and
    `.buckconfig.local`. This command lists only the aliases, not their
    values. To see the values, use the `buck audit config` command.

-   `buck audit cell`

    List the absolute paths to the cells that are specified in the
    [`[repositories]`](/files-and-dirs/buckconfig.html#repositories)
    section of the `.buckconfig` file that is in the root of the current
    cell. The path to each cell is prefixed with the specified alias for
    that cell. For example:

        $ buck audit cell 
        buck: /Users/buxster/local/buck
        bazel_skylib: /Users/buxster/local/buck/third-party/skylark/bazel-skylib

    (In this example, `buxster` is the name of the current user.)

    If you specify the `--paths-only` parameter, Buck outputs only the
    absolute paths to the cells, without the aliases.

        $ buck audit cell --paths-only
        /Users/buxster/local/buck
        /Users/buxster/local/buck/third-party/skylark/bazel-skylib

    If your `.buckconfig` does not contain a `[repositories]` section,
    then `buck audit cell` doesn\'t return any output.

-   `classpath <targets>`

    List the Java classpath used to run the specified targets. This does
    not work for all build rule types.

-   `config {<section> | <section.property>} [...]`

    List the values from `.buckconfig` (and `.buckconfig.local`) for the
    specified sections and properties.

    If you specify only the section name, `buck audit config` lists all
    the properties and values for that section.

    Note that properties and values specified with
    [`--config`](/command/common_parameters.html) are not surfaced by
    this command, and those properties and values override both
    `.buckconfig` and `.buckconfig.local`.

    Use `--tab` to get tab-delimited output.

    Example: To get the C compiler and the C++ compiler, use

    ``` {.prettyprint .lang-py}
    buck audit config cxx.cc cxx.cxx
    ```

    ``` {.prettyprint .lang-py}
    [cxx]
        cc = /usr/bin/gcc
        cxx = /usr/bin/g++
    ```

    or (with `--tab`)

    ``` {.prettyprint .lang-py}
    buck audit config --tab cxx.cc cxx.cxx
    ```

    ``` {.prettyprint .lang-py}
    cxx.cc	/usr/bin/gcc
    cxx.cxx	/usr/bin/g++
    ```

-   `dependencies <targets>`

    List the dependencies used to build the specified targets. Results
    are listed in alphabetical order. By default, only direct
    dependencies are listed; to show transitive dependencies, use the
    `--transitive` parameter. To show tests for a rule, use the
    `--include-tests` parameter. This prints out a rule\'s tests as if
    they were dependencies of the rule. To print out all of the
    *test\'s* dependencies as well, combine `--include-tests` with the
    `--transitive` parameter.

-   `flavors <targets>`

    List the flavors that are available for the specified targets and
    what the default flavor is for each target. If the `flavors` command
    prints `no flavors`, it indicates that, although the target rule
    supports flavors, Buck was not able to extract any. If the `flavors`
    command prints `unknown`, it indicates that the target rule doesn\'t
    support flavors. The `flavors` command supports the `--json`
    parameter for JSON-formatted output.

-   `input <targets>`

    List the input source and resource files used to build the specified
    targets.

-   `includes <build_file>`

    List the [build file](/concept/build_file.html)s, and their
    extensions, that are included in the specified build file.

-   `modules`

    List the Java modules known by Buck as well as their content hashes
    and dependencies.

-   `ruletype <rule>`

    Print the Python signature for the specified rule.

    The following command line uses `buck audit ruletype` to view the
    arguments supported by the [`remote_file`](/rule/remote_file.html)
    rule.

        buck audit ruletype remote_file

        def remote_file (
            name,
            sha1,
            url,
            labels = None,
            licenses = None,
            out = None,
            type = None,
        ):
            ...

-   `ruletypes`

    List all the rules that Buck supports, in alphabetical order.

    **Example**

    The following example prints *all* the rules that Buck supports.
    Note that the output is truncated for brevity.

        buck audit ruletypes

        android_aar
        android_app_modularity
        android_binary
        android_build_config
        android_bundle
        android_instrumentation_apk
        android_instrumentation_test
        android_library
        android_manifest
        android_prebuilt_aar
        android_resource
        apk_genrule
        apple_asset_catalog
        apple_binary
        <truncated>

    **Example**

    The following command line uses `buck audit ruletypes` with the
    `grep` command to print all the build rules that have the string
    `android` in their names.

    ``` {.prettyprint .lang-bash}
    buck audit ruletypes | grep android
    ```

    Note that these are not all the rules that Buck provides for Android
    development. For example, the rules `apk_genrule` and `ndk_library`
    support Android development, but do not themselves contain the
    string `android` in their names.

-   `tests <targets> [...]`

    List the tests for the specified targets. Results are listed in
    alphabetical order. Only tests for the specified targets are
    printed, though multiple targets may be specified on a single
    command line. This command is intended to be used in conjunction
    with the `audit dependencies` command. For example, to retrieve a
    list of all tests for a given project, use:

        buck audit dependencies --transitive PROJECT | xargs buck audit tests

## Parameters

-   `--include-tests`

    Show the tests for the specified targets. Can be combined with the
    `--transitive` parameter. For more information, see the
    `dependencies` command.

-   `--json`

    Output the results as JSON.

-   `--list`

    List `.buckconfig` and `.buckconfig.local` aliases. Used only with
    the `aliases` command. For more information, see that command.

-   `--tab`

    Output the results using tab delimiters. Used only with the `config`
    command. For more information, see that command.

-   `--transitive`

    Show transitive dependencies in addition to direct dependencies. Can
    be combined with the `--include-tests` parameter. For more
    information, see the `dependencies` command.

## Examples

``` {.prettyprint .lang-py}
#
# BUCK
#
# For all of the following examples, assume this BUCK file exists in
# the `examples` directory.
#
java_library(
  name = 'one',
  srcs = [ '1.txt' ],
  deps = [
    ':two',
    ':three',
  ],
)

java_library(
  name = 'two',
  srcs = [ '2.txt' ],
  deps = [
    ':four',
  ],
)

java_library(
  name = 'three',
  srcs = [ '3.txt' ],
  deps = [
    ':four',
    ':five',
  ],
)

java_library(
  name = 'four',
  srcs = [ '4.txt' ],
  deps = [
    ':five',
  ],
)

java_library(
  name = 'five',
  srcs = [ '5.txt' ],
)
```

List all of the source files used to build the `one` library

    buck audit input //examples:one

    examples/1.txt
    examples/2.txt
    examples/3.txt
    examples/4.txt
    examples/5.txt

Output a JSON representation of all of the source files used to build
the `two` library. In this JSON object, each key is a build target and
each value is an array of the source paths used to build that rule.

    buck audit input --json //examples:two

``` {.prettyprint .lang-js}
{
  "//examples:two": ["examples/2.txt"],
  "//examples:four": ["examples/4.txt"],
  "//examples:five": ["examples/5.txt"],
}
```

List all of the rules that the `one` library directly depends on

    buck audit dependencies //examples:one

    //examples:three
    //examples:two

List all of the rules that the `one` library transitively depends on

    buck audit dependencies --transitive //examples:one

    //examples:five
    //examples:four
    //examples:three
    //examples:two

Output a JSON representation of all of the rules that the `two` library
transitively depends on.

    buck audit dependencies --transitive --json //examples:two

``` {.prettyprint .lang-js}
{
  "//examples:two": ["//examples:five","//examples:four"]
}
```

Output a JSON representation of the direct dependencies of the `two` and
`three` libraries.

    buck audit dependencies --json //examples:two //examples:three

``` {.prettyprint .lang-js}
{
  "//examples:three": ["//examples:five","//examples:four"],
  "//examples:two": ["//examples:four"]
}
```

## See also

-   [Build File](/concept/build_file.html)
-   [`.buckconfig`](/files-and-dirs/buckconfig.html)
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
