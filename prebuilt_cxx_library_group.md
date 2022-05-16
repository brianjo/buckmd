/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
prebuilt_cxx_library_group} /\*\*\*/ {template .soyweb} {call buck.page}
{param title: \'prebuilt_cxx_library_group()\' /} {param navid:
\'rule_prebuilt_cxx_library_group\' /} {param prettify: true /} {param
description} A prebuilt_cxx_library_group() rule represents a group of
native libraries which should be handled together in a single rule,
perhaps using special link-line construction. {/param} {param content}
{call buck.rule} {param status: \'UNFROZEN\' /} {param overview} A
`prebuilt_cxx_library_group()` rule represents a group of native
libraries which should be handled together in a single rule, perhaps
using special link-line construction. {/param} {param args} {call
buck.name_arg /} {call cxx_common.exported_preprocessor_flags_arg /}
{call buck.arg} {param name: \'static_link\' /} {param default: \'\[\]\'
/} {param desc} The arguments to use when linking this library group
using the static link style. The actual paths to libraries should be
listed in the `static_libs` parameter, and referenced via the the
`$(lib [index])` macro in these args. {/param} {/call} {call buck.arg}
{param name: \'static_libs\' /} {param default: \'\[\]\' /} {param desc}
The paths to the libraries used when using the static link style. The
`static_link` parameter should refer to these libs using their index
number. {/param} {/call} {call buck.arg} {param name:
\'static_pic_link\' /} {param default: \'\[\]\' /} {param desc} The
arguments to use when linking this library group using the static-pic
link style. The actual paths to libraries should be listed in the
`static_pic_libs` parameter, and referenced via the the `$(lib [index])`
macro in these args. {/param} {/call} {call buck.arg} {param name:
\'static_pic_libs\' /} {param default: \'\[\]\' /} {param desc} The
paths to the libraries used when using the static link style. The
`static_pic_link` parameter should refer to these libs using their index
number. {/param} {/call} {call buck.arg} {param name: \'shared_link\' /}
{param default: \'\[\]\' /} {param desc} The arguments to use when
linking this library group using the shared link style. The actual paths
to libraries should be listed in the `shared_libs` parameter, and
referenced via the the `$(lib [name])` macro (or the `$(rel-lib [name])`
macro, when the shared library should be linked using the
`-L[dir] -l[name]` style) in these args. {/param} {/call} {call
buck.arg} {param name: \'shared_libs\' /} {{param default: \'{}\' /}}
{param desc} The map of shared library names to paths used when using
the shared link style. The `shared_link` parameter should refer to these
libs using their library name. {/param} {/call} {call buck.arg} {param
name: \'provided_shared_libs\' /} {{param default: \'{}\' /}} {param
desc} The map of system-provided shared library names to paths used when
using the shared link style. The `shared_link` parameter should refer to
these libs using their library name. {/param} {/call} {call
cxx_common.exported_deps_arg /} {call
cxx_common.exported_platform_deps_arg /} {/param} // close args {param
examples}

A prebuilt library group wrapping two libraries that must be linked
together.

{literal}

``` {.prettyprint .lang-py}
prebuilt_cxx_library_group(
  name = 'util',
  static_link = [
    '-Wl,--start-group',
    '$(lib 0)',
    '$(lib 1)',
    '-Wl,--end-group',
  ],
  static_libs = [
    'lib/liba.a',
    'lib/libb.a',
  ],
  static_pic_link = [
    '-Wl,--start-group',
    '$(lib 0)',
    '$(lib 1)',
    '-Wl,--end-group',
  ],
  static_libs = [
    'lib/liba_pic.a',
    'lib/libb_pic.a',
  ],
  shared_link = [
    '$(rel-lib liba.so)',
    '$(rel-lib libb.so)',
  ],
  shared_libs = {
    'liba.so': 'lib/liba.so',
  },
  provided_shared_libs = {
    'libb.so': 'lib/libb.so',
  },
)
```

{/literal} {/param} {/call} // close buck.rule {/param} {/call}
{/template}
