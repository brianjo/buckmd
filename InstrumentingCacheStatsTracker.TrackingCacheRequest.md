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
[Package]{.packageLabelInType} [com.facebook.buck.util.cache](package-summary.html)
:::

## Class InstrumentingCacheStatsTracker.TrackingCacheRequest {#class-instrumentingcachestatstracker.trackingcacherequest .title title="Class InstrumentingCacheStatsTracker.TrackingCacheRequest"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.cache.InstrumentingCacheStatsTracker.TrackingCacheRequest

::: description
-   

    All Implemented Interfaces:
    :   `CacheStatsTracker.CacheRequest`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [InstrumentingCacheStatsTracker](InstrumentingCacheStatsTracker.html "class in com.facebook.buck.util.cache")

    ------------------------------------------------------------------------

        public class InstrumentingCacheStatsTracker.TrackingCacheRequest
        extends Object
        implements CacheStatsTracker.CacheRequest

    ::: block
    Class that keeps record and timings of a single cache request
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `recordHit()`         | ::: block             |
        |                       |                       | Records that a cache  |
        |                       |                       | hit has occurred and  |
        |                       |                       | updates the           |
        |                       |                       | corresponding         |
        |                       |                       | Instrument            |
        |                       |                       | ingCacheStatsTracker, |
        |                       |                       | and records the time  |
        |                       |                       | it took for the cache |
        |                       |                       | retrieval             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `recordLoadFail()`    | ::: block             |
        |                       |                       | Records that a cache  |
        |                       |                       | load has failed and   |
        |                       |                       | updates the           |
        |                       |                       | corresponding         |
        |                       |                       | Instrument            |
        |                       |                       | ingCacheStatsTracker, |
        |                       |                       | and records the time  |
        |                       |                       | spent on a cache miss |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `recordLoadSuccess()` | ::: block             |
        |                       |                       | Records that a cache  |
        |                       |                       | load was successful   |
        |                       |                       | and updates the       |
        |                       |                       | corresponding         |
        |                       |                       | Instrument            |
        |                       |                       | ingCacheStatsTracker, |
        |                       |                       | and records the time  |
        |                       |                       | it took to load the   |
        |                       |                       | object and updates    |
        |                       |                       | the total time spent  |
        |                       |                       | on a cache miss       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `recordMiss()`        | ::: block             |
        |                       |                       | Records that a cache  |
        |                       |                       | miss has occurred and |
        |                       |                       | updates the           |
        |                       |                       | corresponding         |
        |                       |                       | Instrument            |
        |                       |                       | ingCacheStatsTracker, |
        |                       |                       | and starts recording  |
        |                       |                       | the load time         |
        |                       |                       | starting at this      |
        |                       |                       | instant.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `recordMissMatch()`   | ::: block             |
        |                       |                       | Records that a cache  |
        |                       |                       | miss due to mismatch  |
        |                       |                       | has occurred and      |
        |                       |                       | updates the           |
        |                       |                       | corresponding         |
        |                       |                       | Instrument            |
        |                       |                       | ingCacheStatsTracker, |
        |                       |                       | and starts recording  |
        |                       |                       | the load time         |
        |                       |                       | starting at this      |
        |                       |                       | instant.              |
        |                       |                       | :::                   |
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

        []{#recordHit()}

        -   #### recordHit

            ``` methodSignature
            public void recordHit()
            ```

            ::: block
            Records that a cache hit has occurred and updates the
            corresponding InstrumentingCacheStatsTracker, and records
            the time it took for the cache retrieval
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `recordHit` in
                interface `CacheStatsTracker.CacheRequest`

        []{#recordMiss()}

        -   #### recordMiss

            ``` methodSignature
            public void recordMiss()
            ```

            ::: block
            Records that a cache miss has occurred and updates the
            corresponding InstrumentingCacheStatsTracker, and starts
            recording the load time starting at this instant. If no load
            event occurs, the current time will be recorded as the time
            it took for a cache miss
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `recordMiss` in
                interface `CacheStatsTracker.CacheRequest`

        []{#recordMissMatch()}

        -   #### recordMissMatch

            ``` methodSignature
            public void recordMissMatch()
            ```

            ::: block
            Records that a cache miss due to mismatch has occurred and
            updates the corresponding InstrumentingCacheStatsTracker,
            and starts recording the load time starting at this instant.
            If no load event occurs, the current time will be recorded
            as the time it took for a cache miss
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `recordMissMatch` in
                interface `CacheStatsTracker.CacheRequest`

        []{#recordLoadSuccess()}

        -   #### recordLoadSuccess

            ``` methodSignature
            public void recordLoadSuccess()
            ```

            ::: block
            Records that a cache load was successful and updates the
            corresponding InstrumentingCacheStatsTracker, and records
            the time it took to load the object and updates the total
            time spent on a cache miss
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `recordLoadSuccess` in
                interface `CacheStatsTracker.CacheRequest`

        []{#recordLoadFail()}

        -   #### recordLoadFail

            ``` methodSignature
            public void recordLoadFail()
            ```

            ::: block
            Records that a cache load has failed and updates the
            corresponding InstrumentingCacheStatsTracker, and records
            the time spent on a cache miss
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `recordLoadFail` in
                interface `CacheStatsTracker.CacheRequest`
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
