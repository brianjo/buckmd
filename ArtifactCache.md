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
[Package]{.packageLabelInType} [com.facebook.buck.artifact_cache](package-summary.html)
:::

## Interface ArtifactCache {#interface-artifactcache .title title="Interface ArtifactCache"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AutoCloseable`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AbstractAsynchronousCache`, `AbstractNetworkCache`,
        `DirArtifactCache`, `HttpArtifactCache`,
        `LoggingArtifactCacheDecorator`, `MultiArtifactCache`,
        `NoopArtifactCache`, `RetryingCacheDecorator`,
        `SQLiteArtifactCache`, `ThriftArtifactCache`,
        `TwoLevelArtifactCacheDecorator`

    ------------------------------------------------------------------------

        public interface ArtifactCache
        extends AutoCloseable
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
        | `com.goo              | `deleteAsync​(Lis      |                       |
        | gle.common.util.concu | t<RuleKey> ruleKeys)` |                       |
        | rrent.ListenableFutur |                       |                       |
        | e<CacheDeleteResult>` |                       |                       |
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
        | `CacheReadMode`       | `getCacheReadMode()`  | ::: block             |
        |                       |                       | This method must      |
        |                       |                       | return the same value |
        |                       |                       | over the lifetime of  |
        |                       |                       | this object.          |
        |                       |                       | :::                   |
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
        | `de                   | `store​(co             | ::: block             |
        | fault com.google.comm | m.google.common.colle | Store the list of     |
        | on.util.concurrent.Li | ct.ImmutableList<Pair | artifacts at path     |
        | stenableFuture<Unit>` | <ArtifactInfo,​Borrowa | specified by output   |
        |                       | blePath>> artifacts)` | to cache in passed    |
        |                       |                       | order, such that it   |
        |                       |                       | can later be fetched  |
        |                       |                       | using ruleKey as the  |
        |                       |                       | lookup key.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#fetchAsync(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rulekey.RuleKey,com.facebook.buck.io.file.LazyPath)}

        -   #### fetchAsync

            ``` methodSignature
            com.google.common.util.concurrent.ListenableFuture<CacheResult> fetchAsync​(@Nullable
                                                                                       BuildTarget target,
                                                                                       RuleKey ruleKey,
                                                                                       LazyPath output)
            ```

            ::: block
            Fetch a cached artifact, keyed by ruleKey, save the artifact
            to path specified by output, and return true on success.
            :::

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

        []{#skipPendingAndFutureAsyncFetches()}

        -   #### skipPendingAndFutureAsyncFetches

            ``` methodSignature
            void skipPendingAndFutureAsyncFetches()
            ```

            ::: block
            All pending (and future) async fetches will be immediately
            marked as skipped.
            :::

        []{#store(com.facebook.buck.artifact_cache.ArtifactInfo,com.facebook.buck.io.file.BorrowablePath)}

        -   #### store

            ``` methodSignature
            com.google.common.util.concurrent.ListenableFuture<Unit> store​(ArtifactInfo info,
                                                                           BorrowablePath output)
            ```

            ::: block
            Store the artifact at path specified by output to cache,
            such that it can later be fetched using ruleKey as the
            lookup key. If any internal errors occur, fail silently and
            continue execution. Store may be performed synchronously or
            asynchronously.
            This is a noop if
            [`getCacheReadMode()`](#getCacheReadMode())} returns
            `READONLY`.
            :::

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
            default com.google.common.util.concurrent.ListenableFuture<Unit> store​(com.google.common.collect.ImmutableList<Pair<ArtifactInfo,​BorrowablePath>> artifacts)
            ```

            ::: block
            Store the list of artifacts at path specified by output to
            cache in passed order, such that it can later be fetched
            using ruleKey as the lookup key. If any internal errors
            occur, fail silently and continue execution. Store may be
            performed synchronously or asynchronously.
            This is a noop if
            [`getCacheReadMode()`](#getCacheReadMode())} returns
            `READONLY`.
            :::

            [Parameters:]{.paramLabel}
            :   `artifacts` - list of artifact info and path to be
                uploaded to the cache in given order.

            [Returns:]{.returnLabel}
            :   `ListenableFuture` that completes once the store has
                finished.

        []{#multiContainsAsync(com.google.common.collect.ImmutableSet)}

        -   #### multiContainsAsync

            ``` methodSignature
            com.google.common.util.concurrent.ListenableFuture<com.google.common.collect.ImmutableMap<RuleKey,​CacheResult>> multiContainsAsync​(com.google.common.collect.ImmutableSet<RuleKey> ruleKeys)
            ```

            ::: block
            Check if the cache contains the given artifacts, keyed by
            ruleKeys, without fetching them, and return a map of results
            wrapped in a `ListenableFuture`. This is supposed to be
            fast, but best-effort, meaning that there will be
            false-positives.
            :::

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

        []{#deleteAsync(java.util.List)}

        -   #### deleteAsync

            ``` methodSignature
            com.google.common.util.concurrent.ListenableFuture<CacheDeleteResult> deleteAsync​(List<RuleKey> ruleKeys)
            ```

        []{#getCacheReadMode()}

        -   #### getCacheReadMode

            ``` methodSignature
            CacheReadMode getCacheReadMode()
            ```

            ::: block
            This method must return the same value over the lifetime of
            this object.
            :::

            [Returns:]{.returnLabel}
            :   whether
                this[`ArtifactCache`](ArtifactCache.html "interface in com.facebook.buck.artifact_cache")
                supports storing artifacts.

        []{#close()}

        -   #### close

            ``` methodSignature
            void close()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`
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
