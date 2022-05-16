/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
filegroup} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'filegroup()\' /} {param navid: \'rule_filegroup\' /} {param prettify:
true /} {param description} A rule that provides access to a set of
files. {/param} {param content} {call buck.rule} {param status:
\'FROZEN\' /} {param overview}

This rule provides access to a set of files.

Files are accessible to {call buck.genrule /}s by using their relative
path after a `$(location)` string parameter macro. Other rules may
handle `filegroup()` rules natively for attributes such as resources.

{/param} {param args} {call buck.name_arg /} {call buck.arg} {param
name: \'srcs\' /} {param desc} The set of files to include in this rule.
{/param} {/call} {/param} {param examples}

In this example a target exports `.xml` files from all subdirectories in
`resources`.

{literal}

``` {.prettyprint .lang-py}
filegroup(
  name = 'example',
  srcs = glob(['resources/**/*.xml']),
)

genrule(
  name = 'process_xml',
  out = 'processed.xml',
  cmd = '$(exe //example:tool) -in $(location :example)/resources/file.xml > $OUT',
)
```

{/literal} {/param} {/call} {/param} {/call} {/template}
