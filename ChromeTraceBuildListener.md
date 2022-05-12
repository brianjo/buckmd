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

## Class ChromeTraceBuildListener {#class-chrometracebuildlistener .title title="Class ChromeTraceBuildListener"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.event.listener.ChromeTraceBuildListener

::: description
-   

    All Implemented Interfaces:
    :   `BuckEventListener`, `Closeable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class ChromeTraceBuildListener
        extends Object
        implements BuckEventListener

    ::: block
    Logs events to a json file formatted to be viewed in Chrome Trace
    View (chrome://tracing).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                    Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `ChromeTraceBuildListener​(ProjectFilesystem projectFilesystem,                         InvocationInfo invocationInfo,                         Clock clock,                         ChromeTraceBuckConfig config,                         TaskManagerCommandScope managerScope,                         Optional<RemoteExecutionStatsProvider> reStatsProvider,                         CriticalPathEventListener criticalPathEventListener)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `actionGrap           |                       |
        |                       | hCacheHit​(ActionGraph |                       |
        |                       | Event.Cache.Hit hit)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `actionGraphCa        |                       |
        |                       | cheMiss​(ActionGraphEv |                       |
        |                       | ent.Cache.Miss miss)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `actionGraphFin       |                       |
        |                       | ished​(ActionGraphEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `actionGraph          |                       |
        |                       | Started​(ActionGraphEv |                       |
        |                       | ent.Started started)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `annotationP          |                       |
        |                       | rocessingFinished​(Ann |                       |
        |                       | otationProcessingEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `annotati             |                       |
        |                       | onProcessingStarted​(A |                       |
        |                       | nnotationProcessingEv |                       |
        |                       | ent.Started started)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `ar                   |                       |
        |                       | tifactCacheEventFinis |                       |
        |                       | hed​(ArtifactCacheEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `artifactCacheEventSt |                       |
        |                       | arted​(ArtifactCacheEv |                       |
        |                       | ent.Started started)` |                       |
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
        | `void`                | `artifa               |                       |
        |                       | ctConnectFinished​(Art |                       |
        |                       | ifactCacheConnectEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `art                  |                       |
        |                       | ifactConnectStarted​(A |                       |
        |                       | rtifactCacheConnectEv |                       |
        |                       | ent.Started started)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `bu                   |                       |
        |                       | ildFinished​(BuildEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `buildStarted​(BuildEv |                       |
        |                       | ent.Started started)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `close()`             | ::: block             |
        |                       |                       | Cleanup, output any   |
        |                       |                       | trace data collected  |
        |                       |                       | to the backing store. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `comman               |                       |
        |                       | dFinished​(CommandEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `com                  |                       |
        |                       | mandStarted​(CommandEv |                       |
        |                       | ent.Started started)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `compilerPluginDurati |                       |
        |                       | onEventFinished​(Compi |                       |
        |                       | lerPluginDurationEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `compilerPluginDur    |                       |
        |                       | ationEventStarted​(Com |                       |
        |                       | pilerPluginDurationEv |                       |
        |                       | ent.Started started)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `e                    |                       |
        |                       | xternalTestRunFinishe |                       |
        |                       | d​(ExternalTestRunEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `externalTestRunStar  |                       |
        |                       | ted​(ExternalTestRunEv |                       |
        |                       | ent.Started started)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `exte                 |                       |
        |                       | rnalTestSpecCalculati |                       |
        |                       | onFinished​(ExternalTe |                       |
        |                       | stSpecCalculationEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `e                    |                       |
        |                       | xternalTestSpecCalcul |                       |
        |                       | ationStarted​(External |                       |
        |                       | TestSpecCalculationEv |                       |
        |                       | ent.Started started)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `instal               |                       |
        |                       | lFinished​(InstallEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `ins                  |                       |
        |                       | tallStarted​(InstallEv |                       |
        |                       | ent.Started started)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `javacPhaseFi         |                       |
        |                       | nished​(JavacPhaseEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `javacPhas            |                       |
        |                       | eStarted​(JavacPhaseEv |                       |
        |                       | ent.Started started)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `                     |                       |
        |                       | memoryPerfStats​(PerfS |                       |
        |                       | tatsTracking.MemoryPe |                       |
        |                       | rfStatsEvent memory)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `on                   | ::: block             |
        |                       | ActionEventFinished​(R | Add metadata for      |
        |                       | emoteExecutionActionE | actions in each       |
        |                       | vent.Finished event)` | Remote Execution      |
        |                       |                       | state                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `                     | ::: block             |
        |                       | onActionEventStarted​( | Add metadata for      |
        |                       | RemoteExecutionAction | actions in each       |
        |                       | Event.Started event)` | Remote Execution      |
        |                       |                       | state                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `onRemoteExecut       | ::: block             |
        |                       | ionSessionFinished​(Re | Mark the end of a     |
        |                       | moteExecutionSessionE | Remote Execution      |
        |                       | vent.Finished event)` | session and write     |
        |                       |                       | down the related      |
        |                       |                       | telemetry.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `onRemoteExec         | ::: block             |
        |                       | utionSessionStarted​(R | Mark the start of a   |
        |                       | emoteExecutionSession | Remote Execution      |
        |                       | Event.Started event)` | session               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `onWatchmanOve        |                       |
        |                       | rflow​(WatchmanStatusE |                       |
        |                       | vent.Overflow event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `parseBuckFileFinis   |                       |
        |                       | hed​(ParseBuckFileEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `parseBuckFileSt      |                       |
        |                       | arted​(ParseBuckFileEv |                       |
        |                       | ent.Started started)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `pa                   |                       |
        |                       | rseFinished​(ParseEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `parseStarted​(ParseEv |                       |
        |                       | ent.Started started)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `processResourceCon   |                       |
        |                       | sumption​(ProcessTrack |                       |
        |                       | er.ProcessResourceCon |                       |
        |                       | sumptionEvent event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `ruleF                |                       |
        |                       | inished​(BuildRuleEven |                       |
        |                       | t.Finished finished)` |                       |
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
        | `void`                | `ru                   |                       |
        |                       | leResumed​(BuildRuleEv |                       |
        |                       | ent.Resumed resumed)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `ru                   |                       |
        |                       | leStarted​(BuildRuleEv |                       |
        |                       | ent.Started started)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `ruleSusp             |                       |
        |                       | ended​(BuildRuleEvent. |                       |
        |                       | Suspended suspended)` |                       |
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
        | `void`                | `s                    |                       |
        |                       | implePerfEvent​(Simple |                       |
        |                       | PerfEvent perfEvent)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `startActivityFinis   |                       |
        |                       | hed​(StartActivityEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `startActivitySt      |                       |
        |                       | arted​(StartActivityEv |                       |
        |                       | ent.Started started)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `                     |                       |
        |                       | stepFinished​(StepEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `stepStarted​(StepEv   |                       |
        |                       | ent.Started started)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `testFinished         |                       |
        |                       | Event​(TestSummaryEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `testStart            |                       |
        |                       | edEvent​(TestSummaryEv |                       |
        |                       | ent.Started started)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `uninstallF           |                       |
        |                       | inished​(UninstallEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `uninsta              |                       |
        |                       | llStarted​(UninstallEv |                       |
        |                       | ent.Started started)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `writeArtifa          |                       |
        |                       | ctCompressionEvent​(Ar |                       |
        |                       | tifactCompressionEven |                       |
        |                       | t event,              |                       |
        |                       |                  Chro |                       |
        |                       | meTraceEvent.Phase ph |                       |
        |                       | ase,                  |                       |
        |                       |              com.goog |                       |
        |                       | le.common.collect.Imm |                       |
        |                       | utableMap.Builder<Str |                       |
        |                       | ing,​String> builder)` |                       |
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.log.InvocationInfo,com.facebook.buck.util.timing.Clock,com.facebook.buck.event.chrome_trace.ChromeTraceBuckConfig,com.facebook.buck.support.bgtasks.TaskManagerCommandScope,java.util.Optional,com.facebook.buck.event.listener.CriticalPathEventListener)}

        -   #### ChromeTraceBuildListener

                public ChromeTraceBuildListener​(ProjectFilesystem projectFilesystem,
                                                InvocationInfo invocationInfo,
                                                Clock clock,
                                                ChromeTraceBuckConfig config,
                                                TaskManagerCommandScope managerScope,
                                                Optional<RemoteExecutionStatsProvider> reStatsProvider,
                                                CriticalPathEventListener criticalPathEventListener)
                                         throws IOException

            [Throws:]{.throwsLabel}
            :   `IOException`
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
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

        []{#commandStarted(com.facebook.buck.event.CommandEvent.Started)}

        -   #### commandStarted

            ``` methodSignature
            public void commandStarted​(CommandEvent.Started started)
            ```

        []{#commandFinished(com.facebook.buck.event.CommandEvent.Finished)}

        -   #### commandFinished

            ``` methodSignature
            public void commandFinished​(CommandEvent.Finished finished)
            ```

        []{#buildStarted(com.facebook.buck.core.build.event.BuildEvent.Started)}

        -   #### buildStarted

            ``` methodSignature
            public void buildStarted​(BuildEvent.Started started)
            ```

        []{#buildFinished(com.facebook.buck.core.build.event.BuildEvent.Finished)}

        -   #### buildFinished

            ``` methodSignature
            public void buildFinished​(BuildEvent.Finished finished)
            ```

        []{#ruleStarted(com.facebook.buck.core.build.event.BuildRuleEvent.Started)}

        -   #### ruleStarted

            ``` methodSignature
            public void ruleStarted​(BuildRuleEvent.Started started)
            ```

        []{#ruleFinished(com.facebook.buck.core.build.event.BuildRuleEvent.Finished)}

        -   #### ruleFinished

            ``` methodSignature
            public void ruleFinished​(BuildRuleEvent.Finished finished)
            ```

        []{#ruleResumed(com.facebook.buck.core.build.event.BuildRuleEvent.Resumed)}

        -   #### ruleResumed

            ``` methodSignature
            public void ruleResumed​(BuildRuleEvent.Resumed resumed)
            ```

        []{#ruleSuspended(com.facebook.buck.core.build.event.BuildRuleEvent.Suspended)}

        -   #### ruleSuspended

            ``` methodSignature
            public void ruleSuspended​(BuildRuleEvent.Suspended suspended)
            ```

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

        []{#parseStarted(com.facebook.buck.parser.ParseEvent.Started)}

        -   #### parseStarted

            ``` methodSignature
            public void parseStarted​(ParseEvent.Started started)
            ```

        []{#parseFinished(com.facebook.buck.parser.ParseEvent.Finished)}

        -   #### parseFinished

            ``` methodSignature
            public void parseFinished​(ParseEvent.Finished finished)
            ```

        []{#simplePerfEvent(com.facebook.buck.event.SimplePerfEvent)}

        -   #### simplePerfEvent

            ``` methodSignature
            public void simplePerfEvent​(SimplePerfEvent perfEvent)
            ```

        []{#parseBuckFileStarted(com.facebook.buck.parser.events.ParseBuckFileEvent.Started)}

        -   #### parseBuckFileStarted

            ``` methodSignature
            public void parseBuckFileStarted​(ParseBuckFileEvent.Started started)
            ```

        []{#parseBuckFileFinished(com.facebook.buck.parser.events.ParseBuckFileEvent.Finished)}

        -   #### parseBuckFileFinished

            ``` methodSignature
            public void parseBuckFileFinished​(ParseBuckFileEvent.Finished finished)
            ```

        []{#actionGraphStarted(com.facebook.buck.event.ActionGraphEvent.Started)}

        -   #### actionGraphStarted

            ``` methodSignature
            public void actionGraphStarted​(ActionGraphEvent.Started started)
            ```

        []{#actionGraphFinished(com.facebook.buck.event.ActionGraphEvent.Finished)}

        -   #### actionGraphFinished

            ``` methodSignature
            public void actionGraphFinished​(ActionGraphEvent.Finished finished)
            ```

        []{#actionGraphCacheHit(com.facebook.buck.event.ActionGraphEvent.Cache.Hit)}

        -   #### actionGraphCacheHit

            ``` methodSignature
            public void actionGraphCacheHit​(ActionGraphEvent.Cache.Hit hit)
            ```

        []{#actionGraphCacheMiss(com.facebook.buck.event.ActionGraphEvent.Cache.Miss)}

        -   #### actionGraphCacheMiss

            ``` methodSignature
            public void actionGraphCacheMiss​(ActionGraphEvent.Cache.Miss miss)
            ```

        []{#installStarted(com.facebook.buck.event.InstallEvent.Started)}

        -   #### installStarted

            ``` methodSignature
            public void installStarted​(InstallEvent.Started started)
            ```

        []{#installFinished(com.facebook.buck.event.InstallEvent.Finished)}

        -   #### installFinished

            ``` methodSignature
            public void installFinished​(InstallEvent.Finished finished)
            ```

        []{#startActivityStarted(com.facebook.buck.event.StartActivityEvent.Started)}

        -   #### startActivityStarted

            ``` methodSignature
            public void startActivityStarted​(StartActivityEvent.Started started)
            ```

        []{#startActivityFinished(com.facebook.buck.event.StartActivityEvent.Finished)}

        -   #### startActivityFinished

            ``` methodSignature
            public void startActivityFinished​(StartActivityEvent.Finished finished)
            ```

        []{#uninstallStarted(com.facebook.buck.event.UninstallEvent.Started)}

        -   #### uninstallStarted

            ``` methodSignature
            public void uninstallStarted​(UninstallEvent.Started started)
            ```

        []{#uninstallFinished(com.facebook.buck.event.UninstallEvent.Finished)}

        -   #### uninstallFinished

            ``` methodSignature
            public void uninstallFinished​(UninstallEvent.Finished finished)
            ```

        []{#artifactCacheEventStarted(com.facebook.buck.artifact_cache.ArtifactCacheEvent.Started)}

        -   #### artifactCacheEventStarted

            ``` methodSignature
            public void artifactCacheEventStarted​(ArtifactCacheEvent.Started started)
            ```

        []{#artifactCacheEventFinished(com.facebook.buck.artifact_cache.ArtifactCacheEvent.Finished)}

        -   #### artifactCacheEventFinished

            ``` methodSignature
            public void artifactCacheEventFinished​(ArtifactCacheEvent.Finished finished)
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

        []{#writeArtifactCompressionEvent(com.facebook.buck.event.ArtifactCompressionEvent,com.facebook.buck.event.chrome_trace.ChromeTraceEvent.Phase,com.google.common.collect.ImmutableMap.Builder)}

        -   #### writeArtifactCompressionEvent

            ``` methodSignature
            public void writeArtifactCompressionEvent​(ArtifactCompressionEvent event,
                                                      ChromeTraceEvent.Phase phase,
                                                      com.google.common.collect.ImmutableMap.Builder<String,​String> builder)
            ```

        []{#artifactConnectStarted(com.facebook.buck.artifact_cache.ArtifactCacheConnectEvent.Started)}

        -   #### artifactConnectStarted

            ``` methodSignature
            public void artifactConnectStarted​(ArtifactCacheConnectEvent.Started started)
            ```

        []{#artifactConnectFinished(com.facebook.buck.artifact_cache.ArtifactCacheConnectEvent.Finished)}

        -   #### artifactConnectFinished

            ``` methodSignature
            public void artifactConnectFinished​(ArtifactCacheConnectEvent.Finished finished)
            ```

        []{#javacPhaseStarted(com.facebook.buck.jvm.java.tracing.JavacPhaseEvent.Started)}

        -   #### javacPhaseStarted

            ``` methodSignature
            public void javacPhaseStarted​(JavacPhaseEvent.Started started)
            ```

        []{#javacPhaseFinished(com.facebook.buck.jvm.java.tracing.JavacPhaseEvent.Finished)}

        -   #### javacPhaseFinished

            ``` methodSignature
            public void javacPhaseFinished​(JavacPhaseEvent.Finished finished)
            ```

        []{#annotationProcessingStarted(com.facebook.buck.jvm.java.AnnotationProcessingEvent.Started)}

        -   #### annotationProcessingStarted

            ``` methodSignature
            public void annotationProcessingStarted​(AnnotationProcessingEvent.Started started)
            ```

        []{#annotationProcessingFinished(com.facebook.buck.jvm.java.AnnotationProcessingEvent.Finished)}

        -   #### annotationProcessingFinished

            ``` methodSignature
            public void annotationProcessingFinished​(AnnotationProcessingEvent.Finished finished)
            ```

        []{#compilerPluginDurationEventStarted(com.facebook.buck.event.CompilerPluginDurationEvent.Started)}

        -   #### compilerPluginDurationEventStarted

            ``` methodSignature
            public void compilerPluginDurationEventStarted​(CompilerPluginDurationEvent.Started started)
            ```

        []{#compilerPluginDurationEventFinished(com.facebook.buck.event.CompilerPluginDurationEvent.Finished)}

        -   #### compilerPluginDurationEventFinished

            ``` methodSignature
            public void compilerPluginDurationEventFinished​(CompilerPluginDurationEvent.Finished finished)
            ```

        []{#memoryPerfStats(com.facebook.buck.util.perf.PerfStatsTracking.MemoryPerfStatsEvent)}

        -   #### memoryPerfStats

            ``` methodSignature
            public void memoryPerfStats​(PerfStatsTracking.MemoryPerfStatsEvent memory)
            ```

        []{#processResourceConsumption(com.facebook.buck.util.perf.ProcessTracker.ProcessResourceConsumptionEvent)}

        -   #### processResourceConsumption

            ``` methodSignature
            public void processResourceConsumption​(ProcessTracker.ProcessResourceConsumptionEvent event)
            ```

        []{#testStartedEvent(com.facebook.buck.core.test.event.TestSummaryEvent.Started)}

        -   #### testStartedEvent

            ``` methodSignature
            public void testStartedEvent​(TestSummaryEvent.Started started)
            ```

        []{#testFinishedEvent(com.facebook.buck.core.test.event.TestSummaryEvent.Finished)}

        -   #### testFinishedEvent

            ``` methodSignature
            public void testFinishedEvent​(TestSummaryEvent.Finished finished)
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

        []{#externalTestSpecCalculationStarted(com.facebook.buck.test.external.ExternalTestSpecCalculationEvent.Started)}

        -   #### externalTestSpecCalculationStarted

            ``` methodSignature
            public void externalTestSpecCalculationStarted​(ExternalTestSpecCalculationEvent.Started started)
            ```

        []{#externalTestSpecCalculationFinished(com.facebook.buck.test.external.ExternalTestSpecCalculationEvent.Finished)}

        -   #### externalTestSpecCalculationFinished

            ``` methodSignature
            public void externalTestSpecCalculationFinished​(ExternalTestSpecCalculationEvent.Finished finished)
            ```

        []{#externalTestRunStarted(com.facebook.buck.test.external.ExternalTestRunEvent.Started)}

        -   #### externalTestRunStarted

            ``` methodSignature
            public void externalTestRunStarted​(ExternalTestRunEvent.Started started)
            ```

        []{#externalTestRunFinished(com.facebook.buck.test.external.ExternalTestRunEvent.Finished)}

        -   #### externalTestRunFinished

            ``` methodSignature
            public void externalTestRunFinished​(ExternalTestRunEvent.Finished finished)
            ```

        []{#onWatchmanOverflow(com.facebook.buck.event.WatchmanStatusEvent.Overflow)}

        -   #### onWatchmanOverflow

            ``` methodSignature
            public void onWatchmanOverflow​(WatchmanStatusEvent.Overflow event)
            ```

        []{#onActionEventStarted(com.facebook.buck.remoteexecution.event.RemoteExecutionActionEvent.Started)}

        -   #### onActionEventStarted

            ``` methodSignature
            public void onActionEventStarted​(RemoteExecutionActionEvent.Started event)
            ```

            ::: block
            Add metadata for actions in each Remote Execution state
            :::

        []{#onActionEventFinished(com.facebook.buck.remoteexecution.event.RemoteExecutionActionEvent.Finished)}

        -   #### onActionEventFinished

            ``` methodSignature
            public void onActionEventFinished​(RemoteExecutionActionEvent.Finished event)
            ```

            ::: block
            Add metadata for actions in each Remote Execution state
            :::

        []{#onRemoteExecutionSessionStarted(com.facebook.buck.remoteexecution.event.RemoteExecutionSessionEvent.Started)}

        -   #### onRemoteExecutionSessionStarted

            ``` methodSignature
            public void onRemoteExecutionSessionStarted​(RemoteExecutionSessionEvent.Started event)
            ```

            ::: block
            Mark the start of a Remote Execution session
            :::

        []{#onRemoteExecutionSessionFinished(com.facebook.buck.remoteexecution.event.RemoteExecutionSessionEvent.Finished)}

        -   #### onRemoteExecutionSessionFinished

            ``` methodSignature
            public void onRemoteExecutionSessionFinished​(RemoteExecutionSessionEvent.Finished event)
            ```

            ::: block
            Mark the end of a Remote Execution session and write down
            the related telemetry.
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
