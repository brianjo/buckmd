/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
robolectric_test} /\*\*\*/ {template .soyweb} {call buck.page} {param
title: \'robolectric_test()\' /} {param navid: \'rule_robolectric_test\'
/} {param prettify: true /} {param description} A rule that is used to
define a set of Java files that contain
[Robolectric](http://robolectric.org/) tests. {/param} {param content}
{call buck.rule} {param status: \'FROZEN\' /} {param overview} A
`robolectric_test()` rule is used to define a set of {sp}`.java` files
that contain tests to run via JUnit with Robolectric test runner. It
extends from `java_test()` rule. {/param} {param args} {call
buck.name_arg /} {call buck.arg} {param name:
\'robolectric_runtime_dependency\' /} {param default : \'None\' /}
{param desc} Robolectric only runs in offline mode with buck. Specify
the relative directory containing all the jars Robolectric uses at
runtime. {/param} {/call} {call buck.arg} {param name:
\'robolectric_manifest\' /} {param default: \'None\' /} {param desc} An
optional [Android
Manifest](http://developer.android.com/guide/topics/manifest/manifest-intro.html)
for the rule to declare any permissions or intents it may need or want
to handle. May either be a file or a {call buck.android_manifest /}
target. {/param} {/call} {call buck.arg} {param name:
\'force_final_resource_ids\' /} {param default : \'True\' /} {param
desc} Set it to false if using Robolectric version greater than 3.2 or
higher as Robolectric requires resources id\'s to be non final. {/param}
{/call} {call test_common.contacts_arg /} {call buck.arg} {param name:
\'free_compiler_args\' /} {param default : \'\[\]\' /} {param desc} List
of additional arguments to pass into the Kotlin compiler. {/param}
{/call} {call buck.arg} {param name: \'use_binary_resources\' /} {param
default : \'False\' /} {param desc} Tells Robolectric to use binary
resources mode, which reads resources from a resource APK rather than
the filesystem. This requires Robolectric 4+. {/param} {/call} {/param}
// close args {/call} // close buck.rule {/param} {/call} {/template}
