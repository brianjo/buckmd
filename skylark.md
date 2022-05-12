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
# Skylark

::: overview
## A bit of history

Historically, Buck relied on a Python DSL to describe [build
file](/concept/build_file.html)s and [macros](/extending/macros.html).
This enabled Buck users to implement many features without having to
modify Buck\'s core. Although Python worked fine for local builds and
small repositories, when used at scale, the ability to access the host
environment and perform arbitrary actions without Buck\'s knowledge led
to non-deterministic builds, hard-to-debug issues, and slow parsing.

To address some of these issues, we introduced features such as
[`allow_unsafe_import()`](/function/allow_unsafe_import.html), but
ultimately we were unable to provide proper sandboxing for deterministic
parsing, and a new solution had to be put in place.

## Present day

In order to tackle the limitations of the Python DSL parser, we added
multiple-language support and a built-in parser for the
[Skylark](https://docs.bazel.build/versions/master/skylark/language.html)
language. The new parser provides an alternative to the Python DSL
parser.

## Enabling the Skylark parser

In order to enable Skylark support for your project, add the following
key to the [`[parser]`](/files-and-dirs/buckconfig.html#parser) section
in your`.buckconfig` file.

    [parser]
      default_build_file_syntax = SKYLARK

We recommend Skylark for new projects and it will become the default in
the future. However, if most of your [build
file](/concept/build_file.html)s or [macros](/extending/macros.html)
rely on Python DSL features and you\'re not ready to invest in migrating
to Skylark, replace

    default_build_file_syntax = SKYLARK 

with

    default_build_file_syntax = PYTHON_DSL 

to use the Python DSL parser by default.

If your project includes build files that rely on legacy Python DSL
features, you can enable *multi-language* support by setting
[`[parser].polyglot_parsing_enabled`](/files-and-dirs/buckconfig.html#parser.polyglot_parsing_enabled)
to `true` in [`.buckconfig`](/files-and-dirs/buckconfig.html) file and
use the file-specific parser directives described below.

We recommend that you migrate Skylark as soon as possible. To make that
easier, Buck gives you control over which parser it uses for individual
[build file](/concept/build_file.html)s. If you add

    # BUILD FILE SYNTAX: SKYLARK 

as the first line of a [build file](/concept/build_file.html), Buck uses
the Skylark parser. If instead, you add

    # BUILD FILE SYNTAX: PYTHON_DSL

then Buck uses the Python DSL parser.

If neither of these lines is present, Buck uses the parser specified in
the [`[parser]`](/files-and-dirs/buckconfig.html#parser) section of
`.buckconfig`.

Because Skylark will eventually become the default, it\'s best to enable
the Skylark parser globally in `.buckconfig` and add

    # BUILD FILE SYNTAX: PYTHON_DSL 

to any [build file](/concept/build_file.html)s that continue to rely on
Python DSL features.

**Note:** The `# BUILD FILE SYNTAX:` parser directive is recognized in
build files only if support for multi-language (polyglot) parsing is
enabled in `.buckconfig`:

    [parser]
      polyglot_parsing_enabled = true

## Migrating from Python to Skylark

The
[Skylark](https://docs.bazel.build/versions/master/skylark/language.html)
language was specifically created to address the issues mentioned
previously---as well as other issues---which is why Skylark will
eventually replace the Python DSL as the language for [build
file](/concept/build_file.html)s and extension files. Unfortunately,
migration cannot be fully automated, so here we describe some ways to
resolve common issues when migrating from the Python DSL to Skylark.

### Like Python, but\...

As Skylark is a subset of Python, there are several features that have
been removed. For features that have been removed like top level
conditionals, unbounded loops, and others, there are design
justifications available in the [specification\'s
repository](https://github.com/bazelbuild/starlark/blob/master/design.md).

### include_defs

The [`include_defs()`](/function/include_defs.html) function is not
supported in Skylark because it can contaminate the symbol table of the
execution environment and make automated refactoring more difficult.

To replace an invocation such as

    include_defs("//tools/my_macro.bzl") 

you should:

1.  find all symbols defined in the `my_macro.bzl` file that are
    *actually used* by the including file, say, for example, `foo` and
    `bar`.

2.  replace the `include_defs` invocation with an equivalent
    [`load()`](/function/load.html)invocation that *explicitly* imports
    the needed symbols:

        load("//tools:my_macro.bzl", "foo", "bar")

**Note:** The [`load()`](/function/load.html) function uses the [build
target pattern](/concept/build_target_pattern.html) syntax as though

    export_file(name="my_macro.bzl")

were defined in a `tools` package [build
file](/concept/build_file.html). This means that instead of using the
`//package/extension.bzl` syntax expected by
[`include_defs()`](/function/include_defs.html), you should use the
`//package:extension.bzl` syntax expected by
[`load()`](/function/load.html).

### Environment variables

For Skylark, replace environment variables with equivalent configuration
variables. The implicit nature of environment variables frequently
results in non-reproducible builds because of differences in the values
of environment variables across machines.

For example, in your [build file](/concept/build_file.html) or extension
file, instead of

    my_var = py_sdk.os.env.get('MY_VAR', 'foo')

use

    my_var = read_config('my_project', 'my_var', 'foo')

Then, when calling Buck, instead of passing

    export MY_VAR='some_value' 
    buck <args>

pass a configuration flag

    buck <args> --config my_project.my_var=foo

or better yet, define these configuration values in your
[`.buckconfig`](/files-and-dirs/buckconfig.html) file.

**Note:** When using the Python DSL parser it\'s possible to invoke the
[`read_config()`](/function/read_config.html) function directly during
extension-file evaluation or indirectly through other function
invocations. Indirect invocation of
[`read_config()`](/function/read_config.html) is not supported with the
Skylark parser in order to track the use of configuration options more
precisely. Because of this, a top-level invocation of
[`read_config()`](/function/read_config.html) such as:

    bar = read_config(<args>)

either has to be performed in a [build file](/concept/build_file.html)
directly or, preferably, moved into a descriptively-named function
within an extension file. In the case where configuration options are
used to instantiate expensive objects which should be created only once,
consider replacing a top-level invocation such as

    FOO = expensive1() if read_config(<args>) else expensive2() 

with something like

    _EXPENSIVE1 = expensive1()
    _EXPENSIVE2 = expensive2()

    def foo():
      return _EXPENSIVE1 if read_config(<args>) else _EXPENSIVE2

While it can result in the instantiation of an unnecessary and expensive
object, it might still be more efficient than instantiating one of the
expensive objects during each`foo` invocation. Having said that, we
recommend that you start simply and optimize only if you notice
performance issues.

### isinstance()

The `isinstance()` function is not available in Skylark because Skylark
does not support inheritance. However, some usages of `isinstance()` can
be replaced with the `type` function. For example,

    isinstance(foo, str)

can be replaced with

    type(foo) == type('str')

### get_base_path

In Skylark, we\'ve replaced the
[`get_base_path()`](/function/get_base_path.html)function with the
equivalent---but more appropriately
named---[package_name()](https://docs.bazel.build/versions/master/skylark/lib/native.html#package_name)
function. Note that in [build file](/concept/build_file.html)s, it\'s
invoked as `package_name()`, but in extension files, it\'s invoked as
`native.package_name()`. Using the `native` prefix is consistent with
the rest of the built-in functions provided by Buck. If there is a
strong desire to use the old name instead, you can assign the new
function to the legacy function name:

    get_base_path = native.package_name
    get_base_path()

### del

Usage of `del arr[1]` and `del dictionary['key']` are not supported.
Instead, use

    arr_val  = arr.pop(1) 
    dict_val = dictionary.pop('key')

### class

Classes are not supported. Replace classes with a combination of structs
and functions. In addition to being simpler, structs are more [memory
efficient](http://blog.explainmydata.com/2012/07/expensive-lessons-in-python-performance.html).
For example, a class such as

    class Foo:
    def __init__(self, foo, bar=None):
    ...
    def some_method(self, param):
    ...
    ...
    foo = Foo('foo', bar='yo')
    res = foo.some_method(some_param)

can be replaced with something such as

    def some_function(foo_instance, param):
    ...
    foo = struct(foo='foo', bar='yo')
    res = some_function(foo, some_param)

You can also track state in variables defined in the same extension
file, but you cannot expose any mutators, since all variables are
immutable once the extension file is evaluated. This is intentional and
prevents race conditions because build files as well as extension files
must support efficient parallel evaluation.

### Regular expressions (import re)

Regular expressions are not supported in Skylark due to unbounded
runtime and resource usage, but often regular expressions can be
replaced with string functions.

##### Example: Match characters at the end of a string

Replace

    re"//libraries/my_lib/.*"

with

    startswith("//libraries/my_lib/")

##### Example: Match characters at the beginning of a string

Replace

    re".*/my_lib/"

with

    endswith("/my_lib/")

##### Example: Match characters at both the beginning and end of a string

Replace

    re".*some_text.*"

with

    "some_text" in foo

### raise Exception

Raising and catching exceptions is not supported. Instead, use the
[`fail`](https://docs.bazel.build/versions/master/skylark/lib/globals.html#fail)
function to stop the evaluation of a build or extension file, and report
an error.

For example, instead of

    raise Exception("foo")

use

    fail("foo") 

Instead of

    raise Exception("attribute_name: foo")

use

    fail("foo", "attribute_name") 

Since usage of `fail` triggers non-recoverable errors and halts parsing,
it cannot be used for control flow.

### while loop

While loops are not supported due to unbounded runtime. Instead, use a
`for` loop with a bounded range. Usage of

    while True: ... 

should be replaced with

    for _ in range(<reasonable limit>): 

followed by an extra check after the loop to make sure the loop
terminated before all the iterations were exhausted.

### python module

Python modules cannot be imported in Skylark. However, you can replace
many safe Python functions with analogous functions from
[Skylib](https://github.com/bazelbuild/bazel-skylib). For example, you
can replace `os.path.basepath` with `paths.basename`, and you can
replace `os.path.join` with `paths.join`.

In order to use Skylib, clone its repository from GitHub into a local
directory. Then, configure that repository as a Buck cell by adding

    [repositories]
      bazel_skylib = path/to/skylib_checkout

to your `.buckconfig` file.

Load the functions that you need, using [`load()`](/function/load.html).
For example,

    load("@bazel_skylib//lib:paths.bzl", "paths").

Here is an example from the Skylib website:

    load("@bazel_skylib//:lib.bzl", "paths", "shell")

    p = paths.basename("foo.bar")
    s = shell.quote(p)

### Skylint

Consider running the
[Skylint](https://github.com/bazelbuild/bazel/blob/master/site/docs/skylark/skylint.md)
linting tool on your extension (`.bzl`) files. Skylint can catch many
common issues and suggest fixes. Unfortunately, some constructs in
Python can cause Skylint to crash. Some examples are:

-   Nested functions. Nested functions should be moved to top-level
    scope.
-   Usage of `not foo in`. You should instead use `foo not in`. Note
    that `foo not in` is recommended by the
    [flake8](http://flake8.pycqa.org/en/latest/) style-enforcement tool.

When debugging an issue, an effective strategy is to bisect your code by
commenting out parts of the file and rerunning Skylint.

### Testing your changes

The easiest way to verify that your changes have not affected your build
rules is by checking if the corresponding rule keys have changed. Before
making your changes, capture rule keys with the following command:

    buck targets --show-rulekey //path/to/targets/... > before

After making your changes, run the command again, redirecting to a
different file.

    buck targets --show-rulekey //path/to/targets/... > after

Now that you have captured the before and after rule keys, use the
following command to compare them:

    diff before after

There should be no differences unless your changes affected the
semantics of some of the build definitions or macros. In order to get
more insight into what exactly has changed, you can use the command

    buck audit rules path/to/BUCK command

on individual [build file](/concept/build_file.html)s to see how Buck
expanded the macros in them.
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
