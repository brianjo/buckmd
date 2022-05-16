/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.include_defs} /\*\*\*/ {template .soyweb} {call buck.page} {param
title: \'include_defs()\' /} {param navid: \'function_include_defs\' /}
{param prettify: true /} {param description} The include_defs() function
is used to include macros and constants from another file. {/param}
{param content} {call buck.function} {param status: \'DEPRECATED\' /}
{param overview}

**NOTE:** We recommend that you do not use this function. This function
can make your builds difficult to maintain and debug, and it will be
deprecated in a future release of Buck. We recommend that you use the
[`load()`](%7BROOT%7Dfunction/load.html) function instead.

The `include_defs()` function is used to include
{sp}[`macros`](%7BROOT%7Dextending/macros.html) and constants from
another file.

The `include_defs()` function executes a file of build-file-style code
in the context of the current build file. Therefore, code in the
included file may reference Buck functions, such as
{sp}`java_library()`, `java_test()`, etc., as well as `include_defs()`
itself!

The motivation behind `include_defs()` is to avoid copy-and-pasting code
across multiple build files. Often, included files will contain data
declarations (as shown in the example below) or definitions of macros
for creating more complex build rules.

{/param} {param args} {call buck.arg} {param name: \'path\' /} {param
desc} A path, of sorts, to a file containing
{sp}[`macros`](%7BROOT%7Dextending/macros.html) and constants. It looks
similar to a build target because it starts with {sp}`//` (indicating
the root of the project), but is not a proper build target because it
identifies a file relative to the root of the project rather than a
build rule. {/param} {/call} {call buck.arg} {param name: \'namespace\'
/} {param default: \'None\' /} {param desc} A string representing a
namespace in which the bindings from the other file will be stored. When
set, an object of the given name that holds the bindings from the other
file is put into the global scope of the current file. If unset, the
bindings from the other file are injected directly into global scope of
the current file.

If the name is already in scope, it is simply overwritten. {/param}
{/call} {/param} {param examples} Suppose the file `core/DEFS` contains
the following: {literal}

``` {.prettyprint .lang-py}
JARS_TO_EXCLUDE_FROM_DX = [
  'third_party/guava/guava-14.0.1.jar',
  'third_party/jackson/jackson-core-2.9.7.jar',
  'third_party/jackson/jackson-databind-2.9.7.jar',
  'third_party/jackson/jackson-datatype-guava-2.9.7.jar',
]
```

{/literal} Then another build file could include the array using
{sp}`include_defs()`. This eliminates the need to copy-and-paste
definitions across build files: {literal}

``` {.prettyprint .lang-py}
include_defs('//core/DEFS', 'core')

android_binary(
  name = 'example',
  # ...
  no_dx = core.JARS_TO_EXCLUDE_FROM_DX,
)
```

{/literal} {/param} {/call} // buck.function {/param} // content {/call}
{/template}
