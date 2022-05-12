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

## Interface CacheStatsTracker.CacheRequest {#interface-cachestatstracker.cacherequest .title title="Interface CacheStatsTracker.CacheRequest"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `InstrumentingCacheStatsTracker.TrackingCacheRequest`,
        `NoOpCacheStatsTracker.NoOpCacheRequest`

    ```{=html}
    <!-- -->
    ```

    Enclosing interface:
    :   [CacheStatsTracker](CacheStatsTracker.html "interface in com.facebook.buck.util.cache")

    ------------------------------------------------------------------------

        public static interface CacheStatsTracker.CacheRequest

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
        |                       |                       | CacheStatsTracker,    |
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
        |                       |                       | CacheStatsTracker,    |
        |                       |                       | and records the time  |
        |                       |                       | spent on a cache miss |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `recordLoadSuccess()` | ::: block             |
        |                       |                       | Records that a cache  |
        |                       |                       | load was successful   |
        |                       |                       | and updates the       |
        |                       |                       | corresponding         |
        |                       |                       | CacheStatsTracker,    |
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
        |                       |                       | CacheStatsTracker,    |
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
        |                       |                       | CacheStatsTracker,    |
        |                       |                       | and starts recording  |
        |                       |                       | the load time         |
        |                       |                       | starting at this      |
        |                       |                       | instant.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

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

        []{#recordHit()}

        -   #### recordHit

            ``` methodSignature
            void recordHit()
            ```

            ::: block
            Records that a cache hit has occurred and updates the
            corresponding CacheStatsTracker, and records the time it
            took for the cache retrieval
            :::

        []{#recordMiss()}

        -   #### recordMiss

            ``` methodSignature
            void recordMiss()
            ```

            ::: block
            Records that a cache miss has occurred and updates the
            corresponding CacheStatsTracker, and starts recording the
            load time starting at this instant. If no load event occurs,
            the current time will be recorded as the time it took for a
            cache miss
            :::

        []{#recordMissMatch()}

        -   #### recordMissMatch

            ``` methodSignature
            void recordMissMatch()
            ```

            ::: block
            Records that a cache miss due to mismatch has occurred and
            updates the corresponding CacheStatsTracker, and starts
            recording the load time starting at this instant. If no load
            event occurs, the current time will be recorded as the time
            it took for a cache miss
            :::

        []{#recordLoadSuccess()}

        -   #### recordLoadSuccess

            ``` methodSignature
            void recordLoadSuccess()
            ```

            ::: block
            Records that a cache load was successful and updates the
            corresponding CacheStatsTracker, and records the time it
            took to load the object and updates the total time spent on
            a cache miss
            :::

        []{#recordLoadFail()}

        -   #### recordLoadFail

            ``` methodSignature
            void recordLoadFail()
            ```

            ::: block
            Records that a cache load has failed and updates the
            corresponding CacheStatsTracker, and records the time spent
            on a cache miss
            :::
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
