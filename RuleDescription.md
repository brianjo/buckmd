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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.description](package-summary.html)
:::

## Interface RuleDescription\<T extends [BuildRuleArg](arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")\> {#interface-ruledescriptiont-extends-buildrulearg .title title="Interface RuleDescription"}
:::

::: contentContainer
::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `T` - the type of args that the rule implementation uses

    ```{=html}
    <!-- -->
    ```

    All Superinterfaces:
    :   `BaseDescription<T>`, `Description<T>`

    ```{=html}
    <!-- -->
    ```

    All Known Subinterfaces:
    :   `RuleDescriptionWithInstanceName<T>`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `LegacyToolchainRuleDescription`,
        `PrebuiltDotnetLibraryRuleDescription`, `SkylarkDescription`

    ------------------------------------------------------------------------

        public interface RuleDescription<T extends BuildRuleArg>
        extends Description<T>

    ::: block
    The new modern
    [`Description`](Description.html "interface in com.facebook.buck.core.description")
    that we will use during the analysis of a rule.
    The
    [`RuleDescription`](RuleDescription.html "interface in com.facebook.buck.core.description")
    will offer
    [`ruleImpl(RuleAnalysisContext, BuildTarget,  BuildRuleArg)`](#ruleImpl(com.facebook.buck.core.rules.analysis.RuleAnalysisContext,com.facebook.buck.core.model.BuildTarget,T))
    method, which provides a set of restricted information via the
    [`RuleAnalysisContext`](../rules/analysis/RuleAnalysisContext.html "interface in com.facebook.buck.core.rules.analysis")
    to run the rule implementation.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `default boolean`     | `produce              | ::: block             |
        |                       | sCacheableSubgraph()` | Whether or not the    |
        |                       |                       | build rule subgraph   |
        |                       |                       | produced by this      |
        |                       |                       | `Description` is safe |
        |                       |                       | to cache in           |
        |                       |                       | [`                    |
        |                       |                       | IncrementalActionGrap |
        |                       |                       | hGenerator`](../model |
        |                       |                       | /actiongraph/computat |
        |                       |                       | ion/IncrementalAction |
        |                       |                       | GraphGenerator.html " |
        |                       |                       | class in com.facebook |
        |                       |                       | .buck.core.model.acti |
        |                       |                       | ongraph.computation") |
        |                       |                       | for incremental       |
        |                       |                       | action graph          |
        |                       |                       | generation.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `ruleImpl​(RuleAnalys  | ::: block             |
        | oviderInfoCollection` | isContext context,    | Runs the rule         |
        |                       |       BuildTarget tar | implementation during |
        |                       | get,         T args)` | the analysis phase.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.BaseDescription}

            ### Methods inherited from interface com.facebook.buck.core.description.[BaseDescription](BaseDescription.html "interface in com.facebook.buck.core.description")

            `getConfigurationDeps, getConstructorArgType`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#producesCacheableSubgraph()}

        -   #### producesCacheableSubgraph

            ``` methodSignature
            default boolean producesCacheableSubgraph()
            ```

            ::: block
            [Description copied from
            interface: `Description`]{.descfrmTypeLabel}
            :::

            ::: block
            Whether or not the build rule subgraph produced by this
            `Description` is safe to cache in
            [`IncrementalActionGraphGenerator`](../model/actiongraph/computation/IncrementalActionGraphGenerator.html "class in com.facebook.buck.core.model.actiongraph.computation")
            for incremental action graph generation.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `producesCacheableSubgraph` in
                interface `Description<T extends BuildRuleArg>`

        []{#ruleImpl(com.facebook.buck.core.rules.analysis.RuleAnalysisContext,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.description.arg.BuildRuleArg)}
        []{#ruleImpl(com.facebook.buck.core.rules.analysis.RuleAnalysisContext,com.facebook.buck.core.model.BuildTarget,T)}

        -   #### ruleImpl

            ``` methodSignature
            ProviderInfoCollection ruleImpl​(RuleAnalysisContext context,
                                            BuildTarget target,
                                            T args)
                                     throws ActionCreationException,
                                            RuleAnalysisException
            ```

            ::: block
            Runs the rule implementation during the analysis phase. The
            rule implementation should create the propagated `Provider`s
            and corresponding `InfoInterface`s, and register its
            corresponding actions.
            :::

            [Parameters:]{.paramLabel}
            :   `context` - a
                [`RuleAnalysisContext`](../rules/analysis/RuleAnalysisContext.html "interface in com.facebook.buck.core.rules.analysis")
                containing all the information usable by this rule for
                it\'s analysis and constructive of its corresponding
                `Provider` and
                [`BuildRule`](../rules/BuildRule.html "interface in com.facebook.buck.core.rules")
                graph.
            :   `target` - the
                [`BuildTarget`](../model/BuildTarget.html "class in com.facebook.buck.core.model")
                of this rule
            :   `args` - The args of type `T` that this rule uses to
                rule its analysis

            [Returns:]{.returnLabel}
            :   a
                [`ProviderInfoCollection`](../rules/providers/collect/ProviderInfoCollection.html "interface in com.facebook.buck.core.rules.providers.collect")
                that contains all the `Provider` and the corresponding
                `InfoInterface` to be propagated by this rule.

            [Throws:]{.throwsLabel}
            :   `ActionCreationException` - If an action cannot be
                created correctly
            :   `RuleAnalysisException` - If the rule implementation
                could not run as expected. e.g. if the implementation
                method of a User Defined Rule fails to eval
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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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
