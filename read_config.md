/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.read_config} /\*\*\*/ {template .soyweb} {call buck.page} {param
title: \'read_config()\' /} {param navid: \'function_read_config\' /}
{param prettify: true /} {param description} The read_config() function
is used to read `.buckconfig` settings. {/param} {param content} {call
buck.function} {param status: \'UNFROZEN\' /} {param overview} The
`read_config()` function is used to read `.buckconfig` {sp}settings from
within a build file. {/param} {param args} {call buck.functionArg}
{param name : \'section\' /} {param desc} The first argument is the name
of the `.buckconfig` section with the desired value. {/param} {/call}
{call buck.functionArg} {param name : \'field\' /} {param desc} The
second argument is the name of the `.buckconfig` field with the desired
value. {/param} {/call} {call buck.functionArg} {param name :
\'default\' /} {param default : \'None\' /} {param desc} The third
argument is a value to return if the desired value is not set in the
`.buckconfig`. {/param} {/call} {/param} {param examples} Use
`read_config()` to define a custom config setting to enable address
sanitizer: {literal}

``` {.prettyprint .lang-py}
cflags = []

sanitizer = read_config('cxx', 'sanitizer')
if sanitizer == 'address':
    cflags.append('-fsanitize=address')

cxx_binary(
  name = 'example',
  # ...
  compiler_flags = cflags,
)
```

{/literal} {/param} {/call} // buck.function {/param} // content {/call}
{/template}
