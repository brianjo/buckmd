/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.server} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'buck server\' /} {param navid: \'command_server\' /} {param
description} A command to find information about the http server run by
Buck. {/param} {param content} {call buck.command} {param overview} Find
information about the http server run by Buck.

    buck server status --http-port

## Commands

{/param} {param params} {call buck.param} {param name: \'json\' /}
{param desc} Outputs the results as JSON. {/param} {/call} {/param}
{/call} {/param} {/call} {/template}
