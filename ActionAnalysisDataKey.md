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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.analysis.action](package-summary.html)
:::

## Interface ActionAnalysisDataKey {#interface-actionanalysisdatakey .title title="Interface ActionAnalysisDataKey"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface ActionAnalysisDataKey

    ::: block
    The key used to look up the corresponding
    [`ActionAnalysisData`](ActionAnalysisData.html "interface in com.facebook.buck.core.rules.analysis.action").
    This key has the
    [`BuildTarget`](../../../model/BuildTarget.html "class in com.facebook.buck.core.model")
    to look up the corresponding rule anlaysis computation that produced
    the desired
    [`ActionAnalysisData`](ActionAnalysisData.html "interface in com.facebook.buck.core.rules.analysis.action").
    The
    [`ActionAnalysisData.ID`](ActionAnalysisData.ID.html "class in com.facebook.buck.core.rules.analysis.action")
    is the unique identifier of the desired
    [`ActionAnalysisData`](ActionAnalysisData.html "interface in com.facebook.buck.core.rules.analysis.action"),
    which is used to identify the
    [`ActionAnalysisData`](ActionAnalysisData.html "interface in com.facebook.buck.core.rules.analysis.action")
    of the many that a single rule analysis of a
    [`BuildTarget`](../../../model/BuildTarget.html "class in com.facebook.buck.core.model")
    could produce.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                Method                                                      Description
          -------------------------------- ----------------------------------------------------------- -------------
          `BuildTarget`                    `getBuildTarget()`                                           
          `ActionAnalysisData.ID`          `getID()`                                                    
          `static ActionAnalysisDataKey`   `of​(BuildTarget buildTarget,   ActionAnalysisData.ID iD)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildTarget()}

        -   #### getBuildTarget

            ``` methodSignature
            BuildTarget getBuildTarget()
            ```

            [Returns:]{.returnLabel}
            :   the
                [`BuildTarget`](../../../model/BuildTarget.html "class in com.facebook.buck.core.model")
                for the rule analysis which the corresponding
                [`ActionAnalysisData`](ActionAnalysisData.html "interface in com.facebook.buck.core.rules.analysis.action")
                is created from

        []{#getID()}

        -   #### getID

            ``` methodSignature
            ActionAnalysisData.ID getID()
            ```

            [Returns:]{.returnLabel}
            :   the unique and stable ID of the corresponding
                [`ActionAnalysisData`](ActionAnalysisData.html "interface in com.facebook.buck.core.rules.analysis.action")

        []{#of(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.analysis.action.ActionAnalysisData.ID)}

        -   #### of

            ``` methodSignature
            static ActionAnalysisDataKey of​(BuildTarget buildTarget,
                                            ActionAnalysisData.ID iD)
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
