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

## Class WatchedFileHashCache {#class-watchedfilehashcache .title title="Class WatchedFileHashCache"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.util.cache.impl.DefaultFileHashCache](DefaultFileHashCache.html "class in com.facebook.buck.util.cache.impl")

    -   -   com.facebook.buck.util.cache.impl.WatchedFileHashCache

::: description
-   

    All Implemented Interfaces:
    :   `ProjectFileHashCache`, `ProjectFileHashLoader`

    ------------------------------------------------------------------------

        public class WatchedFileHashCache
        extends DefaultFileHashCache
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                            Description
          ---------------------------------------------------------------------------------------------------------------------- -------------
          `WatchedFileHashCache​(ProjectFilesystem projectFilesystem,                     FileHashCacheMode fileHashCacheMode)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `onFile               |                       |
        |                       | SystemChange​(Watchman |                       |
        |                       | OverflowEvent event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `on                   | ::: block             |
        |                       | FileSystemChange​(Watc | Called when file      |
        |                       | hmanPathEvent event)` | change events are     |
        |                       |                       | posted to the file    |
        |                       |                       | change EventBus to    |
        |                       |                       | invalidate cached     |
        |                       |                       | build rules if        |
        |                       |                       | required.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.util.cache.impl.DefaultFileHashCache}

            ### Methods inherited from class com.facebook.buck.util.cache.impl.[DefaultFileHashCache](DefaultFileHashCache.html "class in com.facebook.buck.util.cache.impl")

            `createBuckOutFileHashCache, createDefaultFileHashCache, createOsRootDirectoriesCaches, debugDump, get, getDefaultPathPredicate, getFilesystem, getForArchiveMember, getIfPresent, getSize, getStatsEvents, invalidate, invalidateAll, isIgnored, set, verify, willGet, willGet`

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

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.util.cache.FileHashCacheMode)}

        -   #### WatchedFileHashCache

                public WatchedFileHashCache​(ProjectFilesystem projectFilesystem,
                                            FileHashCacheMode fileHashCacheMode)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#onFileSystemChange(com.facebook.buck.io.watchman.WatchmanPathEvent)}

        -   #### onFileSystemChange

            ``` methodSignature
            public void onFileSystemChange​(WatchmanPathEvent event)
            ```

            ::: block
            Called when file change events are posted to the file change
            EventBus to invalidate cached build rules if required.
            [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}s
            contained within events must all be relative to the
            [`ProjectFilesystem`](../../../io/filesystem/ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem")
            root.
            :::

        []{#onFileSystemChange(com.facebook.buck.io.watchman.WatchmanOverflowEvent)}

        -   #### onFileSystemChange

            ``` methodSignature
            public void onFileSystemChange​(WatchmanOverflowEvent event)
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
