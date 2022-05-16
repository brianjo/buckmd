/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.apple_asset_catalog} /\*\*\*/ {template .soyweb} {call buck.page}
{param title: \'apple_asset_catalog()\' /} {param navid:
\'rule_apple_asset_catalog\' /} {param prettify: true /} {param
description} A rule that is used to bundle Apple asset catalogs.
{/param} {param content} {call buck.rule} {param status: \'UNFROZEN\' /}
{param overview} An `apple_asset_catalog()` rule contains resources
stored in Apple asset catalog directories. This rule does not have any
output on its own and can be built only as a dependency (either direct
or transitive) of an [`apple_bundle()`
rule](%7BROOT%7Drule/apple_bundle.html), in which case all
`apple_asset_catalog()` rules that the bundle rule depends on are merged
and placed into the final output bundle together. {/param} {param args}
{call buck.name_arg /} {call buck.arg} {param name: \'dirs\' /} {param
default : \'\[\]\' /} {param desc} Set of paths of Apple asset catalogs
contained by this rule. All paths have to end with the `   .xcassets`
extension and be compatible with the asset catalog format used by Xcode.
{/param} {/call} {call buck.arg} {param name: \'app_icon\' /} {param
default: \'None\' /} {param desc} An optional reference to a
`.appiconset` containing a image set representing an application icon.
(The extension itself should not be included.) This parameter may be
specified at most once in a given `apple_bundle`\'s transitive
dependencies. {/param} {/call} {call buck.arg} {param name:
\'launch_image\' /} {param default: \'None\' /} {param desc} An optional
reference to a `.launchimage` containing a image set representing an
application launch image. (The extension itself should not be included.)
This parameter may be specified at most once in a given
`apple_bundle`\'s transitive dependencies. {/param} {/call} {/param} //
args {param examples} {literal}

``` {.prettyprint .lang-py}
apple_asset_catalog(
  name = 'MyAssetCatalog',
  dirs = [
    'MyResources.xcassets',
  ],
)

# A asset catalog with a app icon and launch image
apple_asset_catalog(
  name = 'AssetCatalog',
  dirs = [ 'AssetCatalog.xcassets' ],
  app_icon = 'Icon',
  launch_image = 'LaunchImage',
)
```

{/literal} {/param} // examples {/call} // buck.rule {/param} {/call}
{/template}
