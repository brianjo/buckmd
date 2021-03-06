/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
go_test} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'go_test()\' /} {param navid: \'rule_go_test\' /} {param prettify: true
/} {param description} A go_test rule builds a Go library from the
specified sources and resources, then runs it as a \"testing\" package
test. {/param} {param content} {call buck.rule} {param status:
\'UNFROZEN\' /} {param overview}

A `go_test()` rule builds a native binary from the specified Go source
and resource files---and a generated main file. It\'s similar to the
`go test` command.

If your test requires static files you should specify these in the
**resources** argument. If you do not specify these files, they won\'t
be available when your test runs.

{call go_common.supported_language_version /}

{/param} {param args} {call buck.name_arg /} {call go_common.srcs_arg /}
{call buck.arg} {param name: \'library\' /} {param default: \'None\' /}
{param desc} Specify the library that this internal test is testing.
This will copy the `srcs`, {sp}`package_name` and `deps` from the target
specified so you don\'t have to duplicate them. {/param} {/call} {call
buck.arg} {param name : \'package_name\' /} {param default :
\'go.prefix + path relative to the buck root + \"\_test\"\' /} {param
desc} Sets the full name of the test package being compiled. This
defaults to the path from the buck root with \"\_test\" appended. (e.g.
given a ./.buckconfig, a rule in ./a/b/BUCK defaults to package
\"a/b_test\")

Note: if you want to test packages internally (i.e. same package name),
use the `library` {sp}parameter instead of setting `package_name` to
include the tested source files.

{/param} {/call} {call buck.arg} {param name : \'coverage_mode\' /}
{param default : \'None\' /} {param desc} Test coverage functionality
will be included in the executable. Modes: set, count, atomic {/param}
{/call} {call go_common.deps_arg /} {call go_common.link_style_arg /}
{call go_common.link_mode_arg /} {call go_common.compiler_flags_arg /}
{call go_common.assembler_flags_arg /} {call go_common.linker_flags_arg
/} {call go_common.external_linker_flags_arg /} {call buck.arg} {param
name: \'resources\' /} {param default : \'\[\]\' /} {param desc} Static
files that are symlinked into the working directory of the test. You can
access these files in your test by opening them using relative paths,
such as `ioutil.ReadFile("testdata/input")`. {/param} {/call} {call
buck.test_label_arg /} {call buck.test_rule_timeout_ms /} {call
buck.arg} {param name: \'env\' /} {{param default : \'{}\' /}} {param
desc} A map of environment variables and values to set when running the
test. {/param} {/call} {call buck.run_test_separately_arg /} {call
test_common.contacts_arg /} {/param} // close args {param examples}
{call go_common.more_examples /} {literal}

``` {.prettyprint .lang-py}
go_library(
  name='greeting',
  srcs=[
    'greeting.go',
  ],
  deps=[
    ':join',
  ],
)

go_test(
  name='greeting-test',
  srcs=[
    'greeting_ext_test.go',
  ],
  deps=[
    ':greeting'
  ],
)

go_test(
  name='greeting-internal-test',
  package_name='greeting',
  srcs=[
    'greeting.go',
    'greeting_test.go',
  ],
  deps=[
    ':join',
  ],
)

# Or

go_test(
  name='greeting-better-internal-test',
  srcs=['greeting_test.go'],
  library=':greeting',
)
```

{/literal} {/param} {/call} // close buck.rule {/param} {/call}
{/template}
