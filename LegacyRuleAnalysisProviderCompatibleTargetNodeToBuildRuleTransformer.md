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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.transformer.impl](package-summary.html)
:::

## Class LegacyRuleAnalysisProviderCompatibleTargetNodeToBuildRuleTransformer {#class-legacyruleanalysisprovidercompatibletargetnodetobuildruletransformer .title title="Class LegacyRuleAnalysisProviderCompatibleTargetNodeToBuildRuleTransformer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.transformer.impl.LegacyRuleAnalysisDelegatingTargetNodeToBuildRuleTransformer](LegacyRuleAnalysisDelegatingTargetNodeToBuildRuleTransformer.html "class in com.facebook.buck.core.rules.transformer.impl")

    -   -   com.facebook.buck.core.rules.transformer.impl.LegacyRuleAnalysisProviderCompatibleTargetNodeToBuildRuleTransformer

::: description
-   

    All Implemented Interfaces:
    :   `TargetNodeToBuildRuleTransformer`

    ------------------------------------------------------------------------

        public class LegacyRuleAnalysisProviderCompatibleTargetNodeToBuildRuleTransformer
        extends LegacyRuleAnalysisDelegatingTargetNodeToBuildRuleTransformer

    ::: block
    A
    [`TargetNodeToBuildRuleTransformer`](../TargetNodeToBuildRuleTransformer.html "interface in com.facebook.buck.core.rules.transformer")
    that delegates to the
    [`RuleAnalysisGraph`](../../analysis/computation/RuleAnalysisGraph.html "interface in com.facebook.buck.core.rules.analysis.computation")
    when descriptions of the new type
    [`RuleDescription`](../../../description/RuleDescription.html "interface in com.facebook.buck.core.description")
    is encountered. A backwards compatible
    [`RuleAnalysisLegacyBuildRuleView`](../../impl/RuleAnalysisLegacyBuildRuleView.html "class in com.facebook.buck.core.rules.impl")
    is returned for that target.
    For any legacy rules, the
    [`Provider`](../../providers/Provider.html "interface in com.facebook.buck.core.rules.providers")s
    from
    [`LegacyProviderCompatibleDescription.createProviders(ProviderCreationContext,  BuildTarget, BuildRuleArg)`](../../LegacyProviderCompatibleDescription.html#createProviders(com.facebook.buck.core.rules.ProviderCreationContext,com.facebook.buck.core.model.BuildTarget,T))
    will be supplied to the
    [`DescriptionWithTargetGraph.createBuildRule(BuildRuleCreationContextWithTargetGraph,  BuildTarget, BuildRuleParams, BuildRuleArg)`](../../DescriptionWithTargetGraph.html#createBuildRule(com.facebook.buck.core.rules.BuildRuleCreationContextWithTargetGraph,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.BuildRuleParams,T))
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.core.rules.transformer.impl.LegacyRuleAnalysisDelegatingTargetNodeToBuildRuleTransformer}

            ### Fields inherited from class com.facebook.buck.core.rules.transformer.impl.[LegacyRuleAnalysisDelegatingTargetNodeToBuildRuleTransformer](LegacyRuleAnalysisDelegatingTargetNodeToBuildRuleTransformer.html "class in com.facebook.buck.core.rules.transformer.impl")

            `delegate, ruleAnalysisComputation`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                        Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `LegacyRuleAnalysisProviderCompatibleTargetNodeToBuildRuleTransformer​(RuleAnalysisGraph ruleAnalysisComputation,                                                                     TargetNodeToBuildRuleTransformer delegate)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `<T extends Bu        | `transform​(To         | ::: block             |
        | ildRuleArg>BuildRule` | olchainProvider toolc | Transform target node |
        |                       | hainProvider,         | to build rule.        |
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

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.transformer.impl.LegacyRuleAnalysisDelegatingTargetNodeToBuildRuleTransformer}

            ### Methods inherited from class com.facebook.buck.core.rules.transformer.impl.[LegacyRuleAnalysisDelegatingTargetNodeToBuildRuleTransformer](LegacyRuleAnalysisDelegatingTargetNodeToBuildRuleTransformer.html "class in com.facebook.buck.core.rules.transformer.impl")

            `transform`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.rules.analysis.computation.RuleAnalysisGraph,com.facebook.buck.core.rules.transformer.TargetNodeToBuildRuleTransformer)}

        -   #### LegacyRuleAnalysisProviderCompatibleTargetNodeToBuildRuleTransformer

                public LegacyRuleAnalysisProviderCompatibleTargetNodeToBuildRuleTransformer​(RuleAnalysisGraph ruleAnalysisComputation,
                                                                                            TargetNodeToBuildRuleTransformer delegate)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#transform(com.facebook.buck.core.toolchain.ToolchainProvider,com.facebook.buck.core.model.targetgraph.TargetGraph,com.facebook.buck.core.rules.config.registry.ConfigurationRuleRegistry,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.model.targetgraph.TargetNode,com.facebook.buck.core.cell.CellPathResolver)}

        -   #### transform

            ``` methodSignature
            public <T extends BuildRuleArg> BuildRule transform​(ToolchainProvider toolchainProvider,
                                                                TargetGraph targetGraph,
                                                                ConfigurationRuleRegistry configurationRuleRegistry,
                                                                ActionGraphBuilder graphBuilder,
                                                                TargetNode<T> targetNode,
                                                                CellPathResolver cellPathResolver)
            ```

            ::: block
            [Description copied from
            interface: `TargetNodeToBuildRuleTransformer`]{.descfrmTypeLabel}
            :::

            ::: block
            Transform target node to build rule.
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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
