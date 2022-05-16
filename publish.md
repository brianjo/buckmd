/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.publish} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'buck publish\' /} {param navid: \'command_publish\' /} {param
prettify: true /} {param description} A command that builds one or more
specified targets and publishes them. {/param} {param content} {call
buck.command} {param overview}

A command that builds one or more {call buck.build_target /}s and
publishes them. This does not support {call buck.build_target_pattern
/}s.

{/param} {param params}

All parameters that can be passed to {call buck.cmd_build /} can be
passed to this command to control how the {call buck.build_target /}s
are built. The following parameters are also supported:

{call buck.param} {param name: \'dry-run\' /} {param desc}

Just print the artifact(s) that would be published for the specified{sp}
{call buck.build_target /}(s).

{/param} {/call} {call buck.param} {param name: \'include-source\' /}
{param alias: \'s\' /} {param desc}

Publish the source code in addition to the artifact(s) for the
specified{sp} {call buck.build_target /}(s).

{/param} {/call} {call buck.param} {param name: \'remote-repo\' /}
{param alias: \'r\' /} {param desc}

A url of the remote repository to publish artifact(s) for the
specified{sp} {call buck.build_target /}(s).

{/param} {/call} {call buck.param} {param name: \'username\' /} {param
alias: \'u\' /} {param desc}

The username to use when authenticating with the remote repository.

{/param} {/call} {call buck.param} {param name: \'password\' /} {param
alias: \'p\' /} {param desc}

The password to use when authenticating with the remote repository.

{/param} {/call} {call buck.param} {param name: \'to-maven-central\' /}
{param desc}

Equivalent to passing{sp}
`--remote-repo https://repo1.maven.org/maven2`.

{/param} {/call} {/param} // params {/call} // buck.param {/param} //
content {/call} // buck.page {/template}
