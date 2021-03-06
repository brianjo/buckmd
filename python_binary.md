/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
python_binary} /\*\*\*/ {template .soyweb} {call buck.page} {param
title: \'python_binary()\' /} {param navid: \'rule_python_binary\' /}
{param prettify: true /} {param description} A rule that is used to
build a PEX file that includes python sources and resources from all
transitive python_library() dependencies. {/param} {param content} {call
buck.rule} {param status: \'UNFROZEN\' /} {param overview} A
`python_binary()` rule is used to build a
[PEX](http://pantsbuild.github.io/pex_design.html) file---an executable
Python package---that includes Python sources and resources from all
transitive {call buck.python_library /} dependencies. {/param} {param
args} {call buck.arg} {param name: \'name\' /} {param desc} The *short
name* for this {call buck.build_target /}. Also, the output PEX file
will have this name as its base filename with an additional `.pex`
extension. {/param} {/call} {call buck.arg} {param name: \'main_module\'
/} {param desc} The python module that should be the entry point of the
binary. This should be a module name within a python_library that this
binary depends on. Note that module names take `base_module` of the
library into account. This property is mutually exclusive with `main`,
and should be preferred to `main`, which is deprecated. {/param} {/call}
{call buck.arg} {param name: \'main\' /} {param deprecated: true /}
{param deprecationAlternative} Use a {call buck.python_library /}
dependency and `main_module` instead {/param} {param default: \'None\'
/} {param desc} The Python file which serves as the entry point for the
PEX. The interpreter initiates execution of the PEX with the code in
this file. {/param} {/call} {call buck.arg} {param name: \'base_module\'
/} {param default : \'None\' /} {param deprecated: true /} {param desc}
The package in which the main module should reside in its final location
in the binary. If unset, Buck uses the project-relative directory that
contains the BUCK file. {/param} {/call} {call
python_common.platform_arg /} {call buck.arg} {param name: \'deps\' /}
{param default : \'\[\]\' /} {param desc} A list of {call
buck.python_library /} rules that specify Python modules to include in
the PEX file---including all transitive dependencies of these rules.
{/param} {/call} {call python_common.preload_deps_arg /} {call
python_common.package_style_arg /} {call python_common.linker_flags_arg
/} {/param} // close args {param examples}

Build a PEX from the Python files in the BUCK directory.

{literal}

``` {.prettyprint .lang-py}
# BUCK

python_binary(
  name = 'tailer',
  main_module = 'tailer',
  deps = [
    ':tailerutils',
  ],
)

python_library(
  name = 'tailerutils',
  # The main module, tailer.py, is specified here.
  # (Separated out from the glob pattern for clarity.)
  srcs = glob(['tailer.py', '*.py']),
)
```

{/literal}

Use the `platform` argument to select the `[python#py2]` platform as
defined in `.buckconfig`.

{literal}

``` {.prettyprint .lang-ini}
; .buckconfig

[python#py2]
  interpreter = /usr/bin/python2.7
```

{/literal} {literal}

``` {.prettyprint .lang-py}
# BUCK

python_binary(
  name = 'bin',
  platform = 'py2',
  main_module = 'main',
  deps = [
    ':bar',
  ],
)
```

{/literal} {/param} {/call} // close buck.rule {/param} {/call}
{/template}
