/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.root} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'buck root\' /} {param navid: \'command_root\' /} {param prettify: true
/} {param description} A command that prints the absolute path to the
root of the buck project. {/param} {param content} {call buck.command}
{param overview}

A command that prints out the absolute path to the root directory of the
current buck project. This is useful from within scripts to help with
navigating the project tree.

    buck root

    /home/buck/example

{/param} // overview {param params} This command takes no parameters.
{/param} {/call} // buck.command {/param} // content {/call} //
buck.page {/template}
