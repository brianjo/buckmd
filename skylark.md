/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.skylark} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'Skylark\' /} {param navid: \'concept_skylark\' /} {param description}
An overview of the Skylark language and its usage. {/param} {param
content}

## A bit of history

Historically, Buck relied on a Python DSL to describe {call
buck.build_file /}s and {call buck.macros/}. This enabled Buck users to
implement many features without having to modify Buck\'s core. Although
Python worked fine for local builds and small repositories, when used at
scale, the ability to access the host environment and perform arbitrary
actions without Buck\'s knowledge led to non-deterministic builds,
hard-to-debug issues, and slow parsing.

To address some of these issues, we introduced features such as {call
buck.function_link}{param name: \'allow_unsafe_import\' /}{/call}, but
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
key to the {call buckconfig.parser /} section in your `.buckconfig`
file.

    {literal}
    [parser]
      default_build_file_syntax = SKYLARK
    {/literal}

We recommend Skylark for new projects and it will become the default in
the future. However, if most of your {call buck.build_file/}s or {call
buck.macros/} rely on Python DSL features and you\'re not ready to
invest in migrating to Skylark, replace

    {literal}
    default_build_file_syntax = SKYLARK 
    {/literal}

with

    {literal}
    default_build_file_syntax = PYTHON_DSL 
    {/literal}

to use the Python DSL parser by default.

If your project includes build files that rely on legacy Python DSL
features, you can enable *multi-language* support by setting {sp}{call
buckconfig.parser_polyglot_parsing_enabled /}{sp} to `true` in {call
buck.buckconfig_link /} file and use the file-specific parser directives
described below.

We recommend that you migrate Skylark as soon as possible. To make that
easier, Buck gives you control over which parser it uses for individual
{call buck.build_file/}s. If you add

    {literal}
    # BUILD FILE SYNTAX: SKYLARK 
    {/literal}

as the first line of a {call buck.build_file/}, Buck uses the Skylark
parser. If instead, you add

    {literal}
    # BUILD FILE SYNTAX: PYTHON_DSL
    {/literal}

then Buck uses the Python DSL parser.

If neither of these lines is present, Buck uses the parser specified in
the {call buckconfig.parser /} section of `.buckconfig`.

Because Skylark will eventually become the default, it\'s best to enable
the Skylark parser globally in `.buckconfig` and add

    {literal}
    # BUILD FILE SYNTAX: PYTHON_DSL 
    {/literal}

to any {call buck.build_file/}s that continue to rely on Python DSL
features.

**Note:** The `# BUILD FILE SYNTAX:` parser directive is recognized in
build files only if support for multi-language (polyglot) parsing is
enabled in `.buckconfig`:

    {literal}
    [parser]
      polyglot_parsing_enabled = true
    {/literal}

## Migrating from Python to Skylark

The
[Skylark](https://docs.bazel.build/versions/master/skylark/language.html)
language was specifically created to address the issues mentioned
previously---as well as other issues---which is why Skylark will
eventually replace the Python DSL as the language for {call
buck.build_file/}s and extension files. Unfortunately, migration cannot
be fully automated, so here we describe some ways to resolve common
issues when migrating from the Python DSL to Skylark.

### Like Python, but\...

As Skylark is a subset of Python, there are several features that have
been removed. For features that have been removed like top level
conditionals, unbounded loops, and others, there are design
justifications available in the [specification\'s
repository](https://github.com/bazelbuild/starlark/blob/master/design.md).

### include_defs

The {call buck.function_link}{param name: \'include_defs\' /}{/call}
function is not supported in Skylark because it can contaminate the
symbol table of the execution environment and make automated refactoring
more difficult.

To replace an invocation such as

    {literal}
    include_defs("//tools/my_macro.bzl") 
    {/literal}

you should:

1.  find all symbols defined in the `my_macro.bzl` file that are
    *actually used* by the including file, say, for example, `foo` and
    `bar`.

2.  replace the `include_defs` invocation with an equivalent {call
    buck.function_link}{param name: \'load\' /}{/call} invocation that
    *explicitly* imports the needed symbols:

        {literal}
        load("//tools:my_macro.bzl", "foo", "bar")
        {/literal}

**Note:** The {call buck.function_link}{param name: \'load\' /}{/call}
function uses the {call buck.build_target_pattern /} syntax as though

    export_file(name="my_macro.bzl")

were defined in a `tools` package {call buck.build_file/}. This means
that instead of using the `//package/extension.bzl` syntax expected by
{call buck.fn_include_defs/}, you should use the
`//package:extension.bzl` syntax expected by {call buck.fn_load/}.

### Environment variables

For Skylark, replace environment variables with equivalent configuration
variables. The implicit nature of environment variables frequently
results in non-reproducible builds because of differences in the values
of environment variables across machines.

For example, in your {call buck.build_file/} or extension file, instead
of

    my_var = py_sdk.os.env.get('MY_VAR', 'foo')

use

    my_var = read_config('my_project', 'my_var', 'foo')

Then, when calling Buck, instead of passing

    {literal}
    export MY_VAR='some_value' 
    buck <args>
    {/literal}

pass a configuration flag

    {literal}
    buck <args> --config my_project.my_var=foo
    {/literal}

or better yet, define these configuration values in your {call
buck.buckconfig_link /} file.

**Note:** When using the Python DSL parser it\'s possible to invoke the
{call buck.fn_read_config/} function directly during extension-file
evaluation or indirectly through other function invocations. Indirect
invocation of {call buck.fn_read_config/} is not supported with the
Skylark parser in order to track the use of configuration options more
precisely. Because of this, a top-level invocation of {call
buck.fn_read_config/} such as:

    {literal}
    bar = read_config(<args>)
    {/literal}

either has to be performed in a {call buck.build_file/} directly or,
preferably, moved into a descriptively-named function within an
extension file. In the case where configuration options are used to
instantiate expensive objects which should be created only once,
consider replacing a top-level invocation such as

    {literal}
    FOO = expensive1() if read_config(<args>) else expensive2() 
    {/literal}

with something like

    {literal}
    _EXPENSIVE1 = expensive1()
    _EXPENSIVE2 = expensive2()

    def foo():
      return _EXPENSIVE1 if read_config(<args>) else _EXPENSIVE2
    {/literal}

While it can result in the instantiation of an unnecessary and expensive
object, it might still be more efficient than instantiating one of the
expensive objects during each `foo` invocation. Having said that, we
recommend that you start simply and optimize only if you notice
performance issues.

### isinstance()

The `isinstance()` function is not available in Skylark because Skylark
does not support inheritance. However, some usages of `isinstance()` can
be replaced with the `type` function. For example,

    {literal}
    isinstance(foo, str)
    {/literal}

can be replaced with

    {literal}
    type(foo) == type('str')
    {/literal}

### get_base_path

In Skylark, we\'ve replaced the {call buck.fn_get_base_path /} function
with the equivalent---but more appropriately
named---[package_name()](https://docs.bazel.build/versions/master/skylark/lib/native.html#package_name)
function. Note that in {call buck.build_file /}s, it\'s invoked as
`package_name()`, but in extension files, it\'s invoked as
`native.package_name()`. Using the `native` prefix is consistent with
the rest of the built-in functions provided by Buck. If there is a
strong desire to use the old name instead, you can assign the new
function to the legacy function name:

    {literal}
    get_base_path = native.package_name
    get_base_path()
    {/literal}

### del

Usage of `del arr[1]` and `del dictionary['key']` are not supported.
Instead, use

    {literal}
    arr_val  = arr.pop(1) 
    dict_val = dictionary.pop('key')
    {/literal}

### class

Classes are not supported. Replace classes with a combination of structs
and functions. In addition to being simpler, structs are more [memory
efficient](http://blog.explainmydata.com/2012/07/expensive-lessons-in-python-performance.html).
For example, a class such as

    {literal}
    class Foo:
    def __init__(self, foo, bar=None):
    ...
    def some_method(self, param):
    ...
    ...
    foo = Foo('foo', bar='yo')
    res = foo.some_method(some_param)
    {/literal}

can be replaced with something such as

    {literal}
    def some_function(foo_instance, param):
    ...
    foo = struct(foo='foo', bar='yo')
    res = some_function(foo, some_param)
    {/literal}

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

    {literal}
    re"//libraries/my_lib/.*"
    {/literal}

with

    {literal}
    startswith("//libraries/my_lib/")
    {/literal}

##### Example: Match characters at the beginning of a string

Replace

    {literal}
    re".*/my_lib/"
    {/literal}

with

    {literal}
    endswith("/my_lib/")
    {/literal}

##### Example: Match characters at both the beginning and end of a string

Replace

    {literal}
    re".*some_text.*"
    {/literal}

with

    {literal}
    "some_text" in foo
    {/literal}

### raise Exception

Raising and catching exceptions is not supported. Instead, use the
[`fail`](https://docs.bazel.build/versions/master/skylark/lib/globals.html#fail)
function to stop the evaluation of a build or extension file, and report
an error.

For example, instead of

    {literal}
    raise Exception("foo")
    {/literal}

use

    {literal}
    fail("foo") 
    {/literal}

Instead of

    {literal}
    raise Exception("attribute_name: foo")
    {/literal}

use

    {literal}
    fail("foo", "attribute_name") 
    {/literal}

Since usage of `fail` triggers non-recoverable errors and halts parsing,
it cannot be used for control flow.

### while loop

While loops are not supported due to unbounded runtime. Instead, use a
`for` loop with a bounded range. Usage of

    {literal}
    while True: ... 
    {/literal}

should be replaced with

    {literal}
    for _ in range(<reasonable limit>): 
    {/literal}

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

    {literal}
    [repositories]
      bazel_skylib = path/to/skylib_checkout
    {/literal}

to your `.buckconfig` file.

Load the functions that you need, using {call buck.function_link}{param
name: \'load\' /}{/call}. For example,

    {literal}
    load("@bazel_skylib//lib:paths.bzl", "paths").
    {/literal}

Here is an example from the Skylib website:

    {literal}
    load("@bazel_skylib//:lib.bzl", "paths", "shell")

    p = paths.basename("foo.bar")
    s = shell.quote(p)
    {/literal}

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

    {literal}
    buck targets --show-rulekey //path/to/targets/... > before
    {/literal}

After making your changes, run the command again, redirecting to a
different file.

    {literal}
    buck targets --show-rulekey //path/to/targets/... > after
    {/literal}

Now that you have captured the before and after rule keys, use the
following command to compare them:

    {literal}
    diff before after
    {/literal}

There should be no differences unless your changes affected the
semantics of some of the build definitions or macros. In order to get
more insight into what exactly has changed, you can use the command

    {literal}
    buck audit rules path/to/BUCK command
    {/literal}

on individual {call buck.build_file /}s to see how Buck expanded the
macros in them.

{/param} {/call} {/template}
