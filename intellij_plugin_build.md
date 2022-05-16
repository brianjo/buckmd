/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.intellij_plugin_build.soy} /\*\*\*/ {template .soyweb} {call
buck.page} {param title: \'Building the IntelliJ Plugin\' /} {param
navid: \'rule_intellij_plugin_build\' /} {param prettify: true /} {param
description} How to build and setup the Intellij Buck plugin for your
project. {/param} {param content}

To build the Buck Intellij Plugin you will have to install Buck, by
following the guide from{sp} {call buck.setup_install /}, the manual
build process to get the repo.

## Building with Buck {#manual-build-buck}

{literal}

    cd third-party/java/intellij/
    sh get_jars.sh "PathToYourIntellijLib" #for unix systems
    get_jars.bat "PathToYourIntellijLib"   #for windows systems
    buck build ideabuck

{/literal} Once you have built the plugin, you can install it by
following the{sp} [Installing a Plugin from
Disk](https://www.jetbrains.com/help/idea/installing-a-plugin-from-disk.html)
guide. In order to access it you have to go to
`View > Tool Windows > Buck`.

## Building with Intellij {#manual-build-intellij}

The ideabuck plugin can also be built with intellij. A big advantage of
this, when working on the plugin, is the fact that you can easily debug
it by creating a new Run/Debug Configuration.

1.  Generate the grammar and the lexer with the Grammar-Kit plugin.
    -   You can install the grammar kit plugin from{sp}
        `third-party/java/grammar-kit/grammar-kit.jar` by following
        the{sp} [Installing Plugin from
        Disk](https://www.jetbrains.com/idea/help/installing-plugin-from-disk.html)
        guide. After you installed Grammar-Kit you can generate the
        files by navigating in Intellij to {literal}

            tools/ideabuck/src/com/facebook/buck/intellij/ideabuck/lang/Buck.bnf
            tools/ideabuck/src/com/facebook/buck/intellij/ideabuck/lang/Buck.flex
                      

        {/literal} and pressing `ctrl-shift-G / meta-shift-G`.

    -   If you don\'t want to install the Grammar-Kit plugin you can run
        {literal}

            python tools/ideabuck/scripts/generate_grammar_kit.py
                      

        {/literal}

        The above mentioned commands will create a `gen` directory in
        {sp} `tools/ideabuck`.
2.  [Configure the Intellij Platform Plugin
    SDK](https://www.jetbrains.com/idea/help/configuring-intellij-platform-plugin-sdk.html)
    and set it as the{sp} [SDK of ideabuck
    module](https://www.jetbrains.com/help/idea/sdk.html#change-module-sdk).
    If you don\'t see \"ideabuck\" in the `Project Settings/Modules`,
    you need to first import ideabuck module by right clicking on
    `tools/ideabuck/ideabuck.iml` and choose `Import "ideabuck" Module`
3.  Remove the Buck Intellij Plugin, `tools/ideabuck` from{sp} [the
    Compiler Excludes
    list](https://www.jetbrains.com/help/idea/15.0/compiler-excludes.html?origin=old_help).
4.  [Create a new Plugin Run/Debug
    configuration](https://www.jetbrains.com/idea/help/creating-and-editing-run-debug-configurations.html#createExplicitly)
    for the Buck Intellij Plugin.
5.  Run/Debug the plugin or create a new release of it by going to
    ` Build > Prepare all plugin modules for deployment`.

{/param} {/call} {/template}
