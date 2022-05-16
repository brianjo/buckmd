/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
python_test} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'python_test()\' /} {param navid: \'rule_python_test\' /} {param
prettify: true /} {param description} A rule that defines a set of
python files that contain tests to run via the Python unit testing
framework. {/param} {param content} {call buck.rule} {param status:
\'UNFROZEN\' /} {param overview}

A `python_test()` rule defines a set of `.py`{sp} files that contain
tests to run via the [Python unit testing
framework](https://docs.python.org/2/library/unittest.html).

If your test requires static files you should specify these in the
**resources** or **platform_resources** arguments. If you do not specify
these files, they won\'t be available when your test runs.

{/param} {param args} {call buck.name_arg /} {call
python_common.srcs_arg /} {call python_common.platform_srcs_arg /} {call
python_common.resources_arg /} {call
python_common.platform_resources_arg /} {call
python_common.base_module_arg /} {call
python_common.exclude_deps_from_merged_linking_arg /} {call buck.arg}
{param name: \'main_module\' /} {param default : \'None\' /} {param
desc} The main module used to run the tests. This parameter is normally
not needed, as Buck will provide a default main module that runs all
tests. However, you can override this with your own module to perform
custom initialization or command line processing. Your custom module can
import the standard Buck test main as `__test_main__`, and can invoke
it\'s normal main function as `__test_main__.main(sys.argv)`. {/param}
{/call} {call python_common.platform_arg /} {call buck.arg} {param name:
\'env\' /} {{param default : \'{}\' /}} {param desc} A map of
environment names and values to set when running the test.\
\
It is also possible to expand references to other rules within the
**values** of these environment variables, using builtin {call
buck.string_parameter_macros /}:

`$(location //path/to:target)`
:   Expands to the location of the output of the build rule. This means
    that you can refer to these without needing to be aware of how Buck
    is storing data on the disk mid-build.

{/param} {/call} {call buck.arg} {param name: \'deps\' /} {param default
: \'\[\]\' /} {param desc} {call buck.python_library /} rules used by
the tests in this rules sources. {/param} {/call} {call buck.arg} {param
name: \'labels\' /} {param default: \'\[\]\' /} {param desc} A list of
labels to be applied to these tests. These labels are arbitrary text
strings and have no meaning within buck itself. They can, however, have
meaning for you as a test author (e.g., `smoke` or `fast`). A label can
be used to filter or include a specific `python_test()` rule when
executing [`buck   test`](%7BROOT%7Dcommand/test.html). {/param} {/call}
{call buck.test_rule_timeout_ms /} {call test_common.contacts_arg /}
{call python_common.package_style_arg /} {call
python_common.preload_deps_arg /} {call python_common.linker_flags_arg
/} {/param} // close args {param examples} {literal}

``` {.prettyprint .lang-py}
# A rule that includes a single .py file containing tests.
python_test(
  name = 'fileutil_test',
  srcs = ['fileutil_tests.py'],
  deps = [
    ':fileutil',
  ],
)

# A rule that uses glob() to include all sources in the directory which the
# rule is defined.  It also lists a resource file that gets packaged with
# the sources in this rule.
python_library(
  name = 'fileutil',
  srcs = glob(['fileutil/**/*.py']),
  resources = [
    'testdata.dat',
  ],
)
```

{/literal}

Here is an example of using the \`platform_srcs\` and
\`platform_resources\` parameters to pull in sources/resources only when
building for a specific Python platform:

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
python_test(
  name = 'test',
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

{/literal}

Here is an example of using the \`platform\` parameter to select the
\"py2\" Python platform as defined in \`.buckconfig\` above:

{literal}

``` {.prettyprint .lang-py}
# BUCK
python_test(
  name = 'bin',
  platform = 'py2',
  srcs = [
    'foo.py',
  ],
)
```

{/literal} {/param} {/call} // close buck.rule {/param} {/call}
{/template}
