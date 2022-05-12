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

-   [Overview](../../../../../index.html)
-   Package
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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
# Package com.facebook.buck.rules.args {#package-com.facebook.buck.rules.args .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [Ad                               | ::: block                         |
    | dsToRuleKeyFunction](AddsToRuleKe | A simple shorthand for `Function` |
    | yFunction.html "interface in com. | and                               |
    | facebook.buck.rules.args")\<T,​F\> | [`Ad                              |
    |                                   | dsToRuleKey`](../../core/rulekey/ |
    |                                   | AddsToRuleKey.html "interface in  |
    |                                   | com.facebook.buck.core.rulekey"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Arg](Arg.html "interface         | ::: block                         |
    | in com.facebook.buck.rules.args") | An abstraction for modeling the   |
    |                                   | arguments that contribute to a    |
    |                                   | command run by a                  |
    |                                   | [`BuildRule`](../../core/         |
    |                                   | rules/BuildRule.html "interface i |
    |                                   | n com.facebook.buck.core.rules"), |
    |                                   | and also carry information for    |
    |                                   | computing a rule key.             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HasSourcePat                     | ::: block                         |
    | h](HasSourcePath.html "interface  | Interface for extracting a        |
    | in com.facebook.buck.rules.args") | SourcePath from an Arg which has  |
    |                                   | one.                              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | ToolArg](ToolArg.html "interface  | An Arg that just wraps a Tool.    |
    | in com.facebook.buck.rules.args") | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [Ar                               | ::: block                         |
    | gFactory](ArgFactory.html "class  | Simple factory class to convert   |
    | in com.facebook.buck.rules.args") | objects from                      |
    |                                   | [`Co                              |
    |                                   | mmandLineArgs`](../../core/rules/ |
    |                                   | actions/lib/args/CommandLineArgs. |
    |                                   | html "interface in com.facebook.b |
    |                                   | uck.core.rules.actions.lib.args") |
    |                                   | to                                |
    |                                   | [`Arg`](Arg.html "interface       |
    |                                   | in com.facebook.buck.rules.args") |
    |                                   | objects                           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Compos                           | ::: block                         |
    | iteArg](CompositeArg.html "class  | CompositeArg holds a list of args |
    | in com.facebook.buck.rules.args") | and appends them all to the       |
    |                                   | command-line.                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [F                                | ::: block                         |
    | ileListableLinkerInputArg](FileLi | Arg that represents object file   |
    | stableLinkerInputArg.html "class  | that should be linked into        |
    | in com.facebook.buck.rules.args") | resulting binary using normal     |
    |                                   | mechanism, e.g.                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | FormatArg](FormatArg.html "class  | Arg that stringifies another      |
    | in com.facebook.buck.rules.args") | [`Arg`](Arg.html "interface i     |
    |                                   | n com.facebook.buck.rules.args"), |
    |                                   | and passes that string            |
    |                                   | representation into               |
    |                                   | [`String.format(java.lang.String, |
    |                                   |  java.lang.Object...)`](http://do |
    |                                   | cs.oracle.com/javase/7/docs/api/j |
    |                                   | ava/lang/String.html?is-external= |
    |                                   | true#format(java.lang.String,java |
    |                                   | .lang.Object...) "class or interf |
    |                                   | ace in java.lang"){.externalLink} |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ProxyArg](ProxyArg.html "class   |                                   |
    | in com.facebook.buck.rules.args") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Saniti                           | ::: block                         |
    | zedArg](SanitizedArg.html "class  | An                                |
    | in com.facebook.buck.rules.args") | [`Arg`](Arg.html "interface       |
    |                                   | in com.facebook.buck.rules.args") |
    |                                   | which must be sanitized before    |
    |                                   | contributing to a                 |
    |                                   | [`RuleKey`](../../cor             |
    |                                   | e/rulekey/RuleKey.html "class in  |
    |                                   | com.facebook.buck.core.rulekey"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [SourcePa                         | ::: block                         |
    | thArg](SourcePathArg.html "class  | An                                |
    | in com.facebook.buck.rules.args") | [`Arg`](Arg.html "interface       |
    |                                   | in com.facebook.buck.rules.args") |
    |                                   | which wraps a                     |
    |                                   | [`So                              |
    |                                   | urcePath`](../../core/sourcepath/ |
    |                                   | SourcePath.html "interface in com |
    |                                   | .facebook.buck.core.sourcepath"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 |                                   |
    | StringArg](StringArg.html "class  |                                   |
    | in com.facebook.buck.rules.args") |                                   |
    +-----------------------------------+-----------------------------------+
    | [WriteToFil                       | ::: block                         |
    | eArg](WriteToFileArg.html "class  | Expands a delegated arg to a file |
    | in com.facebook.buck.rules.args") | and then appends                  |
    |                                   | \@that/file/path.macro to the     |
    |                                   | command line.                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../../index.html)
-   Package
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

[]{#skip.navbar.bottom}
:::
