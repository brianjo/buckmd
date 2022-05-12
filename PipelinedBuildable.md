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
[Package]{.packageLabelInType} [com.facebook.buck.rules.modern](package-summary.html)
:::

## Interface PipelinedBuildable\<State extends [RulePipelineState](../../core/rules/pipeline/RulePipelineState.html "interface in com.facebook.buck.core.rules.pipeline")\> {#interface-pipelinedbuildablestate-extends-rulepipelinestate .title title="Interface PipelinedBuildable"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AddsToRuleKey`, `Buildable`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `CalculateSourceAbi.SourceAbiBuildable`

    ------------------------------------------------------------------------

        public interface PipelinedBuildable<State extends RulePipelineState>
        extends Buildable

    ::: block
    Interface for the buildable of a PipelinedModernBuildRule.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                 Method                                                                                                                                                                                                                                                                             Description
          ------------------------------------------------- ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `com.google.common.collect.ImmutableList<Step>`   `getPipelinedBuildSteps​(BuildContext buildContext,                       ProjectFilesystem filesystem,                       State state,                       OutputPathResolver outputPathResolver,                       BuildCellRelativePathFactory buildCellPathFactory)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.rules.modern.Buildable}

            ### Methods inherited from interface com.facebook.buck.rules.modern.[Buildable](Buildable.html "interface in com.facebook.buck.rules.modern")

            `getBuildSteps`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getPipelinedBuildSteps(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.pipeline.RulePipelineState,com.facebook.buck.rules.modern.OutputPathResolver,com.facebook.buck.rules.modern.BuildCellRelativePathFactory)}
        []{#getPipelinedBuildSteps(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.io.filesystem.ProjectFilesystem,State,com.facebook.buck.rules.modern.OutputPathResolver,com.facebook.buck.rules.modern.BuildCellRelativePathFactory)}

        -   #### getPipelinedBuildSteps

            ``` methodSignature
            com.google.common.collect.ImmutableList<Step> getPipelinedBuildSteps​(BuildContext buildContext,
                                                                                 ProjectFilesystem filesystem,
                                                                                 State state,
                                                                                 OutputPathResolver outputPathResolver,
                                                                                 BuildCellRelativePathFactory buildCellPathFactory)
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
