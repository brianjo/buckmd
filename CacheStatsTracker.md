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
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.util.cache](package-summary.html)
:::

## Interface CacheStatsTracker {#interface-cachestatstracker .title title="Interface CacheStatsTracker"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `InstrumentingCacheStatsTracker`, `NoOpCacheStatsTracker`

    ------------------------------------------------------------------------

        public interface CacheStatsTracker

    ::: block
    Class that tracks cache statistics, including timings.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Interface             | Description           |
        +=======================+=======================+=======================+
        | `static interface `   | `CacheStats           | ::: block             |
        |                       | Tracker.CacheRequest` | Class that keeps      |
        |                       |                       | record and timings of |
        |                       |                       | a single cache        |
        |                       |                       | request               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                  Method                           Description
          ---------------------------------- -------------------------------- -------------
          `long`                             `getAverageLoadTime()`            
          `long`                             `getAverageMissTime()`            
          `long`                             `getAverageRetrievalTime()`       
          `long`                             `getTotalEvictionCount()`         
          `long`                             `getTotalHitCount()`              
          `long`                             `getTotalInvalidationCount()`     
          `long`                             `getTotalLoadExceptionCount()`    
          `long`                             `getTotalLoadSuccessCount()`      
          `long`                             `getTotalLoadTime()`              
          `long`                             `getTotalMissCount()`             
          `long`                             `getTotalMissMatchCount()`        
          `long`                             `getTotalMissTime()`              
          `long`                             `getTotalRetrievalTime()`         
          `void`                             `recordEviction()`                
          `void`                             `recordEviction​(long num)`        
          `void`                             `recordInvalidation()`            
          `void`                             `recordInvalidation​(long num)`    
          `CacheStatsTracker.CacheRequest`   `startRequest()`                  

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#startRequest()}

        -   #### startRequest

            ``` methodSignature
            CacheStatsTracker.CacheRequest startRequest()
            ```

        []{#getTotalHitCount()}

        -   #### getTotalHitCount

            ``` methodSignature
            long getTotalHitCount()
            ```

        []{#getTotalMissCount()}

        -   #### getTotalMissCount

            ``` methodSignature
            long getTotalMissCount()
            ```

        []{#getTotalMissMatchCount()}

        -   #### getTotalMissMatchCount

            ``` methodSignature
            long getTotalMissMatchCount()
            ```

        []{#getTotalEvictionCount()}

        -   #### getTotalEvictionCount

            ``` methodSignature
            long getTotalEvictionCount()
            ```

        []{#getTotalInvalidationCount()}

        -   #### getTotalInvalidationCount

            ``` methodSignature
            long getTotalInvalidationCount()
            ```

        []{#getTotalLoadSuccessCount()}

        -   #### getTotalLoadSuccessCount

            ``` methodSignature
            long getTotalLoadSuccessCount()
            ```

        []{#getTotalLoadExceptionCount()}

        -   #### getTotalLoadExceptionCount

            ``` methodSignature
            long getTotalLoadExceptionCount()
            ```

        []{#getTotalRetrievalTime()}

        -   #### getTotalRetrievalTime

            ``` methodSignature
            long getTotalRetrievalTime()
            ```

        []{#getTotalLoadTime()}

        -   #### getTotalLoadTime

            ``` methodSignature
            long getTotalLoadTime()
            ```

        []{#getTotalMissTime()}

        -   #### getTotalMissTime

            ``` methodSignature
            long getTotalMissTime()
            ```

        []{#getAverageRetrievalTime()}

        -   #### getAverageRetrievalTime

            ``` methodSignature
            long getAverageRetrievalTime()
            ```

        []{#getAverageMissTime()}

        -   #### getAverageMissTime

            ``` methodSignature
            long getAverageMissTime()
            ```

        []{#getAverageLoadTime()}

        -   #### getAverageLoadTime

            ``` methodSignature
            long getAverageLoadTime()
            ```

        []{#recordEviction()}

        -   #### recordEviction

            ``` methodSignature
            void recordEviction()
            ```

        []{#recordEviction(long)}

        -   #### recordEviction

            ``` methodSignature
            void recordEviction​(long num)
            ```

        []{#recordInvalidation()}

        -   #### recordInvalidation

            ``` methodSignature
            void recordInvalidation()
            ```

        []{#recordInvalidation(long)}

        -   #### recordInvalidation

            ``` methodSignature
            void recordInvalidation​(long num)
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
-   [Nested](#nested.class.summary) \| 
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
