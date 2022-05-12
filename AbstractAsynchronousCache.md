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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.artifact_cache](package-summary.html)
:::

## Class AbstractAsynchronousCache {#class-abstractasynchronouscache .title title="Class AbstractAsynchronousCache"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.artifact_cache.AbstractAsynchronousCache

::: description
-   

    All Implemented Interfaces:
    :   `ArtifactCache`, `AutoCloseable`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `AbstractNetworkCache`

    ------------------------------------------------------------------------

        public abstract class AbstractAsynchronousCache
        extends Object
        implements ArtifactCache
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type           Class                                            Description
          --------------------------- ------------------------------------------------ -------------
          `static interface `         `AbstractAsynchronousCache.CacheEventListener`    
          `protected static class `   `AbstractAsynchronousCache.FetchRequest`          
          `static interface `         `AbstractAsynchronousCache.StoreEvents`           

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `AbstractAsynchronousCache​(String name,                          ArtifactCacheMode mode,                          CacheReadMode cacheReadMode,                          com.google.common.util.concurrent.ListeningExecutorService storeExecutorService,                          com.google.common.util.concurrent.ListeningExecutorService fetchExecutorService,                          AbstractAsynchronousCache.CacheEventListener eventListener,                          Optional<Long> maxStoreSize,                          ProjectFilesystem projectFilesystem)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.goo              | `deleteAsync​(Lis      |                       |
        | gle.common.util.concu | t<RuleKey> ruleKeys)` |                       |
        | rrent.ListenableFutur |                       |                       |
        | e<CacheDeleteResult>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected abstra     | `deleteImpl​(Lis       |                       |
        | ct CacheDeleteResult` | t<RuleKey> ruleKeys)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `c                    | `f                    | ::: block             |
        | om.google.common.util | etchAsync​(BuildTarget | Fetch a cached        |
        | .concurrent.Listenabl |  target,           Ru | artifact, keyed by    |
        | eFuture<CacheResult>` | leKey ruleKey,        | ruleKey, save the     |
        |                       |     LazyPath output)` | artifact to path      |
        |                       |                       | specified by output,  |
        |                       |                       | and return true on    |
        |                       |                       | success.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protec               | `fetchImpl​(BuildTarg  |                       |
        | ted abstract com.face | et target,          R |                       |
        | book.buck.artifact_ca | uleKey ruleKey,       |                       |
        | che.AbstractAsynchron |     LazyPath output)` |                       |
        | ousCache.FetchResult` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `CacheReadMode`       | `getCacheReadMode()`  | ::: block             |
        |                       |                       | This method must      |
        |                       |                       | return the same value |
        |                       |                       | over the lifetime of  |
        |                       |                       | this object.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protect              | `getMode()`           |                       |
        | ed ArtifactCacheMode` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected int`       | `getMul               | ::: block             |
        |                       | tiFetchBatchSize​(int  | Used to compute the   |
        |                       | pendingRequestsSize)` | number of keys to     |
        |                       |                       | include in every      |
        |                       |                       | multiFetchRequest.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected String`    | `getName()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protect              | `ge                   |                       |
        | ed ProjectFilesystem` | tProjectFilesystem()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected boolean`   | `i                    |                       |
        |                       | sMultiCheckEnabled()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.goo              | `multiContainsA       | ::: block             |
        | gle.common.util.concu | sync​(com.google.commo | Check if the cache    |
        | rrent.ListenableFutur | n.collect.ImmutableSe | contains the given    |
        | e<com.google.common.c | t<RuleKey> ruleKeys)` | artifacts, keyed by   |
        | ollect.ImmutableMap<R |                       | ruleKeys, without     |
        | uleKey,​CacheResult>>` |                       | fetching them, and    |
        |                       |                       | return a map of       |
        |                       |                       | results wrapped in a  |
        |                       |                       | `ListenableFuture`.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected abst       | `multiContains        |                       |
        | ract com.facebook.buc | Impl​(com.google.commo |                       |
        | k.artifact_cache.Abst | n.collect.ImmutableSe |                       |
        | ractAsynchronousCache | t<RuleKey> ruleKeys)` |                       |
        | .MultiContainsResult` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected a          | `multiFetchI          | ::: block             |
        | bstract com.facebook. | mpl​(Iterable<Abstract | The MultiFetchResult  |
        | buck.artifact_cache.A | AsynchronousCache.Fet | should contain        |
        | bstractAsynchronousCa | chRequest> requests)` | results in the same   |
        | che.MultiFetchResult` |                       | order as the          |
        |                       |                       | requests.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `skipPendingAnd       | ::: block             |
        |                       | FutureAsyncFetches()` | All pending (and      |
        |                       |                       | future) async fetches |
        |                       |                       | will be immediately   |
        |                       |                       | marked as skipped.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.comm      | `store​(Artif          | ::: block             |
        | on.util.concurrent.Li | actInfo info,      Bo | Store the artifact at |
        | stenableFuture<Unit>` | rrowablePath output)` | path specified by     |
        |                       |                       | output to cache, such |
        |                       |                       | that it can later be  |
        |                       |                       | fetched using ruleKey |
        |                       |                       | as the lookup key.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.comm      | `store​(co             | ::: block             |
        | on.util.concurrent.Li | m.google.common.colle | Store the list of     |
        | stenableFuture<Unit>` | ct.ImmutableList<Pair | artifacts at path     |
        |                       | <ArtifactInfo,​Borrowa | specified by output   |
        |                       | blePath>> artifacts)` | to cache in passed    |
        |                       |                       | order, such that it   |
        |                       |                       | can later be fetched  |
        |                       |                       | using ruleKey as the  |
        |                       |                       | lookup key.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protec               | `storeIm              |                       |
        | ted abstract com.face | pl​(ArtifactInfo info, |                       |
        | book.buck.artifact_ca |           Path file)` |                       |
        | che.AbstractAsynchron |                       |                       |
        | ousCache.StoreResult` |                       |                       |
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

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.artifact_cache.ArtifactCache}

            ### Methods inherited from interface com.facebook.buck.artifact_cache.[ArtifactCache](ArtifactCache.html "interface in com.facebook.buck.artifact_cache")

            `close`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.lang.String,com.facebook.buck.artifact_cache.config.ArtifactCacheMode,com.facebook.buck.artifact_cache.config.CacheReadMode,com.google.common.util.concurrent.ListeningExecutorService,com.google.common.util.concurrent.ListeningExecutorService,com.facebook.buck.artifact_cache.AbstractAsynchronousCache.CacheEventListener,java.util.Optional,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### AbstractAsynchronousCache

                public AbstractAsynchronousCache​(String name,
                                                 ArtifactCacheMode mode,
                                                 CacheReadMode cacheReadMode,
                                                 com.google.common.util.concurrent.ListeningExecutorService storeExecutorService,
                                                 com.google.common.util.concurrent.ListeningExecutorService fetchExecutorService,
                                                 AbstractAsynchronousCache.CacheEventListener eventListener,
                                                 Optional<Long> maxStoreSize,
                                                 ProjectFilesystem projectFilesystem)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getName()}

        -   #### getName

            ``` methodSignature
            protected final String getName()
            ```

        []{#getMode()}

        -   #### getMode

            ``` methodSignature
            protected final ArtifactCacheMode getMode()
            ```

        []{#getProjectFilesystem()}

        -   #### getProjectFilesystem

            ``` methodSignature
            protected final ProjectFilesystem getProjectFilesystem()
            ```

        []{#fetchImpl(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rulekey.RuleKey,com.facebook.buck.io.file.LazyPath)}

        -   #### fetchImpl

            ``` methodSignature
            protected abstract com.facebook.buck.artifact_cache.AbstractAsynchronousCache.FetchResult fetchImpl​(@Nullable
                                                                                                                BuildTarget target,
                                                                                                                RuleKey ruleKey,
                                                                                                                LazyPath output)
                                                                                                         throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#multiContainsImpl(com.google.common.collect.ImmutableSet)}

        -   #### multiContainsImpl

            ``` methodSignature
            protected abstract com.facebook.buck.artifact_cache.AbstractAsynchronousCache.MultiContainsResult multiContainsImpl​(com.google.common.collect.ImmutableSet<RuleKey> ruleKeys)
                                                                                                                         throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#storeImpl(com.facebook.buck.artifact_cache.ArtifactInfo,java.nio.file.Path)}

        -   #### storeImpl

            ``` methodSignature
            protected abstract com.facebook.buck.artifact_cache.AbstractAsynchronousCache.StoreResult storeImpl​(ArtifactInfo info,
                                                                                                                Path file)
                                                                                                         throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#deleteImpl(java.util.List)}

        -   #### deleteImpl

            ``` methodSignature
            protected abstract CacheDeleteResult deleteImpl​(List<RuleKey> ruleKeys)
                                                     throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#multiFetchImpl(java.lang.Iterable)}

        -   #### multiFetchImpl

            ``` methodSignature
            protected abstract com.facebook.buck.artifact_cache.AbstractAsynchronousCache.MultiFetchResult multiFetchImpl​(Iterable<AbstractAsynchronousCache.FetchRequest> requests)
                                                                                                                   throws IOException
            ```

            ::: block
            The MultiFetchResult should contain results in the same
            order as the requests.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getMultiFetchBatchSize(int)}

        -   #### getMultiFetchBatchSize

            ``` methodSignature
            protected int getMultiFetchBatchSize​(int pendingRequestsSize)
            ```

            ::: block
            Used to compute the number of keys to include in every
            multiFetchRequest. If \< 1, fetch will be used instead of
            multifetch.
            :::

        []{#isMultiCheckEnabled()}

        -   #### isMultiCheckEnabled

            ``` methodSignature
            protected boolean isMultiCheckEnabled()
            ```

        []{#skipPendingAndFutureAsyncFetches()}

        -   #### skipPendingAndFutureAsyncFetches

            ``` methodSignature
            public void skipPendingAndFutureAsyncFetches()
            ```

            ::: block
            [Description copied from
            interface: `ArtifactCache`]{.descfrmTypeLabel}
            :::

            ::: block
            All pending (and future) async fetches will be immediately
            marked as skipped.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `skipPendingAndFutureAsyncFetches` in
                interface `ArtifactCache`

        []{#fetchAsync(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rulekey.RuleKey,com.facebook.buck.io.file.LazyPath)}

        -   #### fetchAsync

            ``` methodSignature
            public final com.google.common.util.concurrent.ListenableFuture<CacheResult> fetchAsync​(@Nullable
                                                                                                    BuildTarget target,
                                                                                                    RuleKey ruleKey,
                                                                                                    LazyPath output)
            ```

            ::: block
            [Description copied from
            interface: `ArtifactCache`]{.descfrmTypeLabel}
            :::

            ::: block
            Fetch a cached artifact, keyed by ruleKey, save the artifact
            to path specified by output, and return true on success.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `fetchAsync` in interface `ArtifactCache`

            [Parameters:]{.paramLabel}
            :   `target` - rule for which this is an artifact
            :   `ruleKey` - cache fetch key
            :   `output` - Path to store artifact to. Path should not be
                accessed unless store operation is guaranteed by the
                cache, to avoid potential extra disk I/O.

            [Returns:]{.returnLabel}
            :   whether it was a
                [`CacheResultType.MISS`](CacheResultType.html#MISS)
                (indicating a failure) or some type of hit.

        []{#multiContainsAsync(com.google.common.collect.ImmutableSet)}

        -   #### multiContainsAsync

            ``` methodSignature
            public final com.google.common.util.concurrent.ListenableFuture<com.google.common.collect.ImmutableMap<RuleKey,​CacheResult>> multiContainsAsync​(com.google.common.collect.ImmutableSet<RuleKey> ruleKeys)
            ```

            ::: block
            [Description copied from
            interface: `ArtifactCache`]{.descfrmTypeLabel}
            :::

            ::: block
            Check if the cache contains the given artifacts, keyed by
            ruleKeys, without fetching them, and return a map of results
            wrapped in a `ListenableFuture`. This is supposed to be
            fast, but best-effort, meaning that there will be
            false-positives.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `multiContainsAsync` in interface `ArtifactCache`

            [Parameters:]{.paramLabel}
            :   `ruleKeys` - Set of cache fetch keys.

            [Returns:]{.returnLabel}
            :   map of keys to
                [`CacheResult`](CacheResult.html "class in com.facebook.buck.artifact_cache")
                which can be a
                [`CacheResultType.MISS`](CacheResultType.html#MISS) /
                [`CacheResultType.ERROR`](CacheResultType.html#ERROR)
                (indicating a failure) or
                [`CacheResultType.CONTAINS`](CacheResultType.html#CONTAINS).

        []{#store(com.facebook.buck.artifact_cache.ArtifactInfo,com.facebook.buck.io.file.BorrowablePath)}

        -   #### store

            ``` methodSignature
            public final com.google.common.util.concurrent.ListenableFuture<Unit> store​(ArtifactInfo info,
                                                                                        BorrowablePath output)
            ```

            ::: block
            [Description copied from
            interface: `ArtifactCache`]{.descfrmTypeLabel}
            :::

            ::: block
            Store the artifact at path specified by output to cache,
            such that it can later be fetched using ruleKey as the
            lookup key. If any internal errors occur, fail silently and
            continue execution. Store may be performed synchronously or
            asynchronously.
            This is a noop if
            [`ArtifactCache.getCacheReadMode()`](ArtifactCache.html#getCacheReadMode())}
            returns `READONLY`.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `store` in interface `ArtifactCache`

            [Parameters:]{.paramLabel}
            :   `info` - information to store with the artifact
            :   `output` - path to read artifact from. If its
                borrowable, you may freely move the file into cache
                without obtaining a copy of the file.

            [Returns:]{.returnLabel}
            :   `ListenableFuture` that completes once the store has
                finished.

        []{#store(com.google.common.collect.ImmutableList)}

        -   #### store

            ``` methodSignature
            public final com.google.common.util.concurrent.ListenableFuture<Unit> store​(com.google.common.collect.ImmutableList<Pair<ArtifactInfo,​BorrowablePath>> artifacts)
            ```

            ::: block
            [Description copied from
            interface: `ArtifactCache`]{.descfrmTypeLabel}
            :::

            ::: block
            Store the list of artifacts at path specified by output to
            cache in passed order, such that it can later be fetched
            using ruleKey as the lookup key. If any internal errors
            occur, fail silently and continue execution. Store may be
            performed synchronously or asynchronously.
            This is a noop if
            [`ArtifactCache.getCacheReadMode()`](ArtifactCache.html#getCacheReadMode())}
            returns `READONLY`.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `store` in interface `ArtifactCache`

            [Parameters:]{.paramLabel}
            :   `artifacts` - list of artifact info and path to be
                uploaded to the cache in given order.

            [Returns:]{.returnLabel}
            :   `ListenableFuture` that completes once the store has
                finished.

        []{#deleteAsync(java.util.List)}

        -   #### deleteAsync

            ``` methodSignature
            public final com.google.common.util.concurrent.ListenableFuture<CacheDeleteResult> deleteAsync​(List<RuleKey> ruleKeys)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `deleteAsync` in interface `ArtifactCache`

        []{#getCacheReadMode()}

        -   #### getCacheReadMode

            ``` methodSignature
            public final CacheReadMode getCacheReadMode()
            ```

            ::: block
            [Description copied from
            interface: `ArtifactCache`]{.descfrmTypeLabel}
            :::

            ::: block
            This method must return the same value over the lifetime of
            this object.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCacheReadMode` in interface `ArtifactCache`

            [Returns:]{.returnLabel}
            :   whether
                this[`ArtifactCache`](ArtifactCache.html "interface in com.facebook.buck.artifact_cache")
                supports storing artifacts.
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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
