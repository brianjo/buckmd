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
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.actions](package-summary.html)
:::

## Interface ActionWrapperData {#interface-actionwrapperdata .title title="Interface ActionWrapperData"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `ActionAnalysisData`

    ------------------------------------------------------------------------

        public interface ActionWrapperData
        extends ActionAnalysisData

    ::: block
    Implementation of
    [`ActionAnalysisData`](../analysis/action/ActionAnalysisData.html "interface in com.facebook.buck.core.rules.analysis.action")
    that just holds an
    [`Action`](Action.html "interface in com.facebook.buck.core.rules.actions").
    This mimics the effect of having a deferred
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.core.rules.analysis.action.ActionAnalysisData}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.core.rules.analysis.action.[ActionAnalysisData](../analysis/action/ActionAnalysisData.html "interface in com.facebook.buck.core.rules.analysis.action")

            `ActionAnalysisData.ID`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type         Method          Description
          ------------------------- --------------- -------------
          `Action`                  `getAction()`    
          `ActionAnalysisDataKey`   `getKey()`       

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

        []{#getKey()}

        -   #### getKey

            ``` methodSignature
            ActionAnalysisDataKey getKey()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getKey` in interface `ActionAnalysisData`

            [Returns:]{.returnLabel}
            :   the identifier for this
                [`ActionAnalysisData`](../analysis/action/ActionAnalysisData.html "interface in com.facebook.buck.core.rules.analysis.action"),
                which points to the corresponding rule analysis

        []{#getAction()}

        -   #### getAction

            ``` methodSignature
            Action getAction()
            ```

            [Returns:]{.returnLabel}
            :   the
                [`Action`](Action.html "interface in com.facebook.buck.core.rules.actions")
                this wraps
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
-   [Nested](#nested.class.summary) \| 
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
