/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
python_library} /\*\*\*/ {template .soyweb} {call buck.page} {param
title: \'python_library()\' /} {param navid: \'rule_python_library\' /}
{param prettify: true /} {param description} A python_library() rule is
used to group Python source files and resources. {/param} {param
content} {call buck.rule} {param status: \'UNFROZEN\' /} {param
overview} A `python_library()` rule is used to group together Python
source files and resources to package them into a PEX using a top-level
{call buck.python_binary /} rule. {/param} {param args} {call
buck.name_arg /} {call python_common.srcs_arg /} {call
python_common.platform_srcs_arg /} {call python_common.resources_arg /}
{call python_common.platform_resources_arg /} {call
python_common.base_module_arg /} {call buck.arg} {param name: \'deps\'
/} {param default : \'\[\]\' /} {param desc} Other `python_library()`
rules that list `srcs` from which this rule imports modules. {/param}
{/call} {call python_common.exclude_deps_from_merged_linking_arg /}
{/param} // close args {param examples}

Include Python source files and resource files.

{literal}

``` {.prettyprint .lang-py}
# BUCK 

# A rule that includes a single Python file.
python_library(
  name = 'fileutil',
  srcs = ['fileutil.py'],
  deps = [
    '//third_party/python-magic:python-magic',
  ],
)

# A rule that uses glob() to include all Python source files in the
# directory in which the rule is defined. The rule also specifies a 
# resource file that gets packaged with the source file.
python_library(
  name = 'testutil',
  srcs = glob(['testutil/**/*.py']),
  resources = [
    'testdata.dat',
  ],
)
```

{/literal}

Use the `platform_srcs` and `platform_resources` arguments to pull in
source files and resources only when building for a specific Python
platform.

{literal}

``` {.prettyprint .lang-ini}
; .buckconfig

[python#py2]
  interpreter = /usr/bin/python2.7

[python#py3]
  interpreter = /usr/bin/python3.4
```

{/literal} {literal}

``` {.prettyprint .lang-py}
# BUCK

python_library(
  name = 'utils',
  platform_srcs = [
    ('py2', ['foo.py']),
    ('py3', ['bar.py']),
  ],
  platform_resources = [
    ('py2', ['foo.dat']),
    ('py3', ['bar.dat']),
  ],
)
```

{/literal} {/param} {/call} // close buck.rule {/param} {/call}
{/template}
