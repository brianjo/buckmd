/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
android_instrumentation_apk} /\*\*\*/ {template .soyweb} {call
buck.page} {param title: \'android_instrumentation_apk()\' /} {param
navid: \'rule_android_instrumentation_apk\' /} {param prettify: true /}
{param description} A rule that generates an Android Instrumentation
APK. {/param} {param content} {call buck.rule} {param status:
\'UNFROZEN\' /} {param overview}

An `android_instrumentation_apk()` rule is used to generate an Android
Instrumentation APK.

Android\'s [Testing
Fundamentals](http://developer.android.com/tools/testing/testing_android.html)
documentation includes a diagram that shows the relationship between an
\"application package\" and a \"test package\" when running a test. This
rule corresponds to a test package. Note that a test package has an
interesting quirk where it is *compiled against* an application package,
but *must not include* the resources or Java classes of the application
package. Therefore, this class takes responsibility for making sure the
appropriate bits are excluded. Failing to do so will generate mysterious
runtime errors when running the test.

{/param} {param args} {call buck.arg} {param name: \'name\' /} {param
desc} The *short name* for this {call buck.build_target /}. Also, the
name of the APK generated from this target. {/param} {/call} {call
android_common.manifest_apk_arg /} {call buck.arg} {param name: \'apk\'
/} {param desc} APK build target, which should be used for the
instrumentation APK. Can be either a {call buck.android_binary /} or a
{sp}{call buck.apk_genrule /}. {/param} {/call} {call
android_common.deps_apk_arg /} {/param} // close args {param examples}
Here is an example of an `android_instrumentation_apk()`{sp} rule that
tests a `android_binary()`, and depends on a test package. {literal}

``` {.prettyprint .lang-py}
android_library(
  name = 'test',
  srcs = glob(['test/**/*.java']),
)

android_binary(
  name = 'messenger',
  manifest = 'AndroidManifest.xml',
  keystore = '//keystores:prod',
  package_type = 'release',
  proguard_config = 'proguard.cfg',
  deps = [
    ...
  ],
)

# Building this rule will produce a file named messenger_test.apk
android_instrumentation_apk(
  name = 'messenger_test',
  manifest = 'AndroidInstrumentationManifest.xml',
  apk = ':messenger',
  deps = [
    ':test',
  ],
)
```

{/literal} {/param} {/call} // close buck.rule {/param} {/call}
{/template}
