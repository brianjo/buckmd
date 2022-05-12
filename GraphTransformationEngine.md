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
-   [Package](package-summary.html)
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
[Package]{.packageLabelInType} [com.facebook.buck.core.graph.transformation](package-summary.html)
:::

## Interface GraphTransformationEngine {#interface-graphtransformationengine .title title="Interface GraphTransformationEngine"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AutoCloseable`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `DefaultGraphTransformationEngine`

    ------------------------------------------------------------------------

        public interface GraphTransformationEngine
        extends AutoCloseable

    ::: block
    Transformation engine that transforms supplied ComputeKey into
    ComputeResult via
    [`GraphComputation`](GraphComputation.html "interface in com.facebook.buck.core.graph.transformation").
    This engine is able to asynchronously run graph based computation,
    reusing results when possible. Note that the computation graph must
    be an acyclic graph.
    This engine is able to deal with dependencies in the computation
    graph by having
    [`GraphComputation`](GraphComputation.html "interface in com.facebook.buck.core.graph.transformation")
    request dependent results of other transformations through
    [`GraphComputation.discoverPreliminaryDeps(ComputeKey)`](GraphComputation.html#discoverPreliminaryDeps(Key))
    and
    [`GraphComputation.discoverDeps(ComputeKey, ComputationEnvironment)`](GraphComputation.html#discoverDeps(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
    :::
:::

::: summary
-   ::: {.section role="region"}
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
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#close()}

        -   #### close

            ``` methodSignature
            void close()
            ```

            ::: block
            Shuts down the engine and rejects any future computations
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

        []{#compute(com.facebook.buck.core.graph.transformation.model.ComputeKey)}
        []{#compute(KeyType)}

        -   #### compute

            ``` methodSignature
            <KeyType extends ComputeKey<ResultType>,​ResultType extends ComputeResult> Future<ResultType> compute​(KeyType key)
            ```

            ::: block
            Asynchronously computes the result for the given key
            :::

            [Parameters:]{.paramLabel}
            :   `key` - the specific Key on the graph to compute

            [Returns:]{.returnLabel}
            :   future of the result of applying the transformer on the
                graph with the given key

        []{#computeUnchecked(com.facebook.buck.core.graph.transformation.model.ComputeKey)}
        []{#computeUnchecked(KeyType)}

        -   #### computeUnchecked

            ``` methodSignature
            <KeyType extends ComputeKey<ResultType>,​ResultType extends ComputeResult> ResultType computeUnchecked​(KeyType key)
            ```

            ::: block
            Synchronously computes the given key
            :::

            [Parameters:]{.paramLabel}
            :   `key` - the specific Key on the graph to compute

            [Returns:]{.returnLabel}
            :   the result of applying the transformer on the graph with
                the given key

        []{#computeAll(java.util.Set)}

        -   #### computeAll

            ``` methodSignature
            <KeyType extends ComputeKey<ResultType>,​ResultType extends ComputeResult> com.google.common.collect.ImmutableMap<KeyType,​Future<ResultType>> computeAll​(Set<KeyType> keys)
            ```

            ::: block
            Asynchronously computes the result for multiple keys
            :::

            [Parameters:]{.paramLabel}
            :   `keys` - iterable of keys to compute on the graph

            [Returns:]{.returnLabel}
            :   a map of futures of the result for each of the keys
                supplied

        []{#computeAllUnchecked(java.util.Set)}

        -   #### computeAllUnchecked

            ``` methodSignature
            <KeyType extends ComputeKey<ResultType>,​ResultType extends ComputeResult> com.google.common.collect.ImmutableMap<KeyType,​ResultType> computeAllUnchecked​(Set<KeyType> keys)
            ```

            ::: block
            Synchronously computes the result for multiple keys
            :::

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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
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
