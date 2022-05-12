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
[Package]{.packageLabelInType} [com.facebook.buck.core.description.attr](package-summary.html)
:::

## Interface ImplicitInputsInferringDescription\<T\> {#interface-implicitinputsinferringdescriptiont .title title="Interface ImplicitInputsInferringDescription"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `ExportFileDescription`

    ------------------------------------------------------------------------

        public interface ImplicitInputsInferringDescription<T>

    ::: block
    While building up the target graph, we infer implicit inputs of a
    rule if certain fields are absent (e.g. src field). Any
    [`Description`](../Description.html "interface in com.facebook.buck.core.description")
    that implements this interface can modify its implicit inputs by
    poking at the raw build rule params.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                Method                                                                                                                Description
          ---------------------------------------------------------------- --------------------------------------------------------------------------------------------------------------------- -------------
          `com.google.common.collect.ImmutableList<ForwardRelativePath>`   `inferInputsFromConstructorArgs​(UnflavoredBuildTarget buildTarget,                               T constructorArg)`    

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

        []{#inferInputsFromConstructorArgs(com.facebook.buck.core.model.UnflavoredBuildTarget,java.lang.Object)}
        []{#inferInputsFromConstructorArgs(com.facebook.buck.core.model.UnflavoredBuildTarget,T)}

        -   #### inferInputsFromConstructorArgs

            ``` methodSignature
            com.google.common.collect.ImmutableList<ForwardRelativePath> inferInputsFromConstructorArgs​(UnflavoredBuildTarget buildTarget,
                                                                                                        T constructorArg)
            ```
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
