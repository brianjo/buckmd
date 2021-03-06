/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.kill} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'buck kill\' /} {param navid: \'command_kill\' /} {param description}
Kill the Buck Daemon (buckd) for the current project. {/param} {param
content} {call buck.command} {param overview}

Kill the {sp}{call buck.concept_link}{param page: \'buckd\' /}{param
name: \'Buck Daemon (`buckd`)\' /}{/call}{sp} for the current project.
To kill all the Buck Daemon processes running on the host computer, use
{call buck.cmd_killall /}.

For an explanation of Buck\'s concept of a *project*, see the the {call
buck.key_concepts_link}{param rendered_text: \'Key Concepts\' /}{/call}
topic.

{/param} // overview {/call} // buck.command {/param} // content {/call}
// buck.page {/template}
