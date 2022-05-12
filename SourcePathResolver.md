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
[Package]{.packageLabelInType} [com.facebook.buck.core.sourcepath.resolver](package-summary.html)
:::

## Interface SourcePathResolver {#interface-sourcepathresolver .title title="Interface SourcePathResolver"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `AbstractSourcePathResolver`, `DefaultSourcePathResolver`,
        `IjProjectSourcePathResolver`

    ------------------------------------------------------------------------

        public interface SourcePathResolver
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.goog             | `                     | ::: block             |
        | le.common.collect.Imm | createRelativeMap​(Pat | Creates a map where   |
        | utableMap<Path,​Path>` | h basePath,           | given source paths    |
        |                       |         Iterable<Sour | are resolved          |
        |                       | cePath> sourcePaths)` | relatively to the     |
        |                       |                       | given base path and   |
        |                       |                       | stored (as keys) with |
        |                       |                       | their absolute paths  |
        |                       |                       | (as values).          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `filterI              |                       |
        | .common.collect.Immut | nputsToCompareToOutpu |                       |
        | ableCollection<Path>` | t​(Iterable<? extends  |                       |
        |                       | SourcePath> sources)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getAbsolutePath​(So   |                       |
        | e.common.collect.Immu | urcePath sourcePath)` |                       |
        | tableSortedSet<Path>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `get                  |                       |
        | e.common.collect.Immu | AllAbsolutePaths​(Coll |                       |
        | tableSortedSet<Path>` | ection<? extends Sour |                       |
        |                       | cePath> sourcePaths)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ProjectFilesystem`   | `getFilesystem​(So     |                       |
        |                       | urcePath sourcePath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getI                 |                       |
        | e.common.collect.Immu | deallyRelativePath​(So |                       |
        | tableSortedSet<Path>` | urcePath sourcePath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `<T> com.googl        | `getMap               |                       |
        | e.common.collect.Immu | pedPaths​(Map<T,​Source |                       |
        | tableMap<T,​com.google | Path> sourcePathMap)` |                       |
        | .common.collect.Immut |                       |                       |
        | ableSortedSet<Path>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getRelativePath​(So   |                       |
        | e.common.collect.Immu | urcePath sourcePath)` |                       |
        | tableSortedSet<Path>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getRela              |                       |
        | e.common.collect.Immu | tivePath​(ProjectFiles |                       |
        | tableSortedSet<Path>` | ystem projectFilesyst |                       |
        |                       | em,                So |                       |
        |                       | urcePath sourcePath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getSourcePathNa      |                       |
        |                       | me​(BuildTarget target |                       |
        |                       | ,                  So |                       |
        |                       | urcePath sourcePath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `g                    |                       |
        | n.collect.ImmutableMa | etSourcePathNames​(Bui |                       |
        | p<String,​SourcePath>` | ldTarget target,      |                       |
        |                       |               String  |                       |
        |                       | parameter,            |                       |
        |                       |         Iterable<Sour |                       |
        |                       | cePath> sourcePaths)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `<T> com.goo          | `getSou               |                       |
        | gle.common.collect.Im | rcePathNames​(BuildTar |                       |
        | mutableMap<String,​T>` | get target,           |                       |
        |                       |          String param |                       |
        |                       | eter,                 |                       |
        |                       |    Iterable<T> object |                       |
        |                       | s,                    |                       |
        |                       | java.util.function.Pr |                       |
        |                       | edicate<T> filter,    |                       |
        |                       |                 java. |                       |
        |                       | util.function.Functio |                       |
        |                       | n<T,​SourcePath> objec |                       |
        |                       | tSourcePathFunction)` |                       |
        +-----------------------+-----------------------+-----------------------+

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

        []{#getMappedPaths(java.util.Map)}

        -   #### getMappedPaths

            ``` methodSignature
            <T> com.google.common.collect.ImmutableMap<T,​com.google.common.collect.ImmutableSortedSet<Path>> getMappedPaths​(Map<T,​SourcePath> sourcePathMap)
            ```

        []{#getFilesystem(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### getFilesystem

            ``` methodSignature
            ProjectFilesystem getFilesystem​(SourcePath sourcePath)
            ```

        []{#getAbsolutePath(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### getAbsolutePath

            ``` methodSignature
            com.google.common.collect.ImmutableSortedSet<Path> getAbsolutePath​(SourcePath sourcePath)
            ```

        []{#getAllAbsolutePaths(java.util.Collection)}

        -   #### getAllAbsolutePaths

            ``` methodSignature
            com.google.common.collect.ImmutableSortedSet<Path> getAllAbsolutePaths​(Collection<? extends SourcePath> sourcePaths)
            ```

        []{#getRelativePath(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### getRelativePath

            ``` methodSignature
            com.google.common.collect.ImmutableSortedSet<Path> getRelativePath​(SourcePath sourcePath)
            ```

        []{#getIdeallyRelativePath(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### getIdeallyRelativePath

            ``` methodSignature
            com.google.common.collect.ImmutableSortedSet<Path> getIdeallyRelativePath​(SourcePath sourcePath)
            ```

        []{#getSourcePathNames(com.facebook.buck.core.model.BuildTarget,java.lang.String,java.lang.Iterable)}

        -   #### getSourcePathNames

            ``` methodSignature
            com.google.common.collect.ImmutableMap<String,​SourcePath> getSourcePathNames​(BuildTarget target,
                                                                                               String parameter,
                                                                                               Iterable<SourcePath> sourcePaths)
            ```

        []{#getSourcePathNames(com.facebook.buck.core.model.BuildTarget,java.lang.String,java.lang.Iterable,java.util.function.Predicate,java.util.function.Function)}

        -   #### getSourcePathNames

            ``` methodSignature
            <T> com.google.common.collect.ImmutableMap<String,​T> getSourcePathNames​(BuildTarget target,
                                                                                          String parameter,
                                                                                          Iterable<T> objects,
                                                                                          java.util.function.Predicate<T> filter,
                                                                                          java.util.function.Function<T,​SourcePath> objectSourcePathFunction)
            ```

        []{#getSourcePathName(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### getSourcePathName

            ``` methodSignature
            String getSourcePathName​(BuildTarget target,
                                     SourcePath sourcePath)
            ```

        []{#filterInputsToCompareToOutput(java.lang.Iterable)}

        -   #### filterInputsToCompareToOutput

            ``` methodSignature
            com.google.common.collect.ImmutableCollection<Path> filterInputsToCompareToOutput​(Iterable<? extends SourcePath> sources)
            ```

        []{#getRelativePath(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### getRelativePath

            ``` methodSignature
            com.google.common.collect.ImmutableSortedSet<Path> getRelativePath​(ProjectFilesystem projectFilesystem,
                                                                               SourcePath sourcePath)
            ```

            [Returns:]{.returnLabel}
            :   [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
                instances to the given
                [`SourcePath`](../SourcePath.html "interface in com.facebook.buck.core.sourcepath")
                that is relative to the given
                [`ProjectFilesystem`](../../../io/filesystem/ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem")

        []{#createRelativeMap(java.nio.file.Path,java.lang.Iterable)}

        -   #### createRelativeMap

            ``` methodSignature
            com.google.common.collect.ImmutableMap<Path,​Path> createRelativeMap​(Path basePath,
                                                                                      Iterable<SourcePath> sourcePaths)
            ```

            ::: block
            Creates a map where given source paths are resolved
            relatively to the given base path and stored (as keys) with
            their absolute paths (as values).
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
