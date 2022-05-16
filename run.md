/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.command.run} /\*\*\*/ {template .soyweb} {call buck.page} {param
title: \'buck run\' /} {param navid: \'command_run\' /} {param
description} A command that builds and runs an executable. {/param}
{param content} {call buck.command} {param overview}

This command builds and runs an executable resulting from building a
target.

    buck run {literal}//app:app-dist{/literal}

For Android/iOS rules which can\'t be run directly,
[`buck install -r`](install.html) should be used to install the result
of the build on the appropriate emulator/simulator.

## Common Parameters

All the parameters for [`buck build`](build.html) also apply to
`buck run`.

## Passing Arguments

Passing the `--` flag will cause all following arguments to be piped
through to the binary called by `buck run`. For example, calling

    buck run {literal}//:bin{/literal} --no-cache -- --foo=bar arg1 arg2

Will build `{literal}//:bin{/literal}` without the cache and call the
result with the arguments `["--foo=bar", "arg1", "arg2"]`

{/param} {/call} {/param} // content {/call} // buck.page {/template}
