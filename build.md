/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.build} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'buck build\' /} {param navid: \'command_build\' /} {param prettify:
true /} {param description} A command that builds one or more specified
targets. {/param} {param content} {call buck.command} {param overview}

Builds one or more rules specified by a set of {call buck.build_target
/}s and {call buck.build_target_pattern /}s. This is the most commonly
used command in Buck.

Syntax:

    buck build { <build target> | <build target pattern> } . . .

Example:

    buck build //java/com/example/app:amazing

Note that any {call buck.remote_file /} rules referenced by your build
rules must be downloaded with {call buck.cmd_fetch /} prior to calling
this command unless you set `in_build = true   ` in the `[download]`
section of your {call buck.buckconfig_link /}.

{/param} {param params} {call buck.param} {param name: \'build-report\'
/} {param desc} Specifies a file where a JSON summary of the build
output should be written. Note that `--build-report` can be used without
`--keep-going`, though if `--keep-going` is not specified, the generated
report may be partial and not include information about the targets that
buck haven\'t had a chance to try to build. Here is a sample build
report:

``` {.prettyprint .lang-js}
{literal}
{
  "success": false,
  "results": {
    "//fake:rule1": {
      "success": true,
      "type": "BUILT_LOCALLY",
      "output": "buck-out/gen/fake/rule1.txt"
    },
    "//fake:rule2": {
      "success": false
    },
    "//fake:rule3": {
      "success": true,
      "type": "FETCHED_FROM_CACHE"
    }
  }
}
{/literal}
```

In this example, both `//fake:rule1` and `//fake:rule3` were built
successfully, but only `//fake:rule1` had an output file associated with
the rule.

Note that this contains the same information that `--keep-going` prints
to the console, but is easier to parse programmatically. This report may
contain more fields in the future. {/param} {/call} {call buck.param}
{param name: \'keep-going\' /} {param desc} When specified, Buck will
attempt to build all targets specified on the command line, even if some
of the targets fail. (Buck\'s default behavior is to exit immediately
when any of the specified targets fail.)

When `--keep-going` is specified, a report of the build will be printed
to stderr, detailing the build status of each target. Each line of the
report represents the status of one build target, which has up to four
columns:

1.  `OK` or `FAIL`, as per the success of the build rule.
2.  The build target of the rule.
3.  If successful, the type of the success as defined by the{sp}
    [`com.facebook.buck.core.build.engine.BuildRuleSuccessType`](https://buckbuild.com/javadoc/com/facebook/buck/core/build/engine/BuildRuleSuccessType.html)
    enum.
4.  If successful, the path to the output file of the rule, if it
    exists.

For example, if Buck were run with the following arguments:

    buck build
      --keep-going {nil}//fake:rule1 {nil}//fake:rule2 {nil}//fake:rule3
      

Then the report printed to stderr might look like:

      OK   {nil}//fake:rule1 BUILT_LOCALLY buck-out/gen/fake/rule1.txt{\n}
      FAIL {nil}//fake:rule2{\n}
      OK   {nil}//fake:rule3 FETCHED_FROM_CACHE{\n}
      

In this example, both `//fake:rule1` and `//fake:rule3` were built
successfully, but only `//fake:rule1` had an output file associated with
the rule. Admittedly, the state of column 1 could be derived from the
presence of column 3, but the encoding of column 1 makes it easier to
filter out successful rules from failed ones.

Note that when `--keep-going` is specified, the exit code will be 0 only
if all targets were built successfully.

This option is analogous to `-k/--keep-going` in Make. {/param} {/call}
{call buck.param} {param name: \'out\' /} {param desc} Takes the output
of the build target and copies it to the specified path. Only works with
a single build target, and the corresponding build rule must support
this option. {/param} {/call} {call buck.param} {param name:
\'populate-cache\' /} {param desc} Performs a cache population, which
makes the output of all unchanged transitive dependencies available (if
these outputs are available in the remote cache). Does not build changed
or unavailable dependencies locally. {/param} {/call} {call
command_common.show_output_param /} {call
command_common.common_param_xref /} {/param} {param examples}

### View compiler flags using the compilation database

For C++ builds, to view the compiler flags that Buck is passing to the
C++ compiler, tell Buck to generate a *compilation database* for the
target. The compilation database is a JSON file that contains
information about how Buck compiled the target. The syntax is:

{literal}

``` {.prettyprint .lang-bash}
buck build path/to/target#compilation-database
```

{/literal}

You can then get the path to the compilation-database file itself using:

{literal}

``` {.prettyprint .lang-bash}
buck targets --show-output path/to/target#compilation-database
```

{/literal}

For example:

{literal}

``` {.prettyprint .lang-bash}
$ buck clean
Parsing buck files: finished in 1.7 sec (100%)
Building: finished in 1.5 sec (100%) 3/3 jobs, 3 updated, 0.0% cache miss
  Total time: 3.7 sec

$ buck build :main#compilation-database
Building: finished in 1.5 sec (100%) 3/3 jobs, 3 updated, 0.0% cache miss
  Total time: 3.7 sec

$ buck targets --show-output :main#compilation-database
//:main#compilation-database buck-out/gen/__main#compilation-database/compile_commands.json

$ jq . buck-out/gen/__main#compilation-database/compile_commands.json 
[
  {
    "directory": "/Users/devuser/git/gtDev/C++/oop/simple-classes",
    "file": "/Users/devuser/git/gtDev/C++/oop/simple-classes/main.cpp",
    "arguments": [
      "/usr/bin/clang++",
      "-x",
      "c++",
      "-I",
      "buck-out/gen/main#default,private-headers.hmap",
      "-I",
      "buck-out",
      "-Xclang",
      "-fdebug-compilation-dir",
      "-Xclang",
      ".",
      "-fdebug-prefix-map=/Users/devuser/git/gtDev/C++/oop/simple-classes=.",
      "-c",
      "-MD",
      "-MF",
      "buck-out/gen/main#compile-main.cpp.oa5b6a1ba,default/main.cpp.o.dep",
      "main.cpp",
      "-o",
      "buck-out/gen/main#compile-main.cpp.oa5b6a1ba,default/main.cpp.o"
    ]
  }
]
```

{/literal}

In the preceding example `:main` specifies a *relative* build target
that is defined in the build file located in the current directory. The
`jq` tool---available through package managers such as
Homebrew---enables you to pretty-print JSON files.

{/param} // examples {/call} {/param} // content {/call} // buck.page
{/template}
