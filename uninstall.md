/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.command.uninstall} /\*\*\*/ {template .soyweb} {call buck.page}
{param title: \'buck uninstall\' /} {param navid: \'command_uninstall\'
/} {param description} A command that uninstalls the APK for an
android_binary target. {/param} {param content} {call buck.command}
{param overview} Uninstalls the APK for an
[`android_binary`](%7BROOT%7Drule/android_binary.html) target.

Takes an [`android_binary`](%7BROOT%7Drule/android_binary.html) target,
determines the id of the application that it is meant to build, and
uninstalls it by running {sp}`adb uninstall <application_id>`:

    buck uninstall //java/com/myawesomeapp

{/param} {param params} None. {/param} {/call} {/param} // content
{/call} // buck.page {/template}
