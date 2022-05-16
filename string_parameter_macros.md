/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.string_parameter_macros} /\*\*\*/ {template .soyweb} {call
buck.page} {param title: \'String Parameter Macros\' /} {param navid:
\'function_string_parameter_macros\' /} {param prettify: true /} {param
description} Parameter macros provide more expressive power to a rule\'s
string parameters. {/param} {param content} {call buck.function} {param
status: \'UNFROZEN\' /} {param overview}

Some rules allow the use of specialized macros embedded within the
strings of their parameters. These *string parameter macros* provide
additional functionality, such as exposing the output paths of other
rules.

Rules that support string parameter macros are:

-   {call buck.genrule /}
-   {call buck.apk_genrule /}
-   {call buck.cxx_genrule /}
-   {call buck.command_alias /}

Note that {call buck.cxx_genrule /} and {call buck.command_alias /}{sp}
support only the `$(exe ...)` and `$(location ...)`{sp} macros.

### Format

String parameter macros have the form

    {literal}
    $([@]macroname [ argument ... ])
    {/literal}

String parameter macros take a space-separated list of arguments, where
each argument is a {call buck.build_target_pattern /}.

Note that the `$(query_* ...)` macros require a fully-qualified {call
buck.build_target /} and do not support build target patterns.

### How to manage long expanded values

In some cases, the results of the expanded macro might be so long that
they exceed a limit in your operating environment. For example, if you
use the results of an expanded macro in Bash, it could exceed Bash\'s
command-line limits.

To work around these limits, prefix the macro name with the `@`
character. Buck then writes the results of the expanded macro to a
temporary file and replaces the macro with the path to that file *while
keeping the `@` prefix*. For example

    {literal}
    $(@query_targets_and_outputs //...)
    {/literal}

expands to something similar to

    {literal}
    @/tmp/tempfile
    {/literal}

Many applications recognize the `@` prefix to mean: *read the contents
of this file to obtain the necessary arguments*.

### How to prevent expansion

If you need to prevent expansion of a string parameter macro, prefix the
macro with a backslash.

    {literal}
    \$(dirname ...)
    {/literal}

For an example of preventing expansion in the context of a rule, see the
**Examples** section below.

## Supported macros

-   ` {literal}$(classpath //:foo){/literal} ` expands to the set of
    JARs that are in the classpath of the given target.
-   ` {literal} $(classpath_abi //:foo) {/literal} ` expands to the set
    of Application Binary Interface (ABI) JARs that are in the classpath
    of the given target. For more information about using ABI JARs with
    Buck, see the topic {call buck.concept_link}{param page:
    \'java_abis\' /}{param name: \'Java ABIs\' /}{/call}.
-   ` {literal}$(exe //:foo){/literal} ` expands to the executable
    output of the given target---if the target produces such an
    executable.
-   ` {literal}$(location //:foo){/literal} ` expands to the output file
    or directory of the given target.
-   ` {literal}$(location //:foo[output]){/literal} ` expands to the
    named output file or directory of the given target, for rules that
    expose supplementary outputs.
-   ` {literal}$(maven_coords //:foo){/literal} ` expands to the maven
    coordinates associated with the given target.
-   ` {literal}$(output name){/literal} ` expands to the path of the
    named output of the rule in which you use this macro. Used only for
    rules that allow named supplementary outputs.
-   ` {literal}$(query_targets "queryfunction(//:foo)"){/literal} `
    executes the given query and expands to the list of targets that
    match. See the **Query functions** section below for the list of
    supported *queryfunction*s.
-   ` {literal}$(query_outputs "queryfunction(//:foo)"){/literal} `
    executes the given query and expands to the *output files* of the
    targets that match. See the **Query functions** section below for
    the list of supported *queryfunction*s.
-   ` {literal}$(query_targets_and_outputs [SEPARATOR] "queryfunction(//:foo)"){/literal} `
    executes the given query and expands to both the target names *and*
    the output files of the targets that match. Targets and paths are
    separated by *SEPARATOR* if provided, or a space if it is not. See
    the **Query functions** section below for the list of supported
    *queryfunction*s.

### Query functions

The `query_*` macros accept a quoted query expression which supports the
following query functions.

-   `{call buck.cmd_link}{param name: 'query' /}{param section: 'attrfilter'/}{/call}`
-   `{call buck.cmd_link}{param name: 'query' /}{param section: 'attrregexfilter'/}{/call}`
-   `{call buck.cmd_link}{param name: 'audit' /}{param section: 'classpath'/}{/call}`
-   `{call buck.cmd_link}{param name: 'query' /}{param section: 'deps'/}{/call}`
-   `{call buck.cmd_link}{param name: 'query' /}{param section: 'set-operations'/}{param rendered_text: 'except (set-difference)' /}{/call}`
-   `{call buck.cmd_link}{param name: 'query' /}{param section: 'filter'/}{/call}`
-   `{call buck.cmd_link}{param name: 'query' /}{param section: 'set-operations'/}{param rendered_text: 'intersect' /}{/call}`
-   `{call buck.cmd_link}{param name: 'query' /}{param section: 'kind'/}{/call}`
-   `{call buck.cmd_link}{param name: 'query' /}{param section: 'rdeps'/}{/call}`
-   `{call buck.cmd_link}{param name: 'query' /}{param section: 'set'/}{/call}`
-   `{call buck.cmd_link}{param name: 'query' /}{param section: 'union'/}{/call}`

All of these except for `classpath` behave the same as the corresponding
operations in {call buck.cmd_link}{param name: \'query\' /}{/call}.

The `classpath` query function is used to query the classpath of
`java_library` rules. It takes an optional second argument to limit the
depth of the traversal. Its behavior is similar to the corresponding
operation in {call buck.cmd_link}{param name: \'audit\' /}{/call}.

The items in the preceding list link to the corresponding descriptions
in the `buck query` and `buck audit` topics.

{/param} {param examples}

**Example**: Use a string parameter macro in a `genrule()`{sp} to copy
the output of another rule.

    {literal}
    genrule(
      name = 'gen',
      out  = 'out.txt',
      cmd  = 'cp $(location //some/other:rule) $OUT',
    )
    {/literal}

**Example**: Use a backslash to prevent macro expansion. The rule passes
the `dirname` command to the shell to execute in a subshell; `dirname`
is a Unix/Linux command-line utility that returns the directory of a
specified file. We need to use an escape because the syntax for
subshells is the same as the syntax for string parameter macros.

``` {.prettyprint .lang-py}
{literal}
genrule(
  name = 'gen',
  out  = 'out.txt',
  cmd  = 'cp $SRCS \$(dirname $OUT)',
  srcs = [
    'test1.txt',
    'test2.txt',
  ],
)
{/literal}
```

**Example**: Query macro {call
buckquery.example_macro_query_targets_deps /} {/param} {param
furtherexp}

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

{literal}

    macro = "$(", macro_name, whitespace, [arg_list], ")";
    macro_name = {all_ascii_chars - whitespace - parens};
    whitespace = "\t" | "\n" | " " | "\r";
    parens = "(" | ")";
    arg_list = arg | arg, whitespace, arg_list;
    arg = {all_ascii_chars - whitespace - parens}
          | "(", arg, ")"
          | "\"", [{-"\""}], "\""
          | "'", [{-"'"}], "'";

{/literal} {/param} {/call} // buck.function {/param} // content {/call}
{/template}
