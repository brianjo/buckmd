/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.apple_bundle} /\*\*\*/ {template .soyweb} {call buck.page} {param
title: \'apple_bundle()\' /} {param navid: \'rule_apple_bundle\' /}
{param prettify: true /} {param description} A rule that generates an
Apple bundle. {/param} {param content} {call buck.rule} {param status:
\'UNFROZEN\' /} {param overview}

An `apple_bundle()` rule takes an Apple binary and all of the resources
and asset catalogs in the rule\'s transitive dependencies and generates
a bundle containing all of those files. Optionally the generated bundle
can also be signed using specified provisioning profiles.

Code signing will embed entitlements pointed to by the
`entitlements_file` arg in the bundle\'s `apple_binary`. This is the
preferred way to specify entitlements when building with Buck.

If the entitlements file is not present, it falls back to the
`CODE_SIGN_ENTITLEMENTS` entry in `info_plist_substitutions`.

If after these checks, an entitlements file is still not specified, it
will be derived based on the entitlements of the selected provisioning
profile. Provisioning profiles will be selected from profiles pointed to
by `apple.provisioning_profile_search_path`, based on a non-expired
profile that matches the bundle id and entitlements.

Code signing will embed entitlements pointed to by the
`CODE_SIGN_ENTITLEMENTS` entry in `info_plist_substitutions`. If an
entitlements file is omitted, it will be derived based on the
entitlements of the selected provisioning profile. Provisioning profiles
will be selected from profiles pointed to by
`apple.provisioning_profile_search_path`, based on a non-expired profile
that matches the bundle id and entitlements.

{/param} {param args} {call buck.name_arg /} {call buck.arg} {param name
: \'deps\' /} {param default : \'\[\]\' /} {param desc} A list of
dependencies of this bundle as build targets. You can embed application
extensions by specifying the extension\'s bundle target. To include a
WatchKit app, append the flavor `#watch` to the target specification.
Buck will automatically substitute the appropriate platform flavor
(either `watchsimulator` or `watchos`) based on the parent. {/param}
{/call} {call buck.arg} {param name: \'product_name\' /} {param desc}
The name of the resulting bundle and binary. The setting behaves like
PRODUCT_NAME Xcode build setting. For example, if your rule is named
\"MyApp\" and extension is \"app\", by default buck will generate
MyApp.app bundle. But if you will set product name to \"SuperApp\",
bundle will get \"SuperApp.app\" name. {/param} {/call} {call buck.arg}
{param name: \'extension\' /} {param desc} The extension of the
generated bundle. For example `'app'` for an application bundle or
`'appex'` for an application extension bundle. {/param} {/call} {call
buck.arg} {param name: \'binary\' /} {param desc} A [build
target](%7BROOT%7Dconcept/build_target.html) identifying an
[`apple_binary()` rule](%7BROOT%7Drule/apple_binary.html) or an
[`apple_library()` rule](%7BROOT%7Drule/apple_library.html) whose output
will be used as the main executable binary of the generated bundle. The
required rule type depends on the value in the `extension` attribute.
For example, application bundles expect a binary (e.g.
`'//Apps/MyApp:MyApp'`), application extension bundles expect a shared
library (e.g. `'//Libraries/MyLibrary:MyLibrary#shared'`). {/param}
{/call} {call apple_common.info_plist_arg /} {call
apple_common.info_plist_substitutions_arg /} {call buck.tests_apple_arg
/} {call buck.arg} {param name: \'asset_catalogs_compilation_options\'
/} {param desc} A dict holding parameters for asset catalogs compiler
(actool). Its options include:

-   `notices` (defaults to `True`)
-   `warnings` (defaults to `True`)
-   `errors` (defaults to `True`)
-   `compress_pngs` (defaults to `True`)
-   `optimization` (defaults to `'space'`)
-   `output_format` (defaults to `'human-readable-text'`)
-   `extra_flags` (defaults to `[]`)

{/param} {/call} {call buck.arg} {param name: \'ibtool_flags\' /} {param
default : \'\[\]\' /} {param desc} List of flags to be passed to ibtool
during interface builder file compilation. {/param} {/call} {/param} //
args {param examples} {literal}

``` {.prettyprint .lang-py}
apple_bundle(
  name = 'AppBundle',
  binary = ':MyBinary',
  extension = 'app',
  info_plist = 'Info.plist',
)
```

{/literal} {literal}

``` {.prettyprint .lang-py}
# iOS app with embedded WatchOS 2.0 app/extension
apple_bundle(
  name = 'DemoWatchAppExtension',
  binary = ':DemoWatchAppExtensionBinary',
  extension = 'appex',
  info_plist = 'WatchExtension/Resources/Info.plist',
)

apple_bundle(
  name = 'DemoWatchApp',
  binary = ':DemoWatchAppBinary',
  deps = [':DemoWatchAppResources', ':DemoWatchAppExtension'],
  extension = 'app',
  info_plist = 'WatchApplication/Info.plist',
)

apple_bundle(
  name = 'DemoApp',
  binary = ':DemoAppBinary',
  deps = [':DemoWatchApp#watch'],
  extension = 'app',
  info_plist = 'Info.plist',
)
```

{/literal} {literal}

``` {.prettyprint .lang-py}
# iOS app using safeAreaInsets delivering to iOS 9.x
apple_bundle(
  name = 'DemoIBApp',
  binary = ':DemoIBAppBinary',
  deps = [':DemoIBAppResources'],
  extension = 'app',
  ibtool_flags = ["--minimum-deployment-target", "9.0"],
  info_plist = 'Info.plist',
)
```

{/literal} {/param} // examples {/call} // buck.rule {/param} {/call}
{/template}
