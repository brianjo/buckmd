/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.project} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'buck project\' /} {param navid: \'command_project\' /} {param
description} A command that generates the configuration files for an IDE
to work with the project. {/param} {param content} {call buck.command}
{param overview}

This command generates the configuration files for an IDE to work with
the project. This command creates files in-place in the repository,
which is unlike other Buck commands whose output is removed by {call
buck.cmd_clean /}. As a result, it is a good idea to add these generated
files to the list of ignored files by your choice of source control.
IDE-specific details are discussed in each section below.

You can use this command by itself to generate a project for the entire
repository.

{literal}

    buck project

{/literal}

You can also use this command to build a project slice (a project that
represents a subset of the repository). You can pass any number of {call
buck.build_target /}s or {sp}{call buck.build_target_pattern /}s to the
command. The constructed project slice will contain the specified
targets and their dependencies. This is useful for large repositories.

{literal}

    buck project //java/...

{/literal}

## Common Parameters

## Supported IDEs

-   [IntelliJ](#intellij)
-   [Xcode](#xcode)
-   [gobuild (Go IDEs such as Visual Sudio Code,
    GoLand)]{hred="#gobuild"}

### IntelliJ

This command processes all of the {sp}{call buck.build_file /}s whose
targets were specified and uses them to generate the configuration files
for an IDE. The generated files include:

-   `.idea/libraries/*.xml`, each of which defines a library in
    IntelliJ. A library always corresponds to a {call buck.prebuilt_jar
    /}.
-   `.iml` files, each of which defines a module in IntelliJ. A module
    can depend on other modules, as well as libraries. It should be
    noted that although Buck allows multiple build targets per build
    file, IntelliJ\'s modules are only defined at the directory level.
    This means that you may find IntelliJ flagging compilation errors
    because of missing dependencies of classes outside of your project
    slice, but which happen to be in the same directory as classes
    within the slice.
-   `.idea/modules.xml`, which lists all of the IntelliJ modules in the
    project.

### Xcode

This command processes each {call buck.apple_binary /}, {call
buck.apple_bundle /}, and {sp}{call buck.apple_library /} specified, and
uses them to generate the files and directories that Xcode needs. The
generated folders include:

-   For each {call buck.build_target /}, an `*.xcworkspace` directory
    that represents the {sp}
    [workspace](https://developer.apple.com/library/ios/featuredarticles/XcodeConcepts/Concept-Workspace.html)
    and contains one or more {sp}
    [schemes](https://developer.apple.com/library/ios/featuredarticles/XcodeConcepts/Concept-Schemes.html).
-   For each {call buck.build_target /} and its dependencies, an
    `*.xcodeproj` directory that represents the {sp}
    [project](https://developer.apple.com/library/ios/featuredarticles/XcodeConcepts/Concept-Projects.html).
    These generated projects are only buildable within the generated
    workspace.

#### Parameters

### Go IDEs {#gobuild}

Go IDEs, such as Visual Studio Code and GoLand, use the `go build`
command to build Go code. This command requires a proper layout of
source code under `GOPATH`. However, Buck puts generated code in
`buck-out`, which `go build` does not understand. The `project` command
copies generated Go packages from `buck-out` and arranges them in the
same layout as their import paths.

#### Parameters

{/param} {/call} {/param} // content {/call} // buck.page {/template}
