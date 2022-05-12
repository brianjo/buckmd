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
-   Package
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Package com.facebook.buck.event.listener {#package-com.facebook.buck.event.listener .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [CriticalP                        | ::: block                         |
    | athReportableNode](CriticalPathRe | Critical Path Reportable node     |
    | portableNode.html "interface in c | that is used to store information |
    | om.facebook.buck.event.listener") | into report table                 |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [FileSerializa                    | ::: block                         |
    | tionOutputRuleDepsListener.RuleEx | Data object that is used to       |
    | ecutionTimeData](FileSerializatio | serialize rule execution          |
    | nOutputRuleDepsListener.RuleExecu | information into a file           |
    | tionTimeData.html "interface in c | :::                               |
    | om.facebook.buck.event.listener") |                                   |
    +-----------------------------------+-----------------------------------+
    | [MultiStateRenderer](MultiS       |                                   |
    | tateRenderer.html "interface in c |                                   |
    | om.facebook.buck.event.listener") |                                   |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [AbstractConsole                  | ::: block                         |
    | EventBusListener](AbstractConsole | Base class for                    |
    | EventBusListener.html "class in c | [`BuckEventListener`](            |
    | om.facebook.buck.event.listener") | ../BuckEventListener.html "interf |
    |                                   | ace in com.facebook.buck.event")s |
    |                                   | responsible for outputting        |
    |                                   | information about the running     |
    |                                   | build to `stderr`.                |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuckEventOrderer](Buc            | ::: block                         |
    | kEventOrderer.html "class in com. | Orders                            |
    | facebook.buck.event.listener")\<T | [`Buck                            |
    | extends                           | Event`](../BuckEvent.html "interf |
    | [Buck                             | ace in com.facebook.buck.event")s |
    | Event](../BuckEvent.html "interfa | by the                            |
    | ce in com.facebook.buck.event")\> | [`BuckEvent.getNanoTime()`]       |
    |                                   | (../BuckEvent.html#getNanoTime()) |
    |                                   | value.                            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildRuleThreadTracker](BuildR   |                                   |
    | uleThreadTracker.html "class in c |                                   |
    | om.facebook.buck.event.listener") |                                   |
    +-----------------------------------+-----------------------------------+
    | [B                                |                                   |
    | uildThreadStateRenderer](BuildThr |                                   |
    | eadStateRenderer.html "class in c |                                   |
    | om.facebook.buck.event.listener") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CacheRateStatsListener](CacheR   | ::: block                         |
    | ateStatsListener.html "class in c | Posts rate-limited cache rate     |
    | om.facebook.buck.event.listener") | update events for the WebSocket   |
    |                                   | to consume.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [C                                | ::: block                         |
    | hromeTraceBuildListener](ChromeTr | Logs events to a json file        |
    | aceBuildListener.html "class in c | formatted to be viewed in Chrome  |
    | om.facebook.buck.event.listener") | Trace View (chrome://tracing).    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Com                              | ::: block                         |
    | monThreadStateRenderer](CommonThr | Renders the per thread            |
    | eadStateRenderer.html "class in c | information line during build     |
    | om.facebook.buck.event.listener") | phase on super console            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Cri                              | ::: block                         |
    | ticalPathEventListener](CriticalP | [`BuckEventListener`]             |
    | athEventListener.html "class in c | (../BuckEventListener.html "inter |
    | om.facebook.buck.event.listener") | face in com.facebook.buck.event") |
    |                                   | that is intended to build         |
    |                                   | Critical path of the build (The   |
    |                                   | longest by time path )            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [FileSerializationEv              | ::: block                         |
    | entBusListener](FileSerialization | [`BuckEventListener`]             |
    | EventBusListener.html "class in c | (../BuckEventListener.html "inter |
    | om.facebook.buck.event.listener") | face in com.facebook.buck.event") |
    |                                   | that subscribes to                |
    |                                   | [`                                |
    |                                   | IndividualTestEvent.Finished`](.. |
    |                                   | /../core/test/event/IndividualTes |
    |                                   | tEvent.Finished.html "class in co |
    |                                   | m.facebook.buck.core.test.event") |
    |                                   | events and serialize them to      |
    |                                   | outputFile in json-format.        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [FileSerializationOutputRuleDeps  | ::: block                         |
    | Listener](FileSerializationOutput | [`BuckEventListener`]             |
    | RuleDepsListener.html "class in c | (../BuckEventListener.html "inter |
    | om.facebook.buck.event.listener") | face in com.facebook.buck.event") |
    |                                   | that subscribes to                |
    |                                   | [`BuildRuleE                      |
    |                                   | xecutionEvent.Finished`](../../co |
    |                                   | re/build/event/BuildRuleExecution |
    |                                   | Event.Finished.html "class in com |
    |                                   | .facebook.buck.core.build.event") |
    |                                   | events and serialize rule build   |
    |                                   | target, rule type, rule execution |
    |                                   | time, rule\'s dependencies to     |
    |                                   | outputFile in csv format.         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HttpArtifactC                    | ::: block                         |
    | acheEventListener](HttpArtifactCa | Listens to                        |
    | cheEventListener.html "class in c | HttpArtifactCacheEvents and logs  |
    | om.facebook.buck.event.listener") | stats data in Hive row format.    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HttpArtifactCac                  | ::: block                         |
    | heUploadListener](HttpArtifactCac | In charge for monitoring builds   |
    | heUploadListener.html "class in c | that store artifacts to the       |
    | om.facebook.buck.event.listener") | remote cache and computing        |
    |                                   | stateful cache upload stats.      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JavaUtilsLo                      | ::: block                         |
    | ggingBuildListener](JavaUtilsLogg | Logs build events to              |
    | ingBuildListener.html "class in c | java.util.logging.                |
    | om.facebook.buck.event.listener") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [LoadB                            |                                   |
    | alancerEventsListener](LoadBalanc |                                   |
    | erEventsListener.html "class in c |                                   |
    | om.facebook.buck.event.listener") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Lo                               |                                   |
    | adBalancerEventsListener.ServerCo |                                   |
    | unters](LoadBalancerEventsListene |                                   |
    | r.ServerCounters.html "class in c |                                   |
    | om.facebook.buck.event.listener") |                                   |
    +-----------------------------------+-----------------------------------+
    | [LoggingBuildListener](Logg       | ::: block                         |
    | ingBuildListener.html "class in c | Log handler to bridge             |
    | om.facebook.buck.event.listener") | BuckEventBus events to            |
    |                                   | java.util.logging records.        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [LogUploaderListener](Log         | ::: block                         |
    | UploaderListener.html "class in c | Upload the buck log file to the   |
    | om.facebook.buck.event.listener") | trace endpoint when the build is  |
    |                                   | finished.                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [MachineRead                      |                                   |
    | ableLoggerListener](MachineReadab |                                   |
    | leLoggerListener.html "class in c |                                   |
    | om.facebook.buck.event.listener") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ParserPro                        |                                   |
    | filerLoggerListener](ParserProfil |                                   |
    | erLoggerListener.html "class in c |                                   |
    | om.facebook.buck.event.listener") |                                   |
    +-----------------------------------+-----------------------------------+
    | [PerfTimesEventListener](PerfTi   |                                   |
    | mesEventListener.html "class in c |                                   |
    | om.facebook.buck.event.listener") |                                   |
    +-----------------------------------+-----------------------------------+
    | [PerfTimesEventListener.Perf      |                                   |
    | TimesEvent](PerfTimesEventListene |                                   |
    | r.PerfTimesEvent.html "class in c |                                   |
    | om.facebook.buck.event.listener") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Pub                              |                                   |
    | licAnnouncementManager](PublicAnn |                                   |
    | ouncementManager.html "class in c |                                   |
    | om.facebook.buck.event.listener") |                                   |
    +-----------------------------------+-----------------------------------+
    | [RemoteExe                        | ::: block                         |
    | cutionStateRenderer](RemoteExecut | A renderer for creating remote    |
    | ionStateRenderer.html "class in c | execution related lines on the    |
    | om.facebook.buck.event.listener") | console.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RenderingConsole](               | ::: block                         |
    | RenderingConsole.html "class in c | A console that supports           |
    | om.facebook.buck.event.listener") | rendering.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RuleK                            |                                   |
    | eyDiagnosticsListener](RuleKeyDia |                                   |
    | gnosticsListener.html "class in c |                                   |
    | om.facebook.buck.event.listener") |                                   |
    +-----------------------------------+-----------------------------------+
    | [RuleKeyLoggerListener](RuleK     |                                   |
    | eyLoggerListener.html "class in c |                                   |
    | om.facebook.buck.event.listener") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ScribeEventListener](Scr         | ::: block                         |
    | ibeEventListener.html "class in c | [`BuckEventListener`]             |
    | om.facebook.buck.event.listener") | (../BuckEventListener.html "inter |
    |                                   | face in com.facebook.buck.event") |
    |                                   | that serializes events to JSON    |
    |                                   | and sends them to Scribe.         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Scr                              | ::: block                         |
    | ibeEventListenerConfig](ScribeEve | Strong-type configuration for     |
    | ntListenerConfig.html "class in c | \[scribe_event_listener\] section |
    | om.facebook.buck.event.listener") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [SilentConso                      | ::: block                         |
    | leEventBusListener](SilentConsole | A special console event listener  |
    | EventBusListener.html "class in c | for the silent case.              |
    | om.facebook.buck.event.listener") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [SimpleConso                      | ::: block                         |
    | leEventBusListener](SimpleConsole | Implementation of                 |
    | EventBusListener.html "class in c | `AbstractConsoleEventBusListener` |
    | om.facebook.buck.event.listener") | for terminals that don\'t support |
    |                                   | ansi.                             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [SuperConsoleConfig](Su           |                                   |
    | perConsoleConfig.html "class in c |                                   |
    | om.facebook.buck.event.listener") |                                   |
    +-----------------------------------+-----------------------------------+
    | [SuperCons                        | ::: block                         |
    | oleEventBusListener](SuperConsole | Console that provides rich,       |
    | EventBusListener.html "class in c | updating ansi output about the    |
    | om.facebook.buck.event.listener") | current build.                    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [TestResultFormatter](Tes         |                                   |
    | tResultFormatter.html "class in c |                                   |
    | om.facebook.buck.event.listener") |                                   |
    +-----------------------------------+-----------------------------------+
    | [TestThreadStateRenderer](TestThr |                                   |
    | eadStateRenderer.html "class in c |                                   |
    | om.facebook.buck.event.listener") |                                   |
    +-----------------------------------+-----------------------------------+
    | [TimeCostEntry](                  | ::: block                         |
    | TimeCostEntry.html "class in com. | Data class for storing the        |
    | facebook.buck.event.listener")\<T | amortized time and total time of  |
    | extends                           | a start/finished event pair.      |
    | [Buck                             | :::                               |
    | Event](../BuckEvent.html "interfa |                                   |
    | ce in com.facebook.buck.event")\> |                                   |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   
      Enum                                                                                                               Description
      ------------------------------------------------------------------------------------------------------------------ -------------
      [TestResultFormatter.FormatMode](TestResultFormatter.FormatMode.html "enum in com.facebook.buck.event.listener")    

      : Enum Summary[ ]{.tabEnd}
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../../index.html)
-   Package
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

[]{#skip.navbar.bottom}
:::
