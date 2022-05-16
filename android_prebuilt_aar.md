/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
android_prebuilt_aar} /\*\*\*/ {template .soyweb} {call buck.page}
{param title: \'android_prebuilt_aar()\' /} {param navid:
\'rule_android_prebuilt_aar\' /} {param prettify: true /} {param
description} A rule that takes an .aar file and makes it available as an
Android dependency. {/param} {param content} {call buck.rule} {param
status: \'FROZEN\' /} {param overview} An `android_prebuilt_aar()` rule
takes an `.aar` file and makes it available as an Android dependency. As
expected, an {call buck.android_binary /} that transitively depends on
an `android_prebuilt_aar()` will include its contents in the generated
APK.

See the [official Android
documentation](https://developer.android.com/studio/projects/android-library#aar-contents)
for details about the `.aar` format. {/param} {param args} {call
buck.name_arg /} {call buck.arg} {param name: \'aar\' /} {param desc}
Path to the `.aar` file. This may also be a build target to a rule (such
as a {call buck.genrule /}) whose output is an `.aar` file. {/param}
{/call} {call buck.arg} {param name: \'source_jar\' /} {param default :
\'None\' /} {param desc} Path to a JAR file that contains the `.java`
files to create the `.class` in the `aar`. This is frequently provided
for debugging purposes. {/param} {/call} {call buck.arg} {param name:
\'javadoc_url\' /} {param default : \'None\' /} {param desc} URL to the
Javadoc for the `.class` files in the {sp}`aar`. {/param} {/call} {call
buck.arg} {param name: \'use_system_library_loader\' /} {param default :
\'False\' /} {param desc} If this `.aar` file contains native prebuilt
`.so` libraries and the Java code uses these libraries via a call to
`System.loadLibrary()`, then many optimizations---such as exopackage,
compression, or asset packaging---may not be compatible with these
prebuilt libs. Setting this parameter to `True` causes all of these
optimizations to skip the prebuilt `.so` files originating from this
`.aar` file. The `.so` files will always be packaged directly into the
main `.apk`. {/param} {/call} {/param} // close args {param examples}
{literal}

``` {.prettyprint .lang-py}
android_prebuilt_aar(
  name = 'play-services',
  aar = 'play-services-4.0.30.aar',
  source_jar = 'play-services-4.0.30-sources.jar',
  javadoc_url = 'file:///opt/android-sdk/extras/google/google_play_services/docs/reference',
)

android_library(
  name = 'lib',
  # This Java code can compile against Play services and reference its resources.
  srcs = glob(['*.java']),
  deps = [ ':play-services' ],
)
```

{/literal} {/param} {/call} // close buck.rule {/param} {/call}
{/template}
