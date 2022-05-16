/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
android_aar} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'android_aar()\' /} {param navid: \'rule_android_aar\' /} {param
prettify: true /} {param description} A rule that generates an Android
AAR. {/param} {param content} {call buck.rule} {param status: \'FROZEN\'
/} {param overview} An `android_aar()` rule is used to generate an
Android AAR.

See the [official Android
documentation](https://developer.android.com/studio/projects/android-library#aar-contents)
for details about the `.aar` format. {/param} {param args} {call
buck.name_arg /} {call buck.arg} {param name: \'manifest_skeleton\' /}
{param desc} The skeleton manifest file used to generate the final
`AndroidManifest.xml   `. May either be a file or a {call
buck.android_manifest /} target. {/param} {/call} {call buck.arg} {param
name : \'build_config_values\' /} {param default : \'\[\]\' /} {param
desc} See the documentation on the values argument for {call
buck.android_build_config /}. {/param} {/call} {call buck.arg} {param
name: \'include_build_config_class\' /} {param default : \'False\' /}
{param desc} Whether to include the `BuildConfig` class files in the
final .aar file. Needs to be set to `True` if any build_config_values
are specified. This is normally only needed if the build tool that is
consuming the .aar file does not generate {sp}`BuildConfig` classes.
Note: the AAR format does not specify a way to pass defaults that should
be injected into the final `BuildConfig` class, therefore that
information might need to be replicated manually in the build that\'s
consuming the .aar file. {/param} {/call} {call buck.arg} {param name :
\'deps\' /} {param default : \'\[\]\' /} {param desc} List of build
targets whose corresponding compiled Java code, Android resources, and
native libraries will be included in the AAR along with their transitive
dependencies. For compile time deps which should not be included in the
final AAR, use `provided_deps` instead.

-   `android_library()` Will be included in the final `classes.jar`
-   `android_resource()` Will be included in the final `R.txt`,
    {sp}`res/` and `assets/`
-   `android_build_config()` Will be included in the final `classes.jar`
    {sp}if `include_build_config_class` is True
-   `groovy_library()` Will be included in the final `classes.jar`
-   `java_library()` Will be included in the final `classes.jar`
-   `prebuilt_jar()` Will be included in the final `classes.jar`
-   `ndk_library()` Will be included in the final `jni/` or
    {sp}`assets/` if `is_asset` is True
-   `prebuilt_native_library()` Will be included in the final `jni/` or
    {sp}`assets/` if `is_asset` is True

{/param} {/call} {/param} // close args {param examples} {literal}

``` {.prettyprint .lang-py}
android_resource(
  name = 'res',
  res = 'res',
  assets = 'assets',
  package = 'com.example',
)

android_library(
  name = 'lib',
  srcs = glob(['**/*.java']),
)

android_aar(
  name = 'app',
  manifest_skeleton = 'AndroidManifestSkeleton.xml',
  deps = [
    ':res',
    ':lib',
  ],
)
```

{/literal} {/param} {/call} // close buck.rule {/param} {/call}
{/template}
