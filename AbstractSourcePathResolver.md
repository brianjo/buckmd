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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.sourcepath.resolver.impl](package-summary.html)
:::

## Class AbstractSourcePathResolver {#class-abstractsourcepathresolver .title title="Class AbstractSourcePathResolver"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.sourcepath.resolver.impl.AbstractSourcePathResolver

::: description
-   

    All Implemented Interfaces:
    :   `SourcePathResolver`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `DefaultSourcePathResolver`, `IjProjectSourcePathResolver`

    ------------------------------------------------------------------------

        public abstract class AbstractSourcePathResolver
        extends Object
        implements SourcePathResolver

    ::: block
    Abstract implementation of SourcePathResolver.
    Most of the SourcePathResolverAdapter interface can be implemented
    in terms of just a few functions ( the main requirement is resolving
    BuildTargetSourcePaths).

    Existing code may expect to resolve each
    [`SourcePath`](../../SourcePath.html "interface in com.facebook.buck.core.sourcepath")
    to only one
    [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}.
    In such cases,
    [`SourcePathResolverAdapter`](../SourcePathResolverAdapter.html "class in com.facebook.buck.core.sourcepath.resolver")
    is used to convert the resolver to return only one
    [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
    per
    [`SourcePath`](../../SourcePath.html "interface in com.facebook.buck.core.sourcepath").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                      Description
          -------------------------------- -------------
          `AbstractSourcePathResolver()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
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
        | `com.google           | `filterI              | ::: block             |
        | .common.collect.Immut | nputsToCompareToOutpu | Takes an              |
        | ableCollection<Path>` | t​(Iterable<? extends  | [`Iterable`](http:    |
        |                       | SourcePath> sources)` | //docs.oracle.com/jav |
        |                       |                       | ase/7/docs/api/java/l |
        |                       |                       | ang/Iterable.html?is- |
        |                       |                       | external=true "class  |
        |                       |                       | or interface in java. |
        |                       |                       | lang"){.externalLink} |
        |                       |                       | of                    |
        |                       |                       | [`                    |
        |                       |                       | SourcePath`](../../So |
        |                       |                       | urcePath.html "interf |
        |                       |                       | ace in com.facebook.b |
        |                       |                       | uck.core.sourcepath") |
        |                       |                       | objects and filters   |
        |                       |                       | those that represent  |
        |                       |                       | [`Path`](http://docs  |
        |                       |                       | .oracle.com/javase/7/ |
        |                       |                       | docs/api/java/nio/fil |
        |                       |                       | e/Path.html?is-extern |
        |                       |                       | al=true "class or int |
        |                       |                       | erface in java.nio.fi |
        |                       |                       | le"){.externalLink}s. |
        |                       |                       | :::                   |
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
        | `protected abstra     | `getBui               |                       |
        | ct ProjectFilesystem` | ldTargetSourcePathFil |                       |
        |                       | esystem​(BuildTargetSo |                       |
        |                       | urcePath sourcePath)` |                       |
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
        | `abstract String`     | `getSourcePathNa      |                       |
        |                       | me​(BuildTarget target |                       |
        |                       | ,                  So |                       |
        |                       | urcePath sourcePath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `g                    | ::: block             |
        | n.collect.ImmutableMa | etSourcePathNames​(Bui | Resolved the logical  |
        | p<String,​SourcePath>` | ldTarget target,      | names for a group of  |
        |                       |               String  | SourcePath objects    |
        |                       | parameter,            | into a map, throwing  |
        |                       |         Iterable<Sour | an error on           |
        |                       | cePath> sourcePaths)` | duplicates.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `<T> com.goo          | `getSou               | ::: block             |
        | gle.common.collect.Im | rcePathNames​(BuildTar | Resolves the logical  |
        | mutableMap<String,​T>` | get target,           | names for a group of  |
        |                       |          String param | objects that have a   |
        |                       | eter,                 | SourcePath into a     |
        |                       |    Iterable<T> object | map, throwing an      |
        |                       | s,                    | error on duplicates.  |
        |                       | java.util.function.Pr | :::                   |
        |                       | edicate<T> filter,    |                       |
        |                       |                 java. |                       |
        |                       | util.function.Functio |                       |
        |                       | n<T,​SourcePath> objec |                       |
        |                       | tSourcePathFunction)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected abs        | `resolveDefaultBuildT |                       |
        | tract com.google.comm | argetSourcePath​(Defau |                       |
        | on.collect.ImmutableS | ltBuildTargetSourcePa |                       |
        | ortedSet<SourcePath>` | th targetSourcePath)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

        -   #### AbstractSourcePathResolver

                public AbstractSourcePathResolver()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#resolveDefaultBuildTargetSourcePath(com.facebook.buck.core.sourcepath.DefaultBuildTargetSourcePath)}

        -   #### resolveDefaultBuildTargetSourcePath

            ``` methodSignature
            protected abstract com.google.common.collect.ImmutableSortedSet<SourcePath> resolveDefaultBuildTargetSourcePath​(DefaultBuildTargetSourcePath targetSourcePath)
            ```

        []{#getSourcePathName(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### getSourcePathName

            ``` methodSignature
            public abstract String getSourcePathName​(BuildTarget target,
                                                     SourcePath sourcePath)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathName` in interface `SourcePathResolver`

        []{#getBuildTargetSourcePathFilesystem(com.facebook.buck.core.sourcepath.BuildTargetSourcePath)}

        -   #### getBuildTargetSourcePathFilesystem

            ``` methodSignature
            protected abstract ProjectFilesystem getBuildTargetSourcePathFilesystem​(BuildTargetSourcePath sourcePath)
            ```

        []{#getMappedPaths(java.util.Map)}

        -   #### getMappedPaths

            ``` methodSignature
            public <T> com.google.common.collect.ImmutableMap<T,​com.google.common.collect.ImmutableSortedSet<Path>> getMappedPaths​(Map<T,​SourcePath> sourcePathMap)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getMappedPaths` in interface `SourcePathResolver`

        []{#getFilesystem(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### getFilesystem

            ``` methodSignature
            public ProjectFilesystem getFilesystem​(SourcePath sourcePath)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFilesystem` in interface `SourcePathResolver`

            [Returns:]{.returnLabel}
            :   the
                [`ProjectFilesystem`](../../../../io/filesystem/ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem")
                associated with `sourcePath`.

        []{#getAbsolutePath(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### getAbsolutePath

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<Path> getAbsolutePath​(SourcePath sourcePath)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAbsolutePath` in interface `SourcePathResolver`

            [Returns:]{.returnLabel}
            :   the
                [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
                instances for this `sourcePath`, resolved using its
                associated
                [`ProjectFilesystem`](../../../../io/filesystem/ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem").

        []{#getAllAbsolutePaths(java.util.Collection)}

        -   #### getAllAbsolutePaths

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<Path> getAllAbsolutePaths​(Collection<? extends SourcePath> sourcePaths)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAllAbsolutePaths` in interface `SourcePathResolver`

        []{#getRelativePath(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### getRelativePath

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<Path> getRelativePath​(SourcePath sourcePath)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRelativePath` in interface `SourcePathResolver`

            [Returns:]{.returnLabel}
            :   The
                [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
                instances the `sourcePath` refers to, relative to its
                owning
                [`ProjectFilesystem`](../../../../io/filesystem/ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem").

        []{#getIdeallyRelativePath(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### getIdeallyRelativePath

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<Path> getIdeallyRelativePath​(SourcePath sourcePath)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getIdeallyRelativePath` in
                interface `SourcePathResolver`

            [Returns:]{.returnLabel}

            :   The
                [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
                instances the `sourcePath` refers to, ideally relative
                to its owning
                [`ProjectFilesystem`](../../../../io/filesystem/ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem").
                Absolute path may get returned however!

                We should make sure that
                [`getPathPrivateImpl(com.facebook.buck.core.sourcepath.SourcePath)`](#getPathPrivateImpl(com.facebook.buck.core.sourcepath.SourcePath))
                always returns a relative path after which we should
                simply call
                [`getRelativePath(com.facebook.buck.core.sourcepath.SourcePath)`](#getRelativePath(com.facebook.buck.core.sourcepath.SourcePath)).
                Until then we still need this nonsense.

        []{#getSourcePathNames(com.facebook.buck.core.model.BuildTarget,java.lang.String,java.lang.Iterable)}

        -   #### getSourcePathNames

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​SourcePath> getSourcePathNames​(BuildTarget target,
                                                                                                      String parameter,
                                                                                                      Iterable<SourcePath> sourcePaths)
            ```

            ::: block
            Resolved the logical names for a group of SourcePath objects
            into a map, throwing an error on duplicates.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathNames` in interface `SourcePathResolver`

        []{#getSourcePathNames(com.facebook.buck.core.model.BuildTarget,java.lang.String,java.lang.Iterable,java.util.function.Predicate,java.util.function.Function)}

        -   #### getSourcePathNames

            ``` methodSignature
            public <T> com.google.common.collect.ImmutableMap<String,​T> getSourcePathNames​(BuildTarget target,
                                                                                                 String parameter,
                                                                                                 Iterable<T> objects,
                                                                                                 java.util.function.Predicate<T> filter,
                                                                                                 java.util.function.Function<T,​SourcePath> objectSourcePathFunction)
            ```

            ::: block
            Resolves the logical names for a group of objects that have
            a SourcePath into a map, throwing an error on duplicates.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathNames` in interface `SourcePathResolver`

        []{#filterInputsToCompareToOutput(java.lang.Iterable)}

        -   #### filterInputsToCompareToOutput

            ``` methodSignature
            public com.google.common.collect.ImmutableCollection<Path> filterInputsToCompareToOutput​(Iterable<? extends SourcePath> sources)
            ```

            ::: block
            Takes an
            [`Iterable`](http://docs.oracle.com/javase/7/docs/api/java/lang/Iterable.html?is-external=true "class or interface in java.lang"){.externalLink}
            of
            [`SourcePath`](../../SourcePath.html "interface in com.facebook.buck.core.sourcepath")
            objects and filters those that represent
            [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}s.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `filterInputsToCompareToOutput` in
                interface `SourcePathResolver`

        []{#getRelativePath(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### getRelativePath

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<Path> getRelativePath​(ProjectFilesystem projectFilesystem,
                                                                                      SourcePath sourcePath)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRelativePath` in interface `SourcePathResolver`

            [Returns:]{.returnLabel}
            :   [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
                instances to the given
                [`SourcePath`](../../SourcePath.html "interface in com.facebook.buck.core.sourcepath")
                that is relative to the given
                [`ProjectFilesystem`](../../../../io/filesystem/ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem")

        []{#createRelativeMap(java.nio.file.Path,java.lang.Iterable)}

        -   #### createRelativeMap

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<Path,​Path> createRelativeMap​(Path basePath,
                                                                                             Iterable<SourcePath> sourcePaths)
            ```

            ::: block
            [Description copied from
            interface: `SourcePathResolver`]{.descfrmTypeLabel}
            :::

            ::: block
            Creates a map where given source paths are resolved
            relatively to the given base path and stored (as keys) with
            their absolute paths (as values).
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `createRelativeMap` in interface `SourcePathResolver`
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
