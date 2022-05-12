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
[Package]{.packageLabelInType} [com.facebook.buck.features.apple.projectV2](package-summary.html)
:::

## Class Utils {#class-utils .title title="Class Utils"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.apple.projectV2.Utils

::: description
-   

    ------------------------------------------------------------------------

        public class Utils
        extends Object

    ::: block
    Utility functions for project generation.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor   Description
          ------------- -------------
          `Utils()`      

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static void`         | `ad                   | ::: block             |
        |                       | dRequiredBuildTargetF | Adds the input source |
        |                       | romSourcePath​(BuildTa | path object to the    |
        |                       | rgetSourcePath buildT | required build        |
        |                       | argetSourcePath,      | targets builder, if   |
        |                       |                       | needed.               |
        |                       |            com.google | :::                   |
        |                       | .common.collect.Immut |                       |
        |                       | ableSet.Builder<Build |                       |
        |                       | Target> requiredBuild |                       |
        |                       | TargetsBuilder,       |                       |
        |                       |                       |                       |
        |                       |           TargetGraph |                       |
        |                       |  targetGraph,         |                       |
        |                       |                       |                       |
        |                       |         java.util.fun |                       |
        |                       | ction.Function<? supe |                       |
        |                       | r TargetNode<?>,​Actio |                       |
        |                       | nGraphBuilder> action |                       |
        |                       | GraphBuilderForNode)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `getModuleName​(Targe  | ::: block             |
        |                       | tNode<?> targetNode)` | Gets the Swift or Cxx |
        |                       |                       | module name if the    |
        |                       |                       | target node has the   |
        |                       |                       | module name defined.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Optional<Bu   | `sourcePathTryIntoBui |                       |
        | ildTargetSourcePath>` | ldTargetSourcePath​(So |                       |
        |                       | urcePath sourcePath)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
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

        []{#<init>()}

        -   #### Utils

                public Utils()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getModuleName(com.facebook.buck.core.model.targetgraph.TargetNode)}

        -   #### getModuleName

            ``` methodSignature
            public static String getModuleName​(TargetNode<?> targetNode)
            ```

            ::: block
            Gets the Swift or Cxx module name if the target node has the
            module name defined. Otherwise returns the target name.
            :::

        []{#sourcePathTryIntoBuildTargetSourcePath(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### sourcePathTryIntoBuildTargetSourcePath

            ``` methodSignature
            public static Optional<BuildTargetSourcePath> sourcePathTryIntoBuildTargetSourcePath​(SourcePath sourcePath)
            ```

        []{#addRequiredBuildTargetFromSourcePath(com.facebook.buck.core.sourcepath.BuildTargetSourcePath,com.google.common.collect.ImmutableSet.Builder,com.facebook.buck.core.model.targetgraph.TargetGraph,java.util.function.Function)}

        -   #### addRequiredBuildTargetFromSourcePath

            ``` methodSignature
            public static void addRequiredBuildTargetFromSourcePath​(BuildTargetSourcePath buildTargetSourcePath,
                                                                    com.google.common.collect.ImmutableSet.Builder<BuildTarget> requiredBuildTargetsBuilder,
                                                                    TargetGraph targetGraph,
                                                                    java.util.function.Function<? super TargetNode<?>,​ActionGraphBuilder> actionGraphBuilderForNode)
            ```

            ::: block
            Adds the input source path object to the required build
            targets builder, if needed.
            :::

            [Parameters:]{.paramLabel}
            :   `buildTargetSourcePath` - The build target source path
                to add.
            :   `requiredBuildTargetsBuilder` - The builder to add the
                target too, if necessary.
            :   `targetGraph` - The target graph that includes the
                target
            :   `actionGraphBuilderForNode` - The action graph builder
                for the target node.
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
