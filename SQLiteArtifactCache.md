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

## Class SQLiteArtifactCache {#class-sqliteartifactcache .title title="Class SQLiteArtifactCache"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.artifact_cache.SQLiteArtifactCache

::: description
-   

    All Implemented Interfaces:
    :   `ArtifactCache`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class SQLiteArtifactCache
        extends Object
        implements ArtifactCache

    ::: block
    Implementation of
    [`ArtifactCache`](ArtifactCache.html "interface in com.facebook.buck.artifact_cache")
    using SQLite.
    Cache entries are either metadata or content. All metadata contains
    a mapping to a content entry. Content entries with sufficiently
    small content will have their artifacts inlined into the database
    for improved performance.
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
        | `com.google.comm      | `store​(Artifa         | ::: block             |
        | on.util.concurrent.Li | ctInfo info,      Bor | Store the artifact at |
        | stenableFuture<Unit>` | rowablePath content)` | path specified by     |
        |                       |                       | output to cache, such |
        |                       |                       | that it can later be  |
        |                       |                       | fetched using ruleKey |
        |                       |                       | as the lookup key.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
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

            `store`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#fetchAsync(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rulekey.RuleKey,com.facebook.buck.io.file.LazyPath)}

        -   #### fetchAsync

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<CacheResult> fetchAsync​(@Nullable
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

        []{#store(com.facebook.buck.artifact_cache.ArtifactInfo,com.facebook.buck.io.file.BorrowablePath)}

        -   #### store

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<Unit> store​(ArtifactInfo info,
                                                                                  BorrowablePath content)
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
            :   `content` - path to read artifact from. If its
                borrowable, you may freely move the file into cache
                without obtaining a copy of the file.

            [Returns:]{.returnLabel}
            :   `ListenableFuture` that completes once the store has
                finished.

        []{#multiContainsAsync(com.google.common.collect.ImmutableSet)}

        -   #### multiContainsAsync

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<com.google.common.collect.ImmutableMap<RuleKey,​CacheResult>> multiContainsAsync​(com.google.common.collect.ImmutableSet<RuleKey> ruleKeys)
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

        []{#deleteAsync(java.util.List)}

        -   #### deleteAsync

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<CacheDeleteResult> deleteAsync​(List<RuleKey> ruleKeys)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `deleteAsync` in interface `ArtifactCache`

        []{#getCacheReadMode()}

        -   #### getCacheReadMode

            ``` methodSignature
            public CacheReadMode getCacheReadMode()
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

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `ArtifactCache`

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
