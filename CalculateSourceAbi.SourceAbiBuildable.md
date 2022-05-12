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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Class CalculateSourceAbi.SourceAbiBuildable {#class-calculatesourceabi.sourceabibuildable .title title="Class CalculateSourceAbi.SourceAbiBuildable"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.CalculateSourceAbi.SourceAbiBuildable

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`, `Buildable`,
        `PipelinedBuildable<JavacPipelineState>`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [CalculateSourceAbi](CalculateSourceAbi.html "class in com.facebook.buck.jvm.java")

    ------------------------------------------------------------------------

        public static class CalculateSourceAbi.SourceAbiBuildable
        extends Object
        implements PipelinedBuildable<JavacPipelineState>

    ::: block
    Buildable implementation.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                  Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `SourceAbiBuildable​(BuildTarget buildTarget,                   ProjectFilesystem filesystem,                   JarBuildStepsFactory jarBuildStepsFactory)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                 Method                                                                                                                                                                                                                                                                                          Description
          ------------------------------------------------- ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `com.google.common.collect.ImmutableList<Step>`   `getBuildSteps​(BuildContext buildContext,              ProjectFilesystem filesystem,              OutputPathResolver outputPathResolver,              BuildCellRelativePathFactory buildCellPathFactory)`                                                                                        
          `com.google.common.collect.ImmutableList<Step>`   `getPipelinedBuildSteps​(BuildContext buildContext,                       ProjectFilesystem filesystem,                       JavacPipelineState state,                       OutputPathResolver outputPathResolver,                       BuildCellRelativePathFactory buildCellPathFactory)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.jvm.java.JarBuildStepsFactory)}

        -   #### SourceAbiBuildable

                public SourceAbiBuildable​(BuildTarget buildTarget,
                                          ProjectFilesystem filesystem,
                                          JarBuildStepsFactory jarBuildStepsFactory)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildSteps(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.rules.modern.OutputPathResolver,com.facebook.buck.rules.modern.BuildCellRelativePathFactory)}

        -   #### getBuildSteps

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Step> getBuildSteps​(BuildContext buildContext,
                                                                               ProjectFilesystem filesystem,
                                                                               OutputPathResolver outputPathResolver,
                                                                               BuildCellRelativePathFactory buildCellPathFactory)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildSteps` in interface `Buildable`

        []{#getPipelinedBuildSteps(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.jvm.java.JavacPipelineState,com.facebook.buck.rules.modern.OutputPathResolver,com.facebook.buck.rules.modern.BuildCellRelativePathFactory)}

        -   #### getPipelinedBuildSteps

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Step> getPipelinedBuildSteps​(BuildContext buildContext,
                                                                                        ProjectFilesystem filesystem,
                                                                                        JavacPipelineState state,
                                                                                        OutputPathResolver outputPathResolver,
                                                                                        BuildCellRelativePathFactory buildCellPathFactory)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPipelinedBuildSteps` in
                interface `PipelinedBuildable<JavacPipelineState>`
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
