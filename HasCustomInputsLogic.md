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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.modern](package-summary.html)
:::

## Interface HasCustomInputsLogic {#interface-hascustominputslogic .title title="Interface HasCustomInputsLogic"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `VersionedTool`

    ------------------------------------------------------------------------

        public interface HasCustomInputsLogic

    ::: block
    Deriving inputs directly from the
    @[`AddToRuleKey`](../../rulekey/AddToRuleKey.html "annotation in com.facebook.buck.core.rulekey")
    annotated fields of some objects doesn\'t work correctly or is too
    slow. When deriving inputs from an object that implements
    HasCustomInputsLogic, the framework
    ([`BuildableSupport`](../common/BuildableSupport.html "class in com.facebook.buck.core.rules.common")
    /
    [`ModernBuildRule`](../../../rules/modern/ModernBuildRule.html "class in com.facebook.buck.rules.modern"))
    will call computeInputs() instead of deriving from \@AddToRuleKey
    fields.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type             Method                                                     Description
          ----------------------------- ---------------------------------------------------------- -------------
          `<E extends Exception>void`   `computeInputs​(ThrowingConsumer<SourcePath,​E> consumer)`    

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

        []{#computeInputs(com.facebook.buck.util.function.ThrowingConsumer)}

        -   #### computeInputs

            ``` methodSignature
            <E extends Exception> void computeInputs​(ThrowingConsumer<SourcePath,​E> consumer)
                                              throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`
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
