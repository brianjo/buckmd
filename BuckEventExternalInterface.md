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

## Interface BuckEventExternalInterface {#interface-buckeventexternalinterface .title title="Interface BuckEventExternalInterface"}
:::

::: contentContainer
::: description
-   

    All Known Subinterfaces:
    :   `BuckEvent`, `BuildRuleExecutionEvent`,
        `CacheRateStatsUpdateExternalEventInterface`,
        `CompilerErrorEventExternalInterface`,
        `ConsoleEventExternalInterface`,
        `IndividualTestEventFinishedExternalInterface<T>`,
        `InstallFinishedEventExternalInterface`, `LeafEvent`,
        `ProgressEventInterface`, `RuleKeyCalculationEvent`,
        `RuleKeyCalculationEvent.Finished`,
        `RuleKeyCalculationEvent.Started`, `SimplePerfEvent.Started`,
        `StepEventExternalInterface`,
        `TestRunFinishedEventInterface<T>`, `WorkAdvanceEvent`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AbstractBuckEvent`, `ActionGraphEvent`,
        `ActionGraphEvent.Cache`, `ActionGraphEvent.Cache.Hit`,
        `ActionGraphEvent.Cache.Miss`,
        `ActionGraphEvent.Cache.MissWithEmptyCache`,
        `ActionGraphEvent.Cache.MissWithTargetGraphDifference`,
        `ActionGraphEvent.Cache.MissWithTargetGraphHashMatch`,
        `ActionGraphEvent.Finished`, `ActionGraphEvent.IncrementalLoad`,
        `ActionGraphEvent.Started`, `ActionGraphPerfStatEvent`,
        `AnnotationProcessingEvent`,
        `AnnotationProcessingEvent.Finished`,
        `AnnotationProcessingEvent.Started`,
        `ArtifactCacheConnectEvent`,
        `ArtifactCacheConnectEvent.Finished`,
        `ArtifactCacheConnectEvent.Started`, `ArtifactCacheEvent`,
        `ArtifactCacheEvent.Finished`, `ArtifactCacheEvent.Started`,
        `ArtifactCompressionEvent`, `ArtifactCompressionEvent.Finished`,
        `ArtifactCompressionEvent.Started`,
        `BuckInitializationDurationEvent`, `BuildEvent`,
        `BuildEvent.BuildReport`, `BuildEvent.Finished`,
        `BuildEvent.RuleCountCalculated`, `BuildEvent.Started`,
        `BuildEvent.UnskippedRuleCountUpdated`, `BuildRuleEvent`,
        `BuildRuleEvent.BeginningBuildRuleEvent`,
        `BuildRuleEvent.EndingBuildRuleEvent`,
        `BuildRuleEvent.Finished`, `BuildRuleEvent.FinishedRuleKeyCalc`,
        `BuildRuleEvent.Resumed`, `BuildRuleEvent.Started`,
        `BuildRuleEvent.StartedRuleKeyCalc`, `BuildRuleEvent.Suspended`,
        `BuildRuleEvent.WillBuildLocally`,
        `BuildRuleExecutionEvent.Event`,
        `BuildRuleExecutionEvent.Finished`,
        `BuildRuleExecutionEvent.Started`, `CacheCountersSummaryEvent`,
        `CacheRateStatsKeeper.CacheRateStatsUpdateEvent`,
        `CacheStatsEvent`, `CasBlobDownloadEvent`,
        `CasBlobDownloadEvent.Finished`, `CasBlobDownloadEvent.Started`,
        `CasBlobUploadEvent`, `CasBlobUploadEvent.Finished`,
        `CasBlobUploadEvent.Started`, `CommandEvent`,
        `CommandEvent.Finished`, `CommandEvent.Interrupted`,
        `CommandEvent.Started`, `CompilerErrorEvent`,
        `CompilerPluginDurationEvent`,
        `CompilerPluginDurationEvent.Finished`,
        `CompilerPluginDurationEvent.Started`, `ConsoleEvent`,
        `CounterRegistry.AsyncCounterRegistrationEvent`,
        `CountersSnapshotEvent`, `DaemonEvent`,
        `DaemonEvent.NewDaemonInstance`,
        `DirArtifactCacheEvent.Finished`,
        `DirArtifactCacheEvent.Started`, `DownloadEvent`,
        `DownloadEvent.Finished`, `DownloadEvent.Started`,
        `DownloadProgressEvent`, `ExperimentEvent`,
        `ExternalTestRunEvent`, `ExternalTestRunEvent.Finished`,
        `ExternalTestRunEvent.Started`,
        `ExternalTestSpecCalculationEvent`,
        `ExternalTestSpecCalculationEvent.Finished`,
        `ExternalTestSpecCalculationEvent.Started`,
        `FastVersionControlStatsEvent`, `FileHashCacheEvent`,
        `FileHashCacheEvent.InvalidationFinished`,
        `FileHashCacheEvent.InvalidationStarted`,
        `FinalizingBuildRuleEvent`, `FlushConsoleEvent`,
        `GCCollectionEvent`, `GCMajorCollectionEvent`,
        `GCMinorCollectionEvent`, `HttpArtifactCacheEvent`,
        `HttpArtifactCacheEvent.Finished`,
        `HttpArtifactCacheEvent.Scheduled`,
        `HttpArtifactCacheEvent.Shutdown`,
        `HttpArtifactCacheEvent.Started`, `HybridLocalEvent`,
        `HybridLocalEvent.Stolen`, `IndividualTestEvent`,
        `IndividualTestEvent.Finished`, `IndividualTestEvent.Started`,
        `InstallEvent`, `InstallEvent.Finished`, `InstallEvent.Started`,
        `JavacPhaseEvent`, `JavacPhaseEvent.Finished`,
        `JavacPhaseEvent.Started`, `LeafEvents.SimpleLeafEvent`,
        `LeafEvents.SimpleLeafEvent.Finished`,
        `LeafEvents.SimpleLeafEvent.Started`,
        `LoadBalancedServiceEvent`, `LoadBalancerPingEvent`,
        `LocalFallbackEvent`, `LocalFallbackEvent.Finished`,
        `LocalFallbackEvent.Started`, `NetworkEvent`,
        `NetworkEvent.BytesReceivedEvent`, `NetworkInfo.Event`,
        `ParseBuckFileEvent`, `ParseBuckFileEvent.Finished`,
        `ParseBuckFileEvent.Started`, `ParseBuckProfilerReportEvent`,
        `ParseEvent`, `ParseEvent.Finished`, `ParseEvent.Started`,
        `ParsingEvent`, `ParsingEvent.EnvVariableChange`,
        `ParsingEvent.SymlinkInvalidation`,
        `PerfStatsTracking.MemoryPerfStatsEvent`,
        `PerfStatsTracking.PerfStatsEvent`,
        `PerfTimesEventListener.PerfTimesEvent`,
        `ProcessTracker.ProcessResourceConsumptionEvent`,
        `ProgressEvent`, `ProgressEvent.BuildProgressUpdated`,
        `ProgressEvent.ParsingProgressUpdated`,
        `ProgressEvent.ProjectGenerationProgressUpdated`,
        `ProjectBuildFileParseEvents`,
        `ProjectBuildFileParseEvents.Finished`,
        `ProjectBuildFileParseEvents.Started`, `ProjectGenerationEvent`,
        `ProjectGenerationEvent.Finished`,
        `ProjectGenerationEvent.Processed`,
        `ProjectGenerationEvent.Started`,
        `RemoteBuildRuleExecutionEvent`, `RemoteExecutionActionEvent`,
        `RemoteExecutionActionEvent.Finished`,
        `RemoteExecutionActionEvent.InputsUploaded`,
        `RemoteExecutionActionEvent.Scheduled`,
        `RemoteExecutionActionEvent.Started`,
        `RemoteExecutionActionEvent.Terminal`,
        `RemoteExecutionSessionEvent`,
        `RemoteExecutionSessionEvent.Finished`,
        `RemoteExecutionSessionEvent.Started`,
        `RuleKeyCacheResultEvent`,
        `RuleKeyCalculationEvent.DefaultFinished`,
        `RuleKeyCalculationEvent.DefaultStarted`,
        `RuleKeyCalculationEvent.Event`, `ServerHealthManagerEvent`,
        `SimplePerfEvent`, `SimplePerfEvent.Finished`,
        `SQLiteArtifactCacheEvent.Finished`,
        `SQLiteArtifactCacheEvent.Started`, `StartActivityEvent`,
        `StartActivityEvent.Finished`, `StartActivityEvent.Started`,
        `StepEvent`, `StepEvent.Finished`, `StepEvent.Started`,
        `TestRuleEvent`, `TestRuleEvent.Finished`,
        `TestRuleEvent.Started`, `TestRunEvent`,
        `TestRunEvent.Finished`, `TestRunEvent.Started`,
        `TestStatusMessageEvent`, `TestStatusMessageEvent.Finished`,
        `TestStatusMessageEvent.Started`, `TestSummaryEvent`,
        `TestSummaryEvent.Finished`, `TestSummaryEvent.Started`,
        `ThrowableConsoleEvent`, `UninstallEvent`,
        `UninstallEvent.Finished`, `UninstallEvent.Started`,
        `VersionControlStatsEvent`, `VersionedTargetGraphEvent`,
        `VersionedTargetGraphEvent.Cache`,
        `VersionedTargetGraphEvent.Cache.Hit`,
        `VersionedTargetGraphEvent.Cache.Miss`,
        `VersionedTargetGraphEvent.Finished`,
        `VersionedTargetGraphEvent.Started`,
        `VersionedTargetGraphEvent.Timeout`, `WatchmanDiagnosticEvent`,
        `WatchmanStatusEvent`, `WatchmanStatusEvent.FileCreation`,
        `WatchmanStatusEvent.FileDeletion`,
        `WatchmanStatusEvent.Finished`, `WatchmanStatusEvent.Overflow`,
        `WatchmanStatusEvent.Started`,
        `WatchmanStatusEvent.ZeroFileChanges`

    ------------------------------------------------------------------------

        public interface BuckEventExternalInterface

    ::: block
    Describes a generic buck event. This type is intended to be used by
    external applications (like the Intellij Buck plugin) to deserialize
    events coming from the webserver.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                                Description
          ------------------- ------------------------------------ -------------
          `static String`     `BUILD_FINISHED`                      
          `static String`     `BUILD_REPORT`                        
          `static String`     `BUILD_STARTED`                       
          `static String`     `BUILD_STATUS_EVENT`                  
          `static String`     `CACHE_RATE_STATS_UPDATE_EVENT`       
          `static String`     `INDIVIDUAL_TEST_AWAITING_RESULTS`    
          `static String`     `INSTALL_STARTED`                     
          `static String`     `PARSE_FINISHED`                      
          `static String`     `PARSE_STARTED`                       
          `static String`     `PROJECT_GENERATION_FINISHED`         
          `static String`     `PROJECT_GENERATION_STARTED`          
          `static String`     `TEST_RUN_STARTED`                    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `String`              | `getEventName()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `                     |                       |
        |                       | getTimestampMillis()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `                     | ::: block             |
        |                       | storeLastInstanceAndR | By default, events    |
        |                       | eplayForNewClients()` | sent to external      |
        |                       |                       | websocket listeners   |
        |                       |                       | are fire-and-forget;  |
        |                       |                       | a client never        |
        |                       |                       | receives past events. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#INDIVIDUAL_TEST_AWAITING_RESULTS}

        -   #### INDIVIDUAL_TEST_AWAITING_RESULTS

                static final String INDIVIDUAL_TEST_AWAITING_RESULTS

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.event.external.events.BuckEventExternalInterface.INDIVIDUAL_TEST_AWAITING_RESULTS)

        []{#TEST_RUN_STARTED}

        -   #### TEST_RUN_STARTED

                static final String TEST_RUN_STARTED

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.event.external.events.BuckEventExternalInterface.TEST_RUN_STARTED)

        []{#INSTALL_STARTED}

        -   #### INSTALL_STARTED

                static final String INSTALL_STARTED

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.event.external.events.BuckEventExternalInterface.INSTALL_STARTED)

        []{#BUILD_STARTED}

        -   #### BUILD_STARTED

                static final String BUILD_STARTED

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.event.external.events.BuckEventExternalInterface.BUILD_STARTED)

        []{#BUILD_FINISHED}

        -   #### BUILD_FINISHED

                static final String BUILD_FINISHED

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.event.external.events.BuckEventExternalInterface.BUILD_FINISHED)

        []{#BUILD_REPORT}

        -   #### BUILD_REPORT

                static final String BUILD_REPORT

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.event.external.events.BuckEventExternalInterface.BUILD_REPORT)

        []{#PARSE_STARTED}

        -   #### PARSE_STARTED

                static final String PARSE_STARTED

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.event.external.events.BuckEventExternalInterface.PARSE_STARTED)

        []{#PARSE_FINISHED}

        -   #### PARSE_FINISHED

                static final String PARSE_FINISHED

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.event.external.events.BuckEventExternalInterface.PARSE_FINISHED)

        []{#PROJECT_GENERATION_STARTED}

        -   #### PROJECT_GENERATION_STARTED

                static final String PROJECT_GENERATION_STARTED

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.event.external.events.BuckEventExternalInterface.PROJECT_GENERATION_STARTED)

        []{#PROJECT_GENERATION_FINISHED}

        -   #### PROJECT_GENERATION_FINISHED

                static final String PROJECT_GENERATION_FINISHED

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.event.external.events.BuckEventExternalInterface.PROJECT_GENERATION_FINISHED)

        []{#CACHE_RATE_STATS_UPDATE_EVENT}

        -   #### CACHE_RATE_STATS_UPDATE_EVENT

                static final String CACHE_RATE_STATS_UPDATE_EVENT

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.event.external.events.BuckEventExternalInterface.CACHE_RATE_STATS_UPDATE_EVENT)

        []{#BUILD_STATUS_EVENT}

        -   #### BUILD_STATUS_EVENT

                static final String BUILD_STATUS_EVENT

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.event.external.events.BuckEventExternalInterface.BUILD_STATUS_EVENT)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getTimestampMillis()}

        -   #### getTimestampMillis

            ``` methodSignature
            long getTimestampMillis()
            ```

            [Returns:]{.returnLabel}
            :   the time at which the event has been created, in
                milliseconds.

        []{#getEventName()}

        -   #### getEventName

            ``` methodSignature
            String getEventName()
            ```

            [Returns:]{.returnLabel}
            :   the type of the event.

        []{#storeLastInstanceAndReplayForNewClients()}

        -   #### storeLastInstanceAndReplayForNewClients

            ``` methodSignature
            default boolean storeLastInstanceAndReplayForNewClients()
            ```

            ::: block
            By default, events sent to external websocket listeners are
            fire-and-forget; a client never receives past events.
            However events may opt in to a behavior where the last
            instance of the event is stored and sent to new clients as
            they connect. This is useful for \"snapshot\" events which
            provide information about an ongoing event.
            Note that this does not replay multiple instances of an
            event. Only the last instance will be sent to new clients.
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
