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
# Package com.facebook.buck.core.rules.tool {#package-com.facebook.buck.core.rules.tool .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [BinaryBuildRule](Bina            | ::: block                         |
    | ryBuildRule.html "interface in co | Build rules that can be executed  |
    | m.facebook.buck.core.rules.tool") | on the command line.              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [BinaryWrapperRule](Bi            | ::: block                         |
    | naryWrapperRule.html "class in co | A no-op stub class for binary     |
    | m.facebook.buck.core.rules.tool") | rules which delegate to another   |
    |                                   | rule to provide the output path   |
    |                                   | and executable tool.              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RuleAnalysisLegacyBinaryBuil     | ::: block                         |
    | dRuleView](RuleAnalysisLegacyBina | As                                |
    | ryBuildRuleView.html "class in co | [`RuleAnalysisLegacyBuildRul      |
    | m.facebook.buck.core.rules.tool") | eView`](../impl/RuleAnalysisLegac |
    |                                   | yBuildRuleView.html "class in com |
    |                                   | .facebook.buck.core.rules.impl"), |
    |                                   | but also implements               |
    |                                   | [`BinaryBuildRule`](Bina          |
    |                                   | ryBuildRule.html "interface in co |
    |                                   | m.facebook.buck.core.rules.tool") |
    |                                   | so that this rule can be          |
    |                                   | executable (with `buck run`, in   |
    |                                   | the legacy graph, etc)            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RuleAnalysisLegacyTestBu         | ::: block                         |
    | ildRuleView](RuleAnalysisLegacyTe | As                                |
    | stBuildRuleView.html "class in co | [`RuleAnalysisLegacyBuildRul      |
    | m.facebook.buck.core.rules.tool") | eView`](../impl/RuleAnalysisLegac |
    |                                   | yBuildRuleView.html "class in com |
    |                                   | .facebook.buck.core.rules.impl"), |
    |                                   | but also implements               |
    |                                   | [`TestRule`](../../test/r         |
    |                                   | ule/TestRule.html "interface in c |
    |                                   | om.facebook.buck.core.test.rule") |
    |                                   | so that this rule can be run by   |
    |                                   | `buck test`                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RunInfoLegacyTool](Ru            | ::: block                         |
    | nInfoLegacyTool.html "class in co | A legacy                          |
    | m.facebook.buck.core.rules.tool") | [`Tool`](../../toolchain/to       |
    |                                   | ol/Tool.html "interface in com.fa |
    |                                   | cebook.buck.core.toolchain.tool") |
    |                                   | interface to                      |
    |                                   | [`RunInfo`](../providers/lib/R    |
    |                                   | unInfo.html "class in com.faceboo |
    |                                   | k.buck.core.rules.providers.lib") |
    |                                   | provider info objects.            |
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
