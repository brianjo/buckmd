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

-   [Overview](../../../../../../../../index.html)
-   Package
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../../index-all.html)
-   [Help](../../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../../allclasses.html)

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
# Package com.facebook.buck.core.rules.actions.lib.args {#package-com.facebook.buck.core.rules.actions.lib.args .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [CommandLine](CommandLine.        | ::: block                         |
    | html "interface in com.facebook.b | Information needed to execute a   |
    | uck.core.rules.actions.lib.args") | command line program.             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | CommandLineArgs](CommandLineArgs. | Container for a list of objects   |
    | html "interface in com.facebook.b | that can be stringified into      |
    | uck.core.rules.actions.lib.args") | command line arguments for an     |
    |                                   | action that executes a program.   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Comma                            | ::: block                         |
    | ndLineArgs.ArgAndFormatString](Co | Simple container that holds a     |
    | mmandLineArgs.ArgAndFormatString. | single argument, and a formatting |
    | html "interface in com.facebook.b | string that should be run after   |
    | uck.core.rules.actions.lib.args") | [`Co                              |
    |                                   | mmandLineArgs.ArgAndFormatString. |
    |                                   | getObject()`](CommandLineArgs.Arg |
    |                                   | AndFormatString.html#getObject()) |
    |                                   | has been stringified (containing  |
    |                                   | a single %s).                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Comman                           | ::: block                         |
    | dLineArgsApi](CommandLineArgsApi. | Simple interface to expose        |
    | html "interface in com.facebook.b | [`C                               |
    | uck.core.rules.actions.lib.args") | ommandLineArgs`](CommandLineArgs. |
    |                                   | html "interface in com.facebook.b |
    |                                   | uck.core.rules.actions.lib.args") |
    |                                   | to skylark.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Comman                           | ::: block                         |
    | dLineBuilder](CommandLineBuilder. | Build a \"command line\" from     |
    | html "interface in com.facebook.b | [`Co                              |
    | uck.core.rules.actions.lib.args") | mmandLineArgs`](CommandLineArgs.h |
    |                                   | tml "interface in com.facebook.bu |
    |                                   | ck.core.rules.actions.lib.args"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [CommandLin                       | ::: block                         |
    | eArgsFactory](CommandLineArgsFact | Factory class that returns more   |
    | ory.html "class in com.facebook.b | efficient implementations of      |
    | uck.core.rules.actions.lib.args") | [`C                               |
    |                                   | ommandLineArgs`](CommandLineArgs. |
    |                                   | html "interface in com.facebook.b |
    |                                   | uck.core.rules.actions.lib.args") |
    |                                   | depending on what type of         |
    |                                   | arguments are available (e.g.     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CommandLineArgSt                 | ::: block                         |
    | ringifier](CommandLineArgStringif | Helper methods to convert /       |
    | ier.html "class in com.facebook.b | validate objects that are command |
    | uck.core.rules.actions.lib.args") | line arguments for actions        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ExecCompatibleCommandLineBuild   | ::: block                         |
    | er](ExecCompatibleCommandLineBuil | Build a                           |
    | der.html "class in com.facebook.b | [`CommandLine`](CommandLine.      |
    | uck.core.rules.actions.lib.args") | html "interface in com.facebook.b |
    |                                   | uck.core.rules.actions.lib.args") |
    |                                   | that is compatible with           |
    |                                   | \`exec()\` style functions.       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Exception                         | Description                       |
    +===================================+===================================+
    | [CommandLineA                     | ::: block                         |
    | rgException](CommandLineArgExcept | Thrown when trying to create a    |
    | ion.html "class in com.facebook.b | [`CommandLineArgStr               |
    | uck.core.rules.actions.lib.args") | ingifier`](CommandLineArgStringif |
    |                                   | ier.html "class in com.facebook.b |
    |                                   | uck.core.rules.actions.lib.args") |
    |                                   | from an invalid type              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Exception Summary[ ]{.tabEnd}
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../../../../../index.html)
-   Package
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../../index-all.html)
-   [Help](../../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

[]{#skip.navbar.bottom}
:::
