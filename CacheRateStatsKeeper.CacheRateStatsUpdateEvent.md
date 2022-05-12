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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
-   [Field](#field.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.event.listener.stats.cache](package-summary.html)
:::

## Class CacheRateStatsKeeper.CacheRateStatsUpdateEvent {#class-cacheratestatskeeper.cacheratestatsupdateevent .title title="Class CacheRateStatsKeeper.CacheRateStatsUpdateEvent"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.event.AbstractBuckEvent](../../../AbstractBuckEvent.html "class in com.facebook.buck.event")

    -   -   com.facebook.buck.event.listener.stats.cache.CacheRateStatsKeeper.CacheRateStatsUpdateEvent

::: description
-   

    All Implemented Interfaces:
    :   `BuckEvent`, `BuckEventExternalInterface`,
        `CacheRateStatsUpdateExternalEventInterface`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [CacheRateStatsKeeper](CacheRateStatsKeeper.html "class in com.facebook.buck.event.listener.stats.cache")

    ------------------------------------------------------------------------

        public static class CacheRateStatsKeeper.CacheRateStatsUpdateEvent
        extends AbstractBuckEvent
        implements CacheRateStatsUpdateExternalEventInterface
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Fields inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](../../../external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `BUILD_FINISHED, BUILD_REPORT, BUILD_STARTED, BUILD_STATUS_EVENT, CACHE_RATE_STATS_UPDATE_EVENT, INDIVIDUAL_TEST_AWAITING_RESULTS, INSTALL_STARTED, PARSE_FINISHED, PARSE_STARTED, PROJECT_GENERATION_FINISHED, PROJECT_GENERATION_STARTED, TEST_RUN_STARTED`

        ```{=html}
        <!-- -->
        ```
        -   []{#fields.inherited.from.class.com.facebook.buck.event.external.events.CacheRateStatsUpdateExternalEventInterface}

            ### Fields inherited from interface com.facebook.buck.event.external.events.[CacheRateStatsUpdateExternalEventInterface](../../../external/events/CacheRateStatsUpdateExternalEventInterface.html "interface in com.facebook.buck.event.external.events")

            `EVENT_NAME`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                               Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `CacheRateStatsUpdateEvent​(int cacheMissCount,                          int cacheErrorCount,                          int cacheHitCount,                          int ruleCount,                          int updated)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type    Method                     Description
          -------------------- -------------------------- -------------
          `int`                `getCacheErrorCount()`      
          `double`             `getCacheErrorRate()`       
          `int`                `getCacheHitCount()`        
          `int`                `getCacheMissCount()`       
          `double`             `getCacheMissRate()`        
          `String`             `getEventName()`            
          `int`                `getTotalRulesCount()`      
          `int`                `getUpdatedRulesCount()`    
          `protected String`   `getValueString()`          

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.event.AbstractBuckEvent}

            ### Methods inherited from class com.facebook.buck.event.[AbstractBuckEvent](../../../AbstractBuckEvent.html "class in com.facebook.buck.event")

            `configure, equals, getBuildId, getEventKey, getNanoTime, getThreadId, getThreadUserNanoTime, getTimestampMillis, hashCode, isConfigured, isRelatedTo, toLogMessage, toString`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Methods inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](../../../external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `getTimestampMillis, storeLastInstanceAndReplayForNewClients`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(int,int,int,int,int)}

        -   #### CacheRateStatsUpdateEvent

                public CacheRateStatsUpdateEvent​(int cacheMissCount,
                                                 int cacheErrorCount,
                                                 int cacheHitCount,
                                                 int ruleCount,
                                                 int updated)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getValueString()}

        -   #### getValueString

            ``` methodSignature
            protected String getValueString()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getValueString` in class `AbstractBuckEvent`

        []{#getCacheMissCount()}

        -   #### getCacheMissCount

            ``` methodSignature
            public int getCacheMissCount()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCacheMissCount` in
                interface `CacheRateStatsUpdateExternalEventInterface`

            [Returns:]{.returnLabel}
            :   number of cache misses.

        []{#getCacheErrorCount()}

        -   #### getCacheErrorCount

            ``` methodSignature
            public int getCacheErrorCount()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCacheErrorCount` in
                interface `CacheRateStatsUpdateExternalEventInterface`

            [Returns:]{.returnLabel}
            :   number of cache errors.

        []{#getCacheMissRate()}

        -   #### getCacheMissRate

            ``` methodSignature
            public double getCacheMissRate()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCacheMissRate` in
                interface `CacheRateStatsUpdateExternalEventInterface`

            [Returns:]{.returnLabel}
            :   cache miss rate, in percent, as displayed on the buck
                console.

        []{#getCacheErrorRate()}

        -   #### getCacheErrorRate

            ``` methodSignature
            public double getCacheErrorRate()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCacheErrorRate` in
                interface `CacheRateStatsUpdateExternalEventInterface`

            [Returns:]{.returnLabel}
            :   cache error rate, in percent, as displayed on the buck
                console.

        []{#getCacheHitCount()}

        -   #### getCacheHitCount

            ``` methodSignature
            public int getCacheHitCount()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCacheHitCount` in
                interface `CacheRateStatsUpdateExternalEventInterface`

            [Returns:]{.returnLabel}
            :   number of cache hits. This excludes
                [`CacheResultType.IGNORED`](../../../../artifact_cache/CacheResultType.html#IGNORED)
                and
                [`CacheResultType.LOCAL_KEY_UNCHANGED_HIT`](../../../../artifact_cache/CacheResultType.html#LOCAL_KEY_UNCHANGED_HIT)
                result types.

        []{#getUpdatedRulesCount()}

        -   #### getUpdatedRulesCount

            ``` methodSignature
            public int getUpdatedRulesCount()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getUpdatedRulesCount` in
                interface `CacheRateStatsUpdateExternalEventInterface`

            [Returns:]{.returnLabel}
            :   number of rules that have been processed.

        []{#getTotalRulesCount()}

        -   #### getTotalRulesCount

            ``` methodSignature
            public int getTotalRulesCount()
            ```

        []{#getEventName()}

        -   #### getEventName

            ``` methodSignature
            public String getEventName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getEventName` in interface `BuckEventExternalInterface`

            [Returns:]{.returnLabel}
            :   the type of the event.
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   Nested \| 
-   [Field](#field.summary) \| 
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
