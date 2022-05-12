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
[Package]{.packageLabelInType} [com.facebook.buck.event.listener](package-summary.html)
:::

## Class SuperConsoleEventBusListener {#class-superconsoleeventbuslistener .title title="Class SuperConsoleEventBusListener"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.event.listener.AbstractConsoleEventBusListener](AbstractConsoleEventBusListener.html "class in com.facebook.buck.event.listener")

    -   -   com.facebook.buck.event.listener.SuperConsoleEventBusListener

::: description
-   

    All Implemented Interfaces:
    :   `BuckEventListener`, `Closeable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class SuperConsoleEventBusListener
        extends AbstractConsoleEventBusListener

    ::: block
    Console that provides rich, updating ansi output about the current
    build.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.event.listener.AbstractConsoleEventBusListener}

            ### Fields inherited from class com.facebook.buck.event.listener.[AbstractConsoleEventBusListener](AbstractConsoleEventBusListener.html "class in com.facebook.buck.event.listener")

            `actionGraphEvents, actionGraphFinished, actionGraphStarted, ansi, buildDetailsCommands, buildFinished, buildRuleThreadTracker, buildStarted, clock, commandFinished, console, installFinished, installStarted, networkStatsTracker, numRulesCompleted, parseStats, progressEstimator, projectGenerationFinished, projectGenerationStarted, publicAnnouncements, ruleCount, UNFINISHED_EVENT_PAIR, verbosity, watchmanFinished, watchmanStarted`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `SuperConsoleEventBusListener​(SuperConsoleConfig config,                             RenderingConsole renderingConsole,                             Clock clock,                             TestResultSummaryVerbosity summaryVerbosity,                             ExecutionEnvironment executionEnvironment,                             Locale locale,                             Path testLogPath,                             long minimumDurationMillisecondsToShowParse,                             long minimumDurationMillisecondsToShowActionGraph,                             long minimumDurationMillisecondsToShowWatchman,                             boolean hideEmptyDownload,                             BuildId buildId,                             boolean printBuildId,                             Optional<String> buildDetailsTemplate,                             com.google.common.collect.ImmutableSet<String> buildDetailsCommands,                             com.google.common.collect.ImmutableList<AdditionalConsoleLineProvider> additionalConsoleLineProviders,                             int maxConcurrentReExecutions)`    
          `SuperConsoleEventBusListener​(SuperConsoleConfig config,                             RenderingConsole renderingConsole,                             Clock clock,                             TestResultSummaryVerbosity summaryVerbosity,                             ExecutionEnvironment executionEnvironment,                             Locale locale,                             Path testLogPath,                             BuildId buildId,                             boolean printBuildId,                             Optional<String> buildDetailsTemplate,                             com.google.common.collect.ImmutableSet<String> buildDetailsCommands,                             com.google.common.collect.ImmutableList<AdditionalConsoleLineProvider> additionalConsoleLineProviders,                             int maxConcurrentReExecutions)`                                                                                                                                                                                                                                                                                               

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `actionGraphC         |                       |
        |                       | acheHit​(ActionGraphEv |                       |
        |                       | ent.Cache.Hit event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `artifactCacheFinis   |                       |
        |                       | hed​(ArtifactCacheEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `artifactCacheSt      | ::: block             |
        |                       | arted​(ArtifactCacheEv | When a new cache      |
        |                       | ent.Started started)` | event is about to     |
        |                       |                       | start.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `artifactC            |                       |
        |                       | ompressionFinished​(Ar |                       |
        |                       | tifactCompressionEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `artifa               |                       |
        |                       | ctCompressionStarted​( |                       |
        |                       | ArtifactCompressionEv |                       |
        |                       | ent.Started started)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `close()`             | ::: block             |
        |                       |                       | Cleanup, output any   |
        |                       |                       | trace data collected  |
        |                       |                       | to the backing store. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `create               | ::: block             |
        | ogle.common.collect.I | RenderLinesAtTime​(lon | Creates a list of     |
        | mmutableList<String>` | g currentTimeMillis)` | lines to be rendered  |
        |                       |                       | at a given time.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `display              |                       |
        |                       | sEstimatedProgress()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `envVariableCha       |                       |
        |                       | nge​(ParsingEvent.EnvV |                       |
        |                       | ariableChange event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `forceRender​(Flus     |                       |
        |                       | hConsoleEvent event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected String`    | `formatElapsedTime    |                       |
        |                       | ​(long elapsedTimeMs)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `logEvent             |                       |
        |                       | ​(ConsoleEvent event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `                     |                       |
        |                       | onActionEventStarted​( |                       |
        |                       | RemoteExecutionAction |                       |
        |                       | Event.Started event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `onActionE            |                       |
        |                       | ventStolen​(HybridLoca |                       |
        |                       | lEvent.Stolen event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `onAc                 |                       |
        |                       | tionEventTerminated​(R |                       |
        |                       | emoteExecutionActionE |                       |
        |                       | vent.Terminal event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `printSevereWarningD  |                       |
        |                       | irectly​(String line)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `rende                | ::: block             |
        |                       | rLinesWithMaybeCompre | Returns the number of |
        |                       | ssion​(MultiStateRende | lines created.        |
        |                       | rer renderer,         | :::                   |
        |                       |                       |                       |
        |                       |    com.google.common. |                       |
        |                       | collect.ImmutableList |                       |
        |                       | .Builder<String> line |                       |
        |                       | s,                    |                       |
        |                       |              int maxL |                       |
        |                       | ines,                 |                       |
        |                       |                 boole |                       |
        |                       | an alwaysSortByTime)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `rend                 | ::: block             |
        |                       | erLinesWithMaybeTrunc | Returns the number of |
        |                       | ation​(int numLinesAlr | lines created.        |
        |                       | eadyRendered,         | :::                   |
        |                       |                       |                       |
        |                       |   MultiStateRenderer  |                       |
        |                       | renderer,             |                       |
        |                       |                    co |                       |
        |                       | m.google.common.colle |                       |
        |                       | ct.ImmutableList.Buil |                       |
        |                       | der<String> lines,    |                       |
        |                       |                       |                       |
        |                       |        int maxLines)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `ruleKey              |                       |
        |                       | CalculationFinished​(R |                       |
        |                       | uleKeyCalculationEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `rule                 |                       |
        |                       | KeyCalculationStarted |                       |
        |                       | ​(RuleKeyCalculationEv |                       |
        |                       | ent.Started started)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `simpleL              |                       |
        |                       | eafEventFinished​(Leaf |                       |
        |                       | Events.SimpleLeafEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `simp                 |                       |
        |                       | leLeafEventStarted​(Le |                       |
        |                       | afEvents.SimpleLeafEv |                       |
        |                       | ent.Started started)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `                     |                       |
        |                       | stepFinished​(StepEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `stepStarted​(StepEv   |                       |
        |                       | ent.Started started)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `symlinkInvalidatio   |                       |
        |                       | n​(ParsingEvent.Symlin |                       |
        |                       | kInvalidation event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `testRu               |                       |
        |                       | nFinished​(TestRunEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `t                    |                       |
        |                       | estRunStarted​(TestRun |                       |
        |                       | Event.Started event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `testS                |                       |
        |                       | tatusMessageFinished​( |                       |
        |                       | TestStatusMessageEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `te                   |                       |
        |                       | stStatusMessageStarte |                       |
        |                       | d​(TestStatusMessageEv |                       |
        |                       | ent.Started started)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `testSummaryFin       |                       |
        |                       | ished​(TestSummaryEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `testSummary          |                       |
        |                       | Started​(TestSummaryEv |                       |
        |                       | ent.Started started)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `watchmanFileCreatio  |                       |
        |                       | n​(WatchmanStatusEvent |                       |
        |                       | .FileCreation event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `watchmanFileDeletio  |                       |
        |                       | n​(WatchmanStatusEvent |                       |
        |                       | .FileDeletion event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `watchmanOve          |                       |
        |                       | rflow​(WatchmanStatusE |                       |
        |                       | vent.Overflow event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `watc                 |                       |
        |                       | hmanZeroFileChanges​(W |                       |
        |                       | atchmanStatusEvent.Ze |                       |
        |                       | roFileChanges event)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.event.listener.AbstractConsoleEventBusListener}

            ### Methods inherited from class com.facebook.buck.event.listener.[AbstractConsoleEventBusListener](AbstractConsoleEventBusListener.html "class in com.facebook.buck.event.listener")

            `actionGraphFinished, actionGraphStarted, addLineFromEventInterval, addLineFromEvents, aggregateFinishedEvent, aggregateStartedEvent, buildFinished, buildRuleFinished, buildRuleResumed, buildRuleStarted, buildRuleSuspended, buildStarted, commandFinished, commandStartedEvent, convertToAllCapsIfNeeded, formatConsoleEvent, getApproximateBuildProgress, getBuildDetailsLine, getBuildLogLine, getEstimatedProgressOfCreatingActionGraph, getEstimatedProgressOfGeneratingProjectFiles, getEstimatedProgressOfParsingBuckFiles, getEventsBetween, getNetworkStatsLine, getOptionalBuildLineSuffix, getTotalCompletedTimeFromEventIntervals, getWorkingTimeFromLastStartUntilNow, installFinished, installStarted, logEventInterval, logEventInterval, logHttpCacheUploads, projectGenerationFinished, projectGenerationProcessedTarget, projectGenerationStarted, register, renderRemoteUploads, ruleCountCalculated, ruleCountUpdated, setProgressEstimator, setPublicAnnouncements, testRuleFinished, testRuleStarted, watchmanFinished, watchmanStarted`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.event.listener.SuperConsoleConfig,com.facebook.buck.event.listener.RenderingConsole,com.facebook.buck.util.timing.Clock,com.facebook.buck.test.config.TestResultSummaryVerbosity,com.facebook.buck.util.environment.ExecutionEnvironment,java.util.Locale,java.nio.file.Path,com.facebook.buck.core.model.BuildId,boolean,java.util.Optional,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableList,int)}

        -   #### SuperConsoleEventBusListener

                public SuperConsoleEventBusListener​(SuperConsoleConfig config,
                                                    RenderingConsole renderingConsole,
                                                    Clock clock,
                                                    TestResultSummaryVerbosity summaryVerbosity,
                                                    ExecutionEnvironment executionEnvironment,
                                                    Locale locale,
                                                    Path testLogPath,
                                                    BuildId buildId,
                                                    boolean printBuildId,
                                                    Optional<String> buildDetailsTemplate,
                                                    com.google.common.collect.ImmutableSet<String> buildDetailsCommands,
                                                    com.google.common.collect.ImmutableList<AdditionalConsoleLineProvider> additionalConsoleLineProviders,
                                                    int maxConcurrentReExecutions)

        []{#<init>(com.facebook.buck.event.listener.SuperConsoleConfig,com.facebook.buck.event.listener.RenderingConsole,com.facebook.buck.util.timing.Clock,com.facebook.buck.test.config.TestResultSummaryVerbosity,com.facebook.buck.util.environment.ExecutionEnvironment,java.util.Locale,java.nio.file.Path,long,long,long,boolean,com.facebook.buck.core.model.BuildId,boolean,java.util.Optional,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableList,int)}

        -   #### SuperConsoleEventBusListener

                public SuperConsoleEventBusListener​(SuperConsoleConfig config,
                                                    RenderingConsole renderingConsole,
                                                    Clock clock,
                                                    TestResultSummaryVerbosity summaryVerbosity,
                                                    ExecutionEnvironment executionEnvironment,
                                                    Locale locale,
                                                    Path testLogPath,
                                                    long minimumDurationMillisecondsToShowParse,
                                                    long minimumDurationMillisecondsToShowActionGraph,
                                                    long minimumDurationMillisecondsToShowWatchman,
                                                    boolean hideEmptyDownload,
                                                    BuildId buildId,
                                                    boolean printBuildId,
                                                    Optional<String> buildDetailsTemplate,
                                                    com.google.common.collect.ImmutableSet<String> buildDetailsCommands,
                                                    com.google.common.collect.ImmutableList<AdditionalConsoleLineProvider> additionalConsoleLineProviders,
                                                    int maxConcurrentReExecutions)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createRenderLinesAtTime(long)}

        -   #### createRenderLinesAtTime

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> createRenderLinesAtTime​(long currentTimeMillis)
            ```

            ::: block
            Creates a list of lines to be rendered at a given time.
            :::

            [Parameters:]{.paramLabel}
            :   `currentTimeMillis` - The time in ms to use when
                computing elapsed times.

        []{#renderLinesWithMaybeCompression(com.facebook.buck.event.listener.MultiStateRenderer,com.google.common.collect.ImmutableList.Builder,int,boolean)}

        -   #### renderLinesWithMaybeCompression

            ``` methodSignature
            public int renderLinesWithMaybeCompression​(MultiStateRenderer renderer,
                                                       com.google.common.collect.ImmutableList.Builder<String> lines,
                                                       int maxLines,
                                                       boolean alwaysSortByTime)
            ```

            ::: block
            Returns the number of lines created. If the number of lines
            to be created exceeds the given `maxLines`, compress the
            extraneous lines into a single line. See also
            `  #renderLinesWithMaybeTruncation`.
            :::

            [Parameters:]{.paramLabel}
            :   `renderer` - the renderer to use for rendering lines
            :   `lines` - the builder to add the rendered lines to
            :   `maxLines` - the maximum number of lines to render
            :   `alwaysSortByTime` - true if the rendered lines should
                be sorted by time

        []{#renderLinesWithMaybeTruncation(int,com.facebook.buck.event.listener.MultiStateRenderer,com.google.common.collect.ImmutableList.Builder,int)}

        -   #### renderLinesWithMaybeTruncation

            ``` methodSignature
            public int renderLinesWithMaybeTruncation​(int numLinesAlreadyRendered,
                                                      MultiStateRenderer renderer,
                                                      com.google.common.collect.ImmutableList.Builder<String> lines,
                                                      int maxLines)
            ```

            ::: block
            Returns the number of lines created. If the number of lines
            to be created exceeds the given `maxLines`, return early and
            ignore the other lines that were to be rendered. See also
            `#renderLinesWithMaybeCompression`.
            :::

            [Parameters:]{.paramLabel}
            :   `numLinesAlreadyRendered` - the number of lines already
                previously rendered; used to calculate if `maxLines` has
                been reached
            :   `renderer` - the renderer to use for rendering lines
            :   `lines` - the builder to add the rendered lines to
            :   `maxLines` - the maximum number of lines to render

        []{#stepStarted(com.facebook.buck.step.StepEvent.Started)}

        -   #### stepStarted

            ``` methodSignature
            public void stepStarted​(StepEvent.Started started)
            ```

        []{#stepFinished(com.facebook.buck.step.StepEvent.Finished)}

        -   #### stepFinished

            ``` methodSignature
            public void stepFinished​(StepEvent.Finished finished)
            ```

        []{#simpleLeafEventStarted(com.facebook.buck.event.LeafEvents.SimpleLeafEvent.Started)}

        -   #### simpleLeafEventStarted

            ``` methodSignature
            public void simpleLeafEventStarted​(LeafEvents.SimpleLeafEvent.Started started)
            ```

        []{#simpleLeafEventFinished(com.facebook.buck.event.LeafEvents.SimpleLeafEvent.Finished)}

        -   #### simpleLeafEventFinished

            ``` methodSignature
            public void simpleLeafEventFinished​(LeafEvents.SimpleLeafEvent.Finished finished)
            ```

        []{#ruleKeyCalculationStarted(com.facebook.buck.event.RuleKeyCalculationEvent.Started)}

        -   #### ruleKeyCalculationStarted

            ``` methodSignature
            public void ruleKeyCalculationStarted​(RuleKeyCalculationEvent.Started started)
            ```

        []{#ruleKeyCalculationFinished(com.facebook.buck.event.RuleKeyCalculationEvent.Finished)}

        -   #### ruleKeyCalculationFinished

            ``` methodSignature
            public void ruleKeyCalculationFinished​(RuleKeyCalculationEvent.Finished finished)
            ```

        []{#artifactCacheStarted(com.facebook.buck.artifact_cache.ArtifactCacheEvent.Started)}

        -   #### artifactCacheStarted

            ``` methodSignature
            public void artifactCacheStarted​(ArtifactCacheEvent.Started started)
            ```

            ::: block
            When a new cache event is about to start.
            :::

        []{#artifactCacheFinished(com.facebook.buck.artifact_cache.ArtifactCacheEvent.Finished)}

        -   #### artifactCacheFinished

            ``` methodSignature
            public void artifactCacheFinished​(ArtifactCacheEvent.Finished finished)
            ```

        []{#artifactCompressionStarted(com.facebook.buck.event.ArtifactCompressionEvent.Started)}

        -   #### artifactCompressionStarted

            ``` methodSignature
            public void artifactCompressionStarted​(ArtifactCompressionEvent.Started started)
            ```

        []{#artifactCompressionFinished(com.facebook.buck.event.ArtifactCompressionEvent.Finished)}

        -   #### artifactCompressionFinished

            ``` methodSignature
            public void artifactCompressionFinished​(ArtifactCompressionEvent.Finished finished)
            ```

        []{#testRunStarted(com.facebook.buck.core.test.event.TestRunEvent.Started)}

        -   #### testRunStarted

            ``` methodSignature
            public void testRunStarted​(TestRunEvent.Started event)
            ```

        []{#testRunFinished(com.facebook.buck.core.test.event.TestRunEvent.Finished)}

        -   #### testRunFinished

            ``` methodSignature
            public void testRunFinished​(TestRunEvent.Finished finished)
            ```

        []{#testStatusMessageStarted(com.facebook.buck.core.test.event.TestStatusMessageEvent.Started)}

        -   #### testStatusMessageStarted

            ``` methodSignature
            public void testStatusMessageStarted​(TestStatusMessageEvent.Started started)
            ```

        []{#testStatusMessageFinished(com.facebook.buck.core.test.event.TestStatusMessageEvent.Finished)}

        -   #### testStatusMessageFinished

            ``` methodSignature
            public void testStatusMessageFinished​(TestStatusMessageEvent.Finished finished)
            ```

        []{#testSummaryStarted(com.facebook.buck.core.test.event.TestSummaryEvent.Started)}

        -   #### testSummaryStarted

            ``` methodSignature
            public void testSummaryStarted​(TestSummaryEvent.Started started)
            ```

        []{#testSummaryFinished(com.facebook.buck.core.test.event.TestSummaryEvent.Finished)}

        -   #### testSummaryFinished

            ``` methodSignature
            public void testSummaryFinished​(TestSummaryEvent.Finished finished)
            ```

        []{#logEvent(com.facebook.buck.event.ConsoleEvent)}

        -   #### logEvent

            ``` methodSignature
            public void logEvent​(ConsoleEvent event)
            ```

        []{#forceRender(com.facebook.buck.event.FlushConsoleEvent)}

        -   #### forceRender

            ``` methodSignature
            public void forceRender​(FlushConsoleEvent event)
            ```

        []{#printSevereWarningDirectly(java.lang.String)}

        -   #### printSevereWarningDirectly

            ``` methodSignature
            public void printSevereWarningDirectly​(String line)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `printSevereWarningDirectly` in
                class `AbstractConsoleEventBusListener`

        []{#actionGraphCacheHit(com.facebook.buck.event.ActionGraphEvent.Cache.Hit)}

        -   #### actionGraphCacheHit

            ``` methodSignature
            public void actionGraphCacheHit​(ActionGraphEvent.Cache.Hit event)
            ```

        []{#watchmanOverflow(com.facebook.buck.event.WatchmanStatusEvent.Overflow)}

        -   #### watchmanOverflow

            ``` methodSignature
            public void watchmanOverflow​(WatchmanStatusEvent.Overflow event)
            ```

        []{#watchmanFileCreation(com.facebook.buck.event.WatchmanStatusEvent.FileCreation)}

        -   #### watchmanFileCreation

            ``` methodSignature
            public void watchmanFileCreation​(WatchmanStatusEvent.FileCreation event)
            ```

        []{#watchmanFileDeletion(com.facebook.buck.event.WatchmanStatusEvent.FileDeletion)}

        -   #### watchmanFileDeletion

            ``` methodSignature
            public void watchmanFileDeletion​(WatchmanStatusEvent.FileDeletion event)
            ```

        []{#watchmanZeroFileChanges(com.facebook.buck.event.WatchmanStatusEvent.ZeroFileChanges)}

        -   #### watchmanZeroFileChanges

            ``` methodSignature
            public void watchmanZeroFileChanges​(WatchmanStatusEvent.ZeroFileChanges event)
            ```

        []{#symlinkInvalidation(com.facebook.buck.event.ParsingEvent.SymlinkInvalidation)}

        -   #### symlinkInvalidation

            ``` methodSignature
            public void symlinkInvalidation​(ParsingEvent.SymlinkInvalidation event)
            ```

        []{#envVariableChange(com.facebook.buck.event.ParsingEvent.EnvVariableChange)}

        -   #### envVariableChange

            ``` methodSignature
            public void envVariableChange​(ParsingEvent.EnvVariableChange event)
            ```

        []{#onActionEventStarted(com.facebook.buck.remoteexecution.event.RemoteExecutionActionEvent.Started)}

        -   #### onActionEventStarted

            ``` methodSignature
            public void onActionEventStarted​(RemoteExecutionActionEvent.Started event)
            ```

        []{#onActionEventTerminated(com.facebook.buck.remoteexecution.event.RemoteExecutionActionEvent.Terminal)}

        -   #### onActionEventTerminated

            ``` methodSignature
            public void onActionEventTerminated​(RemoteExecutionActionEvent.Terminal event)
            ```

        []{#onActionEventStolen(com.facebook.buck.rules.modern.builders.HybridLocalEvent.Stolen)}

        -   #### onActionEventStolen

            ``` methodSignature
            public void onActionEventStolen​(HybridLocalEvent.Stolen event)
            ```

        []{#formatElapsedTime(long)}

        -   #### formatElapsedTime

            ``` methodSignature
            protected String formatElapsedTime​(long elapsedTimeMs)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `formatElapsedTime` in
                class `AbstractConsoleEventBusListener`

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
                       throws IOException
            ```

            ::: block
            [Description copied from
            interface: `BuckEventListener`]{.descfrmTypeLabel}
            :::

            ::: block
            Cleanup, output any trace data collected to the backing
            store.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `BuckEventListener`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `Closeable`

            [Overrides:]{.overrideSpecifyLabel}
            :   `close` in class `AbstractConsoleEventBusListener`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#displaysEstimatedProgress()}

        -   #### displaysEstimatedProgress

            ``` methodSignature
            public boolean displaysEstimatedProgress()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `displaysEstimatedProgress` in
                class `AbstractConsoleEventBusListener`
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
