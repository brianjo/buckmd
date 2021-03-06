/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.host_info} /\*\*\*/ {template .soyweb} {call buck.page} {param
title: \'host_info()\' /} {param navid: \'function_host_info\' /} {param
prettify: true /} {param description} The host_info() function is used
to get processor and OS information about the host machine {/param}
{param content} {call buck.function} {param status: \'UNFROZEN\' /}
{param overview} The `host_info()` function is used to get the current
OS and processor architecture on the host. This will likely change as
better cross compilation tooling comes to Buck. The structure returned
is laid out thusly: {literal}

``` {.prettyprint .lang-py}
  struct(
      os=struct(
          is_linux=True|False,
          is_macos=True|False,
          is_windows=True|False,
          is_freebsd=True|False,
          is_unknown=True|False,
      ),
      arch=struct(
          is_aarch64=True|False,
          is_arm=True|False,
          is_armeb=True|False,
          is_i386=True|False,
          is_mips=True|False,
          is_mips64=True|False,
          is_mipsel=True|False,
          is_mipsel64=True|False,
          is_powerpc=True|False,
          is_ppc64=True|False,
          is_unknown=True|False,
          is_x86_64=True|False,
      ),
  )
```

{/literal} {/param} {/call} // buck.function {/param} // content {/call}
{/template}
