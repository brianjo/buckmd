/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.overview} /\*\*\*/ {template .soyweb} {call buck.page} {param
title: \'Key concepts\' /} {param navid: \'about_overview\' /} {param
description} An overview of some fundamental concepts in Buck. {/param}
{param content}

Buck has a number of fundamental concepts:

-   A ***{call buck.concept_link}{param name: \'build rule\' /}{param
    page: \'build_rule\' /}{/call}*** describes how to produce an output
    file from a set of input files. Most build rules are specific to a
    particular language or platform. For example, you would use the
    {call buck.cxx_binary /} rule to create a C++ binary, but you would
    use the {call buck.ruleLink}{param name : \'android_binary\'
    /}{/call} rule to create an Android APK.

-   A ***{call buck.concept_link}{param name: \'build target\' /}{param
    page: \'build_target\' /}{/call}*** is a string that uniquely
    identifies a build rule. It can be thought of as a URI for the build
    rule within the Buck project.

-   A ***{call buck.concept_link}{param name: \'build file\' /}{param
    page: \'build_file\' /}{/call}*** defines one or more build rules.
    In Buck, build files are typically named `BUCK`. A `BUCK` file is
    analogous to the `Makefile` used by the Make utility. In your
    project, you will usually have a separate `BUCK` file for each
    buildable unit of software---such as a binary or library. For large
    projects, you could have hundreds of `BUCK` files.

-   A Buck ***package*** comprises: a Buck build file (a `BUCK` file),
    all files---such as source files and headers---in the same directory
    as the `BUCK` file or in subdirectories, provided those
    subdirectories do not themselves contain a `BUCK` file. To say it
    another way, a `BUCK` file defines the root of a package, but Buck
    packages might not include all their subdirectories because Buck
    packages do not overlap or contain other Buck packages.

    For example, in the following diagram, the BUCK file in directory
    `app-dir-1` defines that directory as the root of a package---which
    is labeled **Package A** in the diagram. The directory `app-dir-2`
    is part of Package A because it is a subdirectory of `app-dir-1`,
    but does not itself contain a BUCK file.

    Now, consider directory `app-dir-3`. Because `app-dir-3` contains a
    BUCK file it is the root of a new package (**Package B**). Although
    `app-dir-3` is a subdirectory of `app-dir-1`, it is *not* part of
    Package A.

-   Buck has the concept of a ***cell***, which defines a directory tree
    of one or more Buck packages. A Buck build could involve multiple
    cells. Cells often correspond to repositories, but this isn\'t
    required.

    The root of a Buck cell contains a global configuration file called
    **`{call buck.buckconfig_link /}`**. Note that although the cell
    root should contain a `.buckconfig`, the presence of a `.buckconfig`
    file doesn\'t in itself define a cell. Rather, *the cells involved
    in a build are defined at the time Buck is invoked*; they are
    specified in the `.buckconfig` for the Buck *project* (see below).

-   A Buck ***project*** is defined by the `.buckconfig` where Buck is
    invoked, or if that directory doesn\'t contain a `.buckconfig`, the
    project is defined by the `.buckconfig` in the nearest ancestor
    directory.

    The `.buckconfig` for the project specifies the cells that
    constitute the Buck project. Specifically, these cells are specified
    in the {call buckconfig.repositories /} section of the
    `.buckconfig`. Note that the directory tree rooted at this
    `.buckconfig` is automatically considered a cell by Buck; in other
    words, the project\'s `.buckconfig` doesn\'t need to specify the
    project cell explicitly---although it is a good practice to do so.

### Buck\'s dependency graph

Every build rule can have zero or more dependencies. You can specify
these dependencies using, for example, the `deps` argument to the build
rule. For more information about specifying dependencies, consult the
reference page for the build rule you are using.

These dependencies form a directed graph, called the *target graph*.
Buck requires the graph to be acyclic. When building the output of a
build rule, all of the rule\'s transitive dependencies are built first.
This means that the graph is built in a \"bottom-up\" fashion. A build
rule knows only which rules it depends on, not which rules depend on it.
This makes the graph easier to reason about and enables Buck to identify
independent subgraphs that can be built in parallel. It also enables
Buck to determine the minimal set of build targets that need to be
rebuilt.

For more information about how Buck leverages the graph of build
dependencies, see {call buck.concept_link}{param page:
\'what_makes_buck_so_fast\' /}{param name: \'What Makes Buck so Fast\'
/}{/call}.

### Multiple Buck projects in a single repository

Buck is designed to build multiple deliverables from a single
repository---that is, a *monorepo*---rather than from multiple
repositories. Support for the monorepo design motivated Buck\'s support
for cells and projects.

It is Facebook\'s experience that maintaining all dependencies in the
same repository makes it easier to ensure that all developers have the
correct version of the code and simplifies the process of making atomic
commits.

{/param} {/call} {/template}
