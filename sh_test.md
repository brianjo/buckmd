/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
sh_test} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'sh_test()\' /} {param navid: \'rule_sh_test\' /} {param prettify: true
/} {param description} A rule that runs a test by invoking a shell
script. {/param} {param content} {call buck.rule} {param status:
\'UNFROZEN\' /} {param overview}

A `sh_test()` is a test rule that can pass results to the test runner by
invoking a shell script.

**NOTE:** This rule is not currently supported on Windows. {/param}
{param args} {call buck.name_arg /} {call buck.arg} {param name:
\'test\' /} {param desc} Either the path to the script (relative to the
build file), or a {call buck.build_target /}. This file must be
executable in order to be run. {/param} {/call} {call buck.arg} {param
name: \'args\' /} {param default: \'\[\]\' /} {param desc} The list of
arguments to invoke this script with. These are literal values, and no
shell interpolation is done. These can contain {call
buck.string_parameter_macros /}, for example, to give the location of a
generated binary to the test script. {/param} {/call} {call buck.arg}
{param name: \'env\' /} {{param default: \'{}\' /}} {param desc}
Environment variable overrides that should be used when running the
script. The key is the variable name, and the value is its value. The
values can contain {call buck.string_parameter_macros /} such as the
location of a generated binary to be used by the test script. {/param}
{/call} {call buck.arg} {param name: \'type\' /} {param default:
\'None\' /} {param desc} If provided, this will be sent to any
configured {call buckconfig.entry_link}{param section: \'test\' /}{param
entry: \'external_runner\' /}{param link_text: \'external runner\'
/}{/call} {/param} {/call} {call test_common.contacts_arg /} {/param} //
args {param examples}

This sh_test() fails if a string does not match a value.

{literal}

``` {.prettyprint .lang-py}
# $REPO/BUCK
sh_test(
    name = "script_pass",
    test = "script.sh",
    args = ["--pass"],
)

sh_test(
    name = "script_fail",
    test = "script.sh",
    args = ["--fail"],
)
```

{/literal} {literal}

``` {.prettyprint .lang-sh}
# Create a simple script that prints out the resource
$ cat > script.sh
#!/bin/sh
for arg in $@; do
  if [ "$arg" == "--pass" ]; then
    echo "Passed"
    exit 0;
  fi
done
echo "Failed"
exit 1

# Make sure the script is executable
$ chmod u+x script.sh

# Run the script, and see that one test passes, one fails
$ buck test //:script_pass //:script_fail
FAILURE script.sh sh_test
Building: finished in 0.0 sec (100%) 2/2 jobs, 0 updated
  Total time: 0.0 sec
Testing: finished in 0.0 sec (1 PASS/1 FAIL)
RESULTS FOR //:script_fail //:script_pass
FAIL    <100ms  0 Passed   0 Skipped   1 Failed   //:script_fail
FAILURE script.sh sh_test
====STANDARD OUT====
Failed

PASS    <100ms  1 Passed   0 Skipped   0 Failed   //:script_pass
TESTS FAILED: 1 FAILURE
Failed target: //:script_fail
FAIL //:script_fail
```

{/literal} {/param} // examples {/call} // buck.rule {/param} {/call}
{/template}
