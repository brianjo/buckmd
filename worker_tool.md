/\* \* Copyright (c) Meta Platforms, Inc. and affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.worker_tool} /\*\*\*/ {template .soyweb} {call buck.page} {param
title: \'worker_tool()\' /} {param navid: \'rule_worker_tool\' /} {param
prettify: true /} {param description} A rule to tell Buck that multiple
invocations of an external tool should be multiplexed to a shared
instance of that tool. {/param} {param content} {call buck.rule} {param
status: \'UNFROZEN\' /} {param overview}

Some external tools have high startup costs. To amortize those costs
over the whole build rather than paying them for each rule invocation,
use the `worker_tool()` rule in conjunction with {call buck.genrule /}.
Buck then starts the external tool once and reuses it by communicating
with it over `stdin` and `stdout` using a simple JSON protocol.

A `worker_tool` rule can be referenced in the `cmd` parameter of a
`genrule` by using the macro:

    {literal}
    $(worker //path/to:target)
    {/literal}

{/param} {param args} {call buck.name_arg /} {call buck.arg} {param
name: \'exe\' /} {param desc} A {call buck.build_target /} for a rule
that outputs an executable, such as an {call buck.ruleLink}{param name :
\'sh_binary\' /}{/call}. Buck runs this executable only once per build.
{/param} {/call} {call buck.arg} {param name: \'args\' /} {param
default: \'None\' /} {param desc} A string of args that is passed to the
executable represented by `exe` on initial startup. {/param} {/call}
{call buck.arg} {param name: \'max_workers\' /} {param default: \'1\' /}
{param desc} The maximum number of workers of this type that Buck
starts. Use `-1` to allow the creation of as many workers as necessary.
{/param} {/call} {call buck.arg} {param name:
\'max_workers_per_thread_percent\' /} {param default: \'None\'/} {param
desc} The maximum ratio of workers of this type that Buck starts per
thread, specified as a positive integer percentage{sp} (1-100). Must be
greater than or equal to `1` and less than or equal to `100`. Only one
of `max_workers` and `max_workers_per_thread_percent` may be specified.
{/param} {/call} {call buck.arg} {param name: \'env\' /} {param default:
\'None\' /} {param desc} A map of environment variables that is passed
to the executable represented by `exe` on initial startup. {/param}
{/call} {call buck.arg} {param name: \'persistent\' /} {param default:
\'False\' /} {param desc} If set to true, Buck does not restart the tool
unless the tool itself changes. This means the tool persists across
multiple Buck commands without being shut down and may see the same rule
being built more than once. Be careful not to use this setting with
tools that don\'t expect to process the same input---with different
contents---twice! {/param} {/call} {/param} {param examples}

Consider the following {call buck.concept_link}{param page:
\'build_rule\' /}{param name: \'build rules\' /}{/call}:

{literal}

``` {.prettyprint .lang-py}
#
# Buck
#
worker_tool(
  name = 'ExternalToolWorker',
  exe = ':ExternalTool',
  args = '--arg1 --arg2'
)

sh_binary(
  name = 'ExternalTool',
  main = 'external_tool.sh',
)

genrule(
  name = 'TransformA',
  out = 'OutputA.txt',
  cmd = '$(worker :ExternalToolWorker) argA',
)

genrule(
  name = 'TransformB',
  out = 'OutputB.txt',
  cmd = '$(worker :ExternalToolWorker) argB',
)

genrule(
  name = 'TransformC',
  out = 'OutputC.txt',
  cmd = '$(worker :ExternalToolWorker) argC',
)
```

{/literal}

When doing a `buck build` on all three of the above `genrules`, Buck
first creates the worker process by invoking:

    {literal}
    ./external_tool.sh --arg1 --arg2
    {/literal}

Buck then communicates with this process using JSON over `stdin`,
starting with a handshake:

{literal}

``` {.prettyprint .lang-py}
[
  {
    "id": 0,
    "type": "handshake",
    "protocol_version": "0",
    "capabilities": []
  }
```

{/literal}

Buck then waits for the tool to reply on `stdout`:

{literal}

``` {.prettyprint .lang-py}
[
  {
    "id": 0,
    "type": "handshake",
    "protocol_version": "0",
    "capabilities": []
  }
```

{/literal}

Then, when building the first `genrule`, Buck writes to `stdin`:

{literal}

``` {.prettyprint .lang-py}
  ,{
    "id": 1,
    "type": "command",
    "args_path": "/tmp/1.args",
    "stdout_path": "/tmp/1.out",
    "stderr_path": "/tmp/1.err"
  }
```

{/literal}

The file `/tmp/1.args` contains `argA`. The tool should perform the
necessary work for this job and then write the job\'s output to the
files supplied by Buck---in this case, `/tmp/1.out` and `/tmp/1.err`.
Once the job is done, the tool should reply to Buck on `stdout` with:

{literal}

``` {.prettyprint .lang-py}
  ,{
    "id": 1,
    "type": "result",
    "exit_code": 0
  }
```

{/literal}

Once Buck hears back from the first genrule\'s job, it submits the
second genrule\'s job in the same fashion and awaits the response. When
the build is all finished, Buck closes the JSON by writing to `stdin`:

{literal}

``` {.prettyprint .lang-py}
]
```

{/literal}

which signals the tool that it should exit after replying on `stdout`
with:

{literal}

``` {.prettyprint .lang-py}
]
```

{/literal}

In this example, Buck is guaranteed to invoke

    {literal}
    ./external_tool.sh --arg1 --arg2
    {/literal}

only once during the build. The three jobs corresponding to the three
genrules are submitted synchronously to the single worker process.

Note that the `id` values in the messages are not necessarily increasing
or sequential, but they do have to match between the request message and
the response message of a given job as well as in the initial handshake.

If the tool receives a message type it cannot interpret it should answer
with:

{literal}

``` {.prettyprint .lang-py}
{
  "id": &ltn>,
  "type": "error",
  "exit_code": 1
}
```

{/literal}

If the tool receives a message type it can interpret, but the other
attributes of the message are in an inconsistent state, it should answer
with:

{literal}

``` {.prettyprint .lang-py}
{
  "id": &ltn>,
  "type": "error",
  "exit_code": 2
}
```

{/literal} {/param} {/call} {/param} {/call} {/template}
