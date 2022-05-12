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

## Class CacheStats {#class-cachestats .title title="Class CacheStats"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.cache.CacheStats

::: description
-   

    ------------------------------------------------------------------------

        public abstract class CacheStats
        extends Object

    ::: block
    Class containing various cache statistics
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                  Description
          ------------------- ---------------------- -------------
          `static class `     `CacheStats.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor      Description
          ---------------- -------------
          `CacheStats()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `CacheStats`          | `a                    |                       |
        |                       | dd​(CacheStats stats)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `stati                | `builder()`           |                       |
        | c CacheStats.Builder` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abs                  | `getEvictionCount()`  |                       |
        | tract Optional<Long>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abs                  | `getHitCount()`       |                       |
        | tract Optional<Long>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abs                  | `ge                   |                       |
        | tract Optional<Long>` | tInvalidationCount()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abs                  | `get                  |                       |
        | tract Optional<Long>` | LoadExceptionCount()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abs                  | `g                    |                       |
        | tract Optional<Long>` | etLoadSuccessCount()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abs                  | `getMissCount()`      |                       |
        | tract Optional<Long>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abs                  | `getMissMatchCount()` |                       |
        | tract Optional<Long>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abs                  | `getNumberEntries()`  |                       |
        | tract Optional<Long>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Long>`      | `getRequestCount()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abs                  | `getRetrievalTime()`  |                       |
        | tract Optional<Long>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abs                  | `getTotalLoadTime()`  |                       |
        | tract Optional<Long>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abs                  | `getTotalMissTime()`  |                       |
        | tract Optional<Long>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Double>`    | `hitRate()`           | ::: block             |
        |                       |                       | Returns the ratio of  |
        |                       |                       | cache requests which  |
        |                       |                       | were hits.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Double>`    | `missMatchRate()`     | ::: block             |
        |                       |                       | Returns the ratio of  |
        |                       |                       | cache requests which  |
        |                       |                       | were misses due to    |
        |                       |                       | mismatch.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Double>`    | `missRate()`          | ::: block             |
        |                       |                       | Returns the ratio of  |
        |                       |                       | cache requests which  |
        |                       |                       | were misses.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CacheStats`          | `subtra               | ::: block             |
        |                       | ct​(CacheStats stats)` | Adds or subtract two  |
        |                       |                       | CacheStats if a field |
        |                       |                       | is specified by both  |
        |                       |                       | CacheStats, with a    |
        |                       |                       | minimum value of 0.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

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

        -   #### CacheStats

                public CacheStats()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getHitCount()}

        -   #### getHitCount

            ``` methodSignature
            public abstract Optional<Long> getHitCount()
            ```

        []{#getMissCount()}

        -   #### getMissCount

            ``` methodSignature
            public abstract Optional<Long> getMissCount()
            ```

        []{#getMissMatchCount()}

        -   #### getMissMatchCount

            ``` methodSignature
            public abstract Optional<Long> getMissMatchCount()
            ```

        []{#getEvictionCount()}

        -   #### getEvictionCount

            ``` methodSignature
            public abstract Optional<Long> getEvictionCount()
            ```

        []{#getInvalidationCount()}

        -   #### getInvalidationCount

            ``` methodSignature
            public abstract Optional<Long> getInvalidationCount()
            ```

        []{#getLoadSuccessCount()}

        -   #### getLoadSuccessCount

            ``` methodSignature
            public abstract Optional<Long> getLoadSuccessCount()
            ```

        []{#getLoadExceptionCount()}

        -   #### getLoadExceptionCount

            ``` methodSignature
            public abstract Optional<Long> getLoadExceptionCount()
            ```

        []{#getRetrievalTime()}

        -   #### getRetrievalTime

            ``` methodSignature
            public abstract Optional<Long> getRetrievalTime()
            ```

        []{#getTotalLoadTime()}

        -   #### getTotalLoadTime

            ``` methodSignature
            public abstract Optional<Long> getTotalLoadTime()
            ```

        []{#getTotalMissTime()}

        -   #### getTotalMissTime

            ``` methodSignature
            public abstract Optional<Long> getTotalMissTime()
            ```

        []{#getNumberEntries()}

        -   #### getNumberEntries

            ``` methodSignature
            public abstract Optional<Long> getNumberEntries()
            ```

        []{#getRequestCount()}

        -   #### getRequestCount

            ``` methodSignature
            public Optional<Long> getRequestCount()
            ```

            [Returns:]{.returnLabel}
            :   the total number of requests to the cash defined as
                `getHitCount() +      getMissCount() + getMissMatchCount()`
                if both hitCount and one of missCount or
                missMissMatchCount is set

        []{#hitRate()}

        -   #### hitRate

            ``` methodSignature
            public Optional<Double> hitRate()
            ```

            ::: block
            Returns the ratio of cache requests which were hits. This is
            defined as `getHitCount() /  requestCount`, or `1.0` when
            `requestCount == 0`. Note that `hitRate +  missRate =~ 1.0`.
            :::

        []{#missRate()}

        -   #### missRate

            ``` methodSignature
            public Optional<Double> missRate()
            ```

            ::: block
            Returns the ratio of cache requests which were misses. This
            is defined as `getMissCount()  / requestCount`, or `0.0`
            when `requestCount == 0`. Note that
            `hitRate +  missRate + missMatchRate =~ 1.0`. Cache misses
            include all requests which weren\'t cache hits, including
            requests which resulted in either successful or failed
            loading attempts, and requests which waited for other
            threads to finish loading. It is thus the case that
            `  getMissCount() + getMissMatchCount() &gt;= getLoadSuccessCount() + getLoadExceptionCount()`.
            Multiple concurrent misses for the same key will result in a
            single load operation.
            :::

        []{#missMatchRate()}

        -   #### missMatchRate

            ``` methodSignature
            public Optional<Double> missMatchRate()
            ```

            ::: block
            Returns the ratio of cache requests which were misses due to
            mismatch. This is defined as
            `getMissMatchCount() / requestCount`, or `0.0` when
            `requestCount == 0`. Note that
            `hitRate + missRate + missMatchRate =~ 1.0`. Cache misses
            include all requests which weren\'t cache hits, including
            requests which resulted in either successful or failed
            loading attempts, and requests which waited for other
            threads to finish loading. It is thus the case that
            `getMissCount() + getMissMatchCount() &gt;= getLoadSuccessCount() +  getLoadExceptionCount()`.
            Multiple concurrent misses for the same key will result in a
            single load operation.
            :::

        []{#subtract(com.facebook.buck.util.cache.CacheStats)}

        -   #### subtract

            ``` methodSignature
            public CacheStats subtract​(CacheStats stats)
            ```

            ::: block
            Adds or subtract two CacheStats if a field is specified by
            both CacheStats, with a minimum value of 0. If only one
            CacheStats specifies the field, the unspecified value is
            treated as 0. If non of the CacheStats specifies the field,
            the field will be empty.
            :::

            [Parameters:]{.paramLabel}
            :   `stats` - the stats after the arithmetic operator

            [Returns:]{.returnLabel}
            :   this +/- stats

        []{#add(com.facebook.buck.util.cache.CacheStats)}

        -   #### add

            ``` methodSignature
            public CacheStats add​(CacheStats stats)
            ```

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static CacheStats.Builder builder()
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
