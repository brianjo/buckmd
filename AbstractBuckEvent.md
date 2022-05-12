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
[Package]{.packageLabelInType} [com.facebook.buck.event](package-summary.html)
:::

## Class AbstractBuckEvent {#class-abstractbuckevent .title title="Class AbstractBuckEvent"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.event.AbstractBuckEvent

::: description
-   

    All Implemented Interfaces:
    :   `BuckEvent`, `BuckEventExternalInterface`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `ActionGraphEvent`, `ActionGraphPerfStatEvent`,
        `AnnotationProcessingEvent`, `ArtifactCacheConnectEvent`,
        `ArtifactCacheEvent`, `ArtifactCompressionEvent`,
        `BuckInitializationDurationEvent`, `BuildEvent`,
        `BuildRuleEvent`, `BuildRuleEvent.WillBuildLocally`,
        `BuildRuleExecutionEvent.Event`, `CacheCountersSummaryEvent`,
        `CacheRateStatsKeeper.CacheRateStatsUpdateEvent`,
        `CacheStatsEvent`, `CasBlobDownloadEvent`, `CasBlobUploadEvent`,
        `CommandEvent`, `CompilerErrorEvent`,
        `CompilerPluginDurationEvent`, `ConsoleEvent`,
        `CounterRegistry.AsyncCounterRegistrationEvent`,
        `CountersSnapshotEvent`, `DaemonEvent`, `DownloadEvent`,
        `DownloadProgressEvent`, `ExperimentEvent`,
        `ExternalTestRunEvent`, `ExternalTestSpecCalculationEvent`,
        `FastVersionControlStatsEvent`, `FileHashCacheEvent`,
        `FinalizingBuildRuleEvent`, `FlushConsoleEvent`,
        `GCCollectionEvent`, `HttpArtifactCacheEvent.Shutdown`,
        `HybridLocalEvent`, `IndividualTestEvent`, `InstallEvent`,
        `JavacPhaseEvent`, `LeafEvents.SimpleLeafEvent`,
        `LoadBalancedServiceEvent`, `LoadBalancerPingEvent`,
        `LocalFallbackEvent`, `NetworkEvent`, `NetworkInfo.Event`,
        `ParseBuckFileEvent`, `ParseBuckProfilerReportEvent`,
        `ParseEvent`, `ParsingEvent`,
        `PerfStatsTracking.PerfStatsEvent`,
        `PerfTimesEventListener.PerfTimesEvent`,
        `ProcessTracker.ProcessResourceConsumptionEvent`,
        `ProgressEvent`, `ProjectBuildFileParseEvents`,
        `ProjectGenerationEvent`, `RemoteBuildRuleExecutionEvent`,
        `RemoteExecutionActionEvent`, `RemoteExecutionSessionEvent`,
        `RuleKeyCacheResultEvent`, `RuleKeyCalculationEvent.Event`,
        `ServerHealthManagerEvent`, `SimplePerfEvent`,
        `StartActivityEvent`, `StepEvent`, `TestRuleEvent`,
        `TestRunEvent`, `TestStatusMessageEvent`, `TestSummaryEvent`,
        `UninstallEvent`, `VersionControlStatsEvent`,
        `VersionedTargetGraphEvent`, `WatchmanDiagnosticEvent`,
        `WatchmanStatusEvent`

    ------------------------------------------------------------------------

        public abstract class AbstractBuckEvent
        extends Object
        implements BuckEvent

    ::: block
    Base class for all build events. Using this makes it easy to add a
    wildcard listener to the event bus.
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
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                              Description
          -------------- ---------------------------------------- -------------
          `protected `   `AbstractBuckEvent​(EventKey eventKey)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `configure​(long       | ::: block             |
        |                       |  timestampMillis,     | Method to configure   |
        |                       |       long nanoTime,  | an event before       |
        |                       |          long threadU | posting it to the     |
        |                       | serNanoTime,          | [`BuckEventB          |
        |                       |  long threadId,       | us`](BuckEventBus.htm |
        |                       |     BuildId buildId)` | l "interface in com.f |
        |                       |                       | acebook.buck.event"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `equals​(Object o)`    | ::: block             |
        |                       |                       | The default           |
        |                       |                       | implementation of     |
        |                       |                       | equals checks to see  |
        |                       |                       | if two events are     |
        |                       |                       | related, are on the   |
        |                       |                       | same thread, and are  |
        |                       |                       | the same concrete     |
        |                       |                       | class.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `BuildId`             | `getBuildId()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `EventKey`            | `getEventKey()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `getNanoTime()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `getThreadId()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `get                  |                       |
        |                       | ThreadUserNanoTime()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `                     |                       |
        |                       | getTimestampMillis()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `prote                | `getValueString()`    |                       |
        | cted abstract String` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isConfigured()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isRelate             |                       |
        |                       | dTo​(BuckEvent event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toLogMessage()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Methods inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `getEventName, storeLastInstanceAndReplayForNewClients`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.event.EventKey)}

        -   #### AbstractBuckEvent

                protected AbstractBuckEvent​(EventKey eventKey)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#configure(long,long,long,long,com.facebook.buck.core.model.BuildId)}

        -   #### configure

            ``` methodSignature
            public void configure​(long timestampMillis,
                                  long nanoTime,
                                  long threadUserNanoTime,
                                  long threadId,
                                  BuildId buildId)
            ```

            ::: block
            Method to configure an event before posting it to the
            [`BuckEventBus`](BuckEventBus.html "interface in com.facebook.buck.event").
            This method should only be invoked once per event, and only
            by the
            [`BuckEventBus`](BuckEventBus.html "interface in com.facebook.buck.event")
            in production code.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `configure` in interface `BuckEvent`

        []{#isConfigured()}

        -   #### isConfigured

            ``` methodSignature
            public boolean isConfigured()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isConfigured` in interface `BuckEvent`

        []{#getTimestampMillis()}

        -   #### getTimestampMillis

            ``` methodSignature
            public long getTimestampMillis()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTimestampMillis` in
                interface `BuckEventExternalInterface`

            [Returns:]{.returnLabel}
            :   the time at which the event has been created, in
                milliseconds.

        []{#getNanoTime()}

        -   #### getNanoTime

            ``` methodSignature
            public long getNanoTime()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNanoTime` in interface `BuckEvent`

        []{#getThreadUserNanoTime()}

        -   #### getThreadUserNanoTime

            ``` methodSignature
            public long getThreadUserNanoTime()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getThreadUserNanoTime` in interface `BuckEvent`

        []{#toLogMessage()}

        -   #### toLogMessage

            ``` methodSignature
            public String toLogMessage()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `toLogMessage` in interface `BuckEvent`

        []{#getThreadId()}

        -   #### getThreadId

            ``` methodSignature
            public long getThreadId()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getThreadId` in interface `BuckEvent`

        []{#getBuildId()}

        -   #### getBuildId

            ``` methodSignature
            public BuildId getBuildId()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildId` in interface `BuckEvent`

            [Returns:]{.returnLabel}
            :   an identifier that distinguishes the build with which
                this event is associated.

        []{#getEventKey()}

        -   #### getEventKey

            ``` methodSignature
            public final EventKey getEventKey()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getEventKey` in interface `BuckEvent`

            [Returns:]{.returnLabel}
            :   key used to determine whether this event is related to
                another event.

        []{#isRelatedTo(com.facebook.buck.event.BuckEvent)}

        -   #### isRelatedTo

            ``` methodSignature
            public final boolean isRelatedTo​(BuckEvent event)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isRelatedTo` in interface `BuckEvent`

            [Returns:]{.returnLabel}

            :   Whether or not this event is related to another event.
                Events are related if they pertain to the same event,
                for example if they are measuring the start and stop of
                some phase. For example,

                       
                        (CommandEvent.started("build")).isRelatedTo(CommandEvent.finished("build")) == true
                        (CommandEvent.started("build")).isRelatedTo(CommandEvent.started("build")) == true
                        (CommandEvent.started("build")).isRelatedTo(CommandEvent.finished("install")) == false
                       
                     

        []{#getValueString()}

        -   #### getValueString

            ``` methodSignature
            protected abstract String getValueString()
            ```

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object o)
            ```

            ::: block
            The default implementation of equals checks to see if two
            events are related, are on the same thread, and are the same
            concrete class. Subclasses therefore can simply override
            isRelatedTo, and the equals method will work correctly.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`
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
