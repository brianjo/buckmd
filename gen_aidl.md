/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
gen_aidl} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'gen_aidl()\' /} {param navid: \'rule_gen_aidl\' /} {param prettify:
true /} {param description} A rule that is used to generate .java files
from .aidl files. {/param} {param content} {call buck.rule} {param
status: \'FROZEN\' /} {param overview} A `gen_aidl()` rule is used to
generate `.java` files from `.aidl` files. {/param} {param args} {call
buck.name_arg /} {call buck.arg} {param name: \'aidl\' /} {param desc}
The path to an `.aidl` file to convert to a {sp}`.java` file. {/param}
{/call} {call buck.arg} {param name: \'import_path\' /} {param desc} The
search path for import statements for the aidl command. (This is the
`-I` argument when invoking aidl from the command line. For many apps it
will be the base dir where all aidl files are, with project root as its
parent, e.g. `app/src/main/aidl`.). This is the same as the path to the
{sp}`aidl` file relative to what would be returned from{sp} {call
buck.cmd_root /}. {/param} {/call} {call buck.arg} {param name:
\'aidl_srcs\' /} {param default : \'\[\]\' /} {param desc} Path to
`.aidl` files the target `aidl` file imports. {/param} {/call} {call
buck.arg} {param name: \'deps\' /} {param default : \'\[\]\' /} {param
desc} A list of rules that must be built before this rule. {/param}
{/call} {/param} // close args {param examples} {literal}

``` {.prettyprint .lang-py}
android_library(
  name = 'lib',
  srcs = glob(['**/*.java']) + [':aidl'],
  manifest = '//res/org/opencv:manifest',
  deps = [
    '//res/org/opencv:res',
  ],
  visibility = [ 'PUBLIC' ],
)

gen_aidl(
    name = 'aidl',
    aidl = 'engine/OpenCVEngineInterface.aidl',
    import_path = 'java/',
)
```

{/literal} {/param} // close examples {/call} // close buck.rule
{/param} {/call} {/template}
