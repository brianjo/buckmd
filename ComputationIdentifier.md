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
[Package]{.packageLabelInType} [com.facebook.buck.core.graph.transformation.model](package-summary.html)
:::

## Interface ComputationIdentifier\<ResultType extends [ComputeResult](ComputeResult.html "interface in com.facebook.buck.core.graph.transformation.model")\> {#interface-computationidentifierresulttype-extends-computeresult .title title="Interface ComputationIdentifier"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `ClassBasedComputationIdentifier`,
        `ComposedComputationIdentifier`

    ------------------------------------------------------------------------

        public interface ComputationIdentifier<ResultType extends ComputeResult>

    ::: block
    An Identifier for this
    [`ComputeKey`](ComputeKey.html "interface in com.facebook.buck.core.graph.transformation.model").
    The identifier is used to uniquely identify a
    [`ComputeKey`](ComputeKey.html "interface in com.facebook.buck.core.graph.transformation.model")
    to its corresponding
    [`GraphComputation`](../GraphComputation.html "interface in com.facebook.buck.core.graph.transformation"),
    so that all instances of a
    [`ComputeKey`](ComputeKey.html "interface in com.facebook.buck.core.graph.transformation.model")
    can look up the corresponding
    [`GraphComputation`](../GraphComputation.html "interface in com.facebook.buck.core.graph.transformation")
    correctly.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type     Method                   Description
          --------------------- ------------------------ -------------
          `Class<ResultType>`   `getResultTypeClass()`    

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

        []{#getResultTypeClass()}

        -   #### getResultTypeClass

            ``` methodSignature
            Class<ResultType> getResultTypeClass()
            ```

            [Returns:]{.returnLabel}
            :   the class of the result of the
                [`GraphComputation`](../GraphComputation.html "interface in com.facebook.buck.core.graph.transformation")
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
