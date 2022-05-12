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
-   Tree
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
# Hierarchy For Package com.facebook.buck.util.cache {#hierarchy-for-package-com.facebook.buck.util.cache .title}

[Package Hierarchies:]{.packageHierarchyLabel}

-   [All Packages](../../../../../overview-tree.html)
:::

::: contentContainer
::: {.section role="region"}
## Class Hierarchy {#class-hierarchy title="Class Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   com.facebook.buck.util.cache.[[CacheStats]{.typeNameLink}](CacheStats.html "class in com.facebook.buck.util.cache")
    -   com.facebook.buck.util.cache.[[DelegatingFileHashCacheEngine]{.typeNameLink}](DelegatingFileHashCacheEngine.html "class in com.facebook.buck.util.cache")
        (implements
        com.facebook.buck.util.cache.[FileHashCacheEngine](FileHashCacheEngine.html "interface in com.facebook.buck.util.cache"))
    -   com.facebook.buck.util.cache.[[HashCodeAndFileType]{.typeNameLink}](HashCodeAndFileType.html "class in com.facebook.buck.util.cache")
        -   com.facebook.buck.util.cache.[[JarHashCodeAndFileType]{.typeNameLink}](JarHashCodeAndFileType.html "class in com.facebook.buck.util.cache")
    -   com.facebook.buck.util.cache.ImmutableCacheStats.Builder
        -   com.facebook.buck.util.cache.[[CacheStats.Builder]{.typeNameLink}](CacheStats.Builder.html "class in com.facebook.buck.util.cache")
    -   com.facebook.buck.util.cache.[[InstrumentingCacheStatsTracker]{.typeNameLink}](InstrumentingCacheStatsTracker.html "class in com.facebook.buck.util.cache")
        (implements
        com.facebook.buck.util.cache.[CacheStatsTracker](CacheStatsTracker.html "interface in com.facebook.buck.util.cache"))
    -   com.facebook.buck.util.cache.[[InstrumentingCacheStatsTracker.TrackingCacheRequest]{.typeNameLink}](InstrumentingCacheStatsTracker.TrackingCacheRequest.html "class in com.facebook.buck.util.cache")
        (implements
        com.facebook.buck.util.cache.[CacheStatsTracker.CacheRequest](CacheStatsTracker.CacheRequest.html "interface in com.facebook.buck.util.cache"))
    -   com.facebook.buck.util.cache.[[NoOpCacheStatsTracker]{.typeNameLink}](NoOpCacheStatsTracker.html "class in com.facebook.buck.util.cache")
        (implements
        com.facebook.buck.util.cache.[CacheStatsTracker](CacheStatsTracker.html "interface in com.facebook.buck.util.cache"))
    -   com.facebook.buck.util.cache.[[NoOpCacheStatsTracker.NoOpCacheRequest]{.typeNameLink}](NoOpCacheStatsTracker.NoOpCacheRequest.html "class in com.facebook.buck.util.cache")
        (implements
        com.facebook.buck.util.cache.[CacheStatsTracker.CacheRequest](CacheStatsTracker.CacheRequest.html "interface in com.facebook.buck.util.cache"))
:::

::: {.section role="region"}
## Interface Hierarchy {#interface-hierarchy title="Interface Hierarchy"}

-   com.facebook.buck.util.cache.[[CacheStatsTracker]{.typeNameLink}](CacheStatsTracker.html "interface in com.facebook.buck.util.cache")
-   com.facebook.buck.util.cache.[[CacheStatsTracker.CacheRequest]{.typeNameLink}](CacheStatsTracker.CacheRequest.html "interface in com.facebook.buck.util.cache")
-   com.facebook.buck.util.cache.[[FileHashCache.FileHashCacheVerificationResult]{.typeNameLink}](FileHashCache.FileHashCacheVerificationResult.html "interface in com.facebook.buck.util.cache")
-   com.facebook.buck.util.cache.[[FileHashCacheEngine]{.typeNameLink}](FileHashCacheEngine.html "interface in com.facebook.buck.util.cache")
-   com.facebook.buck.util.cache.[[FileHashCacheEngine.ValueLoader]{.typeNameLink}](FileHashCacheEngine.ValueLoader.html "interface in com.facebook.buck.util.cache")\<T\>
-   com.facebook.buck.util.hashing.[[FileHashLoader]{.typeNameLink}](../hashing/FileHashLoader.html "interface in com.facebook.buck.util.hashing")
    -   com.facebook.buck.util.cache.[[FileHashCache]{.typeNameLink}](FileHashCache.html "interface in com.facebook.buck.util.cache")
-   com.facebook.buck.util.cache.[[JarContentHasher]{.typeNameLink}](JarContentHasher.html "interface in com.facebook.buck.util.cache")
-   com.facebook.buck.util.hashing.[[ProjectFileHashLoader]{.typeNameLink}](../hashing/ProjectFileHashLoader.html "interface in com.facebook.buck.util.hashing")
    -   com.facebook.buck.util.cache.[[ProjectFileHashCache]{.typeNameLink}](ProjectFileHashCache.html "interface in com.facebook.buck.util.cache")
:::

::: {.section role="region"}
## Enum Hierarchy {#enum-hierarchy title="Enum Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   java.lang.[[Enum]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<E\>
        (implements
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   com.facebook.buck.util.cache.[[FileHashCacheMode]{.typeNameLink}](FileHashCacheMode.html "enum in com.facebook.buck.util.cache")
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
-   Tree
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
