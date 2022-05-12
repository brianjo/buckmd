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
-   [Package](package-summary.html)
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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.analysis.impl](package-summary.html)
:::

## Class RuleAnalysisGraphImpl {#class-ruleanalysisgraphimpl .title title="Class RuleAnalysisGraphImpl"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rules.analysis.impl.RuleAnalysisGraphImpl

::: description
-   

    All Implemented Interfaces:
    :   `RuleAnalysisGraph`

    ------------------------------------------------------------------------

        public class RuleAnalysisGraphImpl
        extends Object
        implements RuleAnalysisGraph

    ::: block
    Default implementation of
    [`RuleAnalysisGraph`](../computation/RuleAnalysisGraph.html "interface in com.facebook.buck.core.rules.analysis.computation")
    driven by a
    [`GraphTransformationEngine`](../../../graph/transformation/GraphTransformationEngine.html "interface in com.facebook.buck.core.graph.transformation")
    TODO(bobyf): once we add stages to
    [`GraphTransformationEngine`](../../../graph/transformation/GraphTransformationEngine.html "interface in com.facebook.buck.core.graph.transformation")
    this implementation and the interface will probably change/go away
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `RuleAnalysisResult`  | `get​(RuleAn           | ::: block             |
        |                       | alysisKey lookupKey)` | Finds the             |
        |                       |                       | [`RuleAnalysisResul   |
        |                       |                       | t`](../RuleAnalysisRe |
        |                       |                       | sult.html "interface  |
        |                       |                       | in com.facebook.buck. |
        |                       |                       | core.rules.analysis") |
        |                       |                       | of the given          |
        |                       |                       | [`RuleAnal            |
        |                       |                       | ysisKey`](../RuleAnal |
        |                       |                       | ysisKey.html "class i |
        |                       |                       | n com.facebook.buck.c |
        |                       |                       | ore.rules.analysis"), |
        |                       |                       | starting computation  |
        |                       |                       | as necessary.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `getAll​(Set<RuleAnal  | ::: block             |
        | ommon.collect.Immutab | ysisKey> lookupKeys)` | same as               |
        | leMap<RuleAnalysisKey |                       | [`RuleAnalysis        |
        | ,​RuleAnalysisResult>` |                       | Graph.get(RuleAnalysi |
        |                       |                       | sKey)`](../computatio |
        |                       |                       | n/RuleAnalysisGraph.h |
        |                       |                       | tml#get(com.facebook. |
        |                       |                       | buck.core.rules.analy |
        |                       |                       | sis.RuleAnalysisKey)) |
        |                       |                       | but for multiple      |
        |                       |                       | [`RuleAnal            |
        |                       |                       | ysisKey`](../RuleAnal |
        |                       |                       | ysisKey.html "class i |
        |                       |                       | n com.facebook.buck.c |
        |                       |                       | ore.rules.analysis")s |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static R             | `of​(GraphComputation  | ::: block             |
        | uleAnalysisGraphImpl` | <RuleAnalysisKey,​Rule | creates a new         |
        |                       | AnalysisResult> compu | computation with the  |
        |                       | tation,   TargetGraph | supplied              |
        |                       |  targetGraph,   DepsA | [`Dep                 |
        |                       | wareExecutor<? super  | sAwareExecutor`](../. |
        |                       | ComputeResult,​?> deps | ./../graph/transforma |
        |                       | AwareExecutor,   Rule | tion/executor/DepsAwa |
        |                       | AnalysisCache cache)` | reExecutor.html "inte |
        |                       |                       | rface in com.facebook |
        |                       |                       | .buck.core.graph.tran |
        |                       |                       | sformation.executor") |
        |                       |                       | and using the given   |
        |                       |                       | [`Graph               |
        |                       |                       | EngineCache`](../../. |
        |                       |                       | ./graph/transformatio |
        |                       |                       | n/GraphEngineCache.ht |
        |                       |                       | ml "interface in com. |
        |                       |                       | facebook.buck.core.gr |
        |                       |                       | aph.transformation"), |
        |                       |                       | and computation.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static R             | `of​(TargetGraph tar   | ::: block             |
        | uleAnalysisGraphImpl` | getGraph,   DepsAware | creates a new         |
        |                       | Executor<? super Comp | computation with the  |
        |                       | uteResult,​?> depsAwar | supplied              |
        |                       | eExecutor,   RuleAnal | [`Dep                 |
        |                       | ysisCache cache,   Bu | sAwareExecutor`](../. |
        |                       | ckEventBus eventBus)` | ./../graph/transforma |
        |                       |                       | tion/executor/DepsAwa |
        |                       |                       | reExecutor.html "inte |
        |                       |                       | rface in com.facebook |
        |                       |                       | .buck.core.graph.tran |
        |                       |                       | sformation.executor") |
        |                       |                       | and using the given   |
        |                       |                       | [`Graph               |
        |                       |                       | EngineCache`](../../. |
        |                       |                       | ./graph/transformatio |
        |                       |                       | n/GraphEngineCache.ht |
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

        []{#of(com.facebook.buck.core.model.targetgraph.TargetGraph,com.facebook.buck.core.graph.transformation.executor.DepsAwareExecutor,com.facebook.buck.core.rules.analysis.cache.RuleAnalysisCache,com.facebook.buck.event.BuckEventBus)}

        -   #### of

            ``` methodSignature
            public static RuleAnalysisGraphImpl of​(TargetGraph targetGraph,
                                                   DepsAwareExecutor<? super ComputeResult,​?> depsAwareExecutor,
                                                   RuleAnalysisCache cache,
                                                   BuckEventBus eventBus)
            ```

            ::: block
            creates a new computation with the supplied
            [`DepsAwareExecutor`](../../../graph/transformation/executor/DepsAwareExecutor.html "interface in com.facebook.buck.core.graph.transformation.executor")
            and using the given
            [`GraphEngineCache`](../../../graph/transformation/GraphEngineCache.html "interface in com.facebook.buck.core.graph.transformation").
            All entries present in the cache will be reused, and newly
            computed values will be offered to the cache.
            :::

        []{#of(com.facebook.buck.core.graph.transformation.GraphComputation,com.facebook.buck.core.model.targetgraph.TargetGraph,com.facebook.buck.core.graph.transformation.executor.DepsAwareExecutor,com.facebook.buck.core.rules.analysis.cache.RuleAnalysisCache)}

        -   #### of

            ``` methodSignature
            public static RuleAnalysisGraphImpl of​(GraphComputation<RuleAnalysisKey,​RuleAnalysisResult> computation,
                                                   TargetGraph targetGraph,
                                                   DepsAwareExecutor<? super ComputeResult,​?> depsAwareExecutor,
                                                   RuleAnalysisCache cache)
            ```

            ::: block
            creates a new computation with the supplied
            [`DepsAwareExecutor`](../../../graph/transformation/executor/DepsAwareExecutor.html "interface in com.facebook.buck.core.graph.transformation.executor")
            and using the given
            [`GraphEngineCache`](../../../graph/transformation/GraphEngineCache.html "interface in com.facebook.buck.core.graph.transformation"),
            and computation.
            :::

        []{#get(com.facebook.buck.core.rules.analysis.RuleAnalysisKey)}

        -   #### get

            ``` methodSignature
            public RuleAnalysisResult get​(RuleAnalysisKey lookupKey)
            ```

            ::: block
            [Description copied from
            interface: `RuleAnalysisGraph`]{.descfrmTypeLabel}
            :::

            ::: block
            Finds the
            [`RuleAnalysisResult`](../RuleAnalysisResult.html "interface in com.facebook.buck.core.rules.analysis")
            of the given
            [`RuleAnalysisKey`](../RuleAnalysisKey.html "class in com.facebook.buck.core.rules.analysis"),
            starting computation as necessary. All dependencies required
            will also be transformed, and cached.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `get` in interface `RuleAnalysisGraph`

            [Parameters:]{.paramLabel}
            :   `lookupKey` - the
                [`RuleAnalysisKey`](../RuleAnalysisKey.html "class in com.facebook.buck.core.rules.analysis")
                to find the result for

            [Returns:]{.returnLabel}
            :   the
                [`RuleAnalysisResult`](../RuleAnalysisResult.html "interface in com.facebook.buck.core.rules.analysis")
                from analyzing the given
                [`RuleAnalysisKey`](../RuleAnalysisKey.html "class in com.facebook.buck.core.rules.analysis")

        []{#getAll(java.util.Set)}

        -   #### getAll

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<RuleAnalysisKey,​RuleAnalysisResult> getAll​(Set<RuleAnalysisKey> lookupKeys)
            ```

            ::: block
            [Description copied from
            interface: `RuleAnalysisGraph`]{.descfrmTypeLabel}
            :::

            ::: block
            same as
            [`RuleAnalysisGraph.get(RuleAnalysisKey)`](../computation/RuleAnalysisGraph.html#get(com.facebook.buck.core.rules.analysis.RuleAnalysisKey))
            but for multiple
            [`RuleAnalysisKey`](../RuleAnalysisKey.html "class in com.facebook.buck.core.rules.analysis")s
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAll` in interface `RuleAnalysisGraph`
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
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
