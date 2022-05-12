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
-   Package
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Package com.facebook.buck.util.cache {#package-com.facebook.buck.util.cache .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [CacheStatsTracker](C             | ::: block                         |
    | acheStatsTracker.html "interface  | Class that tracks cache           |
    | in com.facebook.buck.util.cache") | statistics, including timings.    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CacheStatsTra                    | ::: block                         |
    | cker.CacheRequest](CacheStatsTrac | Class that keeps record and       |
    | ker.CacheRequest.html "interface  | timings of a single cache request |
    | in com.facebook.buck.util.cache") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [FileHashCach                     | ::: block                         |
    | e](FileHashCache.html "interface  | A cache which maps Paths to       |
    | in com.facebook.buck.util.cache") | cached hashes of their contents,  |
    |                                   | based on a simplified subset of   |
    |                                   | the java.util.Map\<Path,          |
    |                                   | HashCode\> interface.             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [FileHashCa                       |                                   |
    | che.FileHashCacheVerificationResu |                                   |
    | lt](FileHashCache.FileHashCacheVe |                                   |
    | rificationResult.html "interface  |                                   |
    | in com.facebook.buck.util.cache") |                                   |
    +-----------------------------------+-----------------------------------+
    | [FileHashCacheEngine](Fil         | ::: block                         |
    | eHashCacheEngine.html "interface  | This interface extracts the       |
    | in com.facebook.buck.util.cache") | methods available to a file hash  |
    |                                   | cache, so that the underlying     |
    |                                   | implementation is hidden and can  |
    |                                   | be swapped.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [FileHashCacheEngine.             |                                   |
    | ValueLoader](FileHashCacheEngine. |                                   |
    | ValueLoader.html "interface in co |                                   |
    | m.facebook.buck.util.cache")\<T\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [JarContentHasher](               |                                   |
    | JarContentHasher.html "interface  |                                   |
    | in com.facebook.buck.util.cache") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ProjectFileHashCache](Proj       | ::: block                         |
    | ectFileHashCache.html "interface  | A                                 |
    | in com.facebook.buck.util.cache") | [`FileHashLoader`](../hashing/    |
    |                                   | FileHashLoader.html "interface in |
    |                                   |  com.facebook.buck.util.hashing") |
    |                                   | which manages caching file hashes |
    |                                   | for a given                       |
    |                                   | [`ProjectFiles                    |
    |                                   | ystem`](../../io/filesystem/Proje |
    |                                   | ctFilesystem.html "interface in c |
    |                                   | om.facebook.buck.io.filesystem"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [Ca                               | ::: block                         |
    | cheStats](CacheStats.html "class  | Class containing various cache    |
    | in com.facebook.buck.util.cache") | statistics                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CacheStats.Builder               |                                   |
    | ](CacheStats.Builder.html "class  |                                   |
    | in com.facebook.buck.util.cache") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Delegat                          |                                   |
    | ingFileHashCacheEngine](Delegatin |                                   |
    | gFileHashCacheEngine.html "class  |                                   |
    | in com.facebook.buck.util.cache") |                                   |
    +-----------------------------------+-----------------------------------+
    | [HashCodeAndFileType]             | ::: block                         |
    | (HashCodeAndFileType.html "class  | Data container to hold hash value |
    | in com.facebook.buck.util.cache") | for a file or directory           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Instrumen                        | ::: block                         |
    | tingCacheStatsTracker](Instrument | Class that tracks cache           |
    | ingCacheStatsTracker.html "class  | statistics, including timings.    |
    | in com.facebook.buck.util.cache") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JarHashCodeAndFileType](Ja       | ::: block                         |
    | rHashCodeAndFileType.html "class  | HashCodeAndFileType that also     |
    | in com.facebook.buck.util.cache") | stores and caches hashes or file  |
    |                                   | in a jar                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NoOpCacheStatsTracker](N         | ::: block                         |
    | oOpCacheStatsTracker.html "class  | CacheStats tracker that doesn\'t  |
    | in com.facebook.buck.util.cache") | track any stats                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Enum                              | Description                       |
    +===================================+===================================+
    | [FileHashCacheMo                  | ::: block                         |
    | de](FileHashCacheMode.html "enum  | Defines which file hash cache     |
    | in com.facebook.buck.util.cache") | engine to use.                    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Enum Summary[ ]{.tabEnd}
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../../index.html)
-   Package
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

[]{#skip.navbar.bottom}
:::
