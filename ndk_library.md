/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
ndk_library} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'ndk_library()\' /} {param navid: \'rule_ndk_library\' /} {param
prettify: true /} {param description} A rule that is used to define a
set of C/C++ files, an Android.mk and an Application.mk file that are
used by the Android NDK\'s ndk-build tool to generate one or more shared
objects. {/param} {param content} {call buck.rule} {param status:
\'FROZEN\' /} {param overview} An `ndk_library()` is used to define a
set of C/C++ files, an `Android.mk` and an `Application.mk` file that
are used by the NDK\'s `ndk-build` tool to generate one or more shared
objects. {/param} {param args} {call buck.name_arg /} {call buck.arg}
{param name: \'srcs\' /} {{param default :
\'\[\*\*/\*.{cpp,c,cc,cxx,h,hpp,mk}\]\' /}} {param desc} The set of
files to compile for this rule. If not provided, `buck` assumes that all
files with the following extensions are part of the build:
{sp}`c, cpp, cc, cxx, h, hpp, mk`. {/param} {/call} {call buck.arg}
{param name: \'deps\' /} {param default : \'\[\]\' /} {param desc} List
of build targets to build before this rule. {/param} {/call} {call
buck.arg} {param name: \'flags\' /} {param default : \'\[\]\' /} {param
desc} Array of strings passed verbatim to `ndk-build`. Normally this is
not needed, but in some cases you may want to put something here. For
example, this can be used to build the libraries in debug mode
(`NDK_DEBUG=1`) or set the number of jobs spawned by {sp}`ndk-build` (by
default, the same as the number of cores). {/param} {/call} {call
buck.arg} {param name: \'is_asset\' /} {param default: \'False\' /}
{param desc} Normally native shared objects end up in a directory in the
root of the APK named `lib/`. If this parameter is set to `True`, then
these objects are placed in `assets/lib/`. Placing shared objects in a
non-standard location prevents Android from extracting them to the
device\'s internal storage. {/param} {/call} {/param} // close args
{param furtherexp}

An `android_binary()` that includes this library will aggregate all of
the native shared objects into a directory in the root of the APK named
`lib/` or `assets/lib/`.

Unlike the default invocation of `ndk-build`, {sp}`buck` will put all
intermediate files and build output into a subdirectory under
`buck-out/gen`. {/param} {/call} // close buck.rule {/param} {/call}
{/template}
