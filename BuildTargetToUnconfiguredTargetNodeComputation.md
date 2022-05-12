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
-   [Package](package-summary.html)
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

<div>

-   Summary: 
-   Nested \| 
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
::: subTitle
[Package]{.packageLabelInType} [com.facebook.buck.parser.targetnode](package-summary.html)
:::

## Class BuildTargetToUnconfiguredTargetNodeComputation {#class-buildtargettounconfiguredtargetnodecomputation .title title="Class BuildTargetToUnconfiguredTargetNodeComputation"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.parser.targetnode.BuildTargetToUnconfiguredTargetNodeComputation

::: description
-   

    All Implemented Interfaces:
    :   `GraphComputation<BuildTargetToUnconfiguredTargetNodeKey,​UnconfiguredTargetNode>`

    ------------------------------------------------------------------------

        public class BuildTargetToUnconfiguredTargetNodeComputation
        extends Object
        implements GraphComputation<BuildTargetToUnconfiguredTargetNodeKey,​UnconfiguredTargetNode>

    ::: block
    Transforms one target from specific
    [`BuildFileManifest`](../api/BuildFileManifest.html "class in com.facebook.buck.parser.api")
    to
    [`UnconfiguredTargetNode`](../../core/model/targetgraph/raw/UnconfiguredTargetNode.html "interface in com.facebook.buck.core.model.targetgraph.raw")
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `co                   | `discoverDeps​(        | ::: block             |
        | m.google.common.colle | BuildTargetToUnconfig | Compute dependent     |
        | ct.ImmutableSet<? ext | uredTargetNodeKey key | keys required to      |
        | ends ComputeKey<? ext | ,             Computa | compute given key,    |
        | ends ComputeResult>>` | tionEnvironment env)` | and a set of          |
        |                       |                       | dependencies as       |
        |                       |                       | listed by             |
        |                       |                       | [`GraphComputat       |
        |                       |                       | ion.discoverPrelimina |
        |                       |                       | ryDeps(ComputeKey)`]( |
        |                       |                       | ../../core/graph/tran |
        |                       |                       | sformation/GraphCompu |
        |                       |                       | tation.html#discoverP |
        |                       |                       | reliminaryDeps(Key)). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `co                   | `disco                | ::: block             |
        | m.google.common.colle | verPreliminaryDeps​(Bu | Compute dependent     |
        | ct.ImmutableSet<? ext | ildTargetToUnconfigur | keys required to      |
        | ends ComputeKey<? ext | edTargetNodeKey key)` | compute given the     |
        | ends ComputeResult>>` |                       | current key.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Comp                 | `getIdentifier()`     |                       |
        | utationIdentifier<Unc |                       |                       |
        | onfiguredTargetNode>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Build         | `of​(Unconfigure       | ::: block             |
        | TargetToUnconfiguredT | dTargetNodeFactory un | Create new instance   |
        | argetNodeComputation` | configuredTargetNodeF | of                    |
        |                       | actory,   Cell cell)` | [`B                   |
        |                       |                       | uildTargetToUnconfigu |
        |                       |                       | redTargetNodeComputat |
        |                       |                       | ion`](BuildTargetToUn |
        |                       |                       | configuredTargetNodeC |
        |                       |                       | omputation.html "clas |
        |                       |                       | s in com.facebook.buc |
        |                       |                       | k.parser.targetnode") |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Un                   | `transfo              | ::: block             |
        | configuredTargetNode` | rm​(BuildTargetToUncon | Perform a             |
        |                       | figuredTargetNodeKey  | transformation        |
        |                       | key,          Computa | identified by key     |
        |                       | tionEnvironment env)` | [`GraphC              |
        |                       |                       | omputation`](../../co |
        |                       |                       | re/graph/transformati |
        |                       |                       | on/GraphComputation.h |
        |                       |                       | tml "interface in com |
        |                       |                       | .facebook.buck.core.g |
        |                       |                       | raph.transformation") |
        |                       |                       | into a final type     |
        |                       |                       | [`GraphCo             |
        |                       |                       | mputation`](../../cor |
        |                       |                       | e/graph/transformatio |
        |                       |                       | n/GraphComputation.ht |
        |                       |                       | ml "interface in com. |
        |                       |                       | facebook.buck.core.gr |
        |                       |                       | aph.transformation"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#of(com.facebook.buck.parser.UnconfiguredTargetNodeFactory,com.facebook.buck.core.cell.Cell)}

        -   #### of

            ``` methodSignature
            public static BuildTargetToUnconfiguredTargetNodeComputation of​(UnconfiguredTargetNodeFactory unconfiguredTargetNodeFactory,
                                                                            Cell cell)
            ```

            ::: block
            Create new instance of
            [`BuildTargetToUnconfiguredTargetNodeComputation`](BuildTargetToUnconfiguredTargetNodeComputation.html "class in com.facebook.buck.parser.targetnode")
            :::

            [Parameters:]{.paramLabel}

            `unconfiguredTargetNodeFactory` - An actual factory that
            will create
            [`UnconfiguredTargetNode`](../../core/model/targetgraph/raw/UnconfiguredTargetNode.html "interface in com.facebook.buck.core.model.targetgraph.raw")
            from raw attributes containing in
            [`BuildFileManifest`](../api/BuildFileManifest.html "class in com.facebook.buck.parser.api")

            `cell` - A
            [`Cell`](../../core/cell/Cell.html "interface in com.facebook.buck.core.cell")
            object that contains targets used in this transformation, it
            is mostly used to resolve paths to absolute paths

            [Returns:]{.returnLabel}

        []{#getIdentifier()}

        -   #### getIdentifier

            ``` methodSignature
            public ComputationIdentifier<UnconfiguredTargetNode> getIdentifier()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getIdentifier` in
                interface `GraphComputation<BuildTargetToUnconfiguredTargetNodeKey,​UnconfiguredTargetNode>`

            [Returns:]{.returnLabel}
            :   the identifier of the key for this transformation. This
                should match
                [`ComputeKey.getIdentifier()`](../../core/graph/transformation/model/ComputeKey.html#getIdentifier())

        []{#transform(com.facebook.buck.parser.targetnode.BuildTargetToUnconfiguredTargetNodeKey,com.facebook.buck.core.graph.transformation.ComputationEnvironment)}

        -   #### transform

            ``` methodSignature
            public UnconfiguredTargetNode transform​(BuildTargetToUnconfiguredTargetNodeKey key,
                                                    ComputationEnvironment env)
            ```

            ::: block
            [Description copied from
            interface: `GraphComputation`]{.descfrmTypeLabel}
            :::

            ::: block
            Perform a transformation identified by key
            [`GraphComputation`](../../core/graph/transformation/GraphComputation.html "interface in com.facebook.buck.core.graph.transformation")
            into a final type
            [`GraphComputation`](../../core/graph/transformation/GraphComputation.html "interface in com.facebook.buck.core.graph.transformation").
            This transformation should be performed synchronously.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `transform` in
                interface `GraphComputation<BuildTargetToUnconfiguredTargetNodeKey,​UnconfiguredTargetNode>`

            [Parameters:]{.paramLabel}
            :   `key` - The Key of the requested result
            :   `env` - The execution environment containing results of
                keys from
                [`GraphComputation.discoverDeps(ComputeKey, ComputationEnvironment)`](../../core/graph/transformation/GraphComputation.html#discoverDeps(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
                and
                [`GraphComputation.discoverPreliminaryDeps(ComputeKey)`](../../core/graph/transformation/GraphComputation.html#discoverPreliminaryDeps(Key))

            [Returns:]{.returnLabel}
            :   The result of the transformation

        []{#discoverDeps(com.facebook.buck.parser.targetnode.BuildTargetToUnconfiguredTargetNodeKey,com.facebook.buck.core.graph.transformation.ComputationEnvironment)}

        -   #### discoverDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<? extends ComputeKey<? extends ComputeResult>> discoverDeps​(BuildTargetToUnconfiguredTargetNodeKey key,
                                                                                                                      ComputationEnvironment env)
            ```

            ::: block
            [Description copied from
            interface: `GraphComputation`]{.descfrmTypeLabel}
            :::

            ::: block
            Compute dependent keys required to compute given key, and a
            set of dependencies as listed by
            [`GraphComputation.discoverPreliminaryDeps(ComputeKey)`](../../core/graph/transformation/GraphComputation.html#discoverPreliminaryDeps(Key)).
            The results of those computations will be available in
            [`GraphComputation.transform(ComputeKey, ComputationEnvironment)`](../../core/graph/transformation/GraphComputation.html#transform(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
            as a part of
            [`ComputationEnvironment`](../../core/graph/transformation/ComputationEnvironment.html "interface in com.facebook.buck.core.graph.transformation")
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `discoverDeps` in
                interface `GraphComputation<BuildTargetToUnconfiguredTargetNodeKey,​UnconfiguredTargetNode>`

            [Parameters:]{.paramLabel}
            :   `key` - the current key to transform
            :   `env` - The execution environment containing results of
                keys from
                [`GraphComputation.discoverPreliminaryDeps(ComputeKey)`](../../core/graph/transformation/GraphComputation.html#discoverPreliminaryDeps(Key))

            [Returns:]{.returnLabel}
            :   a set of keys that the transformation of the current key
                depends on

        []{#discoverPreliminaryDeps(com.facebook.buck.parser.targetnode.BuildTargetToUnconfiguredTargetNodeKey)}

        -   #### discoverPreliminaryDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<? extends ComputeKey<? extends ComputeResult>> discoverPreliminaryDeps​(BuildTargetToUnconfiguredTargetNodeKey key)
            ```

            ::: block
            [Description copied from
            interface: `GraphComputation`]{.descfrmTypeLabel}
            :::

            ::: block
            Compute dependent keys required to compute given the current
            key. The results of those computations will be available in
            [`GraphComputation.discoverDeps(ComputeKey, ComputationEnvironment)`](../../core/graph/transformation/GraphComputation.html#discoverDeps(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
            as a part of
            [`ComputationEnvironment`](../../core/graph/transformation/ComputationEnvironment.html "interface in com.facebook.buck.core.graph.transformation"),
            and
            [`GraphComputation.transform(ComputeKey,  ComputationEnvironment)`](../../core/graph/transformation/GraphComputation.html#transform(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `discoverPreliminaryDeps` in
                interface `GraphComputation<BuildTargetToUnconfiguredTargetNodeKey,​UnconfiguredTargetNode>`

            [Parameters:]{.paramLabel}
            :   `key` - the current key to transform

            [Returns:]{.returnLabel}
            :   a set of keys that the
                [`GraphComputation.discoverDeps(ComputeKey, ComputationEnvironment)`](../../core/graph/transformation/GraphComputation.html#discoverDeps(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
                and
                [`GraphComputation.transform(ComputeKey, ComputationEnvironment)`](../../core/graph/transformation/GraphComputation.html#transform(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
                of the current key depends on
    :::
:::
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
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

<div>

-   Summary: 
-   Nested \| 
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
