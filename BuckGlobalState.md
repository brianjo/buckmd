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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.support.state](package-summary.html)
:::

## Class BuckGlobalState {#class-buckglobalstate .title title="Class BuckGlobalState"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.support.state.BuckGlobalState

::: description
-   

    All Implemented Interfaces:
    :   `Closeable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public final class BuckGlobalState
        extends Object
        implements Closeable

    ::: block
    [`BuckGlobalState`](BuckGlobalState.html "class in com.facebook.buck.support.state")
    contains all the global state of Buck which is kept between
    invocations of Buck commands, like caches, global per-process
    objects, etc. Individual caches here can be hooked to
    [`Watchman`](../../io/watchman/Watchman.html "class in com.facebook.buck.io.watchman")
    for proper invalidation.
    This state is uniformly invalidated on major changes, like
    configuration changes, so it is essential all in-proc caches to
    contain in this class for proper invalidation. If caches need to be
    kept between configuration changes, a custom logic should reside in
    [`BuckGlobalStateLifecycleManager`](BuckGlobalStateLifecycleManager.html "class in com.facebook.buck.support.state")

    All Graph Engine caches are required to be kept here.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `close()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ActionGraphCache`    | `g                    |                       |
        |                       | etActionGraphCache()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `getBuild             | ::: block             |
        | .google.common.cache. | FileManifestCaches()` | Return a map of all   |
        | LoadingCache<Path,​Bui |                       | build file manifest   |
        | ldFileManifestCache>` |                       | caches for each cell  |
        |                       |                       | which is a key        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `DaemonicParserState` | `getD                 |                       |
        |                       | aemonicParserState()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `RuleKeyCa            | `getDefaultRuleKeyFa  |                       |
        | cheRecycler<RuleKey>` | ctoryCacheRecycler()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.ca | `getD                 | ::: block             |
        | che.LoadingCache<Path | irectoryListCaches()` | Return a map of all   |
        | ,​DirectoryListCache>` |                       | directory list caches |
        |                       |                       | for each cell which   |
        |                       |                       | is a key.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.comm      | `getFileEventBus()`   | ::: block             |
        | on.eventbus.EventBus` |                       | Global event bus used |
        |                       |                       | to process file       |
        |                       |                       | invalidation events.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.co | `getFileHashCaches()` |                       |
        | llect.ImmutableList<P |                       |                       |
        | rojectFileHashCache>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.comm      | `getFileTreeCaches()` | ::: block             |
        | on.cache.LoadingCache |                       | Return a map of file  |
        | <Path,​FileTreeCache>` |                       | tree caches for each  |
        |                       |                       | cell which is a key.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Kn                   | `getKnow              |                       |
        | ownRuleTypesProvider` | nRuleTypesProvider()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ConcurrentMap<Strin  | `getPer               |                       |
        | g,​WorkerProcessPool>` | sistentWorkerPools()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `TypeCoercerFactory`  | `get                  |                       |
        |                       | TypeCoercerFactory()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `getUptime()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getUsesWatchman()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Versi                | `getVersion           |                       |
        | onedTargetGraphCache` | edTargetGraphCache()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getWatchmanCursor()` |                       |
        | com.google.common.col |                       |                       |
        | lect.ImmutableMap<Abs |                       |                       |
        | Path,​WatchmanCursor>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<WebServer>` | `getWebServer()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `interr               |                       |
        |                       | uptOnClientExit​(Threa |                       |
        |                       | d threadToInterrupt)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `watchFileSystem​(Buck |                       |
        |                       | EventBus eventBus,    |                       |
        |                       |              Watchman |                       |
        |                       | Watcher watchmanWatch |                       |
        |                       | er,                Wa |                       |
        |                       | tchmanWatcher.FreshIn |                       |
        |                       | stanceAction watchman |                       |
        |                       | FreshInstanceAction)` |                       |
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
    -   []{#method.detail}

        ### Method Detail

        []{#getWebServer()}

        -   #### getWebServer

            ``` methodSignature
            public Optional<WebServer> getWebServer()
            ```

        []{#getTypeCoercerFactory()}

        -   #### getTypeCoercerFactory

            ``` methodSignature
            public TypeCoercerFactory getTypeCoercerFactory()
            ```

        []{#getVersionedTargetGraphCache()}

        -   #### getVersionedTargetGraphCache

            ``` methodSignature
            public VersionedTargetGraphCache getVersionedTargetGraphCache()
            ```

        []{#getActionGraphCache()}

        -   #### getActionGraphCache

            ``` methodSignature
            public ActionGraphCache getActionGraphCache()
            ```

        []{#getFileHashCaches()}

        -   #### getFileHashCaches

            ``` methodSignature
            public com.google.common.collect.ImmutableList<ProjectFileHashCache> getFileHashCaches()
            ```

        []{#getDirectoryListCaches()}

        -   #### getDirectoryListCaches

            ``` methodSignature
            public com.google.common.cache.LoadingCache<Path,​DirectoryListCache> getDirectoryListCaches()
            ```

            ::: block
            Return a map of all directory list caches for each cell
            which is a key. For every cell, we cache directory structure
            (i.e. list of files and folders) for all subfolders that
            exist under that cell root folder
            :::

        []{#getBuildFileManifestCaches()}

        -   #### getBuildFileManifestCaches

            ``` methodSignature
            public com.google.common.cache.LoadingCache<Path,​BuildFileManifestCache> getBuildFileManifestCaches()
            ```

            ::: block
            Return a map of all build file manifest caches for each cell
            which is a key
            :::

        []{#getFileTreeCaches()}

        -   #### getFileTreeCaches

            ``` methodSignature
            public com.google.common.cache.LoadingCache<Path,​FileTreeCache> getFileTreeCaches()
            ```

            ::: block
            Return a map of file tree caches for each cell which is a
            key. For every cell and each subfolder under cell root path,
            we cache the whole subtree of folders and files recursively
            :::

        []{#getKnownRuleTypesProvider()}

        -   #### getKnownRuleTypesProvider

            ``` methodSignature
            public KnownRuleTypesProvider getKnownRuleTypesProvider()
            ```

        []{#getPersistentWorkerPools()}

        -   #### getPersistentWorkerPools

            ``` methodSignature
            public ConcurrentMap<String,​WorkerProcessPool> getPersistentWorkerPools()
            ```

        []{#getDefaultRuleKeyFactoryCacheRecycler()}

        -   #### getDefaultRuleKeyFactoryCacheRecycler

            ``` methodSignature
            public RuleKeyCacheRecycler<RuleKey> getDefaultRuleKeyFactoryCacheRecycler()
            ```

        []{#getDaemonicParserState()}

        -   #### getDaemonicParserState

            ``` methodSignature
            public DaemonicParserState getDaemonicParserState()
            ```

        []{#interruptOnClientExit(java.lang.Thread)}

        -   #### interruptOnClientExit

            ``` methodSignature
            public void interruptOnClientExit​(Thread threadToInterrupt)
            ```

        []{#watchFileSystem(com.facebook.buck.event.BuckEventBus,com.facebook.buck.io.watchman.WatchmanWatcher,com.facebook.buck.io.watchman.WatchmanWatcher.FreshInstanceAction)}

        -   #### watchFileSystem

            ``` methodSignature
            public void watchFileSystem​(BuckEventBus eventBus,
                                        WatchmanWatcher watchmanWatcher,
                                        WatchmanWatcher.FreshInstanceAction watchmanFreshInstanceAction)
                                 throws IOException,
                                        InterruptedException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `InterruptedException`

        []{#getFileEventBus()}

        -   #### getFileEventBus

            ``` methodSignature
            public com.google.common.eventbus.EventBus getFileEventBus()
            ```

            ::: block
            Global event bus used to process file invalidation events.
            This event bus is synchronous.
            :::

        []{#getWatchmanCursor()}

        -   #### getWatchmanCursor

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<AbsPath,​WatchmanCursor> getWatchmanCursor()
            ```

        []{#getUsesWatchman()}

        -   #### getUsesWatchman

            ``` methodSignature
            public boolean getUsesWatchman()
            ```

            [Returns:]{.returnLabel}
            :   true if state was created with Watchman service
                initialized

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `Closeable`

        []{#getUptime()}

        -   #### getUptime

            ``` methodSignature
            public long getUptime()
            ```

            [Returns:]{.returnLabel}
            :   the length of time in millis since this daemon was
                started
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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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
