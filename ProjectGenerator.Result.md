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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   Method

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
[Package]{.packageLabelInType} [com.facebook.buck.features.apple.projectV2](package-summary.html)
:::

## Class ProjectGenerator.Result {#class-projectgenerator.result .title title="Class ProjectGenerator.Result"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.apple.projectV2.ProjectGenerator.Result

::: description
-   

    Enclosing class:
    :   [ProjectGenerator](ProjectGenerator.html "class in com.facebook.buck.features.apple.projectV2")

    ------------------------------------------------------------------------

        public static class ProjectGenerator.Result
        extends Object

    ::: block
    The output from generating an Xcode project.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                                  Field                                Description
          ------------------------------------------------------------------ ------------------------------------ -------------
          `com.google.common.collect.ImmutableMap<BuildTarget,​PBXTarget>`    `buildTargetsToGeneratedTargetMap`    
          `PBXProject`                                                       `generatedProject`                    
          `com.google.common.collect.ImmutableList<Path>`                    `headerSymlinkTrees`                  
          `com.google.common.collect.ImmutableSet<BuildTarget>`              `requiredBuildTargets`                
          `com.google.common.collect.ImmutableList<BuildTargetSourcePath>`   `sourcePathsToBuild`                  
          `com.google.common.collect.ImmutableSet<Path>`                     `xcconfigPaths`                       

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                      Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `Result​(PBXProject generatedProject,       com.google.common.collect.ImmutableMap<BuildTarget,​PBXTarget> buildTargetsToGeneratedTargetMap,       com.google.common.collect.ImmutableSet<BuildTarget> requiredBuildTargets,       com.google.common.collect.ImmutableSet<Path> xcconfigPaths,       com.google.common.collect.ImmutableList<Path> headerSymlinkTrees,       com.google.common.collect.ImmutableList<BuildTargetSourcePath> sourcePathsToBuild)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#generatedProject}

        -   #### generatedProject

                public final PBXProject generatedProject

        []{#buildTargetsToGeneratedTargetMap}

        -   #### buildTargetsToGeneratedTargetMap

                public final com.google.common.collect.ImmutableMap<BuildTarget,​PBXTarget> buildTargetsToGeneratedTargetMap

        []{#requiredBuildTargets}

        -   #### requiredBuildTargets

                public final com.google.common.collect.ImmutableSet<BuildTarget> requiredBuildTargets

        []{#xcconfigPaths}

        -   #### xcconfigPaths

                public final com.google.common.collect.ImmutableSet<Path> xcconfigPaths

        []{#headerSymlinkTrees}

        -   #### headerSymlinkTrees

                public final com.google.common.collect.ImmutableList<Path> headerSymlinkTrees

        []{#sourcePathsToBuild}

        -   #### sourcePathsToBuild

                public final com.google.common.collect.ImmutableList<BuildTargetSourcePath> sourcePathsToBuild
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.apple.xcode.xcodeproj.PBXProject,com.google.common.collect.ImmutableMap,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableList)}

        -   #### Result

                public Result​(PBXProject generatedProject,
                              com.google.common.collect.ImmutableMap<BuildTarget,​PBXTarget> buildTargetsToGeneratedTargetMap,
                              com.google.common.collect.ImmutableSet<BuildTarget> requiredBuildTargets,
                              com.google.common.collect.ImmutableSet<Path> xcconfigPaths,
                              com.google.common.collect.ImmutableList<Path> headerSymlinkTrees,
                              com.google.common.collect.ImmutableList<BuildTargetSourcePath> sourcePathsToBuild)
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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   Method

</div>

[]{#skip.navbar.bottom}
:::
