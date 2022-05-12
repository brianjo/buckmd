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

## Class CacheCountersSummary {#class-cachecounterssummary .title title="Class CacheCountersSummary"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.artifact_cache.CacheCountersSummary

::: description
-   

    ------------------------------------------------------------------------

        public abstract class CacheCountersSummary
        extends Object

    ::: block
    Utility class to help outputting the information to the
    machine-readable log. It helps in the serialization &
    deserialization process.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                Description
          -------------------------- -------------
          `CacheCountersSummary()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                    Method                                                                                                                                                                                                                                                                                                                                                                                                                                              Description
          ------------------------------------------------------------------------------------ --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `abstract com.google.common.collect.ImmutableMap<ArtifactCacheMode,​AtomicLong>`      `getCacheBytesPerMode()`                                                                                                                                                                                                                                                                                                                                                                                                                             
          `abstract com.google.common.collect.ImmutableMap<ArtifactCacheMode,​AtomicInteger>`   `getCacheErrorsPerMode()`                                                                                                                                                                                                                                                                                                                                                                                                                            
          `abstract com.google.common.collect.ImmutableMap<ArtifactCacheMode,​AtomicInteger>`   `getCacheHitsPerMode()`                                                                                                                                                                                                                                                                                                                                                                                                                              
          `abstract AtomicInteger`                                                             `getFailureUploadCount()`                                                                                                                                                                                                                                                                                                                                                                                                                            
          `abstract AtomicInteger`                                                             `getSuccessUploadCount()`                                                                                                                                                                                                                                                                                                                                                                                                                            
          `abstract long`                                                                      `getTotalCacheBytes()`                                                                                                                                                                                                                                                                                                                                                                                                                               
          `abstract int`                                                                       `getTotalCacheErrors()`                                                                                                                                                                                                                                                                                                                                                                                                                              
          `abstract int`                                                                       `getTotalCacheHits()`                                                                                                                                                                                                                                                                                                                                                                                                                                
          `abstract int`                                                                       `getTotalCacheIgnores()`                                                                                                                                                                                                                                                                                                                                                                                                                             
          `abstract int`                                                                       `getTotalCacheLocalKeyUnchangedHits()`                                                                                                                                                                                                                                                                                                                                                                                                               
          `abstract int`                                                                       `getTotalCacheMisses()`                                                                                                                                                                                                                                                                                                                                                                                                                              
          `static CacheCountersSummary`                                                        `of​(Map<ArtifactCacheMode,​? extends AtomicInteger> cacheHitsPerMode,   Map<ArtifactCacheMode,​? extends AtomicInteger> cacheErrorsPerMode,   Map<ArtifactCacheMode,​? extends AtomicLong> cacheBytesPerMode,   int totalCacheHits,   int totalCacheErrors,   int totalCacheMisses,   int totalCacheIgnores,   long totalCacheBytes,   int totalCacheLocalKeyUnchangedHits,   AtomicInteger successUploadCount,   AtomicInteger failureUploadCount)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

        []{#<init>()}

        -   #### CacheCountersSummary

                public CacheCountersSummary()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getCacheHitsPerMode()}

        -   #### getCacheHitsPerMode

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<ArtifactCacheMode,​AtomicInteger> getCacheHitsPerMode()
            ```

        []{#getCacheErrorsPerMode()}

        -   #### getCacheErrorsPerMode

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<ArtifactCacheMode,​AtomicInteger> getCacheErrorsPerMode()
            ```

        []{#getCacheBytesPerMode()}

        -   #### getCacheBytesPerMode

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<ArtifactCacheMode,​AtomicLong> getCacheBytesPerMode()
            ```

        []{#getTotalCacheHits()}

        -   #### getTotalCacheHits

            ``` methodSignature
            public abstract int getTotalCacheHits()
            ```

        []{#getTotalCacheErrors()}

        -   #### getTotalCacheErrors

            ``` methodSignature
            public abstract int getTotalCacheErrors()
            ```

        []{#getTotalCacheMisses()}

        -   #### getTotalCacheMisses

            ``` methodSignature
            public abstract int getTotalCacheMisses()
            ```

        []{#getTotalCacheIgnores()}

        -   #### getTotalCacheIgnores

            ``` methodSignature
            public abstract int getTotalCacheIgnores()
            ```

        []{#getTotalCacheBytes()}

        -   #### getTotalCacheBytes

            ``` methodSignature
            public abstract long getTotalCacheBytes()
            ```

        []{#getTotalCacheLocalKeyUnchangedHits()}

        -   #### getTotalCacheLocalKeyUnchangedHits

            ``` methodSignature
            public abstract int getTotalCacheLocalKeyUnchangedHits()
            ```

        []{#getSuccessUploadCount()}

        -   #### getSuccessUploadCount

            ``` methodSignature
            public abstract AtomicInteger getSuccessUploadCount()
            ```

        []{#getFailureUploadCount()}

        -   #### getFailureUploadCount

            ``` methodSignature
            public abstract AtomicInteger getFailureUploadCount()
            ```

        []{#of(java.util.Map,java.util.Map,java.util.Map,int,int,int,int,long,int,java.util.concurrent.atomic.AtomicInteger,java.util.concurrent.atomic.AtomicInteger)}

        -   #### of

            ``` methodSignature
            public static CacheCountersSummary of​(Map<ArtifactCacheMode,​? extends AtomicInteger> cacheHitsPerMode,
                                                  Map<ArtifactCacheMode,​? extends AtomicInteger> cacheErrorsPerMode,
                                                  Map<ArtifactCacheMode,​? extends AtomicLong> cacheBytesPerMode,
                                                  int totalCacheHits,
                                                  int totalCacheErrors,
                                                  int totalCacheMisses,
                                                  int totalCacheIgnores,
                                                  long totalCacheBytes,
                                                  int totalCacheLocalKeyUnchangedHits,
                                                  AtomicInteger successUploadCount,
                                                  AtomicInteger failureUploadCount)
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
