/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
lua_library} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'lua_library()\' /} {param navid: \'rule_lua_library\' /} {param
prettify: true /} {param description} A lua_library() rule is used to
group Lua source files. {/param} {param content} {call buck.rule} {param
status: \'UNFROZEN\' /} {param overview} A `lua_library()` rule is used
to group together Lua sources to be packaged into a top-level {call
buck.lua_binary /} rule. {/param} {param args} {call buck.name_arg /}
{call lua_common.srcs_arg /} {call lua_common.base_module_arg /} {call
buck.arg} {param name: \'deps\' /} {param default : \'\[\]\' /} {param
desc} Other `lua_library()` rules which list `srcs` from which this rule
imports modules. {/param} {/call} {/param} // close args {param
examples} {literal}

``` {.prettyprint .lang-py}
# A rule that includes a single .py file.
lua_library(
  name = 'fileutil',
  srcs = ['fileutil.lua'],
)

# A rule that uses glob() to include all sources in the directory which the
# rule is defined.  It also lists a resource file that gets packaged with
# the sources in this rule.
lua_library(
  name = 'testutil',
  srcs = glob(['testutil/**/*.lua'],
)
```

{/literal} {/param} {/call} // close buck.rule {/param} {/call}
{/template}
