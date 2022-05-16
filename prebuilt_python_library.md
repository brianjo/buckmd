/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
prebuilt_python_library} /\*\*\*/ {template .soyweb} {call buck.page}
{param title: \'prebuilt_python_library()\' /} {param navid:
\'rule_prebuilt_python_library\' /} {param prettify: true /} {param
description} A prebuilt_python_library() rule is used to include binary
python packages (i.e. whls and eggs). {/param} {param content} {call
buck.rule} {param status: \'UNFROZEN\' /} {param overview}

A `prebuilt_python_library()` rule is used to include prebuilt python
packages into the output of a top-level {call buck.python_binary /} or
{call buck.python_test /} rule.

These prebuilt libraries can either be [whl
files](https://www.python.org/dev/peps/pep-0427/) or eggs

whls for most packages are available for download from
[PyPI](https://pypi.org). The whl used may be downloaded with {call
buck.remote_file /}. However, Buck does not attempt to infer dependency
information from pip, so that information will have to be imparted by
the user.

To create an egg for a package, run `python setup.py bdist_egg` in the
package source distribution. {/param} {param args} {call buck.name_arg
/} {call buck.arg} {param name: \'binary_src\' /} {param desc} The path
to the `.whl` or `.egg` to use. Note: `.egg` files have a very
particular naming convention that must be followed - otherwise pex will
not find the dependency properly at runtime! {/param} {/call} {call
buck.arg} {param name: \'deps\' /} {param default : \'\[\]\' /} {param
desc} Other `prebuilt_python_library()` rules which this library depends
on. These may also be `python_library` rules if you want to depend on a
source-based copy of the library. {/param} {/call} {call
python_common.exclude_deps_from_merged_linking_arg /} {/param} // close
args {param examples} {literal}

``` {.prettyprint .lang-py}
# A simple prebuilt_python_library with no external dependencies.
remote_file(
  name = "requests-download",
  url = "https://files.pythonhosted.org/packages/51/bd/23c926cd341ea6b7dd0b2a00aba99ae0f828be89d72b2190f27c11d4b7fb/requests-2.22.0-py2.py3-none-any.whl",
  sha1 = "e1fc28120002395fe1f2da9aacea4e15a449d9ee",
  out = "requests-2.22.0-py2.py3-none-any.whl",
)

prebuilt_python_library(
  name = "requests",
  binary_src = ":requests-download",
)

# A slightly more complex example
prebuilt_python_library(
  name = "greenlet",
  binary_src = "greenlet-0.4.7-py2.7-macosx-10.10-x86_64.egg",
)

prebuilt_python_library(
  name = "gevent",
  binary_src = "gevent-1.0.2-py2.7-macosx-10.10-x86_64.egg",
  deps = [
    ":greenlet",
  ],
)
```

{/literal} {/param} {/call} // close buck.rule {/param} {/call}
{/template}
