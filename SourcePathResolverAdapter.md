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
[Package]{.packageLabelInType} [com.facebook.buck.core.sourcepath.resolver](package-summary.html)
:::

## Class SourcePathResolverAdapter {#class-sourcepathresolveradapter .title title="Class SourcePathResolverAdapter"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter

::: description
-   

    ------------------------------------------------------------------------

        public class SourcePathResolverAdapter
        extends Object

    ::: block
    Adapter that makes
    [`SourcePathResolver`](SourcePathResolver.html "interface in com.facebook.buck.core.sourcepath.resolver")
    compatible with client code that assumes each
    [`SourcePath`](../SourcePath.html "interface in com.facebook.buck.core.sourcepath")
    resolves to only one
    [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}.
    See also
    [`AbstractSourcePathResolver`](impl/AbstractSourcePathResolver.html "class in com.facebook.buck.core.sourcepath.resolver.impl").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                Description
          ---------------------------------------------------------- -------------
          `SourcePathResolverAdapter​(SourcePathResolver resolver)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.goog             | `                     | ::: block             |
        | le.common.collect.Imm | createRelativeMap​(Pat | Returns a map where   |
        | utableMap<Path,​Path>` | h basePath,           | given                 |
        |                       |         Iterable<Sour | [`SourcePath`](../So  |
        |                       | cePath> sourcePaths)` | urcePath.html "interf |
        |                       |                       | ace in com.facebook.b |
        |                       |                       | uck.core.sourcepath") |
        |                       |                       | instances are         |
        |                       |                       | resolved relatively   |
        |                       |                       | to the given base     |
        |                       |                       | path and stored (as   |
        |                       |                       | keys) with their      |
        |                       |                       | absolute paths (as    |
        |                       |                       | values).              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `filterI              | ::: block             |
        | .common.collect.Immut | nputsToCompareToOutpu | Returns a collection  |
        | ableCollection<Path>` | t​(Iterable<? extends  | of                    |
        |                       | SourcePath> sources)` | [`Path`](http://do    |
        |                       |                       | cs.oracle.com/javase/ |
        |                       |                       | 7/docs/api/java/nio/f |
        |                       |                       | ile/Path.html?is-exte |
        |                       |                       | rnal=true "class or i |
        |                       |                       | nterface in java.nio. |
        |                       |                       | file"){.externalLink} |
        |                       |                       | instances by          |
        |                       |                       | filtering the given   |
        |                       |                       | [`SourcePath`](../So  |
        |                       |                       | urcePath.html "interf |
        |                       |                       | ace in com.facebook.b |
        |                       |                       | uck.core.sourcepath") |
        |                       |                       | instances for         |
        |                       |                       | [`Path`](http://do    |
        |                       |                       | cs.oracle.com/javase/ |
        |                       |                       | 7/docs/api/java/nio/f |
        |                       |                       | ile/Path.html?is-exte |
        |                       |                       | rnal=true "class or i |
        |                       |                       | nterface in java.nio. |
        |                       |                       | file"){.externalLink} |
        |                       |                       | instances.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getAbsolutePath​(So   | ::: block             |
        |                       | urcePath sourcePath)` | Returns the           |
        |                       |                       | [`Path`](http://do    |
        |                       |                       | cs.oracle.com/javase/ |
        |                       |                       | 7/docs/api/java/nio/f |
        |                       |                       | ile/Path.html?is-exte |
        |                       |                       | rnal=true "class or i |
        |                       |                       | nterface in java.nio. |
        |                       |                       | file"){.externalLink} |
        |                       |                       | associated with the   |
        |                       |                       | given                 |
        |                       |                       | [`SourcePath`](../Sou |
        |                       |                       | rcePath.html "interfa |
        |                       |                       | ce in com.facebook.bu |
        |                       |                       | ck.core.sourcepath"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `get                  | ::: block             |
        | e.common.collect.Immu | AllAbsolutePaths​(Coll | Returns the           |
        | tableSortedSet<Path>` | ection<? extends Sour | [`Path`](http://do    |
        |                       | cePath> sourcePaths)` | cs.oracle.com/javase/ |
        |                       |                       | 7/docs/api/java/nio/f |
        |                       |                       | ile/Path.html?is-exte |
        |                       |                       | rnal=true "class or i |
        |                       |                       | nterface in java.nio. |
        |                       |                       | file"){.externalLink} |
        |                       |                       | instances associated  |
        |                       |                       | with the given        |
        |                       |                       | [`SourcePath`](../So  |
        |                       |                       | urcePath.html "interf |
        |                       |                       | ace in com.facebook.b |
        |                       |                       | uck.core.sourcepath") |
        |                       |                       | instances.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ProjectFilesystem`   | `getFilesystem​(So     | ::: block             |
        |                       | urcePath sourcePath)` | Returns the           |
        |                       |                       | [`ProjectF            |
        |                       |                       | ilesystem`](../../../ |
        |                       |                       | io/filesystem/Project |
        |                       |                       | Filesystem.html "inte |
        |                       |                       | rface in com.facebook |
        |                       |                       | .buck.io.filesystem") |
        |                       |                       | associated with this  |
        |                       |                       | adapter.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getI                 | ::: block             |
        |                       | deallyRelativePath​(So | Returns the           |
        |                       | urcePath sourcePath)` | [`Path`](http://do    |
        |                       |                       | cs.oracle.com/javase/ |
        |                       |                       | 7/docs/api/java/nio/f |
        |                       |                       | ile/Path.html?is-exte |
        |                       |                       | rnal=true "class or i |
        |                       |                       | nterface in java.nio. |
        |                       |                       | file"){.externalLink} |
        |                       |                       | instances the given   |
        |                       |                       | [`SourcePath`](../So  |
        |                       |                       | urcePath.html "interf |
        |                       |                       | ace in com.facebook.b |
        |                       |                       | uck.core.sourcepath") |
        |                       |                       | refers to, ideally    |
        |                       |                       | relative to its       |
        |                       |                       | owning                |
        |                       |                       | [`ProjectFi           |
        |                       |                       | lesystem`](../../../i |
        |                       |                       | o/filesystem/ProjectF |
        |                       |                       | ilesystem.html "inter |
        |                       |                       | face in com.facebook. |
        |                       |                       | buck.io.filesystem"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `<T> com.g            | `getMap               | ::: block             |
        | oogle.common.collect. | pedPaths​(Map<T,​Source | Returns a list of     |
        | ImmutableMap<T,​Path>` | Path> sourcePathMap)` | values and their      |
        |                       |                       | associated            |
        |                       |                       | [`Path`](http://do    |
        |                       |                       | cs.oracle.com/javase/ |
        |                       |                       | 7/docs/api/java/nio/f |
        |                       |                       | ile/Path.html?is-exte |
        |                       |                       | rnal=true "class or i |
        |                       |                       | nterface in java.nio. |
        |                       |                       | file"){.externalLink} |
        |                       |                       | instances by          |
        |                       |                       | transforming the      |
        |                       |                       | given                 |
        |                       |                       | [`SourcePath`](../So  |
        |                       |                       | urcePath.html "interf |
        |                       |                       | ace in com.facebook.b |
        |                       |                       | uck.core.sourcepath") |
        |                       |                       | instances into        |
        |                       |                       | [`Path`](http://do    |
        |                       |                       | cs.oracle.com/javase/ |
        |                       |                       | 7/docs/api/java/nio/f |
        |                       |                       | ile/Path.html?is-exte |
        |                       |                       | rnal=true "class or i |
        |                       |                       | nterface in java.nio. |
        |                       |                       | file"){.externalLink} |
        |                       |                       | instances.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getRelativePath​(So   | ::: block             |
        |                       | urcePath sourcePath)` | Returns the           |
        |                       |                       | [`Path`](http://do    |
        |                       |                       | cs.oracle.com/javase/ |
        |                       |                       | 7/docs/api/java/nio/f |
        |                       |                       | ile/Path.html?is-exte |
        |                       |                       | rnal=true "class or i |
        |                       |                       | nterface in java.nio. |
        |                       |                       | file"){.externalLink} |
        |                       |                       | associated with the   |
        |                       |                       | given                 |
        |                       |                       | [`SourcePath`](../So  |
        |                       |                       | urcePath.html "interf |
        |                       |                       | ace in com.facebook.b |
        |                       |                       | uck.core.sourcepath") |
        |                       |                       | relative to its       |
        |                       |                       | owning                |
        |                       |                       | [`ProjectFi           |
        |                       |                       | lesystem`](../../../i |
        |                       |                       | o/filesystem/ProjectF |
        |                       |                       | ilesystem.html "inter |
        |                       |                       | face in com.facebook. |
        |                       |                       | buck.io.filesystem"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getRela              | ::: block             |
        |                       | tivePath​(ProjectFiles | Returns the           |
        |                       | ystem projectFilesyst | [`Path`](http://do    |
        |                       | em,                So | cs.oracle.com/javase/ |
        |                       | urcePath sourcePath)` | 7/docs/api/java/nio/f |
        |                       |                       | ile/Path.html?is-exte |
        |                       |                       | rnal=true "class or i |
        |                       |                       | nterface in java.nio. |
        |                       |                       | file"){.externalLink} |
        |                       |                       | associated with the   |
        |                       |                       | given                 |
        |                       |                       | [`SourcePath`](../So  |
        |                       |                       | urcePath.html "interf |
        |                       |                       | ace in com.facebook.b |
        |                       |                       | uck.core.sourcepath") |
        |                       |                       | relative to the given |
        |                       |                       | [`ProjectFi           |
        |                       |                       | lesystem`](../../../i |
        |                       |                       | o/filesystem/ProjectF |
        |                       |                       | ilesystem.html "inter |
        |                       |                       | face in com.facebook. |
        |                       |                       | buck.io.filesystem"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePathResolver`  | `getResolver()`       | ::: block             |
        |                       |                       | Returns the           |
        |                       |                       | [`SourcePathResolver` |
        |                       |                       | ](SourcePathResolver. |
        |                       |                       | html "interface in co |
        |                       |                       | m.facebook.buck.core. |
        |                       |                       | sourcepath.resolver") |
        |                       |                       | associated with this  |
        |                       |                       | adapter.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getSourcePathNa      | ::: block             |
        |                       | me​(BuildTarget target | Returns the logical   |
        |                       | ,                  So | name for a given      |
        |                       | urcePath sourcePath)` | [`SourcePath`](../Sou |
        |                       |                       | rcePath.html "interfa |
        |                       |                       | ce in com.facebook.bu |
        |                       |                       | ck.core.sourcepath"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `g                    | ::: block             |
        | n.collect.ImmutableMa | etSourcePathNames​(Bui | Resolves the logical  |
        | p<String,​SourcePath>` | ldTarget target,      | names for a group of  |
        |                       |               String  | [`SourcePath`](../So  |
        |                       | parameter,            | urcePath.html "interf |
        |                       |         Iterable<Sour | ace in com.facebook.b |
        |                       | cePath> sourcePaths)` | uck.core.sourcepath") |
        |                       |                       | objects into a map,   |
        |                       |                       | throwing an error on  |
        |                       |                       | duplicates.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `<T> com.goo          | `getSou               | ::: block             |
        | gle.common.collect.Im | rcePathNames​(BuildTar | Resolves the logical  |
        | mutableMap<String,​T>` | get target,           | names for a group of  |
        |                       |          String param | [`SourcePath`](../So  |
        |                       | eter,                 | urcePath.html "interf |
        |                       |    Iterable<T> object | ace in com.facebook.b |
        |                       | s,                    | uck.core.sourcepath") |
        |                       | java.util.function.Pr | objects into a map,   |
        |                       | edicate<T> filter,    | throwing an error on  |
        |                       |                 java. | duplicates.           |
        |                       | util.function.Functio | :::                   |
        |                       | n<T,​SourcePath> objec |                       |
        |                       | tSourcePathFunction)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.sourcepath.resolver.SourcePathResolver)}

        -   #### SourcePathResolverAdapter

                public SourcePathResolverAdapter​(SourcePathResolver resolver)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getAbsolutePath(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### getAbsolutePath

            ``` methodSignature
            public Path getAbsolutePath​(SourcePath sourcePath)
            ```

            ::: block
            Returns the
            [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
            associated with the given
            [`SourcePath`](../SourcePath.html "interface in com.facebook.buck.core.sourcepath").
            :::

        []{#getRelativePath(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### getRelativePath

            ``` methodSignature
            public Path getRelativePath​(SourcePath sourcePath)
            ```

            ::: block
            Returns the
            [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
            associated with the given
            [`SourcePath`](../SourcePath.html "interface in com.facebook.buck.core.sourcepath")
            relative to its owning
            [`ProjectFilesystem`](../../../io/filesystem/ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem").
            :::

        []{#getIdeallyRelativePath(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### getIdeallyRelativePath

            ``` methodSignature
            public Path getIdeallyRelativePath​(SourcePath sourcePath)
            ```

            ::: block
            Returns the
            [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
            instances the given
            [`SourcePath`](../SourcePath.html "interface in com.facebook.buck.core.sourcepath")
            refers to, ideally relative to its owning
            [`ProjectFilesystem`](../../../io/filesystem/ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem").
            Absolute path may get returned however!
            :::

        []{#getRelativePath(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### getRelativePath

            ``` methodSignature
            public Path getRelativePath​(ProjectFilesystem projectFilesystem,
                                        SourcePath sourcePath)
            ```

            ::: block
            Returns the
            [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
            associated with the given
            [`SourcePath`](../SourcePath.html "interface in com.facebook.buck.core.sourcepath")
            relative to the given
            [`ProjectFilesystem`](../../../io/filesystem/ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem").
            :::

        []{#getAllAbsolutePaths(java.util.Collection)}

        -   #### getAllAbsolutePaths

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<Path> getAllAbsolutePaths​(Collection<? extends SourcePath> sourcePaths)
            ```

            ::: block
            Returns the
            [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
            instances associated with the given
            [`SourcePath`](../SourcePath.html "interface in com.facebook.buck.core.sourcepath")
            instances.
            :::

        []{#getMappedPaths(java.util.Map)}

        -   #### getMappedPaths

            ``` methodSignature
            public <T> com.google.common.collect.ImmutableMap<T,​Path> getMappedPaths​(Map<T,​SourcePath> sourcePathMap)
            ```

            ::: block
            Returns a list of values and their associated
            [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
            instances by transforming the given
            [`SourcePath`](../SourcePath.html "interface in com.facebook.buck.core.sourcepath")
            instances into
            [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
            instances.
            :::

        []{#getSourcePathNames(com.facebook.buck.core.model.BuildTarget,java.lang.String,java.lang.Iterable)}

        -   #### getSourcePathNames

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​SourcePath> getSourcePathNames​(BuildTarget target,
                                                                                                      String parameter,
                                                                                                      Iterable<SourcePath> sourcePaths)
            ```

            ::: block
            Resolves the logical names for a group of
            [`SourcePath`](../SourcePath.html "interface in com.facebook.buck.core.sourcepath")
            objects into a map, throwing an error on duplicates.
            :::

        []{#filterInputsToCompareToOutput(java.lang.Iterable)}

        -   #### filterInputsToCompareToOutput

            ``` methodSignature
            public com.google.common.collect.ImmutableCollection<Path> filterInputsToCompareToOutput​(Iterable<? extends SourcePath> sources)
            ```

            ::: block
            Returns a collection of
            [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
            instances by filtering the given
            [`SourcePath`](../SourcePath.html "interface in com.facebook.buck.core.sourcepath")
            instances for
            [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
            instances.
            :::

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
            Resolves the logical names for a group of
            [`SourcePath`](../SourcePath.html "interface in com.facebook.buck.core.sourcepath")
            objects into a map, throwing an error on duplicates.
            :::

        []{#getSourcePathName(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### getSourcePathName

            ``` methodSignature
            public String getSourcePathName​(BuildTarget target,
                                            SourcePath sourcePath)
            ```

            ::: block
            Returns the logical name for a given
            [`SourcePath`](../SourcePath.html "interface in com.facebook.buck.core.sourcepath").
            :::

        []{#createRelativeMap(java.nio.file.Path,java.lang.Iterable)}

        -   #### createRelativeMap

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<Path,​Path> createRelativeMap​(Path basePath,
                                                                                             Iterable<SourcePath> sourcePaths)
            ```

            ::: block
            Returns a map where given
            [`SourcePath`](../SourcePath.html "interface in com.facebook.buck.core.sourcepath")
            instances are resolved relatively to the given base path and
            stored (as keys) with their absolute paths (as values).
            :::

        []{#getFilesystem(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### getFilesystem

            ``` methodSignature
            public ProjectFilesystem getFilesystem​(SourcePath sourcePath)
            ```

            ::: block
            Returns the
            [`ProjectFilesystem`](../../../io/filesystem/ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem")
            associated with this adapter.
            :::

        []{#getResolver()}

        -   #### getResolver

            ``` methodSignature
            public SourcePathResolver getResolver()
            ```

            ::: block
            Returns the
            [`SourcePathResolver`](SourcePathResolver.html "interface in com.facebook.buck.core.sourcepath.resolver")
            associated with this adapter.
            :::

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`
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
