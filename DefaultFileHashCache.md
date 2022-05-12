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
[Package]{.packageLabelInType} [com.facebook.buck.util.cache.impl](package-summary.html)
:::

## Class DefaultFileHashCache {#class-defaultfilehashcache .title title="Class DefaultFileHashCache"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.cache.impl.DefaultFileHashCache

::: description
-   

    All Implemented Interfaces:
    :   `ProjectFileHashCache`, `ProjectFileHashLoader`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `WatchedFileHashCache`

    ------------------------------------------------------------------------

        public class DefaultFileHashCache
        extends Object
        implements ProjectFileHashCache
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                                                                                                                                                     Description
          -------------- ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `protected `   `DefaultFileHashCache​(ProjectFilesystem projectFilesystem,                     java.util.function.Predicate<Path> ignoredPredicate,                     FileHashCacheMode fileHashCacheMode)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static               | `c                    |                       |
        | DefaultFileHashCache` | reateBuckOutFileHashC |                       |
        |                       | ache​(ProjectFilesyste |                       |
        |                       | m projectFilesystem,  |                       |
        |                       |                       |                       |
        |                       |      FileHashCacheMod |                       |
        |                       | e fileHashCacheMode)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `c                    |                       |
        | DefaultFileHashCache` | reateDefaultFileHashC |                       |
        |                       | ache​(ProjectFilesyste |                       |
        |                       | m projectFilesystem,  |                       |
        |                       |                       |                       |
        |                       |      FileHashCacheMod |                       |
        |                       | e fileHashCacheMode)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com.googl     | `                     |                       |
        | e.common.collect.Immu | createOsRootDirectori |                       |
        | tableList<? extends P | esCaches​(ProjectFiles |                       |
        | rojectFileHashCache>` | ystemFactory projectF |                       |
        |                       | ilesystemFactory,     |                       |
        |                       |                       |                       |
        |                       |      FileHashCacheMod |                       |
        |                       | e fileHashCacheMode)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `java.util.           | `debugDump()`         |                       |
        | stream.Stream<Map.Ent |                       |                       |
        | ry<Path,​com.google.co |                       |                       |
        | mmon.hash.HashCode>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `ge                   |                       |
        | common.hash.HashCode` | t​(Path relativePath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected            | `getDefaultPathPredi  | ::: block             |
        | static java.util.func | cate​(ProjectFilesyste | This predicate        |
        | tion.Predicate<Path>` | m projectFilesystem)` | matches files that    |
        |                       |                       | might be result of    |
        |                       |                       | builds or files that  |
        |                       |                       | are explicitly        |
        |                       |                       | ignored.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ProjectFilesystem`   | `getFilesystem()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getForArchiveMember  |                       |
        | common.hash.HashCode` | ​(Path relativeArchive |                       |
        |                       | Path,                 |                       |
        |                       |     Path memberPath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getIfPresen          |                       |
        | Optional<com.google.c | t​(Path relativePath)` |                       |
        | ommon.hash.HashCode>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `getSiz               |                       |
        |                       | e​(Path relativePath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Lis                  | `getStatsEvents()`    |                       |
        | t<AbstractBuckEvent>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `invalidat            |                       |
        |                       | e​(Path relativePath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `invalidateAll()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `                     |                       |
        |                       | isIgnored​(Path path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `set​(P                |                       |
        |                       | ath relativePath,     |                       |
        |                       | com.google.common.has |                       |
        |                       | h.HashCode hashCode)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `File                 | `verify()`            |                       |
        | HashCache.FileHashCac |                       |                       |
        | heVerificationResult` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `wil                  |                       |
        |                       | lGet​(ArchiveMemberPat |                       |
        |                       | h archiveMemberPath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `willGe               |                       |
        |                       | t​(Path relativePath)` |                       |
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

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,java.util.function.Predicate,com.facebook.buck.util.cache.FileHashCacheMode)}

        -   #### DefaultFileHashCache

                protected DefaultFileHashCache​(ProjectFilesystem projectFilesystem,
                                               java.util.function.Predicate<Path> ignoredPredicate,
                                               FileHashCacheMode fileHashCacheMode)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createBuckOutFileHashCache(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.util.cache.FileHashCacheMode)}

        -   #### createBuckOutFileHashCache

            ``` methodSignature
            public static DefaultFileHashCache createBuckOutFileHashCache​(ProjectFilesystem projectFilesystem,
                                                                          FileHashCacheMode fileHashCacheMode)
            ```

        []{#createDefaultFileHashCache(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.util.cache.FileHashCacheMode)}

        -   #### createDefaultFileHashCache

            ``` methodSignature
            public static DefaultFileHashCache createDefaultFileHashCache​(ProjectFilesystem projectFilesystem,
                                                                          FileHashCacheMode fileHashCacheMode)
            ```

        []{#getDefaultPathPredicate(com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### getDefaultPathPredicate

            ``` methodSignature
            protected static java.util.function.Predicate<Path> getDefaultPathPredicate​(ProjectFilesystem projectFilesystem)
            ```

            ::: block
            This predicate matches files that might be result of builds
            or files that are explicitly ignored.
            :::

        []{#createOsRootDirectoriesCaches(com.facebook.buck.io.filesystem.ProjectFilesystemFactory,com.facebook.buck.util.cache.FileHashCacheMode)}

        -   #### createOsRootDirectoriesCaches

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<? extends ProjectFileHashCache> createOsRootDirectoriesCaches​(ProjectFilesystemFactory projectFilesystemFactory,
                                                                                                                                FileHashCacheMode fileHashCacheMode)
            ```

        []{#willGet(java.nio.file.Path)}

        -   #### willGet

            ``` methodSignature
            public boolean willGet​(Path relativePath)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `willGet` in interface `ProjectFileHashCache`

        []{#isIgnored(java.nio.file.Path)}

        -   #### isIgnored

            ``` methodSignature
            public boolean isIgnored​(Path path)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isIgnored` in interface `ProjectFileHashCache`

        []{#willGet(com.facebook.buck.core.io.ArchiveMemberPath)}

        -   #### willGet

            ``` methodSignature
            public boolean willGet​(ArchiveMemberPath archiveMemberPath)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `willGet` in interface `ProjectFileHashCache`

        []{#invalidate(java.nio.file.Path)}

        -   #### invalidate

            ``` methodSignature
            public void invalidate​(Path relativePath)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `invalidate` in interface `ProjectFileHashCache`

        []{#invalidateAll()}

        -   #### invalidateAll

            ``` methodSignature
            public void invalidateAll()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `invalidateAll` in interface `ProjectFileHashCache`

        []{#get(java.nio.file.Path)}

        -   #### get

            ``` methodSignature
            public com.google.common.hash.HashCode get​(Path relativePath)
                                                throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `get` in interface `ProjectFileHashLoader`

            [Returns:]{.returnLabel}
            :   The `HashCode` of the contents of path.

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getSize(java.nio.file.Path)}

        -   #### getSize

            ``` methodSignature
            public long getSize​(Path relativePath)
                         throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSize` in interface `ProjectFileHashLoader`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getIfPresent(java.nio.file.Path)}

        -   #### getIfPresent

            ``` methodSignature
            public Optional<com.google.common.hash.HashCode> getIfPresent​(Path relativePath)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getIfPresent` in interface `ProjectFileHashLoader`

        []{#getForArchiveMember(java.nio.file.Path,java.nio.file.Path)}

        -   #### getForArchiveMember

            ``` methodSignature
            public com.google.common.hash.HashCode getForArchiveMember​(Path relativeArchivePath,
                                                                       Path memberPath)
                                                                throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getForArchiveMember` in
                interface `ProjectFileHashLoader`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getFilesystem()}

        -   #### getFilesystem

            ``` methodSignature
            public ProjectFilesystem getFilesystem()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFilesystem` in interface `ProjectFileHashCache`

        []{#set(java.nio.file.Path,com.google.common.hash.HashCode)}

        -   #### set

            ``` methodSignature
            public void set​(Path relativePath,
                            com.google.common.hash.HashCode hashCode)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `set` in interface `ProjectFileHashCache`

        []{#verify()}

        -   #### verify

            ``` methodSignature
            public FileHashCache.FileHashCacheVerificationResult verify()
                                                                 throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `verify` in interface `ProjectFileHashCache`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#debugDump()}

        -   #### debugDump

            ``` methodSignature
            public java.util.stream.Stream<Map.Entry<Path,​com.google.common.hash.HashCode>> debugDump()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `debugDump` in interface `ProjectFileHashCache`

        []{#getStatsEvents()}

        -   #### getStatsEvents

            ``` methodSignature
            public List<AbstractBuckEvent> getStatsEvents()
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
