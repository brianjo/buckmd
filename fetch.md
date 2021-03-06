/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.fetch} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'buck fetch\' /} {param navid: \'command_fetch\' /} {param prettify:
true /} {param description} A command that downloads remote artifacts
from the Internet. {/param} {param content} {call buck.command} {param
overview}

A command that fetches one or more resources defined by {call
buck.remote_file /} rules. This should generally be run before {call
buck.cmd_build /} if {call buck.remote_file /} rules are used in the
repository. You must specify one or more {call buck.build_target /}s on
the command line.

Buck will look at the transitive dependencies of the target you specify,
so it is usually best to specify your top-level target in order to get
all the remote objects you require.

    buck fetch //third-party/jetty:jetty-source

We strongly believe that you and your team will have a better experience
if you check your dependencies into your repository and use one of the
provided `prebuilt_` rules instead. The Buck team encourages you to stop
trying to make fetch happen.

{/param} {param params} {call buck.param} {param name: \'verbose\' /}
{param alias: \'v\'/} {param desc} How verbose logging to the console
should be, with 1 as the minimum and 10 as the most verbose. {/param}
{/call} {/param} {/call} {/param} // content {/call} // buck.page
{/template}
