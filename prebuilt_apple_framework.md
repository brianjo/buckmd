/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
prebuilt_apple_framework} /\*\*\*/ {template .soyweb} {call buck.page}
{param title: \'prebuilt_apple_framework()\' /} {param navid:
\'rule_prebuilt_apple_framework\' /} {param prettify: true /} {param
description} A prebuilt_apple_framework() rule represents an Apple
framework that has already been compiled and exports a set of headers.
{/param} {param content} {call buck.rule} {param status: \'FROZEN\' /}
{param overview} A `prebuilt_apple_framework()` rule represents a set of
Objective-C/C++ source files and is very similar to a
[`prebuilt_cxx_library()`](%7BROOT%7Drule/prebuilt_cxx_library.html)
rule. {/param} {param args} {call buck.name_arg /} {/param} {param args}
{call buck.arg} {param name: \'framework\' /} {param desc} The path to
the precompiled framework. {/param} {/call} {/param} {param args} {call
buck.arg} {param name: \'preferred_linkage\' /} {param desc} How to link
to a binary: use `dynamic` for a dynamic framework, and `static` for old
universal static frameworks manually lipo-ed together. `dynamic` will
copy the frameworks into the `Frameworks` directory of an Apple bundle,
and configure framework search paths and linker flags. `static` will
copy the resources of the framework into an Apple bundle. {/param}
{/call} {/param} {param examples} {literal}

``` {.prettyprint .lang-py}
prebuilt_apple_framework(
  name = 'MyPrebuiltFramework',
  framework = 'myPrebuiltFramework.framework',
  preferred_linkage = 'static',
  visibility = [
    'PUBLIC'
  ]
)
          
```

{/literal} {/param} {/call} {/param} {/call} {/template}
