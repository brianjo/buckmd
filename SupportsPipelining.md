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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.pipeline](package-summary.html)
:::

## Interface SupportsPipelining\<T extends [RulePipelineState](RulePipelineState.html "interface in com.facebook.buck.core.rules.pipeline")\> {#interface-supportspipeliningt-extends-rulepipelinestate .title title="Interface SupportsPipelining"}
:::

::: contentContainer
::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `T` - the type that is used to share build state between rules
        in the pipeline

    ```{=html}
    <!-- -->
    ```

    All Superinterfaces:
    :   `AllowsNonAnnotatedFields`, `BuildEngineAction`, `BuildRule`,
        `Comparable<BuildRule>`, `HasNameAndType`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AndroidLibrary`, `AndroidPrebuiltAar`, `CalculateSourceAbi`,
        `DefaultJavaLibrary`, `PipelinedModernBuildRule`

    ------------------------------------------------------------------------

        @Deprecated
        public interface SupportsPipelining<T extends RulePipelineState>
        extends BuildRule

    ::: deprecationBlock
    [Deprecated.]{.deprecatedLabel}

    ::: deprecationComment
    Rule pipelining couples rules in a way that makes it very easy to
    violate buck\'s assumptions and makes it nearly impossible for buck
    to understand and restrict what rules are doing.
    :::
    :::

    ::: block
    The steps required to build this rule locally can run more
    efficiently when executed immediately after those of a dependency.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.google.com       | `getPipe              | ::: block             |
        | mon.collect.Immutable | linedBuildSteps​(Build | [Deprecate            |
        | List<? extends Step>` | Context context,      | d.]{.deprecatedLabel} |
        |                       |                   Bui | :::                   |
        |                       | ldableContext buildab |                       |
        |                       | leContext,            |                       |
        |                       |             T state)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `RulePip              | `getPi                | ::: block             |
        | elineStateFactory<T>` | pelineStateFactory()` | [Deprecate            |
        |                       |                       | d.]{.deprecatedLabel} |
        |                       |                       | :::                   |
        |                       |                       |                       |
        |                       |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `S                    | `getPrev              | ::: block             |
        | upportsPipelining<T>` | iousRuleInPipeline()` | [Deprecate            |
        |                       |                       | d.]{.deprecatedLabel} |
        |                       |                       | :::                   |
        |                       |                       |                       |
        |                       |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `isSuppo              | ::: block             |
        |                       | rted​(BuildRule rule)` | [Deprecate            |
        |                       |                       | d.]{.deprecatedLabel} |
        |                       |                       | :::                   |
        |                       |                       |                       |
        |                       |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `useRulePipelining()` | ::: block             |
        |                       |                       | [Deprecate            |
        |                       |                       | d.]{.deprecatedLabel} |
        |                       |                       | :::                   |
        |                       |                       |                       |
        |                       |                       |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Deprecated
        Methods](javascript:show(32);)[ ]{.tabEnd}]{#t6 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.build.action.BuildEngineAction}

            ### Methods inherited from interface com.facebook.buck.core.build.action.[BuildEngineAction](../../build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")

            `getDependencies, getSourcePathOutputs`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.BuildRule}

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRule](../BuildRule.html "interface in com.facebook.buck.core.rules")

            `compareTo, getBuildDeps, getBuildSteps, getBuildTarget, getFullyQualifiedName, getProjectFilesystem, getSourcePathToOutput, hasBuildSteps, isCacheable, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.HasNameAndType}

            ### Methods inherited from interface com.facebook.buck.core.rules.[HasNameAndType](../HasNameAndType.html "interface in com.facebook.buck.core.rules")

            `getType`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#isSupported(com.facebook.buck.core.rules.BuildRule)}

        -   #### isSupported

            ``` methodSignature
            static boolean isSupported​(BuildRule rule)
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

        []{#useRulePipelining()}

        -   #### useRulePipelining

            ``` methodSignature
            boolean useRulePipelining()
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

        []{#getPreviousRuleInPipeline()}

        -   #### getPreviousRuleInPipeline

            ``` methodSignature
            @Nullable
            SupportsPipelining<T> getPreviousRuleInPipeline()
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

        []{#getPipelinedBuildSteps(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.build.buildable.context.BuildableContext,com.facebook.buck.core.rules.pipeline.RulePipelineState)}
        []{#getPipelinedBuildSteps(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.build.buildable.context.BuildableContext,T)}

        -   #### getPipelinedBuildSteps

            ``` methodSignature
            com.google.common.collect.ImmutableList<? extends Step> getPipelinedBuildSteps​(BuildContext context,
                                                                                           BuildableContext buildableContext,
                                                                                           T state)
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

        []{#getPipelineStateFactory()}

        -   #### getPipelineStateFactory

            ``` methodSignature
            RulePipelineStateFactory<T> getPipelineStateFactory()
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
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
