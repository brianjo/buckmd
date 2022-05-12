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
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.util.cache.impl](package-summary.html)
:::

## Class StackedFileHashCache {#class-stackedfilehashcache .title title="Class StackedFileHashCache"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.cache.impl.StackedFileHashCache

::: description
-   

    All Implemented Interfaces:
    :   `FileHashCache`, `FileHashLoader`

    ------------------------------------------------------------------------

        public class StackedFileHashCache
        extends Object
        implements FileHashCache

    ::: block
    Wraps a collection of
    [`ProjectFilesystem`](../../../io/filesystem/ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem")-specific
    [`ProjectFileHashCache`](../ProjectFileHashCache.html "interface in com.facebook.buck.util.cache")s
    as a single cache, implementing a Chain of Responsibility to find
    and forward operations to the correct inner cache. As this
    \"multi\"-cache is meant to handle paths across different
    [`ProjectFilesystem`](../../../io/filesystem/ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem")s,
    as opposed to paths within the same
    [`ProjectFilesystem`](../../../io/filesystem/ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem"),
    it is a distinct type from
    [`ProjectFileHashCache`](../ProjectFileHashCache.html "interface in com.facebook.buck.util.cache").
    This \"stacking\" approach provides a few appealing properties:

    1.  It makes it easier to module path roots with differing hash
        cached lifetime requirements. Hashes of paths from roots watched
        by watchman can be cached indefinitely, until a watchman event
        triggers invalidation. Hashes of paths under roots not watched
        by watchman, however, can only be cached for the duration of a
        single build (as we have no way to know when these paths are
        modified). By using separate
        [`ProjectFileHashCache`](../ProjectFileHashCache.html "interface in com.facebook.buck.util.cache")s
        per path root, we can construct a new
        [`StackedFileHashCache`](StackedFileHashCache.html "class in com.facebook.buck.util.cache.impl")
        on each build composed of either persistent or ephemeral
        per-root inner caches that properly manager the lifetime of
        cached hashes from their root.
    2.  Modeling the hash cache around path root and sub-paths also
        works well with a current limitation with our watchman events in
        which they only store relative paths, with no reference to the
        path root they originated from. If we stored hashes internally
        indexed by absolute path, then we wouldn\'t know where to anchor
        the search to resolve the path that a watchman event refers to
        (e.g. a watch event for \`foo.h\` could refer to \`/a/b/foo.h\`
        or \`/a/b/c/foo.h\`, depending on where the project root is). By
        indexing hashes by pairs of project root and sub-path, it\'s
        easier to identity paths to invalidate (e.g. \`foo.h\` would
        invalidate (\`/a/b/\`,\`foo.h\`) and not
        (\`/a/b/\`,\`c/foo.h\`)).
    3.  Since the current implementation of inner caches and callers
        generally use path root and sub-path pairs, it allows avoiding
        any overhead converting to/from absolute paths.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.util.cache.FileHashCache}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.util.cache.[FileHashCache](../FileHashCache.html "interface in com.facebook.buck.util.cache")

            `FileHashCache.FileHashCacheVerificationResult`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                              Description
          -------------------------------------------------------------------------------------------------------- -------------
          `StackedFileHashCache​(com.google.common.collect.ImmutableList<? extends ProjectFileHashCache> caches)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static               | `createDef            |                       |
        | StackedFileHashCache` | aultHashCaches​(Projec |                       |
        |                       | tFilesystem filesyste |                       |
        |                       | m,                    |                       |
        |                       |      FileHashCacheMod |                       |
        |                       | e fileHashCacheMode)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `java.util.           | `debugDump()`         |                       |
        | stream.Stream<Map.Ent |                       |                       |
        | ry<Path,​com.google.co |                       |                       |
        | mmon.hash.HashCode>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `get​(Pr               | ::: block             |
        | common.hash.HashCode` | ojectFilesystem files | Return the `HashCode` |
        |                       | ystem,    Path path)` | for the given         |
        |                       |                       | relative              |
        |                       |                       | [`Path`](http://do    |
        |                       |                       | cs.oracle.com/javase/ |
        |                       |                       | 7/docs/api/java/nio/f |
        |                       |                       | ile/Path.html?is-exte |
        |                       |                       | rnal=true "class or i |
        |                       |                       | nterface in java.nio. |
        |                       |                       | file"){.externalLink} |
        |                       |                       | under the given       |
        |                       |                       | [`ProjectFi           |
        |                       |                       | lesystem`](../../../i |
        |                       |                       | o/filesystem/ProjectF |
        |                       |                       | ilesystem.html "inter |
        |                       |                       | face in com.facebook. |
        |                       |                       | buck.io.filesystem"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `get​(Path path)`      |                       |
        | common.hash.HashCode` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getCaches()`         |                       |
        | e.common.collect.Immu |                       |                       |
        | tableList<? extends P |                       |                       |
        | rojectFileHashCache>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getFo                | ::: block             |
        | common.hash.HashCode` | rArchiveMember​(Projec | Return the `HashCode` |
        |                       | tFilesystem filesyste | for the given         |
        |                       | m,                    | relative              |
        |                       |  Path relativeArchive | [`ArchiveMember       |
        |                       | Path,                 | Path`](../../../core/ |
        |                       |     Path memberPath)` | io/ArchiveMemberPath. |
        |                       |                       | html "class in com.fa |
        |                       |                       | cebook.buck.core.io") |
        |                       |                       | under the given       |
        |                       |                       | [`ProjectFi           |
        |                       |                       | lesystem`](../../../i |
        |                       |                       | o/filesystem/ProjectF |
        |                       |                       | ilesystem.html "inter |
        |                       |                       | face in com.facebook. |
        |                       |                       | buck.io.filesystem"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getForArchiveMember  |                       |
        | common.hash.HashCode` | ​(Path relativeArchive |                       |
        |                       | Path,                 |                       |
        |                       |     Path memberPath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `getSize​(Projec       | ::: block             |
        |                       | tFilesystem filesyste | Return the size of    |
        |                       | m,        Path path)` | the given relative    |
        |                       |                       | [`Path`](http://do    |
        |                       |                       | cs.oracle.com/javase/ |
        |                       |                       | 7/docs/api/java/nio/f |
        |                       |                       | ile/Path.html?is-exte |
        |                       |                       | rnal=true "class or i |
        |                       |                       | nterface in java.nio. |
        |                       |                       | file"){.externalLink} |
        |                       |                       | under the given       |
        |                       |                       | [`ProjectFi           |
        |                       |                       | lesystem`](../../../i |
        |                       |                       | o/filesystem/ProjectF |
        |                       |                       | ilesystem.html "inter |
        |                       |                       | face in com.facebook. |
        |                       |                       | buck.io.filesystem"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `getSize​(Path path)`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `i                    |                       |
        |                       | nvalidate​(Path path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `invalidateAll()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `newDecorat           |                       |
        | StackedFileHashCache` | edFileHashCache​(java. |                       |
        |                       | util.function.Functio |                       |
        |                       | n<ProjectFileHashCach |                       |
        |                       | e,​ProjectFileHashCach |                       |
        |                       | e> decorateDelegate)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `set​(Proje            | ::: block             |
        |                       | ctFilesystem filesyst | Set the `HashCode`    |
        |                       | em,    Path path,     | for the given         |
        |                       | com.google.common.has | relative              |
        |                       | h.HashCode hashCode)` | [`Path`](http://do    |
        |                       |                       | cs.oracle.com/javase/ |
        |                       |                       | 7/docs/api/java/nio/f |
        |                       |                       | ile/Path.html?is-exte |
        |                       |                       | rnal=true "class or i |
        |                       |                       | nterface in java.nio. |
        |                       |                       | file"){.externalLink} |
        |                       |                       | under the given       |
        |                       |                       | [`ProjectFi           |
        |                       |                       | lesystem`](../../../i |
        |                       |                       | o/filesystem/ProjectF |
        |                       |                       | ilesystem.html "inter |
        |                       |                       | face in com.facebook. |
        |                       |                       | buck.io.filesystem"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `set​(Path path,       |                       |
        |                       | com.google.common.has |                       |
        |                       | h.HashCode hashCode)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `File                 | `verify()`            |                       |
        | HashCache.FileHashCac |                       |                       |
        | heVerificationResult` |                       |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
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

        []{#<init>(com.google.common.collect.ImmutableList)}

        -   #### StackedFileHashCache

                public StackedFileHashCache​(com.google.common.collect.ImmutableList<? extends ProjectFileHashCache> caches)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createDefaultHashCaches(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.util.cache.FileHashCacheMode)}

        -   #### createDefaultHashCaches

            ``` methodSignature
            public static StackedFileHashCache createDefaultHashCaches​(ProjectFilesystem filesystem,
                                                                       FileHashCacheMode fileHashCacheMode)
            ```

        []{#invalidate(java.nio.file.Path)}

        -   #### invalidate

            ``` methodSignature
            public void invalidate​(Path path)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `invalidate` in interface `FileHashCache`

        []{#invalidateAll()}

        -   #### invalidateAll

            ``` methodSignature
            public void invalidateAll()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `invalidateAll` in interface `FileHashCache`

        []{#get(java.nio.file.Path)}

        -   #### get

            ``` methodSignature
            public com.google.common.hash.HashCode get​(Path path)
                                                throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `get` in interface `FileHashLoader`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getSize(java.nio.file.Path)}

        -   #### getSize

            ``` methodSignature
            public long getSize​(Path path)
                         throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSize` in interface `FileHashLoader`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getForArchiveMember(java.nio.file.Path,java.nio.file.Path)}

        -   #### getForArchiveMember

            ``` methodSignature
            public com.google.common.hash.HashCode getForArchiveMember​(Path relativeArchivePath,
                                                                       Path memberPath)
                                                                throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getForArchiveMember` in interface `FileHashLoader`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#set(java.nio.file.Path,com.google.common.hash.HashCode)}

        -   #### set

            ``` methodSignature
            public void set​(Path path,
                            com.google.common.hash.HashCode hashCode)
                     throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `set` in interface `FileHashCache`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#verify()}

        -   #### verify

            ``` methodSignature
            public FileHashCache.FileHashCacheVerificationResult verify()
                                                                 throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `verify` in interface `FileHashCache`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#debugDump()}

        -   #### debugDump

            ``` methodSignature
            public java.util.stream.Stream<Map.Entry<Path,​com.google.common.hash.HashCode>> debugDump()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `debugDump` in interface `FileHashCache`

        []{#get(com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path)}

        -   #### get

            ``` methodSignature
            public com.google.common.hash.HashCode get​(ProjectFilesystem filesystem,
                                                       Path path)
                                                throws IOException
            ```

            ::: block
            [Description copied from
            interface: `FileHashLoader`]{.descfrmTypeLabel}
            :::

            ::: block
            Return the `HashCode` for the given relative
            [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
            under the given
            [`ProjectFilesystem`](../../../io/filesystem/ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem").
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `get` in interface `FileHashLoader`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getForArchiveMember(com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path,java.nio.file.Path)}

        -   #### getForArchiveMember

            ``` methodSignature
            public com.google.common.hash.HashCode getForArchiveMember​(ProjectFilesystem filesystem,
                                                                       Path relativeArchivePath,
                                                                       Path memberPath)
                                                                throws IOException
            ```

            ::: block
            [Description copied from
            interface: `FileHashLoader`]{.descfrmTypeLabel}
            :::

            ::: block
            Return the `HashCode` for the given relative
            [`ArchiveMemberPath`](../../../core/io/ArchiveMemberPath.html "class in com.facebook.buck.core.io")
            under the given
            [`ProjectFilesystem`](../../../io/filesystem/ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem").
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getForArchiveMember` in interface `FileHashLoader`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getSize(com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path)}

        -   #### getSize

            ``` methodSignature
            public long getSize​(ProjectFilesystem filesystem,
                                Path path)
                         throws IOException
            ```

            ::: block
            [Description copied from
            interface: `FileHashLoader`]{.descfrmTypeLabel}
            :::

            ::: block
            Return the size of the given relative
            [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
            under the given
            [`ProjectFilesystem`](../../../io/filesystem/ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem").
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSize` in interface `FileHashLoader`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#set(com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path,com.google.common.hash.HashCode)}

        -   #### set

            ``` methodSignature
            public void set​(ProjectFilesystem filesystem,
                            Path path,
                            com.google.common.hash.HashCode hashCode)
                     throws IOException
            ```

            ::: block
            [Description copied from
            interface: `FileHashCache`]{.descfrmTypeLabel}
            :::

            ::: block
            Set the `HashCode` for the given relative
            [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
            under the given
            [`ProjectFilesystem`](../../../io/filesystem/ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem").
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `set` in interface `FileHashCache`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#newDecoratedFileHashCache(java.util.function.Function)}

        -   #### newDecoratedFileHashCache

            ``` methodSignature
            public StackedFileHashCache newDecoratedFileHashCache​(java.util.function.Function<ProjectFileHashCache,​ProjectFileHashCache> decorateDelegate)
            ```

        []{#getCaches()}

        -   #### getCaches

            ``` methodSignature
            public com.google.common.collect.ImmutableList<? extends ProjectFileHashCache> getCaches()
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
-   [Nested](#nested.class.summary) \| 
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
