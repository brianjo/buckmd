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
[Package]{.packageLabelInType} [com.facebook.buck.util.cache](package-summary.html)
:::

## Class NoOpCacheStatsTracker {#class-noopcachestatstracker .title title="Class NoOpCacheStatsTracker"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.cache.NoOpCacheStatsTracker

::: description
-   

    All Implemented Interfaces:
    :   `CacheStatsTracker`

    ------------------------------------------------------------------------

        public class NoOpCacheStatsTracker
        extends Object
        implements CacheStatsTracker

    ::: block
    CacheStats tracker that doesn\'t track any stats
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `class `              | `NoOpCacheStatsTrac   | ::: block             |
        |                       | ker.NoOpCacheRequest` | CacheRequest that     |
        |                       |                       | doesn\'t track stats  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.util.cache.CacheStatsTracker}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.util.cache.[CacheStatsTracker](CacheStatsTracker.html "interface in com.facebook.buck.util.cache")

            `CacheStatsTracker.CacheRequest`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                 Description
          --------------------------- -------------
          `NoOpCacheStatsTracker()`    

          : Constructors[ ]{.tabEnd}
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

        -   #### NoOpCacheStatsTracker

                public NoOpCacheStatsTracker()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#startRequest()}

        -   #### startRequest

            ``` methodSignature
            public CacheStatsTracker.CacheRequest startRequest()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `startRequest` in interface `CacheStatsTracker`

        []{#getTotalHitCount()}

        -   #### getTotalHitCount

            ``` methodSignature
            public long getTotalHitCount()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTotalHitCount` in interface `CacheStatsTracker`

        []{#getTotalMissCount()}

        -   #### getTotalMissCount

            ``` methodSignature
            public long getTotalMissCount()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTotalMissCount` in interface `CacheStatsTracker`

        []{#getTotalMissMatchCount()}

        -   #### getTotalMissMatchCount

            ``` methodSignature
            public long getTotalMissMatchCount()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTotalMissMatchCount` in
                interface `CacheStatsTracker`

        []{#getTotalEvictionCount()}

        -   #### getTotalEvictionCount

            ``` methodSignature
            public long getTotalEvictionCount()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTotalEvictionCount` in interface `CacheStatsTracker`

        []{#getTotalInvalidationCount()}

        -   #### getTotalInvalidationCount

            ``` methodSignature
            public long getTotalInvalidationCount()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTotalInvalidationCount` in
                interface `CacheStatsTracker`

        []{#getTotalLoadSuccessCount()}

        -   #### getTotalLoadSuccessCount

            ``` methodSignature
            public long getTotalLoadSuccessCount()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTotalLoadSuccessCount` in
                interface `CacheStatsTracker`

        []{#getTotalLoadExceptionCount()}

        -   #### getTotalLoadExceptionCount

            ``` methodSignature
            public long getTotalLoadExceptionCount()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTotalLoadExceptionCount` in
                interface `CacheStatsTracker`

        []{#getTotalRetrievalTime()}

        -   #### getTotalRetrievalTime

            ``` methodSignature
            public long getTotalRetrievalTime()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTotalRetrievalTime` in interface `CacheStatsTracker`

        []{#getTotalLoadTime()}

        -   #### getTotalLoadTime

            ``` methodSignature
            public long getTotalLoadTime()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTotalLoadTime` in interface `CacheStatsTracker`

        []{#getTotalMissTime()}

        -   #### getTotalMissTime

            ``` methodSignature
            public long getTotalMissTime()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTotalMissTime` in interface `CacheStatsTracker`

        []{#getAverageRetrievalTime()}

        -   #### getAverageRetrievalTime

            ``` methodSignature
            public long getAverageRetrievalTime()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAverageRetrievalTime` in
                interface `CacheStatsTracker`

        []{#getAverageMissTime()}

        -   #### getAverageMissTime

            ``` methodSignature
            public long getAverageMissTime()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAverageMissTime` in interface `CacheStatsTracker`

        []{#getAverageLoadTime()}

        -   #### getAverageLoadTime

            ``` methodSignature
            public long getAverageLoadTime()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAverageLoadTime` in interface `CacheStatsTracker`

        []{#recordEviction()}

        -   #### recordEviction

            ``` methodSignature
            public void recordEviction()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `recordEviction` in interface `CacheStatsTracker`

        []{#recordEviction(long)}

        -   #### recordEviction

            ``` methodSignature
            public void recordEviction​(long num)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `recordEviction` in interface `CacheStatsTracker`

        []{#recordInvalidation()}

        -   #### recordInvalidation

            ``` methodSignature
            public void recordInvalidation()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `recordInvalidation` in interface `CacheStatsTracker`

        []{#recordInvalidation(long)}

        -   #### recordInvalidation

            ``` methodSignature
            public void recordInvalidation​(long num)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `recordInvalidation` in interface `CacheStatsTracker`
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
