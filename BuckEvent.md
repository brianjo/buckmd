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

## Interface BuckEvent {#interface-buckevent .title title="Interface BuckEvent"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `BuckEventExternalInterface`

    ```{=html}
    <!-- -->
    ```

    All Known Subinterfaces:
    :   `BuildRuleExecutionEvent`, `LeafEvent`,
        `RuleKeyCalculationEvent`, `RuleKeyCalculationEvent.Finished`,
        `RuleKeyCalculationEvent.Started`, `SimplePerfEvent.Started`,
        `WorkAdvanceEvent`

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

        public interface BuckEvent
        extends BuckEventExternalInterface
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

          Modifier and Type   Method                                                                                                                                    Description
          ------------------- ----------------------------------------------------------------------------------------------------------------------------------------- -------------
          `void`              `configure​(long timestamp,          long nanoTime,          long threadUserNanoTime,          long threadId,          BuildId buildId)`    
          `BuildId`           `getBuildId()`                                                                                                                             
          `EventKey`          `getEventKey()`                                                                                                                            
          `long`              `getNanoTime()`                                                                                                                            
          `long`              `getThreadId()`                                                                                                                            
          `long`              `getThreadUserNanoTime()`                                                                                                                  
          `boolean`           `isConfigured()`                                                                                                                           
          `boolean`           `isRelatedTo​(BuckEvent event)`                                                                                                             
          `String`            `toLogMessage()`                                                                                                                           

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Methods inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `getEventName, getTimestampMillis, storeLastInstanceAndReplayForNewClients`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#configure(long,long,long,long,com.facebook.buck.core.model.BuildId)}

        -   #### configure

            ``` methodSignature
            void configure​(long timestamp,
                           long nanoTime,
                           long threadUserNanoTime,
                           long threadId,
                           BuildId buildId)
            ```

        []{#isConfigured()}

        -   #### isConfigured

            ``` methodSignature
            boolean isConfigured()
            ```

        []{#getNanoTime()}

        -   #### getNanoTime

            ``` methodSignature
            long getNanoTime()
            ```

        []{#getThreadUserNanoTime()}

        -   #### getThreadUserNanoTime

            ``` methodSignature
            long getThreadUserNanoTime()
            ```

        []{#toLogMessage()}

        -   #### toLogMessage

            ``` methodSignature
            String toLogMessage()
            ```

        []{#getThreadId()}

        -   #### getThreadId

            ``` methodSignature
            long getThreadId()
            ```

        []{#getBuildId()}

        -   #### getBuildId

            ``` methodSignature
            BuildId getBuildId()
            ```

            [Returns:]{.returnLabel}
            :   an identifier that distinguishes the build with which
                this event is associated.

        []{#isRelatedTo(com.facebook.buck.event.BuckEvent)}

        -   #### isRelatedTo

            ``` methodSignature
            boolean isRelatedTo​(BuckEvent event)
            ```

            [Returns:]{.returnLabel}

            :   Whether or not this event is related to another event.
                Events are related if they pertain to the same event,
                for example if they are measuring the start and stop of
                some phase. For example,

                       
                        (CommandEvent.started("build")).isRelatedTo(CommandEvent.finished("build")) == true
                        (CommandEvent.started("build")).isRelatedTo(CommandEvent.started("build")) == true
                        (CommandEvent.started("build")).isRelatedTo(CommandEvent.finished("install")) == false
                       
                     

        []{#getEventKey()}

        -   #### getEventKey

            ``` methodSignature
            EventKey getEventKey()
            ```

            [Returns:]{.returnLabel}
            :   key used to determine whether this event is related to
                another event.
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
