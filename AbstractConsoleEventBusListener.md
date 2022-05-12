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
-   [Field](#field.detail) \| 
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

## Class AbstractConsoleEventBusListener {#class-abstractconsoleeventbuslistener .title title="Class AbstractConsoleEventBusListener"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.event.listener.AbstractConsoleEventBusListener

::: description
-   

    All Implemented Interfaces:
    :   `BuckEventListener`, `Closeable`, `AutoCloseable`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `SilentConsoleEventBusListener`,
        `SimpleConsoleEventBusListener`, `SuperConsoleEventBusListener`

    ------------------------------------------------------------------------

        public abstract class AbstractConsoleEventBusListener
        extends Object
        implements BuckEventListener

    ::: block
    Base class for
    [`BuckEventListener`](../BuckEventListener.html "interface in com.facebook.buck.event")s
    responsible for outputting information about the running build to
    `stderr`.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `protected            | `actionGraphEvents`   |                       |
        | ConcurrentHashMap<Eve |                       |                       |
        | ntKey,​EventInterval>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected Concurr    | `actionGraphFinished` |                       |
        | entLinkedDeque<Action |                       |                       |
        | GraphEvent.Finished>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected Concur     | `actionGraphStarted`  |                       |
        | rentLinkedDeque<Actio |                       |                       |
        | nGraphEvent.Started>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected Ansi`      | `ansi`                |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected com.g      | `                     | ::: block             |
        | oogle.common.collect. | buildDetailsCommands` | Commands that should  |
        | ImmutableSet<String>` |                       | print out the build   |
        |                       |                       | details, if provided  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected            | `buildFinished`       |                       |
        |  BuildEvent.Finished` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected Bu         | `bu                   |                       |
        | ildRuleThreadTracker` | ildRuleThreadTracker` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protecte             | `buildStarted`        |                       |
        | d BuildEvent.Started` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected Clock`     | `clock`               |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected C          | `commandFinished`     |                       |
        | ommandEvent.Finished` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protec               | `console`             |                       |
        | ted RenderingConsole` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected I          | `installFinished`     |                       |
        | nstallEvent.Finished` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected            | `installStarted`      |                       |
        | InstallEvent.Started` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected            | `networkStatsTracker` |                       |
        |  NetworkStatsTracker` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `pro                  | `numRulesCompleted`   |                       |
        | tected AtomicInteger` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protect              | `parseStats`          |                       |
        | ed ParseStatsTracker` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected Optiona    | `progressEstimator`   |                       |
        | l<ProgressEstimator>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `proje                |                       |
        | protected ProjectGene | ctGenerationFinished` |                       |
        | rationEvent.Finished` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected ProjectGen | `proj                 |                       |
        | erationEvent.Started` | ectGenerationStarted` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protec               | `publicAnnouncements` |                       |
        | ted Optional<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `p                    | `ruleCount`           |                       |
        | rotected OptionalInt` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `p                    | `U                    |                       |
        | rotected static long` | NFINISHED_EVENT_PAIR` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected Verbosity` | `verbosity`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected Watchman   | `watchmanFinished`    |                       |
        | StatusEvent.Finished` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected Watchma    | `watchmanStarted`     |                       |
        | nStatusEvent.Started` |                       |                       |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `AbstractConsoleEventBusListener​(RenderingConsole console,                                Clock clock,                                Locale locale,                                ExecutionEnvironment executionEnvironment,                                boolean showTextInAllCaps,                                int numberOfSlowRulesToShow,                                boolean showSlowRulesInConsole,                                com.google.common.collect.ImmutableSet<String> buildDetailsCommands)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `actionGraphFin       |                       |
        |                       | ished​(ActionGraphEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `actionGraph          |                       |
        |                       | Started​(ActionGraphEv |                       |
        |                       | ent.Started started)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected boolean`   | `addLineFromEventIn   | ::: block             |
        |                       | terval​(String prefix, | Adds a line about an  |
        |                       |                       | [`Event               |
        |                       |     Optional<String>  | Interval`](util/Event |
        |                       | suffix,               | Interval.html "class  |
        |                       |            long curre | in com.facebook.buck. |
        |                       | ntMillis,             | event.listener.util") |
        |                       |              EventInt | to lines.             |
        |                       | erval startAndFinish, | :::                   |
        |                       |                       |                       |
        |                       |     ProgressEstimatio |                       |
        |                       | n progress,           |                       |
        |                       |                Option |                       |
        |                       | al<Long> minimum,     |                       |
        |                       |                       |                       |
        |                       | com.google.common.col |                       |
        |                       | lect.ImmutableList.Bu |                       |
        |                       | ilder<String> lines)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected boolean`   | `ad                   | ::: block             |
        |                       | dLineFromEvents​(Strin | Adds a line about a   |
        |                       | g prefix,             | set of start and      |
        |                       |       Optional<String | finished events to    |
        |                       | > suffix,             | lines.                |
        |                       |       long currentMil | :::                   |
        |                       | lis,                  |                       |
        |                       |  Collection<EventInte |                       |
        |                       | rval> eventIntervals, |                       |
        |                       |                   Pro |                       |
        |                       | gressEstimation progr |                       |
        |                       | ess,                  |                       |
        |                       |  Optional<Long> minim |                       |
        |                       | um,                   |                       |
        |                       | com.google.common.col |                       |
        |                       | lect.ImmutableList.Bu |                       |
        |                       | ilder<String> lines)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `aggrega              |                       |
        |                       | teFinishedEvent​(Concu |                       |
        |                       | rrentHashMap<EventKey |                       |
        |                       | ,​EventInterval> map,  |                       |
        |                       |                       |                       |
        |                       |  BuckEvent finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `aggr                 |                       |
        |                       | egateStartedEvent​(Con |                       |
        |                       | currentHashMap<EventK |                       |
        |                       | ey,​EventInterval> map |                       |
        |                       | ,                     |                       |
        |                       |   BuckEvent started)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `bu                   |                       |
        |                       | ildFinished​(BuildEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `buildRuleF           |                       |
        |                       | inished​(BuildRuleEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `buildRu              |                       |
        |                       | leResumed​(BuildRuleEv |                       |
        |                       | ent.Resumed resumed)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `buildRu              |                       |
        |                       | leStarted​(BuildRuleEv |                       |
        |                       | ent.Started started)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `buildRuleSusp        |                       |
        |                       | ended​(BuildRuleEvent. |                       |
        |                       | Suspended suspended)` |                       |
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
        | `void`                | `com                  |                       |
        |                       | mandFinished​(CommandE |                       |
        |                       | vent.Finished event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `commandStarte        |                       |
        |                       | dEvent​(CommandEvent.S |                       |
        |                       | tarted startedEvent)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected String`    | `convertToAllCaps     |                       |
        |                       | IfNeeded​(String str)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `display              |                       |
        |                       | sEstimatedProgress()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected com.go     | `                     | ::: block             |
        | ogle.common.collect.I | formatConsoleEvent​(Co | Formats a             |
        | mmutableList<String>` | nsoleEvent logEvent)` | [`ConsoleE            |
        |                       |                       | vent`](../ConsoleEven |
        |                       |                       | t.html "class in com. |
        |                       |                       | facebook.buck.event") |
        |                       |                       | and adds it to        |
        |                       |                       | `lines`.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected String`    | `formatElapsedTime    |                       |
        |                       | ​(long elapsedTimeMs)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protec               | `getApprox            |                       |
        | ted Optional<Double>` | imateBuildProgress()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `g                    |                       |
        |                       | etBuildDetailsLine​(Bu |                       |
        |                       | ildId buildId,        |                       |
        |                       |              String b |                       |
        |                       | uildDetailsTemplate)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `getBuildLogL         |                       |
        |                       | ine​(BuildId buildId)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protecte             | `ge                   |                       |
        | d ProgressEstimation` | tEstimatedProgressOfC |                       |
        |                       | reatingActionGraph()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protec               | `getEs                |                       |
        | ted Optional<Double>` | timatedProgressOfGene |                       |
        |                       | ratingProjectFiles()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protecte             | `getEstimatedProgress |                       |
        | d ProgressEstimation` | OfParsingBuckFiles()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `p                    | `getEve               | ::: block             |
        | rotected static Colle | ntsBetween​(long start | Filter a list of      |
        | ction<EventInterval>` | ,                 lon | events and return the |
        |                       | g end,                | subset that fall      |
        |                       |   Iterable<EventInter | between the given     |
        |                       | val> eventIntervals)` | start and end         |
        |                       |                       | timestamps.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected String`    | `getNetworkSta        |                       |
        |                       | tsLine​(BuildEvent.Fin |                       |
        |                       | ished finishedEvent)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protec               | `getOptio             |                       |
        | ted Optional<String>` | nalBuildLineSuffix()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `p                    | `getTotalCompletedTi  | ::: block             |
        | rotected static long` | meFromEventIntervals​( | Get the summed        |
        |                       | Collection<EventInter | elapsed time from all |
        |                       | val> eventIntervals)` | matched event pairs.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `p                    | `getWork              | ::: block             |
        | rotected static long` | ingTimeFromLastStartU | [Deprecate            |
        |                       | ntilNow​(Collection<Ev | d.]{.deprecatedLabel} |
        |                       | entInterval> eventInt | :::                   |
        |                       | ervals,               |                       |
        |                       |                       |                       |
        |                       |  long currentMillis)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `instal               |                       |
        |                       | lFinished​(InstallEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `ins                  |                       |
        |                       | tallStarted​(InstallEv |                       |
        |                       | ent.Started started)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected long`      | `log                  | ::: block             |
        |                       | EventInterval​(String  | Adds a line about a   |
        |                       | prefix,               | pair of start and     |
        |                       |    Optional<String> s | finished events to    |
        |                       | uffix,                | lines.                |
        |                       |   long currentMillis, | :::                   |
        |                       |                  long |                       |
        |                       |  offsetMs,            |                       |
        |                       |       BuckEvent start |                       |
        |                       | Event,                |                       |
        |                       |   BuckEvent finishedE |                       |
        |                       | vent,                 |                       |
        |                       |  Optional<Double> pro |                       |
        |                       | gress,                |                       |
        |                       |   Optional<Long> mini |                       |
        |                       | mum,                  |                       |
        |                       | com.google.common.col |                       |
        |                       | lect.ImmutableList.Bu |                       |
        |                       | ilder<String> lines)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected long`      | `log                  | ::: block             |
        |                       | EventInterval​(String  | [Deprecate            |
        |                       | prefix,               | d.]{.deprecatedLabel} |
        |                       |    Optional<String> s | :::                   |
        |                       | uffix,                |                       |
        |                       |   long currentMillis, |                       |
        |                       |                  long |                       |
        |                       |  offsetMs,            |                       |
        |                       |       Collection<Even |                       |
        |                       | tInterval> eventInter |                       |
        |                       | vals,                 |                       |
        |                       |  Optional<Double> pro |                       |
        |                       | gress,                |                       |
        |                       |   Optional<Long> mini |                       |
        |                       | mum,                  |                       |
        |                       | com.google.common.col |                       |
        |                       | lect.ImmutableList.Bu |                       |
        |                       | ilder<String> lines)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected void`      | `logHttpCacheUploads​( | ::: block             |
        |                       | com.google.common.col | Adds a line about a   |
        |                       | lect.ImmutableList.Bu | the state of cache    |
        |                       | ilder<String> lines)` | uploads to lines.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract void`       | `printSevereWarningD  |                       |
        |                       | irectly​(String line)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `proje                |                       |
        |                       | ctGenerationFinished​( |                       |
        |                       | ProjectGenerationEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `projectGenerat       |                       |
        |                       | ionProcessedTarget​(Pr |                       |
        |                       | ojectGenerationEvent. |                       |
        |                       | Processed processed)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `pr                   |                       |
        |                       | ojectGenerationStarte |                       |
        |                       | d​(ProjectGenerationEv |                       |
        |                       | ent.Started started)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `register​(BuckEve     |                       |
        |                       | ntBus buildEventBus)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected String`    | `r                    | ::: block             |
        |                       | enderRemoteUploads()` | A method to print the |
        |                       |                       | line responsible to   |
        |                       |                       | show how our remote   |
        |                       |                       | cache upload goes.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `                     |                       |
        |                       | ruleCountCalculated​(B |                       |
        |                       | uildEvent.RuleCountCa |                       |
        |                       | lculated calculated)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `                     |                       |
        |                       | ruleCountUpdated​(Buil |                       |
        |                       | dEvent.UnskippedRuleC |                       |
        |                       | ountUpdated updated)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `setProgr             |                       |
        |                       | essEstimator​(Progress |                       |
        |                       | Estimator estimator)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `setPublicAnnounc     |                       |
        |                       | ements​(BuckEventBus e |                       |
        |                       | ventBus,              |                       |
        |                       |           Optional<St |                       |
        |                       | ring> announcements)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `testRule             |                       |
        |                       | Finished​(TestRuleEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `testR                |                       |
        |                       | uleStarted​(TestRuleEv |                       |
        |                       | ent.Started started)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `watchmanFinish       |                       |
        |                       | ed​(WatchmanStatusEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `watchmanSta          |                       |
        |                       | rted​(WatchmanStatusEv |                       |
        |                       | ent.Started started)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4
        .tableTab}[[Deprecated
        Methods](javascript:show(32);)[ ]{.tabEnd}]{#t6 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#UNFINISHED_EVENT_PAIR}

        -   #### UNFINISHED_EVENT_PAIR

                protected static final long UNFINISHED_EVENT_PAIR

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.event.listener.AbstractConsoleEventBusListener.UNFINISHED_EVENT_PAIR)

        []{#console}

        -   #### console

                protected final RenderingConsole console

        []{#clock}

        -   #### clock

                protected final Clock clock

        []{#verbosity}

        -   #### verbosity

                protected final Verbosity verbosity

        []{#ansi}

        -   #### ansi

                protected final Ansi ansi

        []{#projectGenerationStarted}

        -   #### projectGenerationStarted

                @Nullable
                protected volatile ProjectGenerationEvent.Started projectGenerationStarted

        []{#projectGenerationFinished}

        -   #### projectGenerationFinished

                @Nullable
                protected volatile ProjectGenerationEvent.Finished projectGenerationFinished

        []{#watchmanStarted}

        -   #### watchmanStarted

                @Nullable
                protected volatile WatchmanStatusEvent.Started watchmanStarted

        []{#watchmanFinished}

        -   #### watchmanFinished

                @Nullable
                protected volatile WatchmanStatusEvent.Finished watchmanFinished

        []{#actionGraphStarted}

        -   #### actionGraphStarted

                protected ConcurrentLinkedDeque<ActionGraphEvent.Started> actionGraphStarted

        []{#actionGraphFinished}

        -   #### actionGraphFinished

                protected ConcurrentLinkedDeque<ActionGraphEvent.Finished> actionGraphFinished

        []{#actionGraphEvents}

        -   #### actionGraphEvents

                protected ConcurrentHashMap<EventKey,​EventInterval> actionGraphEvents

        []{#buildStarted}

        -   #### buildStarted

                @Nullable
                protected volatile BuildEvent.Started buildStarted

        []{#buildFinished}

        -   #### buildFinished

                @Nullable
                protected volatile BuildEvent.Finished buildFinished

        []{#installStarted}

        -   #### installStarted

                @Nullable
                protected volatile InstallEvent.Started installStarted

        []{#installFinished}

        -   #### installFinished

                @Nullable
                protected volatile InstallEvent.Finished installFinished

        []{#commandFinished}

        -   #### commandFinished

                @Nullable
                protected volatile CommandEvent.Finished commandFinished

        []{#ruleCount}

        -   #### ruleCount

                protected volatile OptionalInt ruleCount

        []{#publicAnnouncements}

        -   #### publicAnnouncements

                protected Optional<String> publicAnnouncements

        []{#numRulesCompleted}

        -   #### numRulesCompleted

                protected final AtomicInteger numRulesCompleted

        []{#progressEstimator}

        -   #### progressEstimator

                protected Optional<ProgressEstimator> progressEstimator

        []{#networkStatsTracker}

        -   #### networkStatsTracker

                protected final NetworkStatsTracker networkStatsTracker

        []{#parseStats}

        -   #### parseStats

                protected final ParseStatsTracker parseStats

        []{#buildRuleThreadTracker}

        -   #### buildRuleThreadTracker

                protected BuildRuleThreadTracker buildRuleThreadTracker

        []{#buildDetailsCommands}

        -   #### buildDetailsCommands

                protected final com.google.common.collect.ImmutableSet<String> buildDetailsCommands

            ::: block
            Commands that should print out the build details, if
            provided
            :::
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.event.listener.RenderingConsole,com.facebook.buck.util.timing.Clock,java.util.Locale,com.facebook.buck.util.environment.ExecutionEnvironment,boolean,int,boolean,com.google.common.collect.ImmutableSet)}

        -   #### AbstractConsoleEventBusListener

                public AbstractConsoleEventBusListener​(RenderingConsole console,
                                                       Clock clock,
                                                       Locale locale,
                                                       ExecutionEnvironment executionEnvironment,
                                                       boolean showTextInAllCaps,
                                                       int numberOfSlowRulesToShow,
                                                       boolean showSlowRulesInConsole,
                                                       com.google.common.collect.ImmutableSet<String> buildDetailsCommands)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#register(com.facebook.buck.event.BuckEventBus)}

        -   #### register

            ``` methodSignature
            public void register​(BuckEventBus buildEventBus)
            ```

        []{#getBuildDetailsLine(com.facebook.buck.core.model.BuildId,java.lang.String)}

        -   #### getBuildDetailsLine

            ``` methodSignature
            public static String getBuildDetailsLine​(BuildId buildId,
                                                     String buildDetailsTemplate)
            ```

        []{#getBuildLogLine(com.facebook.buck.core.model.BuildId)}

        -   #### getBuildLogLine

            ``` methodSignature
            public static String getBuildLogLine​(BuildId buildId)
            ```

        []{#displaysEstimatedProgress()}

        -   #### displaysEstimatedProgress

            ``` methodSignature
            public boolean displaysEstimatedProgress()
            ```

        []{#setProgressEstimator(com.facebook.buck.event.listener.util.ProgressEstimator)}

        -   #### setProgressEstimator

            ``` methodSignature
            public void setProgressEstimator​(ProgressEstimator estimator)
            ```

        []{#formatElapsedTime(long)}

        -   #### formatElapsedTime

            ``` methodSignature
            protected String formatElapsedTime​(long elapsedTimeMs)
            ```

        []{#getApproximateBuildProgress()}

        -   #### getApproximateBuildProgress

            ``` methodSignature
            protected Optional<Double> getApproximateBuildProgress()
            ```

        []{#getEstimatedProgressOfGeneratingProjectFiles()}

        -   #### getEstimatedProgressOfGeneratingProjectFiles

            ``` methodSignature
            protected Optional<Double> getEstimatedProgressOfGeneratingProjectFiles()
            ```

        []{#getEstimatedProgressOfParsingBuckFiles()}

        -   #### getEstimatedProgressOfParsingBuckFiles

            ``` methodSignature
            protected ProgressEstimation getEstimatedProgressOfParsingBuckFiles()
            ```

            [Returns:]{.returnLabel}
            :   Estimated progress of parsing files stage.

        []{#getEstimatedProgressOfCreatingActionGraph()}

        -   #### getEstimatedProgressOfCreatingActionGraph

            ``` methodSignature
            protected ProgressEstimation getEstimatedProgressOfCreatingActionGraph()
            ```

            [Returns:]{.returnLabel}
            :   Estimated progress of parsing files stage.

        []{#setPublicAnnouncements(com.facebook.buck.event.BuckEventBus,java.util.Optional)}

        -   #### setPublicAnnouncements

            ``` methodSignature
            public void setPublicAnnouncements​(BuckEventBus eventBus,
                                               Optional<String> announcements)
            ```

        []{#printSevereWarningDirectly(java.lang.String)}

        -   #### printSevereWarningDirectly

            ``` methodSignature
            public abstract void printSevereWarningDirectly​(String line)
            ```

        []{#getEventsBetween(long,long,java.lang.Iterable)}

        -   #### getEventsBetween

            ``` methodSignature
            protected static Collection<EventInterval> getEventsBetween​(long start,
                                                                        long end,
                                                                        Iterable<EventInterval> eventIntervals)
            ```

            ::: block
            Filter a list of events and return the subset that fall
            between the given start and end timestamps. Preserves
            ordering if the given iterable was ordered. Will replace
            event pairs that straddle the boundary with
            `com.facebook.buck.event.listener.ProxyBuckEvent` instances,
            so that the resulting collection is strictly contained
            within the boundaries.
            :::

            [Parameters:]{.paramLabel}
            :   `start` - the start timestamp (inclusive)
            :   `end` - the end timestamp (also inclusive)
            :   `eventIntervals` - the events to filter.

            [Returns:]{.returnLabel}
            :   a list of all events from the given iterable that fall
                between the given start and end times. If an event
                straddles the given start or end, it will be replaced
                with a proxy event pair that cuts off at exactly the
                start or end.

        []{#convertToAllCapsIfNeeded(java.lang.String)}

        -   #### convertToAllCapsIfNeeded

            ``` methodSignature
            protected String convertToAllCapsIfNeeded​(String str)
            ```

        []{#logEventInterval(java.lang.String,java.util.Optional,long,long,com.facebook.buck.event.BuckEvent,com.facebook.buck.event.BuckEvent,java.util.Optional,java.util.Optional,com.google.common.collect.ImmutableList.Builder)}

        -   #### logEventInterval

            ``` methodSignature
            protected long logEventInterval​(String prefix,
                                            Optional<String> suffix,
                                            long currentMillis,
                                            long offsetMs,
                                            @Nullable
                                            BuckEvent startEvent,
                                            @Nullable
                                            BuckEvent finishedEvent,
                                            Optional<Double> progress,
                                            Optional<Long> minimum,
                                            com.google.common.collect.ImmutableList.Builder<String> lines)
            ```

            ::: block
            Adds a line about a pair of start and finished events to
            lines.
            :::

            [Parameters:]{.paramLabel}
            :   `prefix` - Prefix to print for this event pair.
            :   `suffix` - Suffix to print for this event pair.
            :   `currentMillis` - The current time in milliseconds.
            :   `offsetMs` - Offset to remove from calculated time. Set
                this to a non-zero value if the event pair would contain
                another event. For example, build time includes parse
                time, but to make the events easier to reason about it
                makes sense to pull parse time out of build time.
            :   `startEvent` - The started event.
            :   `finishedEvent` - The finished event.
            :   `lines` - The builder to append lines to.

            [Returns:]{.returnLabel}
            :   The amount of time between start and finished if
                finished is present, otherwise
                [`UNFINISHED_EVENT_PAIR`](#UNFINISHED_EVENT_PAIR).

        []{#logHttpCacheUploads(com.google.common.collect.ImmutableList.Builder)}

        -   #### logHttpCacheUploads

            ``` methodSignature
            protected void logHttpCacheUploads​(com.google.common.collect.ImmutableList.Builder<String> lines)
            ```

            ::: block
            Adds a line about a the state of cache uploads to lines.
            :::

            [Parameters:]{.paramLabel}
            :   `lines` - The builder to append lines to.

        []{#addLineFromEvents(java.lang.String,java.util.Optional,long,java.util.Collection,com.facebook.buck.event.listener.util.ProgressEstimation,java.util.Optional,com.google.common.collect.ImmutableList.Builder)}

        -   #### addLineFromEvents

            ``` methodSignature
            protected boolean addLineFromEvents​(String prefix,
                                                Optional<String> suffix,
                                                long currentMillis,
                                                Collection<EventInterval> eventIntervals,
                                                ProgressEstimation progress,
                                                Optional<Long> minimum,
                                                com.google.common.collect.ImmutableList.Builder<String> lines)
            ```

            ::: block
            Adds a line about a set of start and finished events to
            lines.
            :::

            [Parameters:]{.paramLabel}
            :   `prefix` - Prefix to print for this event pair.
            :   `suffix` - Suffix to print for this event pair.
            :   `currentMillis` - The current time in milliseconds.
            :   `eventIntervals` - the collection of start/end events to
                measure elapsed time.
            :   `lines` - The builder to append lines to.

            [Returns:]{.returnLabel}
            :   True if all events are finished, false otherwise

        []{#addLineFromEventInterval(java.lang.String,java.util.Optional,long,com.facebook.buck.event.listener.util.EventInterval,com.facebook.buck.event.listener.util.ProgressEstimation,java.util.Optional,com.google.common.collect.ImmutableList.Builder)}

        -   #### addLineFromEventInterval

            ``` methodSignature
            protected boolean addLineFromEventInterval​(String prefix,
                                                       Optional<String> suffix,
                                                       long currentMillis,
                                                       EventInterval startAndFinish,
                                                       ProgressEstimation progress,
                                                       Optional<Long> minimum,
                                                       com.google.common.collect.ImmutableList.Builder<String> lines)
            ```

            ::: block
            Adds a line about an
            [`EventInterval`](util/EventInterval.html "class in com.facebook.buck.event.listener.util")
            to lines.
            :::

            [Parameters:]{.paramLabel}
            :   `prefix` - Prefix to print for this event pair.
            :   `suffix` - Suffix to print for this event pair.
            :   `currentMillis` - The current time in milliseconds.
            :   `startAndFinish` - the event interval to measure elapsed
                time.
            :   `lines` - The builder to append lines to.

            [Returns:]{.returnLabel}
            :   True if all events are finished, false otherwise

        []{#logEventInterval(java.lang.String,java.util.Optional,long,long,java.util.Collection,java.util.Optional,java.util.Optional,com.google.common.collect.ImmutableList.Builder)}

        -   #### logEventInterval

            ``` methodSignature
            @Deprecated
            protected long logEventInterval​(String prefix,
                                            Optional<String> suffix,
                                            long currentMillis,
                                            long offsetMs,
                                            Collection<EventInterval> eventIntervals,
                                            Optional<Double> progress,
                                            Optional<Long> minimum,
                                            com.google.common.collect.ImmutableList.Builder<String> lines)
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            ::: block
            Adds a line about a set of start and finished events to
            lines.
            :::

            [Parameters:]{.paramLabel}
            :   `prefix` - Prefix to print for this event pair.
            :   `suffix` - Suffix to print for this event pair.
            :   `currentMillis` - The current time in milliseconds.
            :   `offsetMs` - Offset to remove from calculated time. Set
                this to a non-zero value if the event pair would contain
                another event. For example, build time includes parse
                time, but to make the events easier to reason about it
                makes sense to pull parse time out of build time.
            :   `eventIntervals` - the collection of start/end events to
                sum up when calculating elapsed time.
            :   `lines` - The builder to append lines to.

            [Returns:]{.returnLabel}
            :   The summed time between start and finished events if
                each start event has a matching finished event,
                otherwise
                [`UNFINISHED_EVENT_PAIR`](#UNFINISHED_EVENT_PAIR).

        []{#getWorkingTimeFromLastStartUntilNow(java.util.Collection,long)}

        -   #### getWorkingTimeFromLastStartUntilNow

            ``` methodSignature
            @Deprecated
            protected static long getWorkingTimeFromLastStartUntilNow​(Collection<EventInterval> eventIntervals,
                                                                      long currentMillis)
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            ::: block
            Takes a collection of start and finished events. If there
            are any events that have a start, but no finished time, the
            collection is considered ongoing.
            :::

            [Parameters:]{.paramLabel}
            :   `eventIntervals` - the collection of event starts/stops.
            :   `currentMillis` - the current time.

            [Returns:]{.returnLabel}
            :   -1 if all events are completed, otherwise the time
                elapsed between the latest event and currentMillis.

        []{#getTotalCompletedTimeFromEventIntervals(java.util.Collection)}

        -   #### getTotalCompletedTimeFromEventIntervals

            ``` methodSignature
            protected static long getTotalCompletedTimeFromEventIntervals​(Collection<EventInterval> eventIntervals)
            ```

            ::: block
            Get the summed elapsed time from all matched event pairs.
            Does not consider unmatched event pairs. Pairs are
            determined by their
            [`EventKey`](../EventKey.html "class in com.facebook.buck.event").
            :::

            [Parameters:]{.paramLabel}
            :   `eventIntervals` - a set of paired events (incomplete
                events are okay).

            [Returns:]{.returnLabel}
            :   the sum of all times between matched event pairs.

        []{#formatConsoleEvent(com.facebook.buck.event.ConsoleEvent)}

        -   #### formatConsoleEvent

            ``` methodSignature
            protected com.google.common.collect.ImmutableList<String> formatConsoleEvent​(ConsoleEvent logEvent)
            ```

            ::: block
            Formats a
            [`ConsoleEvent`](../ConsoleEvent.html "class in com.facebook.buck.event")
            and adds it to `lines`.
            :::

        []{#commandStartedEvent(com.facebook.buck.event.CommandEvent.Started)}

        -   #### commandStartedEvent

            ``` methodSignature
            public void commandStartedEvent​(CommandEvent.Started startedEvent)
            ```

        []{#aggregateStartedEvent(java.util.concurrent.ConcurrentHashMap,com.facebook.buck.event.BuckEvent)}

        -   #### aggregateStartedEvent

            ``` methodSignature
            public static void aggregateStartedEvent​(ConcurrentHashMap<EventKey,​EventInterval> map,
                                                     BuckEvent started)
            ```

        []{#aggregateFinishedEvent(java.util.concurrent.ConcurrentHashMap,com.facebook.buck.event.BuckEvent)}

        -   #### aggregateFinishedEvent

            ``` methodSignature
            public static void aggregateFinishedEvent​(ConcurrentHashMap<EventKey,​EventInterval> map,
                                                      BuckEvent finished)
            ```

        []{#projectGenerationStarted(com.facebook.buck.event.ProjectGenerationEvent.Started)}

        -   #### projectGenerationStarted

            ``` methodSignature
            public void projectGenerationStarted​(ProjectGenerationEvent.Started started)
            ```

        []{#projectGenerationProcessedTarget(com.facebook.buck.event.ProjectGenerationEvent.Processed)}

        -   #### projectGenerationProcessedTarget

            ``` methodSignature
            public void projectGenerationProcessedTarget​(ProjectGenerationEvent.Processed processed)
            ```

        []{#projectGenerationFinished(com.facebook.buck.event.ProjectGenerationEvent.Finished)}

        -   #### projectGenerationFinished

            ``` methodSignature
            public void projectGenerationFinished​(ProjectGenerationEvent.Finished finished)
            ```

        []{#watchmanStarted(com.facebook.buck.event.WatchmanStatusEvent.Started)}

        -   #### watchmanStarted

            ``` methodSignature
            public void watchmanStarted​(WatchmanStatusEvent.Started started)
            ```

        []{#watchmanFinished(com.facebook.buck.event.WatchmanStatusEvent.Finished)}

        -   #### watchmanFinished

            ``` methodSignature
            public void watchmanFinished​(WatchmanStatusEvent.Finished finished)
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

        []{#buildStarted(com.facebook.buck.core.build.event.BuildEvent.Started)}

        -   #### buildStarted

            ``` methodSignature
            public void buildStarted​(BuildEvent.Started started)
            ```

        []{#ruleCountCalculated(com.facebook.buck.core.build.event.BuildEvent.RuleCountCalculated)}

        -   #### ruleCountCalculated

            ``` methodSignature
            public void ruleCountCalculated​(BuildEvent.RuleCountCalculated calculated)
            ```

        []{#ruleCountUpdated(com.facebook.buck.core.build.event.BuildEvent.UnskippedRuleCountUpdated)}

        -   #### ruleCountUpdated

            ``` methodSignature
            public void ruleCountUpdated​(BuildEvent.UnskippedRuleCountUpdated updated)
            ```

        []{#getOptionalBuildLineSuffix()}

        -   #### getOptionalBuildLineSuffix

            ``` methodSignature
            protected Optional<String> getOptionalBuildLineSuffix()
            ```

        []{#getNetworkStatsLine(com.facebook.buck.core.build.event.BuildEvent.Finished)}

        -   #### getNetworkStatsLine

            ``` methodSignature
            protected String getNetworkStatsLine​(@Nullable
                                                 BuildEvent.Finished finishedEvent)
            ```

        []{#buildRuleStarted(com.facebook.buck.core.build.event.BuildRuleEvent.Started)}

        -   #### buildRuleStarted

            ``` methodSignature
            public void buildRuleStarted​(BuildRuleEvent.Started started)
            ```

        []{#buildRuleResumed(com.facebook.buck.core.build.event.BuildRuleEvent.Resumed)}

        -   #### buildRuleResumed

            ``` methodSignature
            public void buildRuleResumed​(BuildRuleEvent.Resumed resumed)
            ```

        []{#buildRuleSuspended(com.facebook.buck.core.build.event.BuildRuleEvent.Suspended)}

        -   #### buildRuleSuspended

            ``` methodSignature
            public void buildRuleSuspended​(BuildRuleEvent.Suspended suspended)
            ```

        []{#buildRuleFinished(com.facebook.buck.core.build.event.BuildRuleEvent.Finished)}

        -   #### buildRuleFinished

            ``` methodSignature
            public void buildRuleFinished​(BuildRuleEvent.Finished finished)
            ```

        []{#buildFinished(com.facebook.buck.core.build.event.BuildEvent.Finished)}

        -   #### buildFinished

            ``` methodSignature
            public void buildFinished​(BuildEvent.Finished finished)
            ```

        []{#testRuleStarted(com.facebook.buck.test.TestRuleEvent.Started)}

        -   #### testRuleStarted

            ``` methodSignature
            public void testRuleStarted​(TestRuleEvent.Started started)
            ```

        []{#testRuleFinished(com.facebook.buck.test.TestRuleEvent.Finished)}

        -   #### testRuleFinished

            ``` methodSignature
            public void testRuleFinished​(TestRuleEvent.Finished finished)
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

        []{#commandFinished(com.facebook.buck.event.CommandEvent.Finished)}

        -   #### commandFinished

            ``` methodSignature
            public void commandFinished​(CommandEvent.Finished event)
            ```

        []{#renderRemoteUploads()}

        -   #### renderRemoteUploads

            ``` methodSignature
            protected String renderRemoteUploads()
            ```

            ::: block
            A method to print the line responsible to show how our
            remote cache upload goes.
            :::

            [Returns:]{.returnLabel}
            :   the line

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

            [Throws:]{.throwsLabel}
            :   `IOException`
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
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
