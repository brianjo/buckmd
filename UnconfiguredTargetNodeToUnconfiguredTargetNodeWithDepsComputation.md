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

## Class UnconfiguredTargetNodeToUnconfiguredTargetNodeWithDepsComputation {#class-unconfiguredtargetnodetounconfiguredtargetnodewithdepscomputation .title title="Class UnconfiguredTargetNodeToUnconfiguredTargetNodeWithDepsComputation"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.parser.targetnode.UnconfiguredTargetNodeToUnconfiguredTargetNodeWithDepsComputation

::: description
-   

    All Implemented Interfaces:
    :   `GraphComputation<UnconfiguredTargetNodeToUnconfiguredTargetNodeWithDepsKey,​UnconfiguredTargetNodeWithDeps>`

    ------------------------------------------------------------------------

        public class UnconfiguredTargetNodeToUnconfiguredTargetNodeWithDepsComputation
        extends Object
        implements GraphComputation<UnconfiguredTargetNodeToUnconfiguredTargetNodeWithDepsKey,​UnconfiguredTargetNodeWithDeps>

    ::: block
    Transforms
    [`UnconfiguredTargetNode`](../../core/model/targetgraph/raw/UnconfiguredTargetNode.html "interface in com.facebook.buck.core.model.targetgraph.raw")
    to
    [`UnconfiguredTargetNodeWithDeps`](../../core/model/targetgraph/raw/UnconfiguredTargetNodeWithDeps.html "class in com.facebook.buck.core.model.targetgraph.raw")
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `co                   | `discoverDep          | ::: block             |
        | m.google.common.colle | s​(UnconfiguredTargetN | Compute dependent     |
        | ct.ImmutableSet<? ext | odeToUnconfiguredTarg | keys required to      |
        | ends ComputeKey<? ext | etNodeWithDepsKey key | compute given key,    |
        | ends ComputeResult>>` | ,             Computa | and a set of          |
        |                       | tionEnvironment env)` | dependencies as       |
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
        | `co                   | `dis                  | ::: block             |
        | m.google.common.colle | coverPreliminaryDeps​( | Compute dependent     |
        | ct.ImmutableSet<? ext | UnconfiguredTargetNod | keys required to      |
        | ends ComputeKey<? ext | eToUnconfiguredTarget | compute given the     |
        | ends ComputeResult>>` | NodeWithDepsKey key)` | current key.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ComputationI         | `getIdentifier()`     |                       |
        | dentifier<Unconfigure |                       |                       |
        | dTargetNodeWithDeps>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Unc           | `of​(UnconfiguredTa    | ::: block             |
        | onfiguredTargetNodeTo | rgetNodeToTargetNodeF | Create new instance   |
        | UnconfiguredTargetNod | actory unconfiguredTa | of                    |
        | eWithDepsComputation` | rgetNodeToTargetNodeF | [`UnconfiguredTarget  |
        |                       | actory,   Cell cell)` | NodeToUnconfiguredTar |
        |                       |                       | getNodeWithDepsComput |
        |                       |                       | ation`](UnconfiguredT |
        |                       |                       | argetNodeToUnconfigur |
        |                       |                       | edTargetNodeWithDepsC |
        |                       |                       | omputation.html "clas |
        |                       |                       | s in com.facebook.buc |
        |                       |                       | k.parser.targetnode") |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Unconfigur           | `trans                | ::: block             |
        | edTargetNodeWithDeps` | form​(UnconfiguredTarg | Perform a             |
        |                       | etNodeToUnconfiguredT | transformation        |
        |                       | argetNodeWithDepsKey  | identified by key     |
        |                       | key,          Computa | [`GraphC              |
        |                       | tionEnvironment env)` | omputation`](../../co |
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

        []{#of(com.facebook.buck.parser.UnconfiguredTargetNodeToTargetNodeFactory,com.facebook.buck.core.cell.Cell)}

        -   #### of

            ``` methodSignature
            public static UnconfiguredTargetNodeToUnconfiguredTargetNodeWithDepsComputation of​(UnconfiguredTargetNodeToTargetNodeFactory unconfiguredTargetNodeToTargetNodeFactory,
                                                                                               Cell cell)
            ```

            ::: block
            Create new instance of
            [`UnconfiguredTargetNodeToUnconfiguredTargetNodeWithDepsComputation`](UnconfiguredTargetNodeToUnconfiguredTargetNodeWithDepsComputation.html "class in com.facebook.buck.parser.targetnode")
            :::

            [Parameters:]{.paramLabel}
            :   `unconfiguredTargetNodeToTargetNodeFactory` - An actual
                factory that will create
                [`TargetNode`](../../core/model/targetgraph/TargetNode.html "interface in com.facebook.buck.core.model.targetgraph")
                from
                [`UnconfiguredTargetNode`](../../core/model/targetgraph/raw/UnconfiguredTargetNode.html "interface in com.facebook.buck.core.model.targetgraph.raw")
                in order to resolve deps
            :   `cell` - A
                [`Cell`](../../core/cell/Cell.html "interface in com.facebook.buck.core.cell")
                object that contains targets used in this
                transformation, it is mostly used to resolve paths to
                absolute paths

        []{#getIdentifier()}

        -   #### getIdentifier

            ``` methodSignature
            public ComputationIdentifier<UnconfiguredTargetNodeWithDeps> getIdentifier()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getIdentifier` in
                interface `GraphComputation<UnconfiguredTargetNodeToUnconfiguredTargetNodeWithDepsKey,​UnconfiguredTargetNodeWithDeps>`

            [Returns:]{.returnLabel}
            :   the identifier of the key for this transformation. This
                should match
                [`ComputeKey.getIdentifier()`](../../core/graph/transformation/model/ComputeKey.html#getIdentifier())

        []{#transform(com.facebook.buck.parser.targetnode.UnconfiguredTargetNodeToUnconfiguredTargetNodeWithDepsKey,com.facebook.buck.core.graph.transformation.ComputationEnvironment)}

        -   #### transform

            ``` methodSignature
            public UnconfiguredTargetNodeWithDeps transform​(UnconfiguredTargetNodeToUnconfiguredTargetNodeWithDepsKey key,
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
                interface `GraphComputation<UnconfiguredTargetNodeToUnconfiguredTargetNodeWithDepsKey,​UnconfiguredTargetNodeWithDeps>`

            [Parameters:]{.paramLabel}
            :   `key` - The Key of the requested result
            :   `env` - The execution environment containing results of
                keys from
                [`GraphComputation.discoverDeps(ComputeKey, ComputationEnvironment)`](../../core/graph/transformation/GraphComputation.html#discoverDeps(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
                and
                [`GraphComputation.discoverPreliminaryDeps(ComputeKey)`](../../core/graph/transformation/GraphComputation.html#discoverPreliminaryDeps(Key))

            [Returns:]{.returnLabel}
            :   The result of the transformation

        []{#discoverDeps(com.facebook.buck.parser.targetnode.UnconfiguredTargetNodeToUnconfiguredTargetNodeWithDepsKey,com.facebook.buck.core.graph.transformation.ComputationEnvironment)}

        -   #### discoverDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<? extends ComputeKey<? extends ComputeResult>> discoverDeps​(UnconfiguredTargetNodeToUnconfiguredTargetNodeWithDepsKey key,
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
                interface `GraphComputation<UnconfiguredTargetNodeToUnconfiguredTargetNodeWithDepsKey,​UnconfiguredTargetNodeWithDeps>`

            [Parameters:]{.paramLabel}
            :   `key` - the current key to transform
            :   `env` - The execution environment containing results of
                keys from
                [`GraphComputation.discoverPreliminaryDeps(ComputeKey)`](../../core/graph/transformation/GraphComputation.html#discoverPreliminaryDeps(Key))

            [Returns:]{.returnLabel}
            :   a set of keys that the transformation of the current key
                depends on

        []{#discoverPreliminaryDeps(com.facebook.buck.parser.targetnode.UnconfiguredTargetNodeToUnconfiguredTargetNodeWithDepsKey)}

        -   #### discoverPreliminaryDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<? extends ComputeKey<? extends ComputeResult>> discoverPreliminaryDeps​(UnconfiguredTargetNodeToUnconfiguredTargetNodeWithDepsKey key)
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
                interface `GraphComputation<UnconfiguredTargetNodeToUnconfiguredTargetNodeWithDepsKey,​UnconfiguredTargetNodeWithDeps>`

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
