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
[Package]{.packageLabelInType} [com.facebook.buck.core.toolchain.toolprovider](package-summary.html)
:::

## Interface RuleAnalysisLegacyToolProvider {#interface-ruleanalysislegacytoolprovider .title title="Interface RuleAnalysisLegacyToolProvider"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `BinaryBuildRuleToolProvider`, `SystemToolProvider`

    ------------------------------------------------------------------------

        public interface RuleAnalysisLegacyToolProvider

    ::: block
    Provide
    [`RunInfo`](../../rules/providers/lib/RunInfo.html "class in com.facebook.buck.core.rules.providers.lib")
    from a
    [`ToolProvider`](ToolProvider.html "interface in com.facebook.buck.core.toolchain.toolprovider")
    so that legacy
    [`Tool`](../tool/Tool.html "interface in com.facebook.buck.core.toolchain.tool")s
    can be used in the rule analysis graph
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                       Description
          ------------------- ------------------------------------------------------------------------------------------------------------ -------------
          `RunInfo`           `getRunInfo​(DependencyOnlyRuleAnalysisContext context,           TargetConfiguration targetConfiguration)`    

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

        []{#getRunInfo(com.facebook.buck.core.rules.analysis.context.DependencyOnlyRuleAnalysisContext,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getRunInfo

            ``` methodSignature
            RunInfo getRunInfo​(DependencyOnlyRuleAnalysisContext context,
                               TargetConfiguration targetConfiguration)
            ```

            [Returns:]{.returnLabel}
            :   a
                [`RunInfo`](../../rules/providers/lib/RunInfo.html "class in com.facebook.buck.core.rules.providers.lib")
                that will execute a given tool
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
