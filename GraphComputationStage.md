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
-   Method

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

## Class GraphComputationStage\<KeyType extends [ComputeKey](../model/ComputeKey.html "interface in com.facebook.buck.core.graph.transformation.model")\<ResultType\>,​ResultType extends [ComputeResult](../model/ComputeResult.html "interface in com.facebook.buck.core.graph.transformation.model")\> {#class-graphcomputationstagekeytype-extends-computekeyresulttyperesulttype-extends-computeresult .title title="Class GraphComputationStage"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.graph.transformation.impl.GraphComputationStage\<KeyType,​ResultType\>

::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `KeyType` - the type of the
        [`ComputeKey`](../model/ComputeKey.html "interface in com.facebook.buck.core.graph.transformation.model")
        for this stage
    :   `ResultType` - the type of the
        [`ComputeResult`](../model/ComputeResult.html "interface in com.facebook.buck.core.graph.transformation.model")
        for this stage

    ------------------------------------------------------------------------

        public class GraphComputationStage<KeyType extends ComputeKey<ResultType>,​ResultType extends ComputeResult>
        extends Object

    ::: block
    Represents one \"stage\" of computation in the
    [`GraphTransformationEngine`](../GraphTransformationEngine.html "interface in com.facebook.buck.core.graph.transformation").
    This maps to a single transformation by a
    [`GraphComputation`](../GraphComputation.html "interface in com.facebook.buck.core.graph.transformation")
    from a
    [`ComputeKey`](../model/ComputeKey.html "interface in com.facebook.buck.core.graph.transformation.model")
    to a
    [`ComputeResult`](../model/ComputeResult.html "interface in com.facebook.buck.core.graph.transformation.model").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                  Description
          -------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `GraphComputationStage​(GraphComputation<KeyType,​ResultType> transformer)`                                                                     
          `GraphComputationStage​(GraphComputation<KeyType,​ResultType> transformer,                      GraphEngineCache<KeyType,​ResultType> cache)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.graph.transformation.GraphComputation)}

        -   #### GraphComputationStage

                public GraphComputationStage​(GraphComputation<KeyType,​ResultType> transformer)

        []{#<init>(com.facebook.buck.core.graph.transformation.GraphComputation,com.facebook.buck.core.graph.transformation.GraphEngineCache)}

        -   #### GraphComputationStage

                public GraphComputationStage​(GraphComputation<KeyType,​ResultType> transformer,
                                             GraphEngineCache<KeyType,​ResultType> cache)
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
-   Method

</div>

[]{#skip.navbar.bottom}
:::
