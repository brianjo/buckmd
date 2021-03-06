/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.prebuilt_native_library} /\*\*\*/ {template .soyweb} {call
buck.page} {param title: \'prebuilt_native_library()\' /} {param navid:
\'rule_prebuilt_native_library\' /} {param prettify: true /} {param
description} A rule that is used to identify a native library that is
checked into the project as a precompiled binary. {/param} {param
content} {call buck.rule} {param status: \'FROZEN\' /} {param overview}
A `prebuilt_native_library()` rule is used to bundle native libraries
(i.e., `.so` files) for Android. {/param} {param args} {call
buck.name_arg /} {call buck.arg} {param name: \'native_libs\' /} {param
default : \'None\' /} {param desc} Path to a directory containing native
libraries. This directory has subdirectories for different
architectures, such as `armeabi` and `armeabi-v7a`. {/param} {/call}
{call buck.arg} {param name: \'is_asset\' /} {param default: \'False\'
/} {param desc} Normally native shared objects end up in a directory in
the root of the APK named `lib/`. If this parameter is set to `True`,
then these objects are placed in `assets/lib/`. Placing shared objects
in a non-standard location prevents Android from extracting them to the
device\'s internal storage. {/param} {/call} {/param} // args {param
examples} Most of the time, a `prebuilt_native_library` is private to
the{sp} {call buck.android_library /} that uses it: {literal}

``` {.prettyprint .lang-py}
prebuilt_native_library(
  name = 'native_libs',
  native_libs = 'libs',
)

android_library(
  name = 'my_lib',
  srcs = glob(['*.java']),
  deps = [
    ':native_libs',
  ],
)
```

{/literal} {/param} // examples {/call} // buck.rule {/param} {/call}
{/template}
