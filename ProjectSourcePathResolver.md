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

## Class ProjectSourcePathResolver {#class-projectsourcepathresolver .title title="Class ProjectSourcePathResolver"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.apple.projectV2.ProjectSourcePathResolver

::: description
-   

    ------------------------------------------------------------------------

        public class ProjectSourcePathResolver
        extends Object

    ::: block
    Helper class to resolve
    [`SourcePath`](../../../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")s
    to the cell in which we generate the Xcode project.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                   Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `ProjectSourcePathResolver​(Cell projectCell,                          SourcePathResolverAdapter pathSourcePathResolverAdapter,                          TargetGraph targetGraph,                          java.util.function.Function<? super TargetNode<?>,​ActionGraphBuilder> actionGraphBuilderForNode)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Path`                | `resolveSourcePath​(So | ::: block             |
        |                       | urcePath sourcePath)` | Resolve a relative    |
        |                       |                       | path to the project   |
        |                       |                       | cell\'s filesystem.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

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

        []{#<init>(com.facebook.buck.core.cell.Cell,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.facebook.buck.core.model.targetgraph.TargetGraph,java.util.function.Function)}

        -   #### ProjectSourcePathResolver

                public ProjectSourcePathResolver​(Cell projectCell,
                                                 SourcePathResolverAdapter pathSourcePathResolverAdapter,
                                                 TargetGraph targetGraph,
                                                 java.util.function.Function<? super TargetNode<?>,​ActionGraphBuilder> actionGraphBuilderForNode)

            [Parameters:]{.paramLabel}
            :   `projectCell` - Cell to which the project target
                belongs.
            :   `pathSourcePathResolverAdapter` - Source path resolver
                to use for
                [`PathSourcePath`](../../../core/sourcepath/PathSourcePath.html "class in com.facebook.buck.core.sourcepath")s.
            :   `targetGraph` - Target graph for the project target.
            :   `actionGraphBuilderForNode` - Action graph builder for
                the project target.
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#resolveSourcePath(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### resolveSourcePath

            ``` methodSignature
            public Path resolveSourcePath​(SourcePath sourcePath)
            ```

            ::: block
            Resolve a relative path to the project cell\'s filesystem.
            [`PathSourcePath`](../../../core/sourcepath/PathSourcePath.html "class in com.facebook.buck.core.sourcepath")s
            utilize the
            [`pathSourcePathResolverAdapter`](#pathSourcePathResolverAdapter)
            to resolve the path. Otherwise the `sourcePath` is expected
            to be a
            [`BuildTargetSourcePath`](../../../core/sourcepath/BuildTargetSourcePath.html "interface in com.facebook.buck.core.sourcepath")
            for which we derive the target and resolve it\'s output to
            the cell.
            :::

            [Parameters:]{.paramLabel}
            :   `sourcePath` - Source path to resolve.

            [Returns:]{.returnLabel}
            :   A path relative to the cell.
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
