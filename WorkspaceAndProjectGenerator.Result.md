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

## Class WorkspaceAndProjectGenerator.Result {#class-workspaceandprojectgenerator.result .title title="Class WorkspaceAndProjectGenerator.Result"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.apple.projectV2.WorkspaceAndProjectGenerator.Result

::: description
-   

    Enclosing class:
    :   [WorkspaceAndProjectGenerator](WorkspaceAndProjectGenerator.html "class in com.facebook.buck.features.apple.projectV2")

    ------------------------------------------------------------------------

        public static class WorkspaceAndProjectGenerator.Result
        extends Object

    ::: block
    The result of generating a workspace project.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                                 Field                      Description
          ----------------------------------------------------------------- -------------------------- -------------
          `com.google.common.collect.ImmutableMap<BuildTarget,​PBXTarget>`   `buildTargetToPBXTarget`    
          `PBXProject`                                                      `project`                   
          `Path`                                                            `workspacePath`             

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                          Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `Result​(Path workspacePath,       PBXProject project,       com.google.common.collect.ImmutableMap<BuildTarget,​PBXTarget> buildTargetToPBXTarget)`    

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

        []{#workspacePath}

        -   #### workspacePath

                public final Path workspacePath

        []{#project}

        -   #### project

                public final PBXProject project

        []{#buildTargetToPBXTarget}

        -   #### buildTargetToPBXTarget

                public final com.google.common.collect.ImmutableMap<BuildTarget,​PBXTarget> buildTargetToPBXTarget
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.nio.file.Path,com.facebook.buck.apple.xcode.xcodeproj.PBXProject,com.google.common.collect.ImmutableMap)}

        -   #### Result

                public Result​(Path workspacePath,
                              PBXProject project,
                              com.google.common.collect.ImmutableMap<BuildTarget,​PBXTarget> buildTargetToPBXTarget)
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
