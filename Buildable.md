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

## Interface Buildable {#interface-buildable .title title="Interface Buildable"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AddsToRuleKey`

    ```{=html}
    <!-- -->
    ```

    All Known Subinterfaces:
    :   `PipelinedBuildable<State>`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `CalculateSourceAbi.SourceAbiBuildable`, `CxxLink.Impl`,
        `CxxThinLTOIndex.Impl`, `CxxThinLTOOpt.Impl`, `Filegroup`,
        `GenruleBuildable`, `MergeThirdPartyJarResources`,
        `SplitUberRDotJavaJar`, `WriteFileHashCode`, `Zip`

    ------------------------------------------------------------------------

        public interface Buildable
        extends AddsToRuleKey

    ::: block
    A Buildable is the core of a ModernBuildRule. A ModernBuildRule\'s
    deps, rulekey, inputs, outputs, etc are all derived (via reflection)
    from the fields of a Buildable.
    Buildables must be a top-level class or static inner class.
    Buildable fields must be final. Fields are limited to primitive
    types, Strings, Input/OutputPath, Input/OutputData and
    ImmutableList, Optional, ImmutableSortedSet, ImmutableSortedMap, and
    Pair composed of those.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                 Method                                                                                                                                                                                                      Description
          ------------------------------------------------- ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `com.google.common.collect.ImmutableList<Step>`   `getBuildSteps​(BuildContext buildContext,              ProjectFilesystem filesystem,              OutputPathResolver outputPathResolver,              BuildCellRelativePathFactory buildCellPathFactory)`    

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

        []{#getBuildSteps(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.rules.modern.OutputPathResolver,com.facebook.buck.rules.modern.BuildCellRelativePathFactory)}

        -   #### getBuildSteps

            ``` methodSignature
            com.google.common.collect.ImmutableList<Step> getBuildSteps​(BuildContext buildContext,
                                                                        ProjectFilesystem filesystem,
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
