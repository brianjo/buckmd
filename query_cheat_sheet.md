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
# Buck Cheat Sheet

::: overview
This section provides example command lines that you can use to obtain
information about Buck and about your build. These techniques can help
you to understand how your build works and to troubleshoot issues with
your build.

Most of these examples use the [`buck query`](/command/query.html),
[`buck targets`](/command/targets.html), and
[`buck audit`](/command/audit.html) commands. For more information and
examples, see the reference pages for those commands.

------------------------------------------------------------------------

-   [How do I get a list of all the rules that Buck supports from the
    command line?](#list-all-rules)
-   [How do I see the arguments for a given rule from the command
    line?](#list-args-for-rule)
-   [How do I find all the targets for a
    package?](#find-existing-targets)
-   [How do I specify more than one target to
    `buck query`?](#query-multiple-targets)
-   [How do I get the attribute names and values for the targets that
    result from a query?](#output-target-attributes)
-   [How do I perform a query *inside* of a rule?](#queries-in-rules)
-   [How do I find the dependencies for a target, that is, the targets
    on which a specified target depends?](#find-dependencies)
-   [How do I find the reverse-dependencies for a target, that is, the
    targets that *depend on* a specified
    target?](#find-reverse-dependencies)
-   [How do I find the build file that contains the target that owns a
    source file?](#find-buildfile-owner)

------------------------------------------------------------------------

\

::: {#list-all-rules .faq}
::: faq_q
How do I get a list of all the rules that Buck supports, *from the
command line*, so that I can process them with `grep`, `sed`, etc?
:::

::: faq_a
Use [`buck audit`](/command/audit.html) with the `ruletypes` (plural)
subcommand, which returns an alphabetized list of all the rules that
Buck supports.

The following command line uses `buck audit ruletypes` with the `grep`
command to print all the build rules that have the string `android` in
their names.

``` {.prettyprint .lang-bash}
buck audit ruletypes | grep android
```

Note that these are not all the rules that Buck provides for Android
development. For example, the rules `apk_genrule` and `ndk_library`
support Android development, but do not themselves contain the string
`android` in their names.
:::
:::

::: {#list-args-for-rule .faq}
::: faq_q
How do I see the arguments for a rule from the command line?
:::

::: faq_a
Use [`buck audit`](/command/audit.html) with the `ruletype` (singular)
subcommand followed by the name of the rule.

The following command line uses `buck audit ruletype` to view the
arguments supported by the [`remote_file`](/rule/remote_file.html) rule.

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
:::
:::

::: {#find-existing-targets .faq}
::: faq_q
How do I find all the targets for a package?
:::

::: faq_a
Specify a *build target pattern* that represents the targets in the
package.

``` {.prettyprint .lang-js}
buck query //path/to/dir/...
```

The `buck query` command can accept a [build target
pattern](/concept/build_target_pattern.html) as a parameter. If you
specify a build target pattern, Buck evaluates this pattern and shows
all the build targets that match it.
:::
:::

::: {#query-multiple-targets .faq}
::: faq_q
How do I specify more than one target to `buck query`?
:::

::: faq_a
Use the [`buck query set()`](/command/query.html#set) operator.

The following command line returns the target `main` in the build file
in the root of the Buck project and all the targets from the build file
in the `myclass` subdirectory of the root.

    buck query "set( '//:main' '//myclass:' )"
:::
:::

::: {#output-target-attributes .faq}
::: faq_q
How do I get the attribute names and values for the targets returned by
a query?
:::

::: faq_a
Add the `--output-attributes` option to the command line, followed by
regular expressions that represent the attributes of interest.

``` {.prettyprint .lang-js}
buck query "deps(//foo:bar)" --output-attributes 'name' 'exported_headers'
```

The `--output-attributes` option enables you to specify which attributes
Buck should return. Instead of returning the names of the targets that
match the query expression, Buck returns the names and values of the
specified attributes for those targets in JSON format. Attributes are
specified as regular expressions. For example, `'.*'` matches all
attributes. See the [buck query
page](/command/query.html#output-attributes) for more details. The
output for the example query above might look something like the
following.

``` {.prettyprint .lang-js}
{
  "//foo/bar/lib:lib" : {
    "exported_headers" : [ "App/util.h" ],
    "name" : "lib"
  },
  "//foo/bar:app" : {
    "exported_headers" : [ "App/lib.h" ],
    "name" : "app"
  }
}
```
:::
:::

::: {#queries-in-rules .faq}
::: faq_q
How do I perform a query *inside* of a rule?
:::

::: faq_a
Use **[string parameter
macros](/function/string_parameter_macros.html)**, specifically, the
*query* macros:

    $(query_targets "queryfunction(//:foo)")
    $(query_outputs "queryfunction(//:foo)")
    $(query_targets_and_outputs [SEPARATOR] "queryfunction(//:foo)")

Note, however, that the query macros are supported only for
[`genrule`](/rule/genrule.html) and
[`apk_genrule`](/rule/apk_genrule.html).
:::
:::

::: {#find-dependencies .faq}
::: faq_q
How do I find the dependencies for a target?
:::

::: faq_a
Use the `deps()` operator.

``` {.prettyprint .lang-js}
buck query "deps('//foo:bar')"
buck query "deps('//foo:bar', 1, first_order_deps())"
buck query "deps(set('//foo:bar' '//foo:lib' '//foo/baz:util'))"
```

The [deps](/command/query.html#deps) operator finds the dependencies of
the specified targets. The first argument represents the targets of
interest. This can be a single [build
target](/concept/build_target.html) or [build target
pattern](/concept/build_target_pattern.html), or a set of these.

The optional second argument is the *depth* of the search for
dependencies from the specified targets. For example, `1`, as shown in
the example above, returns only the direct dependencies. If you do not
provide this argument, the output is the complete set of transitive
dependencies.
:::
:::

::: {#find-reverse-dependencies .faq}
::: faq_q
How do I find the reverse-dependencies for a target, that is, the
targets that *depend on* a specified target?
:::

::: faq_a
Use the `buck query` [`rdeps`](/command/query.html#rdeps) (reverse
dependencies) operator.

The following example, returns the targets in the [transitive
closure](https://en.wikipedia.org/wiki/Transitive_closure) of
`//foo:bar` that depend directly on `//example:baz`.

    buck query "rdeps('//foo:bar', '//example:baz', 1)"
:::
:::

::: {#find-buildfile-owner .faq}
::: faq_q
How do I find the buildfile that contains the target that owns a source
file?
:::

::: faq_a
In order to find the build file associated with a source file, combine
the `owner` operator with `buildfile`. For example,

    buck query "buildfile(owner('foo/bar/main.cpp'))" 

first finds the targets that *own* `foo/bar/main.cpp` and then returns
the build files, such as `foo/bar/BUCK`, that define those targets.
:::
:::
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
