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
# String Parameter Macros

::: overview
[This is liable to change in the future.]{.small}

Some rules allow the use of specialized macros embedded within the
strings of their parameters. These *string parameter macros* provide
additional functionality, such as exposing the output paths of other
rules.

Rules that support string parameter macros are:

-   [`genrule`](/rule/genrule.html)
-   [`apk_genrule`](/rule/apk_genrule.html)
-   [`cxx_genrule`](/rule/cxx_genrule.html)
-   [`command_alias`](/rule/command_alias.html)

Note that [`cxx_genrule`](/rule/cxx_genrule.html) and
[`command_alias`](/rule/command_alias.html) support only the
`$(exe ...)` and `$(location ...)` macros.

### Format

String parameter macros have the form

    $([@]macroname [ argument ... ])

String parameter macros take a space-separated list of arguments, where
each argument is a [build target
pattern](/concept/build_target_pattern.html).

Note that the `$(query_* ...)` macros require a fully-qualified [build
target](/concept/build_target.html) and do not support build target
patterns.

### How to manage long expanded values

In some cases, the results of the expanded macro might be so long that
they exceed a limit in your operating environment. For example, if you
use the results of an expanded macro in Bash, it could exceed Bash\'s
command-line limits.

To work around these limits, prefix the macro name with the `@`
character. Buck then writes the results of the expanded macro to a
temporary file and replaces the macro with the path to that file *while
keeping the `@` prefix*. For example

    $(@query_targets_and_outputs //...)

expands to something similar to

    @/tmp/tempfile

Many applications recognize the `@` prefix to mean: *read the contents
of this file to obtain the necessary arguments*.

### How to prevent expansion

If you need to prevent expansion of a string parameter macro, prefix the
macro with a backslash.

    \$(dirname ...)

For an example of preventing expansion in the context of a rule, see the
**Examples** section below.

## Supported macros

-   ` $(classpath //:foo) `expands to the set of JARs that are in the
    classpath of the given target.
-   `  $(classpath_abi //:foo)  `expands to the set of Application
    Binary Interface (ABI) JARs that are in the classpath of the given
    target. For more information about using ABI JARs with Buck, see the
    topic [Java ABIs](/concept/java_abis.html).
-   ` $(exe //:foo) `expands to the executable output of the given
    target---if the target produces such an executable.
-   ` $(location //:foo) `expands to the output file or directory of the
    given target.
-   ` $(location //:foo[output]) `expands to the named output file or
    directory of the given target, for rules that expose supplementary
    outputs.
-   ` $(maven_coords //:foo) `expands to the maven coordinates
    associated with the given target.
-   ` $(output name) `expands to the path of the named output of the
    rule in which you use this macro. Used only for rules that allow
    named supplementary outputs.
-   ` $(query_targets "queryfunction(//:foo)") `executes the given query
    and expands to the list of targets that match. See the **Query
    functions** section below for the list of supported
    *queryfunction*s.
-   ` $(query_outputs "queryfunction(//:foo)") `executes the given query
    and expands to the *output files* of the targets that match. See the
    **Query functions** section below for the list of supported
    *queryfunction*s.
-   ` $(query_targets_and_outputs [SEPARATOR] "queryfunction(//:foo)") `executes
    the given query and expands to both the target names *and* the
    output files of the targets that match. Targets and paths are
    separated by *SEPARATOR* if provided, or a space if it is not. See
    the **Query functions** section below for the list of supported
    *queryfunction*s.

### Query functions

The `query_*` macros accept a quoted query expression which supports the
following query functions.

-   `attrfilter`
-   `attrregexfilter`
-   `classpath`
-   `deps`
-   `except (set-difference)`
-   `filter`
-   `intersect`
-   `kind`
-   `rdeps`
-   `set`
-   `union`

All of these except for `classpath` behave the same as the corresponding
operations in [`buck query`](/command/query.html).

The `classpath` query function is used to query the classpath of
`java_library` rules. It takes an optional second argument to limit the
depth of the traversal. Its behavior is similar to the corresponding
operation in [`buck audit`](/command/audit.html).

The items in the preceding list link to the corresponding descriptions
in the `buck query` and `buck audit` topics.

## Examples

**Example**: Use a string parameter macro in a `genrule()` to copy the
output of another rule.

    genrule(
      name = 'gen',
      out  = 'out.txt',
      cmd  = 'cp $(location //some/other:rule) $OUT',
    )

**Example**: Use a backslash to prevent macro expansion. The rule passes
the `dirname` command to the shell to execute in a subshell; `dirname`
is a Unix/Linux command-line utility that returns the directory of a
specified file. We need to use an escape because the syntax for
subshells is the same as the syntax for string parameter macros.

``` {.prettyprint .lang-py}
genrule(
  name = 'gen',
  out  = 'out.txt',
  cmd  = 'cp $SRCS \$(dirname $OUT)',
  srcs = [
    'test1.txt',
    'test2.txt',
  ],
)
```

**Example**: Query macro

The following example adds an `apk_genrule` to the BUCK file that is
used in the [cross-platform Buck
sample](https://github.com/fbsamples/bucksamples) from GitHub. The
genrule, `string_param`, writes the transitive closure of dependencies
for the android_binary rule, `demo-app`, to the file `deps.txt`.

    android_binary(
      name = 'demo-app',
      manifest = 'AndroidManifest.xml',
      keystore = '//android/keystores:debug',
      deps = [
        '//android/java/com/facebook/buck/demo:lib',
      ],
    )

    apk_genrule(
      name = 'string_param',
      apk  = ':demo-app',
      srcs = [ '//android/java/com/facebook/buck/demo:lib' ],
      cmd = 'mkdir $OUT; echo deps: $(query_targets deps(//android:demo-app)) > $OUT/deps.txt',
      out = 'out-dir'
    )

## Frequently Asked Questions (FAQ)

-   **When are macros evaluated?** Macros are evaluated before the
    command is passed to the shell for execution. You can think of them
    as simple string replacements.
-   **Can macros be nested?** Macros cannot be nested. If you need to
    run an additional macro on the output of a previous macro, create a
    nested `genrule` definition and use the `$(location)` macro to read
    the output of the previous macro.
-   **Are parentheses okay inside a macro?** Inside a macro, parentheses
    must be balanced. Parentheses which are part of a quoted string are
    ignored.
-   **Is white space okay inside a macro?** Macro arguments are white
    space separated, so arguments which contain white space must be
    quoted.
-   **Are nested quotes allowed?** A single level of nested quotes is
    allowed, such as `"My name is 'Buck'."` or `'My name is "Buck".'`).
    Note that when you use a macro in a BUCK file, you must ensure that
    quotes are properly escaped, so that the shell command that uses the
    macro forms a proper string.

## Extended Backus---Naur form

The Extended Backus---Naur form (EBNF) grammar for a macro is as
follows:

    macro = "$(", macro_name, whitespace, [arg_list], ")";
    macro_name = {all_ascii_chars - whitespace - parens};
    whitespace = "\t" | "\n" | " " | "\r";
    parens = "(" | ")";
    arg_list = arg | arg, whitespace, arg_list;
    arg = {all_ascii_chars - whitespace - parens}
          | "(", arg, ")"
          | "\"", [{-"\""}], "\""
          | "'", [{-"'"}], "'";
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
