/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.intellij_plugin_install.soy} /\*\*\*/ {template .soyweb} {call
buck.page} {param title: \'Installing and using the IntelliJ Plugin\' /}
{param navid: \'setup_intellij_plugin_install\' /} {param prettify: true
/} {param description} How to install and use the Intellij Buck plugin
for your project. {/param} {param content}

To use the Buck Intellij Plugin you will have to install Buck, by
following the guide from{sp} {call buck.setup_install /}.

## Installing the plugin {#manual-install-buck}

You can download the plugin from
[here](https://plugins.jetbrains.com/plugin/7826-buck-for-idea) or
manually build it by following the guide from{sp} {call
buck.setup_build_intellij_plugin/}. After that, you can install it by
following the{sp} [Installing a Plugin from
Disk](https://www.jetbrains.com/help/idea/installing-a-plugin-from-disk.html)
guide.

## Using the plugin {#manual-use-intellij}

After you have installed it, you can view the Buck Plugin Tool Window by
accessing `View > Tool Windows > Buck`.

### Utility Functions {#buck-plugin-utility}

1.  Buck Code Completion

    Helps you complete the names of keywords and buck rule names within
    the visibility scope.

2.  Go to Buck File

    Jump to the BUCK file of current source file. To access it you can:

    -   `Tools > Buck > Go to Buck file`
    -   `Right click > Buck > Go to Buck file`
    -   `⇧ + ⌘ + P`

3.  Go to Buck Dependencies

    Quickly jump to other BUCK files with `⌘ + Click`{sp} or `⌘ + B`.

4.  Reformat BUCK files

    The Buck Plugin lets you reformat source code to meet the
    requirements of your code style. The plugin also supports customized
    spacing and indenting in the buck code style settings. You can
    access it by going to `Code > Reformat Code`{sp} or by pressing
    `⌥ + ⌘ + L`.

5.  Sort buck dependencies

    You can access it by going to `Code > Optimise Imports`{sp} or by
    pressing `^ + ⌥ + O`.

6.  Automatically Convert to Buck Dependencies after Paste in BUCK file

    For example:

    -   \"import com.example.activity.MyFirstActivity\" -\>
        \"//java/com/example/activity:activity\"
    -   \"package com.example.activity;\" -\>
        \"//java/com/example/activity:activity\"
    -   \"com.example.activity.MyFirstActivity\" -\>
        \"//java/com/example/activity:activity\"

7.  Error Annotation

    If a Buck dependency does not exist, it will be marked with red.

8.  Commenting and Uncommenting

    You can comment or uncomment selected lines of a BUCK file by
    accessing{sp} `Code > Comment with Line Comment` or by pressing
    `⌘ + /`.

### Executing Buck Commands {#buck-plugin-commands}

1.  Select target

    Before you start doing any of the below mentioned actions you will
    have to select a buck target.

    You can start selecting the buck target either by pressing the
    associated icon from the Buck Plugin tool window or by using
    `⇧ + ⌘ + J`.

    If you have an alias, you can just search for it. If you don\'t have
    an alias you have to write the whole path to the BUCK file. Once you
    are at the directory with the BUCK file, the plugin will search for
    all the available targets, which may take some time.

    You can use autocomplete by pressing → and navigate through the
    search by pressing ↑ and ↓.

2.  Build target

    Once you selected the target you can start a buck build either by
    pressing the associated icon from the Buck Plugin tool window or by
    using{sp} `⇧ + ⌘ + S`.

3.  Show Buck/compiler errors and easily go through them

    When building, you may receive compiler errors. You can easily
    navigate through them and on double click you will be sent to the
    appropriate column and line.

4.  Install target

    Once you selected the target you can start a buck install either by
    pressing the associated icon from the Buck Plugin tool window or by
    using{sp} `⇧ + ⌘ + X`.

5.  Uninstall target

    Once you selected the target you can start a buck uninstall either
    by pressing the associated icon from the Buck Plugin tool window or
    by using{sp} `⇧ + ⌘ + M`.

6.  Test target

    Once you selected the target you can start a buck test either by
    pressing the associated icon from the Buck Plugin tool window or by
    using{sp} `⇧ + ⌘ + Y`.

7.  Buck project target

    Once you selected the target you can start a buck project either by
    pressing the associated icon from the Buck Plugin tool window or by
    using{sp} `⇧ + ⌘ + B`.

8.  Buck kill

    Once you started one of the above mentioned actions you can stop it
    either by pressing the associated icon from the Buck Plugin tool
    window or by using{sp} `⇧ + ⌘ + L`.

### Settings {#buck-plugin-settings}

1.  Buck Settings

    You can set your buck executable path and other install settings by
    going to {sp} `Preferences > Tools > Buck`.

2.  Code Style Settings

    You can set code style settings by going to {sp}
    `Preferences > Editor > Code Style > Buck`.

3.  Colors & Font Settings

    You can set the syntax highlighting colors from{sp}
    `Preferences > Editor > Colors & Fonts > Buck`.

{/param} {/call} {/template}
