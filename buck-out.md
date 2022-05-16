/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.buck_out} /\*\*\*/ {template .soyweb} {call buck.page} {param
title: \'buck-out\' /} {param navid: \'buck-out\' /} {param description}
Output directory for build artifacts. {/param} {param prettify: true /}
{param content}

Buck stores build artifacts in a directory named `buck-out` in the root
of your {call buck.key_concepts_link}{param rendered_text: \'project\'
/}{/call}.

You should not make assumptions about where Buck places your build
artifacts within the directory structure beneath `buck-out` as these
locations depend on Buck\'s implementation and could potentially change
over time. Instead, to obtain the location of the build artifact for a
particular target, use the `--show-output` option with the {call
buck.cmd_build /} or the {call buck.cmd_targets /} command.

    {literal}
    buck targets --show-output <target>
    {/literal}

    {literal}
    buck build --show-output <target>
    {/literal}

You can also obtain the locations of your build artifacts by specifying
either the `--build-report` or `--keep-going` options with `buck build`.

Note that `--show-output` is going to be deprecated soon for
`buck build`   and replaced with `--show-outputs`. `--show-outputs` may
print more than one build artifact per build target.

    {literal}
    buck build --build-report <target>
    {/literal}

    {literal}
    buck build --keep-going <target>
    {/literal}

For more information about these options, see the topics for the {call
buck.cmd_build /} and {call buck.cmd_targets /} commands.

{/param} {/call} {/template}
