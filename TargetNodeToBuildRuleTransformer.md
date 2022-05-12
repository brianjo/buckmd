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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.transformer](package-summary.html)
:::

## Interface TargetNodeToBuildRuleTransformer {#interface-targetnodetobuildruletransformer .title title="Interface TargetNodeToBuildRuleTransformer"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `DefaultTargetNodeToBuildRuleTransformer`,
        `LegacyRuleAnalysisDelegatingTargetNodeToBuildRuleTransformer`,
        `LegacyRuleAnalysisProviderCompatibleTargetNodeToBuildRuleTransformer`

    ------------------------------------------------------------------------

        public interface TargetNodeToBuildRuleTransformer
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `                     | `transform​(To         | ::: block             |
        | default <T extends Bu | olchainProvider toolc | Transform target node |
        | ildRuleArg>BuildRule` | hainProvider,         | to build rule.        |
        |                       |   TargetGraph targetG | :::                   |
        |                       | raph,          Config |                       |
        |                       | urationRuleRegistry c |                       |
        |                       | onfigurationRuleRegis |                       |
        |                       | try,          ActionG |                       |
        |                       | raphBuilder graphBuil |                       |
        |                       | der,          TargetN |                       |
        |                       | ode<T> targetNode,    |                       |
        |                       |        CellPathResolv |                       |
        |                       | er cellPathResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `<T extends Bu        | `trans                | ::: block             |
        | ildRuleArg>BuildRule` | form​(ToolchainProvide | Converts a given      |
        |                       | r toolchainProvider,  | [`Targ                |
        |                       |          TargetGraph  | etNode`](../../model/ |
        |                       | targetGraph,          | targetgraph/TargetNod |
        |                       |  ConfigurationRuleReg | e.html "interface in  |
        |                       | istry configurationRu | com.facebook.buck.cor |
        |                       | leRegistry,           | e.model.targetgraph") |
        |                       | ActionGraphBuilder gr | to a                  |
        |                       | aphBuilder,           | [`BuildRule`]         |
        |                       | TargetNode<T> targetN | (../BuildRule.html "i |
        |                       | ode,          Provide | nterface in com.faceb |
        |                       | rInfoCollection provi | ook.buck.core.rules") |
        |                       | derInfoCollection,    | as part of action     |
        |                       |        CellPathResolv | graph construction.   |
        |                       | er cellPathResolver)` | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#transform(com.facebook.buck.core.toolchain.ToolchainProvider,com.facebook.buck.core.model.targetgraph.TargetGraph,com.facebook.buck.core.rules.config.registry.ConfigurationRuleRegistry,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.model.targetgraph.TargetNode,com.facebook.buck.core.cell.CellPathResolver)}

        -   #### transform

            ``` methodSignature
            default <T extends BuildRuleArg> BuildRule transform​(ToolchainProvider toolchainProvider,
                                                                 TargetGraph targetGraph,
                                                                 ConfigurationRuleRegistry configurationRuleRegistry,
                                                                 ActionGraphBuilder graphBuilder,
                                                                 TargetNode<T> targetNode,
                                                                 CellPathResolver cellPathResolver)
            ```

            ::: block
            Transform target node to build rule.
            :::

        []{#transform(com.facebook.buck.core.toolchain.ToolchainProvider,com.facebook.buck.core.model.targetgraph.TargetGraph,com.facebook.buck.core.rules.config.registry.ConfigurationRuleRegistry,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.model.targetgraph.TargetNode,com.facebook.buck.core.rules.providers.collect.ProviderInfoCollection,com.facebook.buck.core.cell.CellPathResolver)}

        -   #### transform

            ``` methodSignature
            <T extends BuildRuleArg> BuildRule transform​(ToolchainProvider toolchainProvider,
                                                         TargetGraph targetGraph,
                                                         ConfigurationRuleRegistry configurationRuleRegistry,
                                                         ActionGraphBuilder graphBuilder,
                                                         TargetNode<T> targetNode,
                                                         ProviderInfoCollection providerInfoCollection,
                                                         CellPathResolver cellPathResolver)
            ```

            ::: block
            Converts a given
            [`TargetNode`](../../model/targetgraph/TargetNode.html "interface in com.facebook.buck.core.model.targetgraph")
            to a
            [`BuildRule`](../BuildRule.html "interface in com.facebook.buck.core.rules")
            as part of action graph construction. The providers computed
            from
            [`LegacyProviderCompatibleDescription.createProviders(ProviderCreationContext,  BuildTarget, BuildRuleArg)`](../LegacyProviderCompatibleDescription.html#createProviders(com.facebook.buck.core.rules.ProviderCreationContext,com.facebook.buck.core.model.BuildTarget,T))
            will be passed to this function to be used to construct the
            [`BuildRule`](../BuildRule.html "interface in com.facebook.buck.core.rules")
            :::
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
