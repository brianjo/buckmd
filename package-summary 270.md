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

-   [Overview](../../../../../../../index.html)
-   Package
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
# Package com.facebook.buck.core.model.targetgraph.raw {#package-com.facebook.buck.core.model.targetgraph.raw .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [UnconfiguredT                    | ::: block                         |
    | argetNode](UnconfiguredTargetNode | A target node with attributes     |
    | .html "interface in com.facebook. | kept in a map as oppose to in a   |
    | buck.core.model.targetgraph.raw") | structured object like in         |
    |                                   | [`TargetNode`](../TargetN         |
    |                                   | ode.html "interface in com.facebo |
    |                                   | ok.buck.core.model.targetgraph"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [UnconfiguredTargetNo             | ::: block                         |
    | deWithDeps.UnconfiguredTargetNode | This mixin is used by JSON        |
    | WithDepsUnwrappedMixin](Unconfigu | serializer to flatten             |
    | redTargetNodeWithDeps.Unconfigure | [`UnconfiguredTa                  |
    | dTargetNodeWithDepsUnwrappedMixin | rgetNode`](UnconfiguredTargetNode |
    | .html "interface in com.facebook. | .html "interface in com.facebook. |
    | buck.core.model.targetgraph.raw") | buck.core.model.targetgraph.raw") |
    |                                   | properties We cannot use          |
    |                                   | `JsonUnwrapped` directly on       |
    |                                   | [`UnconfiguredTargetNodeWith      |
    |                                   | Deps.getUnconfiguredTargetNode()` |
    |                                   | ](UnconfiguredTargetNodeWithDeps. |
    |                                   | html#getUnconfiguredTargetNode()) |
    |                                   | because it is not supported by    |
    |                                   | typed deserializer                |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [UnconfiguredTargetNodeWit        | ::: block                         |
    | hDeps](UnconfiguredTargetNodeWith | A pair of                         |
    | Deps.html "class in com.facebook. | [`UnconfiguredTa                  |
    | buck.core.model.targetgraph.raw") | rgetNode`](UnconfiguredTargetNode |
    |                                   | .html "interface in com.facebook. |
    |                                   | buck.core.model.targetgraph.raw") |
    |                                   | and its dependencies              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Unconf                           | ::: block                         |
    | iguredTargetNodeWithDepsPackage]( | Represents all                    |
    | UnconfiguredTargetNodeWithDepsPac | [`UnconfiguredTargetNodeWith      |
    | kage.html "class in com.facebook. | Deps`](UnconfiguredTargetNodeWith |
    | buck.core.model.targetgraph.raw") | Deps.html "class in com.facebook. |
    |                                   | buck.core.model.targetgraph.raw") |
    |                                   | that result from parsing a single |
    |                                   | build file                        |
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

-   [Overview](../../../../../../../index.html)
-   Package
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

[]{#skip.navbar.bottom}
:::
