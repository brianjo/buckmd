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
-   [Field](#field.detail) \| 
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

## Class LegacyRuleAnalysisDelegatingTargetNodeToBuildRuleTransformer {#class-legacyruleanalysisdelegatingtargetnodetobuildruletransformer .title title="Class LegacyRuleAnalysisDelegatingTargetNodeToBuildRuleTransformer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rules.transformer.impl.LegacyRuleAnalysisDelegatingTargetNodeToBuildRuleTransformer

::: description
-   

    All Implemented Interfaces:
    :   `TargetNodeToBuildRuleTransformer`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `LegacyRuleAnalysisProviderCompatibleTargetNodeToBuildRuleTransformer`

    ------------------------------------------------------------------------

        public class LegacyRuleAnalysisDelegatingTargetNodeToBuildRuleTransformer
        extends Object
        implements TargetNodeToBuildRuleTransformer

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
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                              Field                       Description
          ---------------------------------------------- --------------------------- -------------
          `protected TargetNodeToBuildRuleTransformer`   `delegate`                   
          `protected RuleAnalysisGraph`                  `ruleAnalysisComputation`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                        Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `LegacyRuleAnalysisDelegatingTargetNodeToBuildRuleTransformer​(RuleAnalysisGraph ruleAnalysisComputation,                                                             TargetNodeToBuildRuleTransformer delegate)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `<T extends Bu        | `trans                | ::: block             |
        | ildRuleArg>BuildRule` | form​(ToolchainProvide | Converts a given      |
        |                       | r toolchainProvider,  | [`TargetN             |
        |                       |          TargetGraph  | ode`](../../../model/ |
        |                       | targetGraph,          | targetgraph/TargetNod |
        |                       |  ConfigurationRuleReg | e.html "interface in  |
        |                       | istry configurationRu | com.facebook.buck.cor |
        |                       | leRegistry,           | e.model.targetgraph") |
        |                       | ActionGraphBuilder gr | to a                  |
        |                       | aphBuilder,           | [`BuildRule`](..      |
        |                       | TargetNode<T> targetN | /../BuildRule.html "i |
        |                       | ode,          Provide | nterface in com.faceb |
        |                       | rInfoCollection provi | ook.buck.core.rules") |
        |                       | derInfoCollection,    | as part of action     |
        |                       |        CellPathResolv | graph construction.   |
        |                       | er cellPathResolver)` | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.transformer.TargetNodeToBuildRuleTransformer}

            ### Methods inherited from interface com.facebook.buck.core.rules.transformer.[TargetNodeToBuildRuleTransformer](../TargetNodeToBuildRuleTransformer.html "interface in com.facebook.buck.core.rules.transformer")

            `transform`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#ruleAnalysisComputation}

        -   #### ruleAnalysisComputation

                protected final RuleAnalysisGraph ruleAnalysisComputation

        []{#delegate}

        -   #### delegate

                protected final TargetNodeToBuildRuleTransformer delegate
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.rules.analysis.computation.RuleAnalysisGraph,com.facebook.buck.core.rules.transformer.TargetNodeToBuildRuleTransformer)}

        -   #### LegacyRuleAnalysisDelegatingTargetNodeToBuildRuleTransformer

                public LegacyRuleAnalysisDelegatingTargetNodeToBuildRuleTransformer​(RuleAnalysisGraph ruleAnalysisComputation,
                                                                                    TargetNodeToBuildRuleTransformer delegate)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#transform(com.facebook.buck.core.toolchain.ToolchainProvider,com.facebook.buck.core.model.targetgraph.TargetGraph,com.facebook.buck.core.rules.config.registry.ConfigurationRuleRegistry,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.model.targetgraph.TargetNode,com.facebook.buck.core.rules.providers.collect.ProviderInfoCollection,com.facebook.buck.core.cell.CellPathResolver)}

        -   #### transform

            ``` methodSignature
            public <T extends BuildRuleArg> BuildRule transform​(ToolchainProvider toolchainProvider,
                                                                TargetGraph targetGraph,
                                                                ConfigurationRuleRegistry configurationRuleRegistry,
                                                                ActionGraphBuilder graphBuilder,
                                                                TargetNode<T> targetNode,
                                                                ProviderInfoCollection providerInfoCollection,
                                                                CellPathResolver cellPathResolver)
            ```

            ::: block
            [Description copied from
            interface: `TargetNodeToBuildRuleTransformer`]{.descfrmTypeLabel}
            :::

            ::: block
            Converts a given
            [`TargetNode`](../../../model/targetgraph/TargetNode.html "interface in com.facebook.buck.core.model.targetgraph")
            to a
            [`BuildRule`](../../BuildRule.html "interface in com.facebook.buck.core.rules")
            as part of action graph construction. The providers computed
            from
            [`LegacyProviderCompatibleDescription.createProviders(ProviderCreationContext,  BuildTarget, BuildRuleArg)`](../../LegacyProviderCompatibleDescription.html#createProviders(com.facebook.buck.core.rules.ProviderCreationContext,com.facebook.buck.core.model.BuildTarget,T))
            will be passed to this function to be used to construct the
            [`BuildRule`](../../BuildRule.html "interface in com.facebook.buck.core.rules")
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `transform` in
                interface `TargetNodeToBuildRuleTransformer`
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
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
