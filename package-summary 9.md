<div>

JavaScript is disabled on your browser.

</div>

::: {role="banner"}
::: fixedNav
::: topNav
[]{#navbar.top}

::: skipNav
[Skip navigation links](#skip.navbar.top "Skip navigation links")
:::

[]{#navbar.top.firstrow}

-   [Overview](../../../../../../index.html)
-   Package
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

```{=html}
<!-- -->
```
-   SEARCH:

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Package com.facebook.buck.support.cli.args {#package-com.facebook.buck.support.cli.args .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [PluginBasedCommand](PluginBa     | ::: block                         |
    | sedCommand.html "interface in com | An abstract class that provides   |
    | .facebook.buck.support.cli.args") | basic capabilities for commands   |
    |                                   | that use subcommands loaded from  |
    |                                   | plugins.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [P                                | ::: block                         |
    | luginBasedSubCommand](PluginBased | A common interface that needs to  |
    | SubCommand.html "interface in com | be implemented by subcommands     |
    | .facebook.buck.support.cli.args") | loaded from plugins.              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PluginBasedSubComm               | ::: block                         |
    | andFactory](PluginBasedSubCommand | Creates an instance of            |
    | Factory.html "interface in com.fa | [`Pl                              |
    | cebook.buck.support.cli.args")\<T | uginBasedSubCommand`](PluginBased |
    | extends                           | SubCommand.html "interface in com |
    | [Plu                              | .facebook.buck.support.cli.args") |
    | ginBasedSubCommand](PluginBasedSu | used by plugin-based subcommands  |
    | bCommand.html "interface in com.f | framework.                        |
    | acebook.buck.support.cli.args")\> | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [BuckArgsMethods](B               | ::: block                         |
    | uckArgsMethods.html "class in com | Utility class for methods related |
    | .facebook.buck.support.cli.args") | to args handling.                 |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuckCellAr                       | ::: block                         |
    | g](BuckCellArg.html "class in com | Helps parse common command line   |
    | .facebook.buck.support.cli.args") | argument formats                  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CmdLineParserWithPrin            | ::: block                         |
    | tInformation](CmdLineParserWithPr | An implementation of              |
    | intInformation.html "class in com | `CmdLineParser` that can provide  |
    | .facebook.buck.support.cli.args") | some information that can be used |
    |                                   | to print help in more flexible    |
    |                                   | form than `CmdLineParser`.        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [GlobalCliOptions](Gl             | ::: block                         |
    | obalCliOptions.html "class in com | Contains CLI options that are     |
    | .facebook.buck.support.cli.args") | common to all of the commands.    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PluginBasedCo                    | ::: block                         |
    | mmandHelpPrinter](PluginBasedComm | A helper class that encapsulate   |
    | andHelpPrinter.html "class in com | printing of usage tests for a     |
    | .facebook.buck.support.cli.args") | given command                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Annotation Type                   | Description                       |
    +===================================+===================================+
    | [Plug                             | ::: block                         |
    | inBasedSubCommands](PluginBasedSu | This annotation indicates that    |
    | bCommands.html "annotation in com | the options should be loaded      |
    | .facebook.buck.support.cli.args") | using plugin framework.           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Annotation Types Summary[ ]{.tabEnd}
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../../../index.html)
-   Package
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

[]{#skip.navbar.bottom}
:::
