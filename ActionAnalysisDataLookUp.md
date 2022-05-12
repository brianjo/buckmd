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

## Interface ActionAnalysisDataLookUp {#interface-actionanalysisdatalookup .title title="Interface ActionAnalysisDataLookUp"}
:::

::: contentContainer
::: description
-   

    All Known Subinterfaces:
    :   `RuleAnalysisResult`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `LegacyProviderRuleAnalysisResult`

    ------------------------------------------------------------------------

        public interface ActionAnalysisDataLookUp

    ::: block
    Interface for querying for
    [`ActionAnalysisData`](ActionAnalysisData.html "interface in com.facebook.buck.core.rules.analysis.action")
    via their unique
    [`ActionAnalysisData.ID`](ActionAnalysisData.ID.html "class in com.facebook.buck.core.rules.analysis.action").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                    Method                                           Description
          ------------------------------------------------------------------------------------ ------------------------------------------------ -------------
          `boolean`                                                                            `actionExists​(ActionAnalysisData.ID key)`         
          `Optional<ActionAnalysisData>`                                                       `getActionOptional​(ActionAnalysisData.ID key)`    
          `com.google.common.collect.ImmutableMap<ActionAnalysisData.ID,​ActionAnalysisData>`   `getRegisteredActions()`                          

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

        []{#actionExists(com.facebook.buck.core.rules.analysis.action.ActionAnalysisData.ID)}

        -   #### actionExists

            ``` methodSignature
            boolean actionExists​(ActionAnalysisData.ID key)
            ```

            [Returns:]{.returnLabel}
            :   if the given key exists in the look up

        []{#getActionOptional(com.facebook.buck.core.rules.analysis.action.ActionAnalysisData.ID)}

        -   #### getActionOptional

            ``` methodSignature
            Optional<ActionAnalysisData> getActionOptional​(ActionAnalysisData.ID key)
            ```

            [Returns:]{.returnLabel}
            :   the
                [`ActionAnalysisData`](ActionAnalysisData.html "interface in com.facebook.buck.core.rules.analysis.action")
                if exists, else `Optional.empty`

        []{#getRegisteredActions()}

        -   #### getRegisteredActions

            ``` methodSignature
            com.google.common.collect.ImmutableMap<ActionAnalysisData.ID,​ActionAnalysisData> getRegisteredActions()
            ```

            [Returns:]{.returnLabel}
            :   all the registered
                [`ActionAnalysisData`](ActionAnalysisData.html "interface in com.facebook.buck.core.rules.analysis.action")
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