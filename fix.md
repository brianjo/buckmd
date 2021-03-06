/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.fix} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'buck fix\' /} {param navid: \'command_fix\' /} {param prettify: true
/} {param description} A command that attempts to fix errors and
warnings encountered during the previous command. {/param} {param
content} {call buck.command} {param overview}

Attempts to fix errors and warnings encountered during the previous
command.

Commands such as {call buck.cmd_build /} may fail with errors from Buck
itself or another tool (such as a compiler or linker) that is invoked by
Buck. In some cases, such errors can be fixed automatically. In such
cases, running

    buck fix

may fix the error.

`buck fix` prints nothing to the console unless a catastrophic failure
occurs.

Note that `buck fix` will edit files in place. It is therefore
recommended that any pending changes be saved to source control before
running this command.

{/param} {/call} {/param} // content {/call} // buck.page {/template}
