/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.android_resource} /\*\*\*/ {template .soyweb} {call buck.page}
{param title: \'android_resource()\' /} {param navid:
\'rule_android_resource\' /} {param prettify: true /} {param
description} A rule that is used to bundle Android resources that are
traditionally stored in res and assets directories. {/param} {param
content} {call buck.rule} {param status: \'FROZEN\' /} {param overview}
An `android_resource()` rule is used to bundle Android resources that
are traditionally stored in `res` and `assets` directories.

The output of an `android_resource()` is an `R.txt` file generated via
`aapt --output-text-symbols`. {/param} {param args} {call buck.name_arg
/} {call buck.arg} {param name: \'res\' /} {param default : \'None\' /}
{param desc} A dictionary mapping relative resource paths to either the
resource files or the build targets that generate them. The
[`subdir_glob()`](%7BROOT%7Dfunction/subdir_glob.html) function can be
used to generate dictionaries based on a directory structure of files
checked into the repository. Alternatively, this can be a path to a
directory containing Android resources, although this option is
deprecated and might be removed in the future. {/param} {/call} {call
buck.arg} {param name: \'package\' /} {param default : \'None\' /}
{param desc} Java package for the `R.java` file that will be generated
for these resources. {/param} {/call} {call buck.arg} {param name:
\'assets\' /} {param default : \'None\' /} {param desc} A dictionary
mapping relative asset paths to either the asset files or the build
targets that generate them. The
[`subdir_glob()`](%7BROOT%7Dfunction/subdir_glob.html) function can be
used to generate dictionaries based on a directory structure of files
checked into the repository. Alternatively, this can be a path to a
directory containing Android assets, although this option is deprecated
and might be removed in the future. {/param} {/call} {call buck.arg}
{param name: \'project_res\' /} {param default : \'None\' /} {param
desc} A directory containing resources to be used for project
generation. If not provided, defaults to whatever the build uses.
{/param} {/call} {call buck.arg} {param name: \'project_assets\' /}
{param default : \'None\' /} {param desc} A directory containing assets
to be used for project generation. If not provided, defaults to whatever
the build uses. {/param} {/call} {call android_common.manifest_arg}
{param type: \'resource\' /} {/call} {call buck.arg} {param name:
\'deps\' /} {param default : \'None\' /} {param desc} Other
`android_resource` rules to include via `-S` when running `aapt`.
{/param} {/call} {/param} // args {param examples} Most of the time, an
`android_resource` rule defines only{sp} `name`, `res`, and `package`.
By convention, such simple rules are often named `res`: {literal}

``` {.prettyprint .lang-py}
android_resource(
  name = 'res',
  res = subdir_glob([('res', '**')]),
  package = 'com.example',
)
```

{/literal} {/param} // examples {/call} // buck.rule {/param} {/call}
{/template}
