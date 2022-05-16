/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.buildtargetpattern} /\*\*\*/ {template .soyweb} {call buck.page}
{param title: \'Build Target Pattern\' /} {param navid:
\'concept_build_target_pattern\' /} {param description} A string that
describes a set of one or more build targets. {/param} {param content}

A *build target pattern* is a string that describes a set of one or more
{call buck.build_target /}s. You can use build target patterns as
arguments to commands, such as {call buck.cmd_build /} and {call
buck.cmd_query /}. You can also use build target patterns in the {call
buck.concept_link}{param page: \'visibility\' /}{param name:
\'Visibility\' /}{/call} argument of your build rules.

The simplest build target pattern matches the build target of the same
name:

    {literal}
    #
    # Matches //apps/myapp:app
    #
    //apps/myapp:app
    {/literal}

A build target pattern that ends with a colon matches all build targets
in the build file at the preceding directory path. For example, suppose
that the build file

    {literal}
    apps/myapp/BUCK
    {/literal}

defines the rules: `app_debug` and `app_release`, then the following
build target pattern would match both of those rules:

    {literal}
    #
    # Matches //apps/myapp:app_debug and //apps/myapp:app_release
    #
    //apps/myapp:
    {/literal}

A build target pattern that ends with an ellipsis (`/...`) matches all
build targets in the build file in the directory that precedes the
ellipsis and also *all build targets in build files in subdirectories*.
For example, suppose that you have the following build files:

    {literal}
    apps/BUCK
    apps/myapp/BUCK
    {/literal}

then the following pattern would match all build targets in both of
those files:

{literal}

    #
    # Matches (for example) //apps:common and //apps/myapp:app
    #
    //apps/...
    {/literal}

### Build target patterns are not allowed in the deps argument

Build target patterns cannot be used with the `deps` argument of a build
rule. Buck requires that you specify all dependencies explicitly as
either fully-qualified or relative build targets.

By making dependencies explicit, Buck prevents build rules from
*inadvertently* adding new dependencies, which can result in
non-reproducible builds. In addition, if the added dependencies are not
actually required, they can unnecessarily drive up the computational
cost of the build.

### Target aliases

Buck supports the ability to define *aliases* for build targets; using
aliases can improve brevity when specifying targets on the Buck command
line. For more information, see the {call buckconfig.alias /} section in
the documentation for {call buck.buckconfig_link /}.

{/param} {/call} {/template}
