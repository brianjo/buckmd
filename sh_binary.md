/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
sh_binary} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'sh_binary()\' /} {param navid: \'rule_sh_binary\' /} {param prettify:
true /} {param description} A rule that is used to invoke a shell
script. {/param} {param content} {call buck.rule} {param status:
\'UNFROZEN\' /} {param overview} A `sh_binary()` is used to execute a
shell script. {/param} {param args} {call buck.name_arg /} {call
buck.arg} {param name: \'main\' /} {param desc} Either the path to the
script (relative to the build file), or a {call buck.build_target /}.
This file must be executable in order to be run. {/param} {/call} {call
buck.arg} {param name: \'resources\' /} {param default: \'\[\]\' /}
{param desc} A list of files or build rules that this rule requires in
order to run. These could be things such as random data files.

When the script runs, the `$BUCK_DEFAULT_RUNTIME_RESOURCES` environment
variable specifies the directory that contains these resources. This
directory\'s location is determined entirely by Buck; the script should
not assume the directory\'s location.

The `$BUCK_EXTERNAL_RUNTIME_RESOURCES` variable is also defined.
Resources that are targets from external cells are placed in this
directory.

The resources are also made available in a tree structure that mirrors
their locations in the source and `buck-out` trees. The environment
variable `$BUCK_PROJECT_ROOT` specifies a directory that contains all
the resources, laid out in their locations relative to the original buck
project root.

{/param} {/call} {/param} // args {param examples}

This sh_binary() just cats a sample data file back at the user.

{literal}

``` {.prettyprint .lang-py}
# $REPO/BUCK
sh_binary(
    name = "script",
    main = "script.sh",
    resources = [
        "data.dat",
    ],
)
```

{/literal} {literal}

``` {.prettyprint .lang-sh}
# Sample data file with data we need at runtime
$ echo "I'm a datafile" > data.dat

# Create a simple script that prints out the resource
$ cat > script.sh
#!/bin/sh
cat $BUCK_DEFAULT_RUNTIME_RESOURCES/data.dat

# Make sure the script is executable
$ chmod u+x script.sh

# Run the script, and see that it prints out the resource we provided
$ buck run //:script
Building: finished in 1.9 sec (100%) 1/1 jobs, 1 updated
  Total time: 2.1 sec
I'm a datafile
```

{/literal} {/param} // examples {/call} // buck.rule {/param} {/call}
{/template}
