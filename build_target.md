/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.build_target} /\*\*\*/ {template .soyweb} {call buck.page} {param
title: \'Build Target\' /} {param navid: \'concept_build_target\' /}
{param prettify: true /} {param description} A string that is used to
identify a build rule in a project. {/param} {param content}

A *build target* is a string that identifies a build rule in your
project. Build targets are used as arguments to Buck commands, such as
{call buck.cmd_build /} and {call buck.cmd_run /}. Build targets are
also used as arguments to {call buck.concept_link}{param page:
\'build_rule\' /}{param name: \'build rules\' /}{/call} to enable one
build rule to reference another. For example, a build rule might use a
build target to reference another rule in order to specify that rule as
a *dependency*.

#### Fully-qualified build targets

Here is an example of a *fully-qualified* build target:

    {literal}
    //java/com/facebook/share:ui
    {/literal}

A fully-qualified build target has three components:

1.  The `//` prefix indicates that the subsequent path is from the
    *root* of your project. You can use the {call buck.cmd_root /}
    command to identify the root of your project.
2.  The `java/com/facebook/share` between the `//` prefix and the colon
    (`:`) indicates that the {call buck.build_file /} (usually named
    `BUCK`) is located in the directory{sp} `java/com/facebook/share`.
3.  The `ui` after the colon (`:`) indicates the name of the build rule
    within the build file. Build rule names must be unique within a
    build file. By *name* we mean, more formally, the value of the
    `name` argument to the build rule.

Note that the name of the build file itself---usually BUCK---does *not*
occur in the build target. All build files within a given Buck project
must have the same name---defined in the {call buckconfig.buildfile_name
/} entry of `.buckconfig`. Therefore, it is unnecessary to include the
name in the target.

The full regular expression for a fully-qualified build target is as
follows:

{literal}

    [A-Za-z0-9._-]*//[A-Za-z0-9/._-]*:[A-Za-z0-9_/.=,@~+-]+
    |- cell name -|  | package path | |--- rule name ----|

{/literal}

In Buck, a *cell* defines a directory tree of one or more Buck packages.
For more information about Buck cells and their relationship to packages
and projects, see the {call buck.key_concepts_link}{param rendered_text:
\'Key Concepts\' /}{/call} topic.

**NOTE:** All target paths are assumed to start from the root of the
Buck project. Buck does not support specifying a target path that starts
from a directory below the root. Although the double forward slash
(`//`) that prefixes target paths can be ommitted when specifying a
target from the command line (see **Pro Tips** below), Buck still
assumes that the path is from the root. Buck does support *relative*
build paths, but in Buck, that concept refers to specifying build
targets *from within* a build file. See **Relative build targets** below
for more details.

#### Relative build targets

A *relative* build target can be used to reference a {call
buck.build_rule /} *within the same {call buck.build_file /}*. A
relative build target starts with a colon (`:`) and is followed by only
the third component (or *short name*) of the fully-qualified build
target.

The following snippet from a build file shows an example of using a
relative path.

``` {.prettyprint .lang-py}
{literal}
#
# Assume this rule is in //java/com/facebook/share/BUCK
#
java_binary(
  name = 'ui_jar',
  deps = [
    #
    # The following target path
    #
    #   //java/com/facebook/share:ui
    #
    # is the same as using the following relative path.
    #
    ':ui',
  ],
)
{/literal}
```

## Command-line Pro Tips

Here are some ways that you can reduce your typing when you specify
build targets as command-line arguments to the {call buck.cmd_build /}
or {call buck.cmd_run /} commands.

Consider the following example of a fully-qualified build target used
with the `buck build` command:

    {literal}
    buck build //java/com/facebook/share:share
    {/literal}

Although Buck is always strict when parsing build targets in build
files, Buck is flexible when parsing build targets on the command-line.
Specifically, the leading `//` is optional on the command line, so the
above could be:

    {literal}
    buck build java/com/facebook/share:share
    {/literal}

Also, if there is a forward slash before the colon, it is ignored, so
this could also be written as:

    {literal}
    buck build java/com/facebook/share/:share
    {/literal}

which enables you to produce the red text shown below using
tab-completion, which dramatically reduces how much you need to type:

    {literal}
    buck build java/com/facebook/share/:share
    {/literal}

Finally, if the final path element matches the value specified after the
colon, it can be omitted:

    # This is treated as //java/com/facebook/share:share.

    buck build java/com/facebook/share/

which makes the build target even easier to tab-complete. For this
reason, the name of the build rule for the primary deliverable in a
build file is often named the same as the parent directory. That way, it
can be built from the command-line with less typing.

## See also

Buck supports the ability to define ***aliases* for build targets**;
using aliases can improve brevity when specifying targets on the Buck
command line. For more information, see the {call buckconfig.alias /}
section in the documentation for {call buck.buckconfig_link /}.

A **{call buck.build_target_pattern /}** is a string that describes a
set of one or more build targets. For example, the pattern `//...` is
used to build an entire project. For more information, see the **Build
Target Pattern** topic.

{/param} {/call} {/template}
