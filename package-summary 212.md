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
# Package com.facebook.buck.core.graph.transformation.composition {#package-com.facebook.buck.core.graph.transformation.composition .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [ComposedComputation](Compos      | ::: block                         |
    | edComputation.html "interface in  | A                                 |
    | com.facebook.buck.core.graph.tran | [`Grap                            |
    | sformation.composition")\<BaseKey | hComputation`](../GraphComputatio |
    | extends                           | n.html "interface in com.facebook |
    | [ComputeKey](../m                 | .buck.core.graph.transformation") |
    | odel/ComputeKey.html "interface i | that represents the               |
    | n com.facebook.buck.core.graph.tr | [                                 |
    | ansformation.model")\<?\>,​Result2 | `Composition`](Composition.html " |
    | extends                           | class in com.facebook.buck.core.g |
    | [ComputeResu                      | raph.transformation.composition") |
    | lt](../model/ComputeResult.html " | of a                              |
    | interface in com.facebook.buck.co | [`ComposedComputation             |
    | re.graph.transformation.model")\> | `](ComposedComputation.html "inte |
    |                                   | rface in com.facebook.buck.core.g |
    |                                   | raph.transformation.composition") |
    |                                   | that we can the base computation, |
    |                                   | a                                 |
    |                                   | [`Composer`](Composer.html "inter |
    |                                   | face in com.facebook.buck.core.gr |
    |                                   | aph.transformation.composition"), |
    |                                   | and a                             |
    |                                   | [`Tran                            |
    |                                   | sformer`](Transformer.html "inter |
    |                                   | face in com.facebook.buck.core.gr |
    |                                   | aph.transformation.composition"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Composer](Co                     | ::: block                         |
    | mposer.html "interface in com.fac | The function for composing        |
    | ebook.buck.core.graph.transformat | [`Graph                           |
    | ion.composition")\<Key1,​Result1\> | Computation`](../GraphComputation |
    |                                   | .html "interface in com.facebook. |
    |                                   | buck.core.graph.transformation")s |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [KeyCompo                         | ::: block                         |
    | ser](KeyComposer.html "interface  | A specific                        |
    | in com.facebook.buck.core.graph.t | [`Composer`](Composer.html "inte  |
    | ransformation.composition")\<Key1 | rface in com.facebook.buck.core.g |
    | extends                           | raph.transformation.composition") |
    | [ComputeKey](../model/C           | that has output key restrictions  |
    | omputeKey.html "interface in com. | :::                               |
    | facebook.buck.core.graph.transfor |                                   |
    | mation.model")\<Result1\>,​Result1 |                                   |
    | extends                           |                                   |
    | [ComputeResult]                   |                                   |
    | (../model/ComputeResult.html "int |                                   |
    | erface in com.facebook.buck.core. |                                   |
    | graph.transformation.model"),​Key2 |                                   |
    | extends                           |                                   |
    | [ComputeKey                       |                                   |
    | ](../model/ComputeKey.html "inter |                                   |
    | face in com.facebook.buck.core.gr |                                   |
    | aph.transformation.model")\<?\>\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [RightComposingC                  | ::: block                         |
    | omputation.RightComposer](RightCo | Specific                          |
    | mposingComputation.RightComposer. | [`Composer`](Composer.html "inte  |
    | html "interface in com.facebook.b | rface in com.facebook.buck.core.g |
    | uck.core.graph.transformation.com | raph.transformation.composition") |
    | position")\<Key1,​Result1,​RightKey | that the right computation is a   |
    | extends                           | [`ComposedComputation             |
    | [ComputeKey](../model             | `](ComposedComputation.html "inte |
    | /ComputeKey.html "interface in co | rface in com.facebook.buck.core.g |
    | m.facebook.buck.core.graph.transf | raph.transformation.composition") |
    | ormation.model")\<?\>,​RightResult | :::                               |
    | extends                           |                                   |
    | [ComputeResu                      |                                   |
    | lt](../model/ComputeResult.html " |                                   |
    | interface in com.facebook.buck.co |                                   |
    | re.graph.transformation.model")\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [Transformer]                     | ::: block                         |
    | (Transformer.html "interface in c | Generic transform API that given  |
    | om.facebook.buck.core.graph.trans | all dependencies through the      |
    | formation.composition")\<KeyInput | [`ComputationEnviro               |
    | extends                           | nment`](../ComputationEnvironment |
    | [ComputeKey](../model/ComputeKe   | .html "interface in com.facebook. |
    | y.html "interface in com.facebook | buck.core.graph.transformation"), |
    | .buck.core.graph.transformation.m | computes the desired result of    |
    | odel")\<ResultInput\>,​ResultInput | ResultType.                       |
    | extends                           | :::                               |
    | [ComputeResult](../mo             |                                   |
    | del/ComputeResult.html "interface |                                   |
    |  in com.facebook.buck.core.graph. |                                   |
    | transformation.model"),​ResultType |                                   |
    | extends                           |                                   |
    | [ComputeResu                      |                                   |
    | lt](../model/ComputeResult.html " |                                   |
    | interface in com.facebook.buck.co |                                   |
    | re.graph.transformation.model")\> |                                   |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [Composition](Composition.html "  | ::: block                         |
    | class in com.facebook.buck.core.g | Performs a composition over two   |
    | raph.transformation.composition") | [`GraphC                          |
    |                                   | omputation`](../GraphComputation. |
    |                                   | html "interface in com.facebook.b |
    |                                   | uck.core.graph.transformation")s. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | LeftComposingComputation](LeftCom | An implementation of              |
    | posingComputation.html "class in  | [`ComposedComputation             |
    | com.facebook.buck.core.graph.tran | `](ComposedComputation.html "inte |
    | sformation.composition")\<BaseKey | rface in com.facebook.buck.core.g |
    | extends                           | raph.transformation.composition") |
    | [ComputeKey](.                    | that takes a base                 |
    | ./model/ComputeKey.html "interfac | [`ComposedComputation`            |
    | e in com.facebook.buck.core.graph | ](ComposedComputation.html "inter |
    | .transformation.model")\<?\>,​Key1 | face in com.facebook.buck.core.gr |
    | extends                           | aph.transformation.composition"), |
    | [ComputeKey](../model/C           | a                                 |
    | omputeKey.html "interface in com. | [`Composer`](Composer.html "inter |
    | facebook.buck.core.graph.transfor | face in com.facebook.buck.core.gr |
    | mation.model")\<Result1\>,​Result1 | aph.transformation.composition"), |
    | extends                           | and                               |
    | [ComputeResult](..                | [`Tra                             |
    | /model/ComputeResult.html "interf | nsformer`](Transformer.html "inte |
    | ace in com.facebook.buck.core.gra | rface in com.facebook.buck.core.g |
    | ph.transformation.model"),​Result2 | raph.transformation.composition") |
    | extends                           | and returns a new                 |
    | [ComputeResu                      | [`Composed                        |
    | lt](../model/ComputeResult.html " | Result`](../model/ComposedResult. |
    | interface in com.facebook.buck.co | html "class in com.facebook.buck. |
    | re.graph.transformation.model")\> | core.graph.transformation.model") |
    |                                   | of                                |
    |                                   | [`LeftComposingComputation`       |
    |                                   | ](LeftComposingComputation.html " |
    |                                   | class in com.facebook.buck.core.g |
    |                                   | raph.transformation.composition") |
    |                                   | type.                             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RightCompo                       | ::: block                         |
    | singComputation](RightComposingCo | An implementation of              |
    | mputation.html "class in com.face | [`ComposedComputation             |
    | book.buck.core.graph.transformati | `](ComposedComputation.html "inte |
    | on.composition")\<KeyIntermediate | rface in com.facebook.buck.core.g |
    | extends                           | raph.transformation.composition") |
    | [ComputeKey](.                    | that takes a base                 |
    | ./model/ComputeKey.html "interfac | [`Graph                           |
    | e in com.facebook.buck.core.graph | Computation`](../GraphComputation |
    | .transformation.model")\<?\>,​Key1 | .html "interface in com.facebook. |
    | extends                           | buck.core.graph.transformation"), |
    | [ComputeKey](../model/C           | a                                 |
    | omputeKey.html "interface in com. | [`Composer`](Composer.html "inter |
    | facebook.buck.core.graph.transfor | face in com.facebook.buck.core.gr |
    | mation.model")\<Result1\>,​Result1 | aph.transformation.composition"), |
    | extends                           | and                               |
    | [ComputeResult]                   | [`Tra                             |
    | (../model/ComputeResult.html "int | nsformer`](Transformer.html "inte |
    | erface in com.facebook.buck.core. | rface in com.facebook.buck.core.g |
    | graph.transformation.model"),​Key2 | raph.transformation.composition") |
    | extends                           | and returns a new                 |
    | [ComputeKey](../model/C           | [`Composed                        |
    | omputeKey.html "interface in com. | Result`](../model/ComposedResult. |
    | facebook.buck.core.graph.transfor | html "class in com.facebook.buck. |
    | mation.model")\<Result2\>,​Result2 | core.graph.transformation.model") |
    | extends                           | of                                |
    | [ComputeResu                      | [`RightComposingComputation`]     |
    | lt](../model/ComputeResult.html " | (RightComposingComputation.html " |
    | interface in com.facebook.buck.co | class in com.facebook.buck.core.g |
    | re.graph.transformation.model")\> | raph.transformation.composition") |
    |                                   | type.                             |
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
