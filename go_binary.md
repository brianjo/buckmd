/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
go_binary} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'go_binary()\' /} {param navid: \'rule_go_binary\' /} {param prettify:
true /} {param description} A go_binary() rule builds a native Go
executable. {/param} {param content} {call buck.rule} {param status:
\'UNFROZEN\' /} {param overview}

A go_binary() rule builds a native executable from the supplied set of
Go source files and dependencies. The files supplied are expected to be
in the main package, implicitly.

{call go_common.supported_language_version /}

{/param} {param args} {call buck.name_arg /} {call go_common.srcs_arg /}
{call go_common.deps_arg /} {call go_common.link_style_arg /} {call
go_common.link_mode_arg /} {call go_common.compiler_flags_arg /} {call
go_common.assembler_flags_arg /} {call go_common.linker_flags_arg /}
{call go_common.external_linker_flags_arg /} {call buck.arg} {param
name: \'resources\' /} {param default : \'\[\]\' /} {param desc} Static
files to be symlinked into the working directory of the test. You can
access these in your by opening the files as relative paths, e.g.
`ioutil.ReadFile("testdata/input")`. {/param} {/call} {/param} // close
args {param examples} {call go_common.more_examples /} {literal}

``` {.prettyprint .lang-py}
go_binary(
  name='greet',
  srcs=[
    'main.go',
  ],
  deps=[
    ':greeting',
  ],
)

go_library(
  name='greeting',
  srcs=[
    'greeting.go',
  ],
  deps=[
    ':join',
  ],
)

go_library(
  name='join',
  srcs=[
    'join.go',
  ],
)
```

{/literal} {/param} {/call} // close buck.rule {/param} {/call}
{/template}
