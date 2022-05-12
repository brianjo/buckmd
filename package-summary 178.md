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
# Package com.facebook.buck.core.graph.transformation.model {#package-com.facebook.buck.core.graph.transformation.model .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [ComputationIdentifier](Compu     | ::: block                         |
    | tationIdentifier.html "interface  | An Identifier for this            |
    | in com.facebook.buck.core.graph.t | [`ComputeKey`](ComputeKey.html    |
    | ransformation.model")\<ResultType | "interface in com.facebook.buck.c |
    | extends                           | ore.graph.transformation.model"). |
    | [Co                               | :::                               |
    | mputeResult](ComputeResult.html " |                                   |
    | interface in com.facebook.buck.co |                                   |
    | re.graph.transformation.model")\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [Comput                           | ::: block                         |
    | eKey](ComputeKey.html "interface  | This is an interface for all keys |
    | in com.facebook.buck.core.graph.t | to be used in                     |
    | ransformation.model")\<ResultType | [`Graph                           |
    | extends                           | Computation`](../GraphComputation |
    | [Co                               | .html "interface in com.facebook. |
    | mputeResult](ComputeResult.html " | buck.core.graph.transformation"). |
    | interface in com.facebook.buck.co | :::                               |
    | re.graph.transformation.model")\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | ComputeResult](ComputeResult.html | This is a marker interface for    |
    |  "interface in com.facebook.buck. | result types of                   |
    | core.graph.transformation.model") | [`Graph                           |
    |                                   | Computation`](../GraphComputation |
    |                                   | .html "interface in com.facebook. |
    |                                   | buck.core.graph.transformation"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [ClassBasedC                      | ::: block                         |
    | omputationIdentifier](ClassBasedC | A                                 |
    | omputationIdentifier.html "class  | [`ComputationIdenti               |
    | in com.facebook.buck.core.graph.t | fier`](ComputationIdentifier.html |
    | ransformation.model")\<ResultType |  "interface in com.facebook.buck. |
    | extends                           | core.graph.transformation.model") |
    | [Co                               | that identifies uniqueness by the |
    | mputeResult](ComputeResult.html " | class of the                      |
    | interface in com.facebook.buck.co | [`ComputeKey`](ComputeKey.html    |
    | re.graph.transformation.model")\> |  "interface in com.facebook.buck. |
    |                                   | core.graph.transformation.model") |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Compose                          | ::: block                         |
    | dComputationIdentifier](ComposedC | A                                 |
    | omputationIdentifier.html "class  | [`ComputationIdenti               |
    | in com.facebook.buck.core.graph.t | fier`](ComputationIdentifier.html |
    | ransformation.model")\<ResultType |  "interface in com.facebook.buck. |
    | extends                           | core.graph.transformation.model") |
    | [Co                               | for a composed                    |
    | mputeResult](ComputeResult.html " | [`Grap                            |
    | interface in com.facebook.buck.co | hComputation`](../GraphComputatio |
    | re.graph.transformation.model")\> | n.html "interface in com.facebook |
    |                                   | .buck.core.graph.transformation") |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Co                               | ::: block                         |
    | mposedKey](ComposedKey.html "clas | The                               |
    | s in com.facebook.buck.core.graph | [`ComputeKey`](ComputeKey.html    |
    | .transformation.model")\<KeyType1 |  "interface in com.facebook.buck. |
    | extends                           | core.graph.transformation.model") |
    | [ComputeKey]                      | for a composed computation        |
    | (ComputeKey.html "interface in co | :::                               |
    | m.facebook.buck.core.graph.transf |                                   |
    | ormation.model")\<?\>,​ResultType2 |                                   |
    | extends                           |                                   |
    | [Co                               |                                   |
    | mputeResult](ComputeResult.html " |                                   |
    | interface in com.facebook.buck.co |                                   |
    | re.graph.transformation.model")\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [Compose                          | ::: block                         |
    | dResult](ComposedResult.html "cla | The                               |
    | ss in com.facebook.buck.core.grap | [`C                               |
    | h.transformation.model")\<KeyType | omputeResult`](ComputeResult.html |
    | extends                           |  "interface in com.facebook.buck. |
    | [ComputeKey](Compute              | core.graph.transformation.model") |
    | Key.html "interface in com.facebo | for a composed computation.       |
    | ok.buck.core.graph.transformation | :::                               |
    | .model")\<ResultType\>,​ResultType |                                   |
    | extends                           |                                   |
    | [Co                               |                                   |
    | mputeResult](ComputeResult.html " |                                   |
    | interface in com.facebook.buck.co |                                   |
    | re.graph.transformation.model")\> |                                   |
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
