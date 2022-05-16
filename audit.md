/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.audit} /\*\* \* Use to format parameters of buck audit commands
with complex syntax. \* \* \@param name Name of the parameter;
noAutoescape enables more complex \* syntax for subcommands. \* \@param?
nodash If set, do not add \"\--\" prefix to \$name. \* \@param? alias
The alias for this parameter. \* \@param desc Prose description of the
parameter. \*/ {template .param}

`{if not $nodash}--{/if}{$name|noAutoescape}` {sp} {if \$alias}
`(-{$alias})` {/if} {sp} {\$desc\|noAutoescape} {/template} /\*\*\*/
{template .soyweb} {call buck.page} {param title: \'buck audit\' /}
{param navid: \'command_audit\' /} {param prettify: true /} {param
description} Provide information about the build configuration
parameters, targets, and rules. {/param} {param content} {call
buck.command} {param overview}

Provide information about build configuration parameters, targets, and
rules.

Syntax:

    buck audit <command> [ <parameter> . . . ] <target>  . . .

Example:

    buck audit input //java/com/example/app:amazing

For more examples, see the command descriptions and **Examples** section
below.

## Commands

{/param} {param params} {call buck.param} {param name: \'include-tests\'
/} {param desc}

Show the tests for the specified targets. Can be combined with the
`--transitive` parameter. For more information, see the `dependencies`
command.

{/param} {/call} {call buck.param} {param name: \'json\' /} {param desc}

Output the results as JSON.

{/param} {/call} {call buck.param} {param name: \'list\' /} {param desc}

List `.buckconfig` and `.buckconfig.local` aliases. Used only with the
`aliases` command. For more information, see that command.

{/param} {/call} {call buck.param} {param name: \'tab\' /} {param desc}

Output the results using tab delimiters. Used only with the `config`
command. For more information, see that command.

{/param} {/call} {call buck.param} {param name: \'transitive\' /} {param
desc}

Show transitive dependencies in addition to direct dependencies. Can be
combined with the `--include-tests` parameter. For more information, see
the `dependencies` command.

{/param} {/call} {/param} {param examples}

``` {.prettyprint .lang-py}
{literal}
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
{/literal}
```

List all of the source files used to build the `one` library

    {literal}
    buck audit input //examples:one
    {/literal}

    {literal}
    examples/1.txt
    examples/2.txt
    examples/3.txt
    examples/4.txt
    examples/5.txt
    {/literal}

Output a JSON representation of all of the source files used to build
the{sp} `two` library. In this JSON object, each key is a build target
and each value is an array of the source paths used to build that rule.

    {literal}
    buck audit input --json //examples:two
    {/literal}

``` {.prettyprint .lang-js}
{literal}
{
  "//examples:two": ["examples/2.txt"],
  "//examples:four": ["examples/4.txt"],
  "//examples:five": ["examples/5.txt"],
}
{/literal}
```

List all of the rules that the `one` library directly depends on

    {literal}
    buck audit dependencies //examples:one
    {/literal}

    {literal}
    //examples:three
    //examples:two
    {/literal}

List all of the rules that the `one` library transitively depends on

    {literal}
    buck audit dependencies --transitive //examples:one
    {/literal}

    {literal}
    //examples:five
    //examples:four
    //examples:three
    //examples:two
    {/literal}

Output a JSON representation of all of the rules that the `two`{sp}
library transitively depends on.

    {literal}
    buck audit dependencies --transitive --json //examples:two
    {/literal}

``` {.prettyprint .lang-js}
{literal}
{
  "//examples:two": ["//examples:five","//examples:four"]
}
{/literal}
```

Output a JSON representation of the direct dependencies of the{sp} `two`
and `three` libraries.

    {literal}
    buck audit dependencies --json //examples:two //examples:three
    {/literal}

``` {.prettyprint .lang-js}
{literal}
{
  "//examples:three": ["//examples:five","//examples:four"],
  "//examples:two": ["//examples:four"]
}
{/literal}
```

{/param} {/call}

## See also

-   {call buck.concept_link}{param page: \'build_file\' /}{param name:
    \'Build File\' /}{/call}
-   {call buck.buckconfig_link /}

{/param} // content {/call} // buck.page {/template}
