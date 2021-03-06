/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
cxx_binary} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'cxx_binary()\' /} {param navid: \'rule_cxx_binary\' /} {param
prettify: true /} {param description} A cxx_binary() rule builds a
native C/C++ executable. {/param} {param content} {call buck.rule}
{param status: \'UNFROZEN\' /} {param overview} A cxx_binary() rule
builds a native executable from the supplied set of C/C++ source files
and dependencies. If C/C++ library dependencies are listed, the
generated native executable will request and link against their static
archives (which are \*not\* built using {sp}
[PIC](http://en.wikipedia.org/wiki/Position-independent_code)). {/param}
{param args} {call buck.name_arg /} {call cxx_common.srcs_arg /} {call
cxx_common.platform_srcs_arg /} {call cxx_common.headers_arg /} {call
cxx_common.platform_headers_arg /} {call cxx_common.header_namespace_arg
/} {call cxx_common.preprocessor_flags_arg /} {call
cxx_common.platform_preprocessor_flags_arg /} {call
cxx_common.compiler_flags_arg /} {call
cxx_common.platform_compiler_flags_arg /} {call
cxx_common.linker_extra_outputs_arg /} {call cxx_common.linker_flags_arg
/} {call cxx_common.platform_linker_flags_arg /} {call
cxx_common.precompiled_header_arg /} {call native_common.link_style /}
{call buck.deps_query_arg /} {call buck.tests_arg /} {call
apple_common.extra_xcode_sources /} {call apple_common.extra_xcode_files
/} {call cxx_common.raw_headers_arg /} {call
cxx_common.include_directories_arg /} {/param} // close args {param
flavors} {call buck.arg} {param name : \'#strip-debug\' /} {param desc}
If appended to the target name, it will strip debugging symbols, but
saving local and global symbols. {/param} {/call} {call buck.arg} {param
name : \'#strip-non-global\' /} {param desc} If appended to the target
name, it will strip non-global symbols, but keeping external symbols.
This is preferred for dynamic shared libraries. {/param} {/call} {call
buck.arg} {param name : \'#strip-all\' /} {param desc} If appended to
the target name, it will completely strip the binary, removing the
symbol table and relocation information. This is preferred for
executable files. {/param} {/call} {/param} // close flavors {param
examples} {literal}

``` {.prettyprint .lang-py}
# A rule that builds a C/C++ native executable from a single .cpp file
# its corresponding header, and a C/C++ library dependency.
cxx_binary(
  name = 'echo',
  srcs = [
    'echo.cpp',
  ],
  headers = [
    'echo.h',
  ],
  deps = [
    ':util',
  ],
)

cxx_library(
  name = 'util',
  srcs = [
    'util.cpp',
  ],
  headers = [
    'util.h',
  ],
)

# To build without stripping:
buck build :echo

# To build with stripping debug symbols only:
buck build :echo#strip-debug
```

{/literal} {/param} {/call} // close buck.rule {/param} {/call}
{/template}
