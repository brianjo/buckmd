/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.apple_resource} /\*\*\*/ {template .soyweb} {call buck.page} {param
title: \'apple_resource()\' /} {param navid: \'rule_apple_resource\' /}
{param prettify: true /} {param description} A rule that is used to
bundle resource directories, files and file variants. {/param} {param
content} {call buck.rule} {param status: \'UNFROZEN\' /} {param
overview} An `apple_resource()` rule contains sets of resource
directories, files and file variants that can be bundled in an
application bundle. This rule does not have any output on its own and
can be built only as a dependency (either direct or transitive) of an
[`apple_bundle()` rule](%7BROOT%7Drule/apple_bundle.html). {/param}
{param args} {call buck.name_arg /} {call buck.arg} {param name:
\'dirs\' /} {param desc} Set of paths of resource directories that
should be placed in an application bundle. {/param} {/call} {call
buck.arg} {param name: \'files\' /} {param desc} Set of paths of
resource files that should be placed in an application bundle. {/param}
{/call} {call buck.arg} {param name: \'variants\' /} {param default :
\'\[\]\' /} {param desc} Set of paths of resource file variants that
should be placed in an application bundle. The files mentioned here
should be placed in a directory named `$VARIANT_NAME.lproj`, where
`$VARIANT_NAME` is the name of the variant (e.g. `Base`, `en`). This
argument makes it possible to use different resource files based on the
active locale. {/param} {/call} {call buck.arg} {param name:
\'resources_from_deps\' /} {param default : \'\[\]\' /} {param desc} Set
of build targets whose transitive `apple_resource`s should be considered
as part of the current resource when collecting resources for bundles.
Usually, an `apple_bundle` collects all `apple_resource` rules
transitively reachable through apple_library rules. This field allows
for resources which are not reachable using the above traversal strategy
to be considered for inclusion in the bundle. {/param} {/call} {call
buck.arg} {param name: \'destination\' /} {param default : \'resources\'
/} {param desc} Specifies the destination in the final application
bundle where resource will be copied. Possible values: \"resources\",
\"frameworks\", \"executables\", \"plugins\", \"xpcservices\". {/param}
{/call} {call buck.arg} {param name: \'codesign_on_copy\' /} {param
default : \'False\' /} {param desc} Indicates whether the files
specified in the files arg in this resource should be code signed with
the identity used to sign the overall bundle. This is useful for e.g.
dylibs or other additional binaries copied into the bundle. The caller
is responsible to ensure that the file format is valid for codesigning.
{/param} {/call} {/param} // args {param examples} {literal}

``` {.prettyprint .lang-py}
apple_resource(
  name = 'Images',
  files = glob([
    '*.png',
  ]),
  dirs = [
    'PrettyImages',
  ],
)
```

{/literal} {/param} // examples {/call} // buck.rule {/param} {/call}
{/template}
