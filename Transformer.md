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
[Package]{.packageLabelInType} [com.facebook.buck.core.graph.transformation.composition](package-summary.html)
:::

## Interface Transformer\<KeyInput extends [ComputeKey](../model/ComputeKey.html "interface in com.facebook.buck.core.graph.transformation.model")\<ResultInput\>,​ResultInput extends [ComputeResult](../model/ComputeResult.html "interface in com.facebook.buck.core.graph.transformation.model"),​ResultType extends [ComputeResult](../model/ComputeResult.html "interface in com.facebook.buck.core.graph.transformation.model")\> {#interface-transformerkeyinput-extends-computekeyresultinputresultinput-extends-computeresultresulttype-extends-computeresult .title title="Interface Transformer"}
:::

::: contentContainer
::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `KeyInput` - the key type that the
        [`transform(Map)`](#transform(java.util.Map)) receive
    :   `ResultInput` - the result type that the
        [`transform(Map)`](#transform(java.util.Map)) receive
    :   `ResultType` - the type of the result from this transform

    ```{=html}
    <!-- -->
    ```

    Functional Interface:
    :   This is a functional interface and can therefore be used as the
        assignment target for a lambda expression or method reference.

    ------------------------------------------------------------------------

        @FunctionalInterface
        public interface Transformer<KeyInput extends ComputeKey<ResultInput>,​ResultInput extends ComputeResult,​ResultType extends ComputeResult>

    ::: block
    Generic transform API that given all dependencies through the
    [`ComputationEnvironment`](../ComputationEnvironment.html "interface in com.facebook.buck.core.graph.transformation"),
    computes the desired result of ResultType.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                          Method                                        Description
          ------------------------------------------ --------------------------------------------- -------------
          `Map<ComputeKey<ResultType>,​ResultType>`   `transform​(Map<KeyInput,​ResultInput> deps)`    

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

        []{#transform(java.util.Map)}

        -   #### transform

            ``` methodSignature
            Map<ComputeKey<ResultType>,​ResultType> transform​(Map<KeyInput,​ResultInput> deps)
            ```

            [Parameters:]{.paramLabel}
            :   `deps` - the results that the correspond to the keys
                [`Composer`](Composer.html "interface in com.facebook.buck.core.graph.transformation.composition")
                returned

            [Returns:]{.returnLabel}
            :   the results to be aggregate into a
                [`ComposedResult`](../model/ComposedResult.html "class in com.facebook.buck.core.graph.transformation.model")
                by the
                [`ComposedComputation`](ComposedComputation.html "interface in com.facebook.buck.core.graph.transformation.composition")
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
