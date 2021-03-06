/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.load} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'load()\' /} {param navid: \'function_load\' /} {param prettify: true
/} {param description} The load() function is used to include
definitions (macros and constants) from another file. {/param} {param
content} {call buck.function} {param status: \'FROZEN\' /} {param
overview} The {call buck.fn_load/} function is used to include
definitions ({call buck.macros/} and constants) from another file.

The {call buck.fn_load/} function executes a file of build-file-style
code in the context of the current build file, so code in the included
file may reference Buck functions, such as {call buck.java_library/},
{call buck.java_test/}, etc., as well as {call buck.fn_load/} itself!

The motivation behind {call buck.fn_load/} is to avoid copy-and-pasting
code across multiple build files. Often, loaded files will contain data
declarations (as shown in the example below) or definitions of macros
for creating more complex build rules. {/param} {param args} {call
buck.arg} {param name: \'label\' /} {param desc} The label identifying
file containing {call buck.macros/} and constants. It\'s exactly the
same as build target syntax but all macro files are assumed to be
implicitly exported using `buck.export_file` with its original name, so
a macro file `defs` from `package` directory is accessible using
`//package:defs` syntax. {/param} {/call} {call buck.arg} {param name:
\'\*\*symbols\' /} {param desc} Names of macros and constants to import
from `path`. In {call buck.fn_load/} function keyword arguments have
special meaning and can be used to change names of imported symbols. For
example, `load("//tools/build_rules:build_defs", my_rule="some_rule")`
will export{sp} `some_rule` from `build_defs` and make it available
under the name{sp} `my_rule`. This can be useful to avoid name
collisions with local definitions. {/param} {/call} {/param} {param
examples} Suppose the file `core/DEFS` contains the following: {literal}

``` {.prettyprint .lang-py}
JARS_TO_EXCLUDE_FROM_DX = [
  'third_party/guava/guava-14.0.1.jar',
  'third_party/jackson/jackson-core-2.9.7.jar',
  'third_party/jackson/jackson-databind-2.9.7.jar',
  'third_party/jackson/jackson-datatype-guava-2.9.7.jar',
]
```

{/literal} Then another build file could include the array using
{sp}`load()`. This eliminates the need to copy-and-paste definitions
across build files: {literal}

``` {.prettyprint .lang-py}
load('//core:DEFS', 'JARS_TO_EXCLUDE_FROM_DX')

android_binary(
  name = 'example',
  # ...
  no_dx = JARS_TO_EXCLUDE_FROM_DX,
)
```

{/literal} Alternatively, to make an imported symbol available under a
different name, keywords can be used instead: {literal}

``` {.prettyprint .lang-py}
load('//core:DEFS', no_dx='JARS_TO_EXCLUDE_FROM_DX')

android_binary(
  name = 'example',
  # ...
  no_dx = no_dx,
)
```

{/literal} {/param} {/call} // buck.function {/param} // content {/call}
{/template}
