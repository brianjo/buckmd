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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.graph.transformation.impl](package-summary.html)
:::

## Class DefaultGraphTransformationEngine {#class-defaultgraphtransformationengine .title title="Class DefaultGraphTransformationEngine"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.graph.transformation.impl.DefaultGraphTransformationEngine

::: description
-   

    All Implemented Interfaces:
    :   `GraphTransformationEngine`, `AutoCloseable`

    ------------------------------------------------------------------------

        public final class DefaultGraphTransformationEngine
        extends Object
        implements GraphTransformationEngine

    ::: block
    Transformation engine that transforms supplied
    [`ComputeKey`](../model/ComputeKey.html "interface in com.facebook.buck.core.graph.transformation.model")
    into
    [`ComputeResult`](../model/ComputeResult.html "interface in com.facebook.buck.core.graph.transformation.model")
    via
    [`GraphComputation`](../GraphComputation.html "interface in com.facebook.buck.core.graph.transformation").
    This engine is able to asynchronously run graph based computation,
    reusing results when possible. Note that the computation dependency
    graph must be an acyclic graph.
    This engine is able to deal with dependencies in the computation
    graph by having Transformer request dependent results of other
    transformations through
    [`GraphComputation.discoverPreliminaryDeps(ComputeKey)`](../GraphComputation.html#discoverPreliminaryDeps(Key))
    and
    [`GraphComputation.discoverDeps(ComputeKey, ComputationEnvironment)`](../GraphComputation.html#discoverDeps(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment)).
    The engine guarantees that all dependencies are completed before
    performing the transformation.

    This engine allows for multiple stages of transformations via
    different
    [`GraphComputation`](../GraphComputation.html "interface in com.facebook.buck.core.graph.transformation")s.
    These are specified during construction of the engine by supplying
    multiple
    [`GraphComputationStage`](GraphComputationStage.html "class in com.facebook.buck.core.graph.transformation.impl")s.
    Different stages are allowed to depend on other stages, as long as
    the computation nodes do not form a cyclic dependency.

    [`GraphComputation.discoverPreliminaryDeps(ComputeKey)`](../GraphComputation.html#discoverPreliminaryDeps(Key))
    will be ran first to discover a set of dependencies based only on
    the
    [`ComputeKey`](../model/ComputeKey.html "interface in com.facebook.buck.core.graph.transformation.model").
    The keys are then computed, and the results passed via the
    [`ComputationEnvironment`](../ComputationEnvironment.html "interface in com.facebook.buck.core.graph.transformation")
    to
    [`GraphComputation.discoverDeps(ComputeKey, ComputationEnvironment)`](../GraphComputation.html#discoverDeps(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
    for a second stage of dependency discovery, where the dependency
    discovery can use the dependencies previously specified. The results
    of dependencies returned via both
    [`GraphComputation.discoverPreliminaryDeps(ComputeKey)`](../GraphComputation.html#discoverPreliminaryDeps(Key))
    and
    [`GraphComputation.discoverDeps(ComputeKey, ComputationEnvironment)`](../GraphComputation.html#discoverDeps(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
    will be available for the
    [`GraphComputation.transform(ComputeKey, ComputationEnvironment)`](../GraphComputation.html#transform(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
    operation.

    Transformations also should never block waiting for each other in
    any manner. If required to wait, the transformation must declare it
    through
    [`GraphComputation.discoverPreliminaryDeps(ComputeKey)`](../GraphComputation.html#discoverPreliminaryDeps(Key))
    or
    [`GraphComputation.discoverDeps(ComputeKey, ComputationEnvironment)`](../GraphComputation.html#discoverDeps(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))

    The transformation is incremental, so cached portions of the
    transformation will be used whenever possible based on
    `ComputeKey.equals()`. Therefore,
    [`ComputeKey`](../model/ComputeKey.html "interface in com.facebook.buck.core.graph.transformation.model")
    should be immutable, and have deterministic equals. For future
    perspective, we want to have
    [`ComputeKey`](../model/ComputeKey.html "interface in com.facebook.buck.core.graph.transformation.model")
    be serializable, so that we can eventually send keys to be computed
    remotely.

    A custom cache can be supplied to the engine to cache the
    computation as desired.

    Transformations will be applied asynchronously, so independent
    transformations can be executed in parallel. It is therefore
    important that transformations are thread safe.

    By using all callback based operations and queue based operations,
    this engine will also reduce stack usage, eliminating stack overflow
    for large graph computations, provided that the
    [`GraphComputation`](../GraphComputation.html "interface in com.facebook.buck.core.graph.transformation")
    itself does not stack overflow within its
    [`GraphComputation.discoverPreliminaryDeps(ComputeKey)`](../GraphComputation.html#discoverPreliminaryDeps(Key)),
    [`GraphComputation.discoverDeps(ComputeKey, ComputationEnvironment)`](../GraphComputation.html#discoverDeps(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment)),
    and
    [`GraphComputation.transform(ComputeKey, ComputationEnvironment)`](../GraphComputation.html#transform(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
    methods.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `DefaultGraphTran                 | ::: block                         |
        | sformationEngine​(com.google.commo | Constructs a                      |
        | n.collect.ImmutableList<GraphComp | [`D                               |
        | utationStage<?,​?>> stages,        | efaultGraphTransformationEngine`] |
        |                           int est | (DefaultGraphTransformationEngine |
        | imatedNumOps,                     | .html "class in com.facebook.buck |
        |              DepsAwareExecutor<?  | .core.graph.transformation.impl") |
        | super ComputeResult,​?> executor)` | with the given transformations.   |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `close()`             | ::: block             |
        |                       |                       | Shuts down the engine |
        |                       |                       | and rejects any       |
        |                       |                       | future computations   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `<KeyType             | `                     | ::: block             |
        |  extends ComputeKey<R | compute​(KeyType key)` | Asynchronously        |
        | esultType>,​ResultType |                       | computes the result   |
        |  extends ComputeResul |                       | for the given key     |
        | t>Future<ResultType>` |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `<KeyType exten       | `computeAl            | ::: block             |
        | ds ComputeKey<ResultT | l​(Set<KeyType> keys)` | Asynchronously        |
        | ype>,​ResultType exten |                       | computes the result   |
        | ds ComputeResult>com. |                       | for multiple keys     |
        | google.common.collect |                       | :::                   |
        | .ImmutableMap<KeyType |                       |                       |
        | ,​Future<ResultType>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `<KeyTy               | `computeAllUnchecke   | ::: block             |
        | pe extends ComputeKey | d​(Set<KeyType> keys)` | Synchronously         |
        | <ResultType>,​ResultTy |                       | computes the result   |
        | pe extends ComputeRes |                       | for multiple keys     |
        | ult>com.google.common |                       | :::                   |
        | .collect.ImmutableMap |                       |                       |
        | <KeyType,​ResultType>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `computeUn            | ::: block             |
        | <KeyType extends Comp | checked​(KeyType key)` | Synchronously         |
        | uteKey<ResultType>,​Re |                       | computes the given    |
        | sultType extends Comp |                       | key                   |
        | uteResult>ResultType` |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.google.common.collect.ImmutableList,int,com.facebook.buck.core.graph.transformation.executor.DepsAwareExecutor)}

        -   #### DefaultGraphTransformationEngine

                public DefaultGraphTransformationEngine​(com.google.common.collect.ImmutableList<GraphComputationStage<?,​?>> stages,
                                                        int estimatedNumOps,
                                                        DepsAwareExecutor<? super ComputeResult,​?> executor)

            ::: block
            Constructs a
            [`DefaultGraphTransformationEngine`](DefaultGraphTransformationEngine.html "class in com.facebook.buck.core.graph.transformation.impl")
            with the given transformations.
            :::

            [Parameters:]{.paramLabel}
            :   `stages` - all of the available transformation stages
                this engine can execute
            :   `estimatedNumOps` - the estimated number of operations
                this engine will execute given a computation, to reserve
                the size of its computation index
            :   `executor` - the custom
                [`DepsAwareExecutor`](../executor/DepsAwareExecutor.html "interface in com.facebook.buck.core.graph.transformation.executor")
                the engine uses to execute tasks
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
            ```

            ::: block
            [Description copied from
            interface: `GraphTransformationEngine`]{.descfrmTypeLabel}
            :::

            ::: block
            Shuts down the engine and rejects any future computations
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `GraphTransformationEngine`

        []{#compute(com.facebook.buck.core.graph.transformation.model.ComputeKey)}
        []{#compute(KeyType)}

        -   #### compute

            ``` methodSignature
            public final <KeyType extends ComputeKey<ResultType>,​ResultType extends ComputeResult> Future<ResultType> compute​(KeyType key)
            ```

            ::: block
            [Description copied from
            interface: `GraphTransformationEngine`]{.descfrmTypeLabel}
            :::

            ::: block
            Asynchronously computes the result for the given key
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `compute` in interface `GraphTransformationEngine`

            [Parameters:]{.paramLabel}
            :   `key` - the specific Key on the graph to compute

            [Returns:]{.returnLabel}
            :   future of the result of applying the transformer on the
                graph with the given key

        []{#computeUnchecked(com.facebook.buck.core.graph.transformation.model.ComputeKey)}
        []{#computeUnchecked(KeyType)}

        -   #### computeUnchecked

            ``` methodSignature
            public final <KeyType extends ComputeKey<ResultType>,​ResultType extends ComputeResult> ResultType computeUnchecked​(KeyType key)
            ```

            ::: block
            [Description copied from
            interface: `GraphTransformationEngine`]{.descfrmTypeLabel}
            :::

            ::: block
            Synchronously computes the given key
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `computeUnchecked` in
                interface `GraphTransformationEngine`

            [Parameters:]{.paramLabel}
            :   `key` - the specific Key on the graph to compute

            [Returns:]{.returnLabel}
            :   the result of applying the transformer on the graph with
                the given key

        []{#computeAll(java.util.Set)}

        -   #### computeAll

            ``` methodSignature
            public final <KeyType extends ComputeKey<ResultType>,​ResultType extends ComputeResult> com.google.common.collect.ImmutableMap<KeyType,​Future<ResultType>> computeAll​(Set<KeyType> keys)
            ```

            ::: block
            [Description copied from
            interface: `GraphTransformationEngine`]{.descfrmTypeLabel}
            :::

            ::: block
            Asynchronously computes the result for multiple keys
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `computeAll` in interface `GraphTransformationEngine`

            [Parameters:]{.paramLabel}
            :   `keys` - iterable of keys to compute on the graph

            [Returns:]{.returnLabel}
            :   a map of futures of the result for each of the keys
                supplied

        []{#computeAllUnchecked(java.util.Set)}

        -   #### computeAllUnchecked

            ``` methodSignature
            public final <KeyType extends ComputeKey<ResultType>,​ResultType extends ComputeResult> com.google.common.collect.ImmutableMap<KeyType,​ResultType> computeAllUnchecked​(Set<KeyType> keys)
            ```

            ::: block
            [Description copied from
            interface: `GraphTransformationEngine`]{.descfrmTypeLabel}
            :::

            ::: block
            Synchronously computes the result for multiple keys
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `computeAllUnchecked` in
                interface `GraphTransformationEngine`

            [Parameters:]{.paramLabel}
            :   `keys` - iterable of the keys to compute on the graph

            [Returns:]{.returnLabel}
            :   a map of the results for each of the keys supplied
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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
