/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
cxx_test} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'cxx_test()\' /} {param navid: \'rule_cxx_test\' /} {param prettify:
true /} {param description} A cxx_test() rule builds a native C/C++
executable. {/param} {param content} {call buck.rule} {param status:
\'UNFROZEN\' /} {param overview} A cxx_test() rule builds a C/C++ binary
against a C/C++ testing framework and runs it as part of {call
buck.cmd_test /}. {/param} {param args} {call buck.name_arg /} {call
cxx_common.srcs_arg /} {call cxx_common.headers_arg /} {call
cxx_common.preprocessor_flags_arg /} {call cxx_common.compiler_flags_arg
/} {call cxx_common.linker_flags_arg /} {call
cxx_common.precompiled_header_arg /} {call buck.deps_query_arg /} {call
buck.arg} {param name : \'resources\' /} {param default : \'\[\]\' /}
{param desc}

This attribute is currently not implemented, and just causes buck to
rebuild the test file if any of the resources change. This will change
in the future to provide a more reliable interface for resource files.

Additional data or source files which this test uses. {/param} {/call}
{call cxx_common.raw_headers_arg /} {call
cxx_common.include_directories_arg /} {call buck.arg} {param name:
\'framework\' /} {param default : \'\"gtest\"\' /} {param desc}

The testing framework to build against and run with. We currently
support [`gtest`](https://github.com/google/googletest) and
[`boost`](http://www.boost.org/doc/libs/1_57_0/libs/test/doc/html/index.html).

When set to `gtest`, you must also set {call buckconfig.cxx_gtest_dep
/}.

{/param} {/call} {call buck.arg} {param name: \'env\' /} {{param default
: \'{}\' /}} {param desc} A map of environment names and values to set
when running the test.\
\
It is also possible to expand references to other rules within the
**values** of these environment variables, using builtin {call
buck.string_parameter_macros /}:

`$(location //path/to:target)`
:   Expands to the location of the output of the build rule. This means
    that you can refer to these without needing to be aware of how Buck
    is storing data on the disk mid-build.

{/param} {/call} {call buck.arg} {param name: \'args\' /} {{param
default : \'\[\]\' /}} {param desc} A list of additional arguments to
pass to the test when it\'s run.\
\
It is also possible to expand references to other rules within these
arguments, using builtin {call buck.string_parameter_macros /}:

`$(location //path/to:target)`
:   Expands to the location of the output of the build rule. This means
    that you can refer to these without needing to be aware of how Buck
    is storing data on the disk mid-build.

{/param} {/call} {call test_common.contacts_arg /} {call
buck.run_test_separately_arg /} {call buck.test_rule_timeout_ms /} {call
apple_common.extra_xcode_sources /} {call apple_common.extra_xcode_files
/} {/param} // close args {param examples} {literal}

``` {.prettyprint .lang-py}
# A rule that builds and runs C/C++ test using gtest.
cxx_test(
  name = 'echo_test',
  srcs = [
    'echo_test.cpp',
  ],
)
```

{/literal} {/param} {/call} // close buck.rule {/param} {/call}
{/template}
