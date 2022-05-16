/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.build_rule} /\*\*\*/ {template .soyweb} {call buck.page} {param
title: \'Build Rule\' /} {param navid: \'concept_build_rule\' /} {param
description} A procedure for producing output files from a set of input
files in the context of a specified build configuration. {/param} {param
content}

A *build rule* is a procedure for producing output files from a set of
input files in the context of a specified build configuration. Build
rules are specified in {call buck.build_file /}s---typically named BUCK.

**Note:** A build rule must explicitly specify, in its arguments, all of
its required inputs in order for Buck to be able to build the rule\'s
output in a way that is deterministic and reproducible.

## Buck\'s collection of build rules

Buck comes with a collection of built-in build rules for many common
build procedures. For example, compiling Java code against the Android
SDK is a common procedure, so Buck provides the build rule {sp}{call
buck.android_library /} to do that. Similarly, the final product of most
Android development is an APK, so you can use the build rule {sp}{call
buck.android_binary /} to create an APK.

This documentation organizes Buck\'s build rules by development language
and by target platform. Examples are: **C++**, **Java**, **Python**
(development languages) and **Android**, **iOS**, **.NET** (target
platforms). Consult the table of contents to locate the build rules that
are appropriate for your development project.

You can view a list of Buck\'s build rules from the command line with
the command:

    {literal}
    buck audit ruletypes
    {/literal}

You can view the arguments supported by a particular rule with the
command:

    {literal}
    buck audit ruletype <rule>
    {/literal}

Note that the first of these commands uses the *plural* `ruletypes`, and
the second uses the *singular* `ruletype`. For more information, see the
{call buck.cmd_audit /} documentation.

## Source files as inputs to build rules

Most build rules specify source files as inputs. For example, a {call
buck.cxx_library /} rule would specify `.cpp` files as inputs. To
support specifying these files, a `cxx_library` rule provides the `srcs`
argument. Some languages, such as C++, use header files as well. To
specify these, `cxx_library` provides a `headers` argument.

In addition to `srcs` and `headers`, some rules provide variants of
these arguments, such as `platform_srcs` and `platform_headers`. These
arguments support groups of source files that should be used as inputs
only when building for specific platforms. For more information, see the
descriptions for `platform_srcs` and {sp}`platform_headers` in, for
example, the {call buck.cxx_library /} topic.

### Package boundaries and access to source files

In Buck, a BUCK file defines a *package*, which corresponds *roughly* to
the directory that contains the BUCK file and those subdirectories that
do not themselves contain BUCK files. (To learn more, see the {call
buck.key_concepts_link}{param rendered_text: \'Key Concepts\' /}{/call}
topic.)

A rule in a BUCK file cannot specify a source file as an input unless
that source file is in that BUCK file\'s package. An exception to this
restriction exists for header files, but only if a rule in the package
that contains the header file *exports* that header file using the
`exported_headers` argument. For more details, see the description for
`exported_headers` in, for example, the {call buck.cxx_library /} topic.

More commonly though, the package for a BUCK file contains all the
source files required for the rules defined in that BUCK file.
Functionality in source files from other packages is made available
through the artifacts produced by the rules in the BUCK files for those
packages. For example, a {call buck.cxx_binary /} might use the
functionality in a `cxx_library` that is defined in another package. To
access that functionality, the `cxx_binary` would take that
`cxx_library` as a *dependency*.

##### Symlinks: Use with caution if at all

We recommend that you do *not* use symlinks---either absolute or
relative---to specify input files to build rules. Although using
symlinks in this context does sometimes work, it can lead to unexpected
behavior and errors.

## Dependencies: Output from one rule as input to another rule

A build rule can use the output from another build rule as one of its
inputs by specifying that rule as a *dependency*. Typically, a build
rule specifies its dependencies as a list of {call buck.build_target /}s
in its `deps` argument. However, the rule can also specify
dependencies---as build targets---in other arguments, such as `srcs`.

**Example:** The output of a {call buck.java_library /}{sp} rule is a
JAR file. If a `java_library`{sp} rule specifies another `java_library`
rule as a dependency, the JAR file produced by the specified rule is
added to the classpath for the `java_library` that depends on it.

**Example:** If a {call buck.java_binary /}{sp} rule specifies a
`java_library` rule as a dependency, the JAR file for the specified
`java_library` is available on the classpath for the `java_binary`. In
addition, in the case of `java_binary`, the JAR files for any
dependencies of the `java_library` rule *are also* made available to the
`java_binary` rule---and if those dependencies have dependencies of
their own, they are added as well. This exhaustive cascade of
dependencies is referred to as the rule\'s *transitive closure*.

### Required dependencies are always built first

Buck guarantees that any dependencies that a rule lists that are
required in order to build that rule are built successfully *before*
Buck builds the rule itself. Note though that there can be special
cases---such as {call buck.apple_bundle /}---where a rule\'s listed
dependencies do not actually need to be built before the rule.

### Visibility

In order for a build rule to take a dependency on another build rule,
the build rule on which the dependency is taken must be *visible* to the
build rule taking the dependency. A build rule\'s `visibility` argument
is a list of {call buck.build_target_pattern /}s that specify the rules
that can take that rule as a dependency. For more information about the
concept of visibility in Buck, see the {call buck.concept_link}{param
page: \'Visibility\' /}{param name: \'Visibility\' /}{/call} topic.

### Dependencies define a graph

Build rules and their dependencies define a directed acyclic graph
(DAG). Buck requires this graph to be acyclic to make it possible to
build independent subgraphs in parallel.

## How to handle special cases: genrules and macros

Although Buck provides a rich set of built-in build rules for
developers, it is not able to address all possible needs. As an \"escape
hatch,\" Buck provides a category of generic build rules called
*genrules*. With genrules, you can perform arbitrary operations using
shell scripts. The genrules supported by Buck are:

-   {call buck.genrule /}
-   {call buck.apk_genrule /}
-   {call buck.cxx_genrule /}

### Multiple output files with genrules

In most cases, a build rule produces exactly one output file. However,
with genrules, you can specify an output *directory* and write arbitrary
files to that directory.

### Macros

Finally, note that you can define functions that generate build rules.
In general, this should not be something that you need to do, but taking
advantage of this option might help you add needed functionality to
Buck\'s without editing its source code. For more details, see the
{sp}[Custom Macros](%7BROOT%7Dextending/macros.html) topic.

{/param} {/call} {/template}
