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
[Package]{.packageLabelInType} [com.facebook.buck.features.project.intellij](package-summary.html)
:::

## Class IjProjectSourcePathResolver {#class-ijprojectsourcepathresolver .title title="Class IjProjectSourcePathResolver"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.sourcepath.resolver.impl.AbstractSourcePathResolver](../../../core/sourcepath/resolver/impl/AbstractSourcePathResolver.html "class in com.facebook.buck.core.sourcepath.resolver.impl")

    -   -   com.facebook.buck.features.project.intellij.IjProjectSourcePathResolver

::: description
-   

    All Implemented Interfaces:
    :   `SourcePathResolver`

    ------------------------------------------------------------------------

        public class IjProjectSourcePathResolver
        extends AbstractSourcePathResolver

    ::: block
    A SourcePathResolver implementation that uses only information found
    in the target graph when converting a BuildTargetSourcePath to an
    outputPath. This allows the IjProject code to rely only on the
    TargetGraph when constructing a project.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                              Description
          -------------------------------------------------------- -------------
          `IjProjectSourcePathResolver​(TargetGraph targetGraph)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `O                    | `getBuildTarget​(So    |                       |
        | ptional<BuildTarget>` | urcePath sourcePath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protect              | `getBui               |                       |
        | ed ProjectFilesystem` | ldTargetSourcePathFil |                       |
        |                       | esystem​(BuildTargetSo |                       |
        |                       | urcePath sourcePath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `s                    | `getOutputPathF       |                       |
        | tatic Optional<Path>` | romJavaTargetNode​(Tar |                       |
        |                       | getNode<?> targetNode |                       |
        |                       | ,                     |                       |
        |                       |             BuildTarg |                       |
        |                       | et buildTarget,       |                       |
        |                       |                       |                       |
        |                       |      ProjectFilesyste |                       |
        |                       | m projectFilesystem)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getSourcePathNa      | ::: block             |
        |                       | me​(BuildTarget target | Source path names are |
        |                       | ,                  So | only used when        |
        |                       | urcePath sourcePath)` | constructing the      |
        |                       |                       | ActionGraph, so we    |
        |                       |                       | don\'t need to        |
        |                       |                       | support them here.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `isJvmLan             |                       |
        |                       | guageTargetNode​(Targe |                       |
        |                       | tNode<?> targetNode)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `isJv                 |                       |
        |                       | mTestTargetNode​(Targe |                       |
        |                       | tNode<?> targetNode)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `prot                 | `resolveDefaultBuildT | ::: block             |
        | ected com.google.comm | argetSourcePath​(Defau | Resolve the default   |
        | on.collect.ImmutableS | ltBuildTargetSourcePa | output path for the   |
        | ortedSet<SourcePath>` | th targetSourcePath)` | given                 |
        |                       |                       | targetSourcePath,     |
        |                       |                       | returning a           |
        |                       |                       | sourcepath pointing   |
        |                       |                       | to the output.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.sourcepath.resolver.impl.AbstractSourcePathResolver}

            ### Methods inherited from class com.facebook.buck.core.sourcepath.resolver.impl.[AbstractSourcePathResolver](../../../core/sourcepath/resolver/impl/AbstractSourcePathResolver.html "class in com.facebook.buck.core.sourcepath.resolver.impl")

            `createRelativeMap, filterInputsToCompareToOutput, getAbsolutePath, getAllAbsolutePaths, getFilesystem, getIdeallyRelativePath, getMappedPaths, getRelativePath, getRelativePath, getSourcePathNames, getSourcePathNames`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.targetgraph.TargetGraph)}

        -   #### IjProjectSourcePathResolver

                public IjProjectSourcePathResolver​(TargetGraph targetGraph)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#resolveDefaultBuildTargetSourcePath(com.facebook.buck.core.sourcepath.DefaultBuildTargetSourcePath)}

        -   #### resolveDefaultBuildTargetSourcePath

            ``` methodSignature
            protected com.google.common.collect.ImmutableSortedSet<SourcePath> resolveDefaultBuildTargetSourcePath​(DefaultBuildTargetSourcePath targetSourcePath)
            ```

            ::: block
            Resolve the default output path for the given
            targetSourcePath, returning a sourcepath pointing to the
            output.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolveDefaultBuildTargetSourcePath` in
                class `AbstractSourcePathResolver`

        []{#getSourcePathName(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### getSourcePathName

            ``` methodSignature
            public String getSourcePathName​(BuildTarget target,
                                            SourcePath sourcePath)
            ```

            ::: block
            Source path names are only used when constructing the
            ActionGraph, so we don\'t need to support them here.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathName` in interface `SourcePathResolver`

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathName` in
                class `AbstractSourcePathResolver`

        []{#getBuildTargetSourcePathFilesystem(com.facebook.buck.core.sourcepath.BuildTargetSourcePath)}

        -   #### getBuildTargetSourcePathFilesystem

            ``` methodSignature
            protected ProjectFilesystem getBuildTargetSourcePathFilesystem​(BuildTargetSourcePath sourcePath)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildTargetSourcePathFilesystem` in
                class `AbstractSourcePathResolver`

            [Returns:]{.returnLabel}
            :   the filesystem instance that corresponds to the given
                BuildTargetSourcePath

        []{#getBuildTarget(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### getBuildTarget

            ``` methodSignature
            public Optional<BuildTarget> getBuildTarget​(SourcePath sourcePath)
            ```

            [Returns:]{.returnLabel}
            :   The BuildTarget portion of the sourcePath if present

        []{#isJvmLanguageTargetNode(com.facebook.buck.core.model.targetgraph.TargetNode)}

        -   #### isJvmLanguageTargetNode

            ``` methodSignature
            public static boolean isJvmLanguageTargetNode​(TargetNode<?> targetNode)
            ```

            [Returns:]{.returnLabel}
            :   true if the given target node describes a rule targeting
                the JVM

        []{#isJvmTestTargetNode(com.facebook.buck.core.model.targetgraph.TargetNode)}

        -   #### isJvmTestTargetNode

            ``` methodSignature
            public static boolean isJvmTestTargetNode​(TargetNode<?> targetNode)
            ```

            [Returns:]{.returnLabel}
            :   true if the given target node describes a junit/ngtest
                rule targeting the JVM

        []{#getOutputPathFromJavaTargetNode(com.facebook.buck.core.model.targetgraph.TargetNode,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### getOutputPathFromJavaTargetNode

            ``` methodSignature
            public static Optional<Path> getOutputPathFromJavaTargetNode​(TargetNode<?> targetNode,
                                                                         BuildTarget buildTarget,
                                                                         ProjectFilesystem projectFilesystem)
            ```

            [Returns:]{.returnLabel}
            :   the output path for the given buildTarget assuming that
                the buildTarget points to something like a JavaLibrary
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
