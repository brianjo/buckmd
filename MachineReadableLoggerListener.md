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

## Class MachineReadableLoggerListener {#class-machinereadableloggerlistener .title title="Class MachineReadableLoggerListener"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.event.listener.MachineReadableLoggerListener

::: description
-   

    All Implemented Interfaces:
    :   `BuckEventListener`, `Closeable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class MachineReadableLoggerListener
        extends Object
        implements BuckEventListener
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           Description
          --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `MachineReadableLoggerListener​(InvocationInfo info,                              ProjectFilesystem filesystem,                              ExecutorService executor,                              com.google.common.collect.ImmutableSet<ArtifactCacheMode> cacheModes,                              ChromeTraceBuckConfig chromeTraceConfig,                              Path logFilePath,                              Path logDirectoryPath,                              BuildId buildId,                              TaskManagerCommandScope managerScope)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `actionGraphFinis     |                       |
        |                       | hedEvent​(ActionGraphE |                       |
        |                       | vent.Finished event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `actionGraphSta       |                       |
        |                       | rtedEvent​(ActionGraph |                       |
        |                       | Event.Started event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `artifa               |                       |
        |                       | ctCompressionFinished |                       |
        |                       | ​(ArtifactCompressionE |                       |
        |                       | vent.Finished event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `arti                 |                       |
        |                       | factCompressionStarte |                       |
        |                       | d​(ArtifactCompression |                       |
        |                       | Event.Started event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `buildFinished​(BuildE |                       |
        |                       | vent.Finished event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `buildRuleEve         |                       |
        |                       | ntFinished​(BuildRuleE |                       |
        |                       | vent.Finished event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `buildRuleE           |                       |
        |                       | ventFinishedRuleCalc​( |                       |
        |                       | BuildRuleEvent.Finish |                       |
        |                       | edRuleKeyCalc event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `buildRuleE           |                       |
        |                       | ventResumed​(BuildRule |                       |
        |                       | Event.Resumed event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `buildRuleE           |                       |
        |                       | ventStarted​(BuildRule |                       |
        |                       | Event.Started event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `buildRul             |                       |
        |                       | eEventStartedRuleCalc |                       |
        |                       | ​(BuildRuleEvent.Start |                       |
        |                       | edRuleKeyCalc event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `buildRuleEvent       |                       |
        |                       | Suspended​(BuildRuleEv |                       |
        |                       | ent.Suspended event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `buildRu              |                       |
        |                       | leEventWillBuildLocal |                       |
        |                       | ly​(BuildRuleEvent.Wil |                       |
        |                       | lBuildLocally event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `buildRule            |                       |
        |                       | ExecutionFinishedEven |                       |
        |                       | t​(BuildRuleExecutionE |                       |
        |                       | vent.Finished event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `buildRu              |                       |
        |                       | leExecutionStartedEve |                       |
        |                       | nt​(BuildRuleExecution |                       |
        |                       | Event.Started event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `buildRuleRemoteExe   |                       |
        |                       | cutionFinishedEvent​(R |                       |
        |                       | emoteExecutionActionE |                       |
        |                       | vent.Finished event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `buildRuleRemoteExecu |                       |
        |                       | tionScheduledEvent​(Re |                       |
        |                       | moteExecutionActionEv |                       |
        |                       | ent.Scheduled event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `buildRuleRemoteE     |                       |
        |                       | xecutionStartedEvent​( |                       |
        |                       | RemoteExecutionAction |                       |
        |                       | Event.Started event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `buildRuleRemoteExe   |                       |
        |                       | cutionTerminalEvent​(R |                       |
        |                       | emoteExecutionActionE |                       |
        |                       | vent.Terminal event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `close()`             | ::: block             |
        |                       |                       | Cleanup, output any   |
        |                       |                       | trace data collected  |
        |                       |                       | to the backing store. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `com                  |                       |
        |                       | mandFinished​(CommandE |                       |
        |                       | vent.Finished event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `commandIn            |                       |
        |                       | terrupted​(CommandEven |                       |
        |                       | t.Interrupted event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `environmentalCha     |                       |
        |                       | nge​(ParsingEvent.EnvV |                       |
        |                       | ariableChange event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `g                    |                       |
        |                       | arbageCollection​(GCCo |                       |
        |                       | llectionEvent event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `onArtifactCacheEve   |                       |
        |                       | nt​(HttpArtifactCacheE |                       |
        |                       | vent.Finished event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `parseFinished​(ParseE |                       |
        |                       | vent.Finished event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `parseStarted​(Parse   |                       |
        |                       | Event.Started event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `symlinkInvalidatio   |                       |
        |                       | n​(ParsingEvent.Symlin |                       |
        |                       | kInvalidation event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `t                    |                       |
        |                       | imePerfStatsEvent​(Per |                       |
        |                       | fTimesEventListener.P |                       |
        |                       | erfTimesEvent event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `versionC             |                       |
        |                       | ontrolStats​(VersionCo |                       |
        |                       | ntrolStatsEvent versi |                       |
        |                       | onControlStatsEvent)` |                       |
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

        []{#<init>(com.facebook.buck.log.InvocationInfo,com.facebook.buck.io.filesystem.ProjectFilesystem,java.util.concurrent.ExecutorService,com.google.common.collect.ImmutableSet,com.facebook.buck.event.chrome_trace.ChromeTraceBuckConfig,java.nio.file.Path,java.nio.file.Path,com.facebook.buck.core.model.BuildId,com.facebook.buck.support.bgtasks.TaskManagerCommandScope)}

        -   #### MachineReadableLoggerListener

                public MachineReadableLoggerListener​(InvocationInfo info,
                                                     ProjectFilesystem filesystem,
                                                     ExecutorService executor,
                                                     com.google.common.collect.ImmutableSet<ArtifactCacheMode> cacheModes,
                                                     ChromeTraceBuckConfig chromeTraceConfig,
                                                     Path logFilePath,
                                                     Path logDirectoryPath,
                                                     BuildId buildId,
                                                     TaskManagerCommandScope managerScope)
                                              throws FileNotFoundException

            [Throws:]{.throwsLabel}
            :   `FileNotFoundException`
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#versionControlStats(com.facebook.buck.util.versioncontrol.VersionControlStatsEvent)}

        -   #### versionControlStats

            ``` methodSignature
            public void versionControlStats​(VersionControlStatsEvent versionControlStatsEvent)
            ```

        []{#parseStarted(com.facebook.buck.parser.ParseEvent.Started)}

        -   #### parseStarted

            ``` methodSignature
            public void parseStarted​(ParseEvent.Started event)
            ```

        []{#parseFinished(com.facebook.buck.parser.ParseEvent.Finished)}

        -   #### parseFinished

            ``` methodSignature
            public void parseFinished​(ParseEvent.Finished event)
            ```

        []{#buildFinished(com.facebook.buck.core.build.event.BuildEvent.Finished)}

        -   #### buildFinished

            ``` methodSignature
            public void buildFinished​(BuildEvent.Finished event)
            ```

        []{#buildRuleEventStarted(com.facebook.buck.core.build.event.BuildRuleEvent.Started)}

        -   #### buildRuleEventStarted

            ``` methodSignature
            public void buildRuleEventStarted​(BuildRuleEvent.Started event)
            ```

        []{#buildRuleEventResumed(com.facebook.buck.core.build.event.BuildRuleEvent.Resumed)}

        -   #### buildRuleEventResumed

            ``` methodSignature
            public void buildRuleEventResumed​(BuildRuleEvent.Resumed event)
            ```

        []{#buildRuleEventSuspended(com.facebook.buck.core.build.event.BuildRuleEvent.Suspended)}

        -   #### buildRuleEventSuspended

            ``` methodSignature
            public void buildRuleEventSuspended​(BuildRuleEvent.Suspended event)
            ```

        []{#buildRuleEventStartedRuleCalc(com.facebook.buck.core.build.event.BuildRuleEvent.StartedRuleKeyCalc)}

        -   #### buildRuleEventStartedRuleCalc

            ``` methodSignature
            public void buildRuleEventStartedRuleCalc​(BuildRuleEvent.StartedRuleKeyCalc event)
            ```

        []{#buildRuleEventFinishedRuleCalc(com.facebook.buck.core.build.event.BuildRuleEvent.FinishedRuleKeyCalc)}

        -   #### buildRuleEventFinishedRuleCalc

            ``` methodSignature
            public void buildRuleEventFinishedRuleCalc​(BuildRuleEvent.FinishedRuleKeyCalc event)
            ```

        []{#buildRuleEventWillBuildLocally(com.facebook.buck.core.build.event.BuildRuleEvent.WillBuildLocally)}

        -   #### buildRuleEventWillBuildLocally

            ``` methodSignature
            public void buildRuleEventWillBuildLocally​(BuildRuleEvent.WillBuildLocally event)
            ```

        []{#buildRuleExecutionStartedEvent(com.facebook.buck.core.build.event.BuildRuleExecutionEvent.Started)}

        -   #### buildRuleExecutionStartedEvent

            ``` methodSignature
            public void buildRuleExecutionStartedEvent​(BuildRuleExecutionEvent.Started event)
            ```

        []{#buildRuleExecutionFinishedEvent(com.facebook.buck.core.build.event.BuildRuleExecutionEvent.Finished)}

        -   #### buildRuleExecutionFinishedEvent

            ``` methodSignature
            public void buildRuleExecutionFinishedEvent​(BuildRuleExecutionEvent.Finished event)
            ```

        []{#buildRuleRemoteExecutionStartedEvent(com.facebook.buck.remoteexecution.event.RemoteExecutionActionEvent.Started)}

        -   #### buildRuleRemoteExecutionStartedEvent

            ``` methodSignature
            public void buildRuleRemoteExecutionStartedEvent​(RemoteExecutionActionEvent.Started event)
            ```

        []{#buildRuleRemoteExecutionFinishedEvent(com.facebook.buck.remoteexecution.event.RemoteExecutionActionEvent.Finished)}

        -   #### buildRuleRemoteExecutionFinishedEvent

            ``` methodSignature
            public void buildRuleRemoteExecutionFinishedEvent​(RemoteExecutionActionEvent.Finished event)
            ```

        []{#buildRuleRemoteExecutionScheduledEvent(com.facebook.buck.remoteexecution.event.RemoteExecutionActionEvent.Scheduled)}

        -   #### buildRuleRemoteExecutionScheduledEvent

            ``` methodSignature
            public void buildRuleRemoteExecutionScheduledEvent​(RemoteExecutionActionEvent.Scheduled event)
            ```

        []{#buildRuleRemoteExecutionTerminalEvent(com.facebook.buck.remoteexecution.event.RemoteExecutionActionEvent.Terminal)}

        -   #### buildRuleRemoteExecutionTerminalEvent

            ``` methodSignature
            public void buildRuleRemoteExecutionTerminalEvent​(RemoteExecutionActionEvent.Terminal event)
            ```

        []{#actionGraphStartedEvent(com.facebook.buck.event.ActionGraphEvent.Started)}

        -   #### actionGraphStartedEvent

            ``` methodSignature
            public void actionGraphStartedEvent​(ActionGraphEvent.Started event)
            ```

        []{#actionGraphFinishedEvent(com.facebook.buck.event.ActionGraphEvent.Finished)}

        -   #### actionGraphFinishedEvent

            ``` methodSignature
            public void actionGraphFinishedEvent​(ActionGraphEvent.Finished event)
            ```

        []{#artifactCompressionStarted(com.facebook.buck.event.ArtifactCompressionEvent.Started)}

        -   #### artifactCompressionStarted

            ``` methodSignature
            public void artifactCompressionStarted​(ArtifactCompressionEvent.Started event)
            ```

        []{#artifactCompressionFinished(com.facebook.buck.event.ArtifactCompressionEvent.Finished)}

        -   #### artifactCompressionFinished

            ``` methodSignature
            public void artifactCompressionFinished​(ArtifactCompressionEvent.Finished event)
            ```

        []{#buildRuleEventFinished(com.facebook.buck.core.build.event.BuildRuleEvent.Finished)}

        -   #### buildRuleEventFinished

            ``` methodSignature
            public void buildRuleEventFinished​(BuildRuleEvent.Finished event)
            ```

        []{#garbageCollection(com.facebook.buck.support.jvm.GCCollectionEvent)}

        -   #### garbageCollection

            ``` methodSignature
            public void garbageCollection​(GCCollectionEvent event)
            ```

        []{#commandFinished(com.facebook.buck.event.CommandEvent.Finished)}

        -   #### commandFinished

            ``` methodSignature
            public void commandFinished​(CommandEvent.Finished event)
            ```

        []{#commandInterrupted(com.facebook.buck.event.CommandEvent.Interrupted)}

        -   #### commandInterrupted

            ``` methodSignature
            public void commandInterrupted​(CommandEvent.Interrupted event)
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

        []{#watchmanOverflow(com.facebook.buck.event.WatchmanStatusEvent.Overflow)}

        -   #### watchmanOverflow

            ``` methodSignature
            public void watchmanOverflow​(WatchmanStatusEvent.Overflow event)
            ```

        []{#symlinkInvalidation(com.facebook.buck.event.ParsingEvent.SymlinkInvalidation)}

        -   #### symlinkInvalidation

            ``` methodSignature
            public void symlinkInvalidation​(ParsingEvent.SymlinkInvalidation event)
            ```

        []{#environmentalChange(com.facebook.buck.event.ParsingEvent.EnvVariableChange)}

        -   #### environmentalChange

            ``` methodSignature
            public void environmentalChange​(ParsingEvent.EnvVariableChange event)
            ```

        []{#timePerfStatsEvent(com.facebook.buck.event.listener.PerfTimesEventListener.PerfTimesEvent)}

        -   #### timePerfStatsEvent

            ``` methodSignature
            public void timePerfStatsEvent​(PerfTimesEventListener.PerfTimesEvent event)
            ```

        []{#onArtifactCacheEvent(com.facebook.buck.artifact_cache.HttpArtifactCacheEvent.Finished)}

        -   #### onArtifactCacheEvent

            ``` methodSignature
            public void onArtifactCacheEvent​(HttpArtifactCacheEvent.Finished event)
            ```

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
