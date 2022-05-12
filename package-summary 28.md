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
-   Package
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Package com.facebook.buck.event {#package-com.facebook.buck.event .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [BuckEvent](BuckEvent.html "inter |                                   |
    | face in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [BuckE                            | ::: block                         |
    | ventBus](BuckEventBus.html "inter | Thin wrapper around guava event   |
    | face in com.facebook.buck.event") | bus.                              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuckEventListen                  |                                   |
    | er](BuckEventListener.html "inter |                                   |
    | face in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [EventDispat                      | ::: block                         |
    | cher](EventDispatcher.html "inter | Thin wrapper around guava event   |
    | face in com.facebook.buck.event") | bus.                              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [LeafEvent](LeafEvent.html "inter | ::: block                         |
    | face in com.facebook.buck.event") | LeafEvents represent events that  |
    |                                   | have no logical children and are  |
    |                                   | useful for tracking the time buck |
    |                                   | is spending logically grouped by  |
    |                                   | categories, such as Parse, Javac, |
    |                                   | or Dx.                            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RuleKeyCalculationEvent](Ru      | ::: block                         |
    | leKeyCalculationEvent.html "inter | Events used to track time spent   |
    | face in com.facebook.buck.event") | calculating rule keys.            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RuleKeyCalcu                     |                                   |
    | lationEvent.Finished](RuleKeyCalc |                                   |
    | ulationEvent.Finished.html "inter |                                   |
    | face in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [RuleKeyCal                       |                                   |
    | culationEvent.Started](RuleKeyCal |                                   |
    | culationEvent.Started.html "inter |                                   |
    | face in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [SimplePerfEvent.Scope](          | ::: block                         |
    | SimplePerfEvent.Scope.html "inter | Represents the scope within which |
    | face in com.facebook.buck.event") | a particular performance          |
    |                                   | operation is taking place.        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [SimplePerfEvent.Started](Si      |                                   |
    | mplePerfEvent.Started.html "inter |                                   |
    | face in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [WorkAdvanceEv                    | ::: block                         |
    | ent](WorkAdvanceEvent.html "inter | Interface for events that are     |
    | face in com.facebook.buck.event") | only sent out after there was     |
    |                                   | some work done towards completing |
    |                                   | the current command.              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [AbstractBuc                      | ::: block                         |
    | kEvent](AbstractBuckEvent.html "c | Base class for all build events.  |
    | lass in com.facebook.buck.event") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ActionGra                        | ::: block                         |
    | phEvent](ActionGraphEvent.html "c | Base class for events about       |
    | lass in com.facebook.buck.event") | building up the action graph from |
    |                                   | the target graph.                 |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ActionGraphEvent.Cach            |                                   |
    | e](ActionGraphEvent.Cache.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ActionGraphEvent.Cache.Hit](A    |                                   |
    | ctionGraphEvent.Cache.Hit.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ActionGraphEvent.Cache.Miss](Ac  |                                   |
    | tionGraphEvent.Cache.Miss.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ActionGraphEvent.Cache.Mis       |                                   |
    | sWithEmptyCache](ActionGraphEvent |                                   |
    | .Cache.MissWithEmptyCache.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ActionGraphEven                  |                                   |
    | t.Cache.MissWithTargetGraphDiffer |                                   |
    | ence](ActionGraphEvent.Cache.Miss |                                   |
    | WithTargetGraphDifference.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ActionGraphEv                    |                                   |
    | ent.Cache.MissWithTargetGraphHash |                                   |
    | Match](ActionGraphEvent.Cache.Mis |                                   |
    | sWithTargetGraphHashMatch.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ActionGraphEvent.Finished](      |                                   |
    | ActionGraphEvent.Finished.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ActionGr                         | ::: block                         |
    | aphEvent.IncrementalLoad](ActionG | Event for incremental action      |
    | raphEvent.IncrementalLoad.html "c | graph construction.               |
    | lass in com.facebook.buck.event") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ActionGraphEvent.Started]        |                                   |
    | (ActionGraphEvent.Started.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ActionGraphPerfStatEvent]        | ::: block                         |
    | (ActionGraphPerfStatEvent.html "c | Event Class containing the perf   |
    | lass in com.facebook.buck.event") | data regarding action graph       |
    |                                   | building                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Acti                             | ::: block                         |
    | onGraphPerfStatEvent.Start](Actio | Class representing the start of   |
    | nGraphPerfStatEvent.Start.html "c | timing                            |
    | lass in com.facebook.buck.event") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ArtifactCompressionEvent]        | ::: block                         |
    | (ArtifactCompressionEvent.html "c | Event for artifact compression /  |
    | lass in com.facebook.buck.event") | decompression                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ArtifactCo                       | ::: block                         |
    | mpressionEvent.Finished](Artifact | Event for when a artifact         |
    | CompressionEvent.Finished.html "c | finishes                          |
    | lass in com.facebook.buck.event") | compression/decompression         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Artifact                         | ::: block                         |
    | CompressionEvent.Started](Artifac | Event for when a artifact starts  |
    | tCompressionEvent.Started.html "c | compression/decompression         |
    | lass in com.facebook.buck.event") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuckIn                           | ::: block                         |
    | itializationDurationEvent](BuckIn | Event that contains the duration  |
    | itializationDurationEvent.html "c | of time Buck took to perform      |
    | lass in com.facebook.buck.event") | initializations before command is |
    |                                   | about to be executed, starting    |
    |                                   | from call to main().              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuckTracingEventBusBridge](      | ::: block                         |
    | BuckTracingEventBusBridge.html "c | Bridges the                       |
    | lass in com.facebook.buck.event") | [`BuckTrac                        |
    |                                   | ing`](api/BuckTracing.html "class |
    |                                   |  in com.facebook.buck.event.api") |
    |                                   | API (in the system ClassLoader)   |
    |                                   | with                              |
    |                                   | [`BuckEve                         |
    |                                   | ntBus`](BuckEventBus.html "interf |
    |                                   | ace in com.facebook.buck.event"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CacheSt                          | ::: block                         |
    | atsEvent](CacheStatsEvent.html "c | BuckEvent for passing cache stats |
    | lass in com.facebook.buck.event") | through the event bus             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [C                                | ::: block                         |
    | ommandEvent](CommandEvent.html "c | Events tracking the start and     |
    | lass in com.facebook.buck.event") | stop of a buck command.           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CommandEvent.Finish              |                                   |
    | ed](CommandEvent.Finished.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CommandEvent.Interrupted]        |                                   |
    | (CommandEvent.Interrupted.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CommandEvent.Star                |                                   |
    | ted](CommandEvent.Started.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CompilerError                    |                                   |
    | Event](CompilerErrorEvent.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CompilerPluginDurationEvent](Co  | ::: block                         |
    | mpilerPluginDurationEvent.html "c | Base class for events being       |
    | lass in com.facebook.buck.event") | reported by plugins to in-process |
    |                                   | compilers such as JSR199 javac.   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CompilerPluginDu                 |                                   |
    | rationEvent.Finished](CompilerPlu |                                   |
    | ginDurationEvent.Finished.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CompilerPlugin                   |                                   |
    | DurationEvent.Started](CompilerPl |                                   |
    | uginDurationEvent.Started.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [C                                | ::: block                         |
    | onsoleEvent](ConsoleEvent.html "c | Event for messages.               |
    | lass in com.facebook.buck.event") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DaemonEvent](DaemonEvent.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Da                               |                                   |
    | emonEvent.NewDaemonInstance](Daem |                                   |
    | onEvent.NewDaemonInstance.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [DefaultBuckEven                  | ::: block                         |
    | tBus](DefaultBuckEventBus.html "c | Thin wrapper around guava event   |
    | lass in com.facebook.buck.event") | bus.                              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [EventKey](EventKey.html "c       | ::: block                         |
    | lass in com.facebook.buck.event") | Used to associate sets of         |
    |                                   | [`B                               |
    |                                   | uckEvent`](BuckEvent.html "interf |
    |                                   | ace in com.facebook.buck.event")s |
    |                                   | with each other.                  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Experim                          |                                   |
    | entEvent](ExperimentEvent.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [FileHashCache                    |                                   |
    | Event](FileHashCacheEvent.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [FileHashCacheEvent.Inv           |                                   |
    | alidationFinished](FileHashCacheE |                                   |
    | vent.InvalidationFinished.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [FileHashCacheEvent.I             |                                   |
    | nvalidationStarted](FileHashCache |                                   |
    | Event.InvalidationStarted.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [FlushConsol                      | ::: block                         |
    | eEvent](FlushConsoleEvent.html "c | Event to tell the console that it |
    | lass in com.facebook.buck.event") | needs to flush now.               |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [I                                |                                   |
    | nstallEvent](InstallEvent.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [InstallEvent.Finish              |                                   |
    | ed](InstallEvent.Finished.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [InstallEvent.Star                |                                   |
    | ted](InstallEvent.Started.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [LeafEvents](LeafEvents.html "c   |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [LeafEvents.SimpleLeafEvent](L    |                                   |
    | eafEvents.SimpleLeafEvent.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [LeafEvents.Sim                   |                                   |
    | pleLeafEvent.Finished](LeafEvents |                                   |
    | .SimpleLeafEvent.Finished.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [LeafEvents.S                     |                                   |
    | impleLeafEvent.Started](LeafEvent |                                   |
    | s.SimpleLeafEvent.Started.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [N                                |                                   |
    | etworkEvent](NetworkEvent.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Networ                           |                                   |
    | kEvent.BytesReceivedEvent](Networ |                                   |
    | kEvent.BytesReceivedEvent.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [P                                |                                   |
    | arsingEvent](ParsingEvent.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Pars                             |                                   |
    | ingEvent.EnvVariableChange](Parsi |                                   |
    | ngEvent.EnvVariableChange.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ParsingE                         |                                   |
    | vent.SymlinkInvalidation](Parsing |                                   |
    | Event.SymlinkInvalidation.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Pro                              |                                   |
    | gressEvent](ProgressEvent.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ProgressEven                     |                                   |
    | t.BuildProgressUpdated](ProgressE |                                   |
    | vent.BuildProgressUpdated.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ProgressEvent.Pa                 |                                   |
    | rsingProgressUpdated](ProgressEve |                                   |
    | nt.ParsingProgressUpdated.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Pro                              |                                   |
    | gressEvent.ProjectGenerationProgr |                                   |
    | essUpdated](ProgressEvent.Project |                                   |
    | GenerationProgressUpdated.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ProjectGenerationEven            |                                   |
    | t](ProjectGenerationEvent.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Projec                           |                                   |
    | tGenerationEvent.Finished](Projec |                                   |
    | tGenerationEvent.Finished.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ProjectG                         |                                   |
    | enerationEvent.Processed](Project |                                   |
    | GenerationEvent.Processed.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Proj                             |                                   |
    | ectGenerationEvent.Started](Proje |                                   |
    | ctGenerationEvent.Started.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [RuleKeyCalculationEven           |                                   |
    | t.DefaultFinished](RuleKeyCalcula |                                   |
    | tionEvent.DefaultFinished.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [RuleKeyCalculationEv             |                                   |
    | ent.DefaultStarted](RuleKeyCalcul |                                   |
    | ationEvent.DefaultStarted.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Ru                               |                                   |
    | leKeyCalculationEvent.Event](Rule |                                   |
    | KeyCalculationEvent.Event.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ScubaData](ScubaData.html "c     |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ScubaData.B                      |                                   |
    | uilder](ScubaData.Builder.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [SimpleP                          | ::: block                         |
    | erfEvent](SimplePerfEvent.html "c | An implementation of              |
    | lass in com.facebook.buck.event") | [`B                               |
    |                                   | uckEvent`](BuckEvent.html "interf |
    |                                   | ace in com.facebook.buck.event")s |
    |                                   | used for gathering performance    |
    |                                   | statistics.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [SimplePerfEvent.Finished]        |                                   |
    | (SimplePerfEvent.Finished.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [SimplePerfEvent.PerfEventId](Si  |                                   |
    | mplePerfEvent.PerfEventId.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [StartActivity                    | ::: block                         |
    | Event](StartActivityEvent.html "c | Events for timing the starting of |
    | lass in com.facebook.buck.event") | android events.                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [StartActivityEvent.Finished](St  |                                   |
    | artActivityEvent.Finished.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [StartActivityEvent.Started](S    |                                   |
    | tartActivityEvent.Started.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ThrowableConsoleEve              | Deprecated.                       |
    | nt](ThrowableConsoleEvent.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Unins                            |                                   |
    | tallEvent](UninstallEvent.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [UninstallEvent.Finished          |                                   |
    | ](UninstallEvent.Finished.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [UninstallEvent.Starte            |                                   |
    | d](UninstallEvent.Started.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [WatchmanStatusE                  |                                   |
    | vent](WatchmanStatusEvent.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Watchman                         |                                   |
    | StatusEvent.FileCreation](Watchma |                                   |
    | nStatusEvent.FileCreation.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Watchman                         |                                   |
    | StatusEvent.FileDeletion](Watchma |                                   |
    | nStatusEvent.FileDeletion.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [                                 |                                   |
    | WatchmanStatusEvent.Finished](Wat |                                   |
    | chmanStatusEvent.Finished.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [                                 |                                   |
    | WatchmanStatusEvent.Overflow](Wat |                                   |
    | chmanStatusEvent.Overflow.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [WatchmanStatusEvent.Started](Wa  |                                   |
    | tchmanStatusEvent.Started.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [WatchmanStatus                   | ::: block                         |
    | Event.ZeroFileChanges](WatchmanSt | This event is to be posted when   |
    | atusEvent.ZeroFileChanges.html "c | Watchman does not report any      |
    | lass in com.facebook.buck.event") | altered files.                    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Enum                              | Description                       |
    +===================================+===================================+
    | [ArtifactCom                      |                                   |
    | pressionEvent.Operation](Artifact |                                   |
    | CompressionEvent.Operation.html " |                                   |
    | enum in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Compi                            |                                   |
    | lerErrorEvent.CompilerType](Compi |                                   |
    | lerErrorEvent.CompilerType.html " |                                   |
    | enum in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Lo                               | ::: block                         |
    | gUploadMode](LogUploadMode.html " | Whether and when to upload logs.  |
    | enum in com.facebook.buck.event") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RuleKeyCalculationEvent.Type](Ru |                                   |
    | leKeyCalculationEvent.Type.html " |                                   |
    | enum in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [SimplePerfEvent.                 |                                   |
    | Type](SimplePerfEvent.Type.html " |                                   |
    | enum in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+

    : Enum Summary[ ]{.tabEnd}
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../index.html)
-   Package
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

[]{#skip.navbar.bottom}
:::
