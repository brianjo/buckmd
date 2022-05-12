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
[Package]{.packageLabelInType} [com.facebook.buck.core.model.platform](package-summary.html)
:::

## Interface ConstraintResolver {#interface-constraintresolver .title title="Interface ConstraintResolver"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `RuleBasedConstraintResolver`, `ThrowingConstraintResolver`

    ------------------------------------------------------------------------

        public interface ConstraintResolver

    ::: block
    An interface to access constraints using
    [`BuildTarget`](../BuildTarget.html "class in com.facebook.buck.core.model").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type     Method                                                                                                 Description
          --------------------- ------------------------------------------------------------------------------------------------------ -------------
          `ConstraintSetting`   `getConstraintSetting​(BuildTarget buildTarget,                     DependencyStack dependencyStack)`    
          `ConstraintValue`     `getConstraintValue​(BuildTarget buildTarget,                   DependencyStack dependencyStack)`        

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

        []{#getConstraintSetting(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.exceptions.DependencyStack)}

        -   #### getConstraintSetting

            ``` methodSignature
            ConstraintSetting getConstraintSetting​(BuildTarget buildTarget,
                                                   DependencyStack dependencyStack)
            ```

            [Returns:]{.returnLabel}
            :   [`ConstraintSetting`](ConstraintSetting.html "class in com.facebook.buck.core.model.platform")
                identified by a given
                [`BuildTarget`](../BuildTarget.html "class in com.facebook.buck.core.model").

        []{#getConstraintValue(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.exceptions.DependencyStack)}

        -   #### getConstraintValue

            ``` methodSignature
            ConstraintValue getConstraintValue​(BuildTarget buildTarget,
                                               DependencyStack dependencyStack)
            ```

            [Returns:]{.returnLabel}
            :   [`ConstraintValue`](ConstraintValue.html "class in com.facebook.buck.core.model.platform")
                identified by a given
                [`BuildTarget`](../BuildTarget.html "class in com.facebook.buck.core.model").
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
