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
-   Method

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

## Interface WorkAdvanceEvent {#interface-workadvanceevent .title title="Interface WorkAdvanceEvent"}
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
        `ActionGraphEvent.Started`, `AnnotationProcessingEvent`,
        `AnnotationProcessingEvent.Finished`,
        `AnnotationProcessingEvent.Started`, `ArtifactCompressionEvent`,
        `ArtifactCompressionEvent.Finished`,
        `ArtifactCompressionEvent.Started`, `BuildEvent`,
        `BuildEvent.BuildReport`, `BuildEvent.Finished`,
        `BuildEvent.RuleCountCalculated`, `BuildEvent.Started`,
        `BuildEvent.UnskippedRuleCountUpdated`, `BuildRuleEvent`,
        `BuildRuleEvent.BeginningBuildRuleEvent`,
        `BuildRuleEvent.EndingBuildRuleEvent`,
        `BuildRuleEvent.Finished`, `BuildRuleEvent.FinishedRuleKeyCalc`,
        `BuildRuleEvent.Resumed`, `BuildRuleEvent.Started`,
        `BuildRuleEvent.StartedRuleKeyCalc`, `BuildRuleEvent.Suspended`,
        `BuildRuleEvent.WillBuildLocally`, `CasBlobDownloadEvent`,
        `CasBlobDownloadEvent.Finished`, `CasBlobDownloadEvent.Started`,
        `CasBlobUploadEvent`, `CasBlobUploadEvent.Finished`,
        `CasBlobUploadEvent.Started`, `CommandEvent`,
        `CommandEvent.Finished`, `CommandEvent.Interrupted`,
        `CommandEvent.Started`, `CompilerPluginDurationEvent`,
        `CompilerPluginDurationEvent.Finished`,
        `CompilerPluginDurationEvent.Started`, `DownloadEvent`,
        `DownloadEvent.Finished`, `DownloadEvent.Started`,
        `DownloadProgressEvent`, `ExternalTestRunEvent`,
        `ExternalTestRunEvent.Finished`, `ExternalTestRunEvent.Started`,
        `ExternalTestSpecCalculationEvent`,
        `ExternalTestSpecCalculationEvent.Finished`,
        `ExternalTestSpecCalculationEvent.Started`,
        `IndividualTestEvent`, `IndividualTestEvent.Finished`,
        `IndividualTestEvent.Started`, `InstallEvent`,
        `InstallEvent.Finished`, `InstallEvent.Started`,
        `JavacPhaseEvent`, `JavacPhaseEvent.Finished`,
        `JavacPhaseEvent.Started`, `ParseBuckFileEvent`,
        `ParseBuckFileEvent.Finished`, `ParseBuckFileEvent.Started`,
        `ParseEvent`, `ParseEvent.Finished`, `ParseEvent.Started`,
        `ProjectBuildFileParseEvents`,
        `ProjectBuildFileParseEvents.Finished`,
        `ProjectBuildFileParseEvents.Started`, `ProjectGenerationEvent`,
        `ProjectGenerationEvent.Finished`,
        `ProjectGenerationEvent.Processed`,
        `ProjectGenerationEvent.Started`, `RemoteExecutionActionEvent`,
        `RemoteExecutionActionEvent.Finished`,
        `RemoteExecutionActionEvent.InputsUploaded`,
        `RemoteExecutionActionEvent.Scheduled`,
        `RemoteExecutionActionEvent.Started`,
        `RemoteExecutionActionEvent.Terminal`,
        `RemoteExecutionSessionEvent`,
        `RemoteExecutionSessionEvent.Finished`,
        `RemoteExecutionSessionEvent.Started`,
        `RuleKeyCalculationEvent.DefaultFinished`,
        `RuleKeyCalculationEvent.DefaultStarted`,
        `RuleKeyCalculationEvent.Event`, `StartActivityEvent`,
        `StartActivityEvent.Finished`, `StartActivityEvent.Started`,
        `StepEvent`, `StepEvent.Finished`, `StepEvent.Started`,
        `TestRuleEvent`, `TestRuleEvent.Finished`,
        `TestRuleEvent.Started`, `TestRunEvent`,
        `TestRunEvent.Finished`, `TestRunEvent.Started`,
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

        public interface WorkAdvanceEvent
        extends BuckEvent

    ::: block
    Interface for events that are only sent out after there was some
    work done towards completing the current command. Absence of those
    events can be used to detect a possible deadlock.
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
-   Method

</div>

[]{#skip.navbar.bottom}
:::
