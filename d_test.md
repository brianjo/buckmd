/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace d_test}
/\*\*\*/ {template .soyweb} {call buck.page} {param title: \'d_test()\'
/} {param navid: \'rule_d\_test\' /} {param prettify: true /} {param
description} A rule that is used to define a set of python files that
contian tests to run via D\'s unit testing support. {/param} {param
content} {call buck.rule} {param status: \'UNFROZEN\' /} {param
overview} A `d_test()` rule is used to define a set of D source files
that contain tests to run via D\'s unittest support. The source code of
the test must provide a main() function. {/param} {param args} {call
buck.name_arg /} {call d_common.srcs_arg /} {call buck.arg} {param name:
\'labels\' /} {param default: \'\[\]\' /} {param desc} A list of labels
to be applied to these tests. These labels are arbitrary text strings
and have no meaning within buck itself. They can, however, have meaning
for you as a test author (e.g., `smoke` or `fast`). A label can be used
to filter or include a specific `d_test()` rule when executing
[`buck   test`](%7BROOT%7Dcommand/test.html). {/param} {/call} {call
buck.test_rule_timeout_ms /} {call d_common.deps_arg /} {call
test_common.contacts_arg /} {/param} // close args {param examples}
{literal}

``` {.prettyprint .lang-py}
# A rule that builds and runs D test with a single source file.
d_test(
  name = 'test',
  srcs = [
    'test.d',
  ],
)
```

{/literal} {/param} {/call} // close buck.rule {/param} {/call}
{/template}
