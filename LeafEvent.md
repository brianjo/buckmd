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
-   [Field](#field.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.event](package-summary.html)
:::

## Interface LeafEvent {#interface-leafevent .title title="Interface LeafEvent"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `BuckEvent`, `BuckEventExternalInterface`

    ```{=html}
    <!-- -->
    ```

    All Known Subinterfaces:
    :   `RuleKeyCalculationEvent`, `RuleKeyCalculationEvent.Finished`,
        `RuleKeyCalculationEvent.Started`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `ActionGraphEvent`, `ActionGraphEvent.Cache`,
        `ActionGraphEvent.Cache.Hit`, `ActionGraphEvent.Cache.Miss`,
        `ActionGraphEvent.Cache.MissWithEmptyCache`,
        `ActionGraphEvent.Cache.MissWithTargetGraphDifference`,
        `ActionGraphEvent.Cache.MissWithTargetGraphHashMatch`,
        `ActionGraphEvent.Finished`, `ActionGraphEvent.IncrementalLoad`,
        `ActionGraphEvent.Started`, `ArtifactCacheConnectEvent`,
        `ArtifactCacheConnectEvent.Finished`,
        `ArtifactCacheConnectEvent.Started`, `ArtifactCacheEvent`,
        `ArtifactCacheEvent.Finished`, `ArtifactCacheEvent.Started`,
        `ArtifactCompressionEvent`, `ArtifactCompressionEvent.Finished`,
        `ArtifactCompressionEvent.Started`,
        `BuildRuleEvent.FinishedRuleKeyCalc`,
        `BuildRuleEvent.StartedRuleKeyCalc`,
        `DirArtifactCacheEvent.Finished`,
        `DirArtifactCacheEvent.Started`, `FileHashCacheEvent`,
        `FileHashCacheEvent.InvalidationFinished`,
        `FileHashCacheEvent.InvalidationStarted`,
        `HttpArtifactCacheEvent`, `HttpArtifactCacheEvent.Finished`,
        `HttpArtifactCacheEvent.Scheduled`,
        `HttpArtifactCacheEvent.Started`, `InstallEvent`,
        `InstallEvent.Finished`, `InstallEvent.Started`,
        `LeafEvents.SimpleLeafEvent`,
        `LeafEvents.SimpleLeafEvent.Finished`,
        `LeafEvents.SimpleLeafEvent.Started`, `ParseEvent`,
        `ParseEvent.Finished`, `ParseEvent.Started`,
        `ProjectBuildFileParseEvents`,
        `ProjectBuildFileParseEvents.Finished`,
        `ProjectBuildFileParseEvents.Started`,
        `RuleKeyCalculationEvent.DefaultFinished`,
        `RuleKeyCalculationEvent.DefaultStarted`,
        `RuleKeyCalculationEvent.Event`,
        `SQLiteArtifactCacheEvent.Finished`,
        `SQLiteArtifactCacheEvent.Started`, `StartActivityEvent`,
        `StartActivityEvent.Finished`, `StartActivityEvent.Started`,
        `StepEvent`, `StepEvent.Finished`, `StepEvent.Started`,
        `TestStatusMessageEvent`, `TestStatusMessageEvent.Finished`,
        `TestStatusMessageEvent.Started`, `TestSummaryEvent`,
        `TestSummaryEvent.Finished`, `TestSummaryEvent.Started`,
        `UninstallEvent`, `UninstallEvent.Finished`,
        `UninstallEvent.Started`, `VersionedTargetGraphEvent`,
        `VersionedTargetGraphEvent.Cache`,
        `VersionedTargetGraphEvent.Cache.Hit`,
        `VersionedTargetGraphEvent.Cache.Miss`,
        `VersionedTargetGraphEvent.Finished`,
        `VersionedTargetGraphEvent.Started`,
        `VersionedTargetGraphEvent.Timeout`

    ------------------------------------------------------------------------

        public interface LeafEvent
        extends BuckEvent

    ::: block
    LeafEvents represent events that have no logical children and are
    useful for tracking the time buck is spending logically grouped by
    categories, such as Parse, Javac, or Dx. An example of something
    that wouldn\'t be a good candidate for a LeafEvent would be a
    RuleEvent since we\'re not spending an appreciable amount of time in
    the rules but in the steps instead.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Fields inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `BUILD_FINISHED, BUILD_REPORT, BUILD_STARTED, BUILD_STATUS_EVENT, CACHE_RATE_STATS_UPDATE_EVENT, INDIVIDUAL_TEST_AWAITING_RESULTS, INSTALL_STARTED, PARSE_FINISHED, PARSE_STARTED, PROJECT_GENERATION_FINISHED, PROJECT_GENERATION_STARTED, TEST_RUN_STARTED`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method            Description
          ------------------- ----------------- -------------
          `String`            `getCategory()`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.event.BuckEvent}

            ### Methods inherited from interface com.facebook.buck.event.[BuckEvent](BuckEvent.html "interface in com.facebook.buck.event")

            `configure, getBuildId, getEventKey, getNanoTime, getThreadId, getThreadUserNanoTime, isConfigured, isRelatedTo, toLogMessage`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Methods inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `getEventName, getTimestampMillis, storeLastInstanceAndReplayForNewClients`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getCategory()}

        -   #### getCategory

            ``` methodSignature
            String getCategory()
            ```

            [Returns:]{.returnLabel}
            :   The category time spent in this event should be
                accounted under.
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
-   [Field](#field.summary) \| 
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
