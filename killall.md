/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.killall} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'buck killall\' /} {param navid: \'command_killall\' /} {param
description} Kill all the Buck Daemon (buckd) processes running on the
host computer. {/param} {param content} {call buck.command} {param
overview}

Kill *all* the {sp}{call buck.concept_link}{param page: \'buckd\'
/}{param name: \'Buck Daemon (`buckd`)\' /}{/call}{sp} processes that
are running on the host computer.

To kill only the Buck Daemon process for the *current* Buck {call
buck.key_concepts_link}{param rendered_text: \'project\' /}{/call}, use
{call buck.cmd_kill /}.

In general, we recommend using `buck kill` rather than `buck killall`.
The `buck killall` command is an aggressive way of terminating the
`buckd` processes and might leave your build environment in an
inconsistent state.

{/param} // overview {/call} // buck.command {/param} // content {/call}
// buck.page {/template}
