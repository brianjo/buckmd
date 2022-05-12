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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.event.external.events](package-summary.html)
:::

## Interface CacheRateStatsUpdateExternalEventInterface {#interface-cacheratestatsupdateexternaleventinterface .title title="Interface CacheRateStatsUpdateExternalEventInterface"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `BuckEventExternalInterface`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `CacheRateStatsKeeper.CacheRateStatsUpdateEvent`

    ------------------------------------------------------------------------

        public interface CacheRateStatsUpdateExternalEventInterface
        extends BuckEventExternalInterface

    ::: block
    Sent to update the WebSocket clients about cache misses and errors.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field          Description
          ------------------- -------------- -------------
          `static String`     `EVENT_NAME`    

          : Fields[ ]{.tabEnd}

        -   []{#fields.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Fields inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `BUILD_FINISHED, BUILD_REPORT, BUILD_STARTED, BUILD_STATUS_EVENT, CACHE_RATE_STATS_UPDATE_EVENT, INDIVIDUAL_TEST_AWAITING_RESULTS, INSTALL_STARTED, PARSE_FINISHED, PARSE_STARTED, PROJECT_GENERATION_FINISHED, PROJECT_GENERATION_STARTED, TEST_RUN_STARTED`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                     Description
          ------------------- -------------------------- -------------
          `int`               `getCacheErrorCount()`      
          `double`            `getCacheErrorRate()`       
          `int`               `getCacheHitCount()`        
          `int`               `getCacheMissCount()`       
          `double`            `getCacheMissRate()`        
          `int`               `getUpdatedRulesCount()`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Methods inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `getEventName, getTimestampMillis, storeLastInstanceAndReplayForNewClients`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#EVENT_NAME}

        -   #### EVENT_NAME

                static final String EVENT_NAME

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.event.external.events.CacheRateStatsUpdateExternalEventInterface.EVENT_NAME)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getCacheMissCount()}

        -   #### getCacheMissCount

            ``` methodSignature
            int getCacheMissCount()
            ```

            [Returns:]{.returnLabel}
            :   number of cache misses.

        []{#getCacheErrorCount()}

        -   #### getCacheErrorCount

            ``` methodSignature
            int getCacheErrorCount()
            ```

            [Returns:]{.returnLabel}
            :   number of cache errors.

        []{#getCacheMissRate()}

        -   #### getCacheMissRate

            ``` methodSignature
            double getCacheMissRate()
            ```

            [Returns:]{.returnLabel}
            :   cache miss rate, in percent, as displayed on the buck
                console.

        []{#getCacheErrorRate()}

        -   #### getCacheErrorRate

            ``` methodSignature
            double getCacheErrorRate()
            ```

            [Returns:]{.returnLabel}
            :   cache error rate, in percent, as displayed on the buck
                console.

        []{#getCacheHitCount()}

        -   #### getCacheHitCount

            ``` methodSignature
            int getCacheHitCount()
            ```

            [Returns:]{.returnLabel}
            :   number of cache hits. This excludes
                [`CacheResultType.IGNORED`](../../../artifact_cache/CacheResultType.html#IGNORED)
                and
                [`CacheResultType.LOCAL_KEY_UNCHANGED_HIT`](../../../artifact_cache/CacheResultType.html#LOCAL_KEY_UNCHANGED_HIT)
                result types.

        []{#getUpdatedRulesCount()}

        -   #### getUpdatedRulesCount

            ``` methodSignature
            int getUpdatedRulesCount()
            ```

            [Returns:]{.returnLabel}
            :   number of rules that have been processed.
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   Nested \| 
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
