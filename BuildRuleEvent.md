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
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.build.event](package-summary.html)
:::

## Class BuildRuleEvent {#class-buildruleevent .title title="Class BuildRuleEvent"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.event.AbstractBuckEvent](../../../event/AbstractBuckEvent.html "class in com.facebook.buck.event")

    -   -   com.facebook.buck.core.build.event.BuildRuleEvent

::: description
-   

    All Implemented Interfaces:
    :   `BuckEvent`, `BuckEventExternalInterface`, `WorkAdvanceEvent`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `BuildRuleEvent.BeginningBuildRuleEvent`,
        `BuildRuleEvent.EndingBuildRuleEvent`

    ------------------------------------------------------------------------

        public abstract class BuildRuleEvent
        extends AbstractBuckEvent
        implements WorkAdvanceEvent

    ::: block
    Base class for events about build rules.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `BuildRuleEvent.Beg   | ::: block             |
        |                       | inningBuildRuleEvent` | A                     |
        |                       |                       | [                     |
        |                       |                       | `BuildRuleEvent`](Bui |
        |                       |                       | ldRuleEvent.html "cla |
        |                       |                       | ss in com.facebook.bu |
        |                       |                       | ck.core.build.event") |
        |                       |                       | that denotes          |
        |                       |                       | beginning of          |
        |                       |                       | computation for a     |
        |                       |                       | particular            |
        |                       |                       | [`                    |
        |                       |                       | BuildRule`](../../rul |
        |                       |                       | es/BuildRule.html "in |
        |                       |                       | terface in com.facebo |
        |                       |                       | ok.buck.core.rules"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `BuildRuleEvent.      | ::: block             |
        |                       | EndingBuildRuleEvent` | A                     |
        |                       |                       | [                     |
        |                       |                       | `BuildRuleEvent`](Bui |
        |                       |                       | ldRuleEvent.html "cla |
        |                       |                       | ss in com.facebook.bu |
        |                       |                       | ck.core.build.event") |
        |                       |                       | that denotes ending   |
        |                       |                       | of computation for a  |
        |                       |                       | particular            |
        |                       |                       | [`                    |
        |                       |                       | BuildRule`](../../rul |
        |                       |                       | es/BuildRule.html "in |
        |                       |                       | terface in com.facebo |
        |                       |                       | ok.buck.core.rules"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `Bui                  | ::: block             |
        |                       | ldRuleEvent.Finished` | Marks the end of      |
        |                       |                       | processing a build    |
        |                       |                       | rule.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `BuildRuleEvent       | ::: block             |
        |                       | .FinishedRuleKeyCalc` | Marks the completion  |
        |                       |                       | of processing a rule  |
        |                       |                       | to calculate its rule |
        |                       |                       | key.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `Bu                   | ::: block             |
        |                       | ildRuleEvent.Resumed` | Marks the             |
        |                       |                       | continuation of       |
        |                       |                       | processing a rule.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `Bu                   | ::: block             |
        |                       | ildRuleEvent.Started` | Marks the start of    |
        |                       |                       | processing a build    |
        |                       |                       | rule.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `BuildRuleEven        | ::: block             |
        |                       | t.StartedRuleKeyCalc` | Marks the start of    |
        |                       |                       | processing a rule to  |
        |                       |                       | calculate its rule    |
        |                       |                       | key.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `Buil                 | ::: block             |
        |                       | dRuleEvent.Suspended` | Marks a rule is       |
        |                       |                       | suspended from        |
        |                       |                       | processing.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `BuildRuleEv          | ::: block             |
        |                       | ent.WillBuildLocally` | Denotes that a        |
        |                       |                       | particular build rule |
        |                       |                       | will be built         |
        |                       |                       | locally.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `pro                  | `duration`            | ::: block             |
        | tected ClockDuration` |                       | Accumulated duration  |
        |                       |                       | of work spent on this |
        |                       |                       | rule up until this    |
        |                       |                       | event occurred.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}

        -   []{#fields.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Fields inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](../../../event/external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `BUILD_FINISHED, BUILD_REPORT, BUILD_STARTED, BUILD_STATUS_EVENT, CACHE_RATE_STATS_UPDATE_EVENT, INDIVIDUAL_TEST_AWAITING_RESULTS, INSTALL_STARTED, PARSE_FINISHED, PARSE_STARTED, PROJECT_GENERATION_FINISHED, PROJECT_GENERATION_STARTED, TEST_RUN_STARTED`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                         Description
          -------------- ------------------------------------------------------------------- -------------
          `protected `   `BuildRuleEvent​(EventKey eventKey,               BuildRule rule)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                             Method                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Description
          --------------------------------------------- ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `static BuildRuleEvent.Finished`              `finished​(BuildRuleEvent.BeginningBuildRuleEvent beginning,         BuildRuleKeys ruleKeys,         BuildRuleStatus status,         CacheResult cacheResult,         Optional<BuildId> origin,         Optional<BuildRuleSuccessType> successType,         UploadToCacheResultType uploadToCacheResultType,         Optional<com.google.common.hash.HashCode> outputHash,         Optional<Long> outputSize,         Optional<BuildRuleDiagnosticData> diagnosticData,         Optional<ManifestFetchResult> manifestFetchResult,         Optional<ManifestStoreResult> manifestStoreResult,         Optional<Pair<Long,​Long>> ruleKeyCacheCheckTimestamps,         Optional<Pair<Long,​Long>> inputRuleKeyCacheCheckTimestamps,         Optional<Pair<Long,​Long>> manifestRuleKeyCacheCheckTimestamps,         Optional<Pair<Long,​Long>> buildTimestamps,         Optional<String> strategyResult)`    
          `BuildRule`                                   `getBuildRule()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       
          `ClockDuration`                               `getDuration()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        
          `String`                                      `getEventName()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       
          `String`                                      `getValueString()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     
          `abstract boolean`                            `isRuleRunningAfterThisEvent()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        
          `static BuildRuleEvent.Resumed`               `resumed​(BuildRule rule,        BuildRuleDurationTracker tracker,        RuleKeyFactory<RuleKey> ruleKeyFactory)`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      
          `static BuildRuleEvent.FinishedRuleKeyCalc`   `ruleKeyCalculationFinished​(BuildRuleEvent.StartedRuleKeyCalc started,                           RuleKeyFactory<RuleKey> ruleKeyFactory)`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              
          `static Scope`                                `ruleKeyCalculationScope​(BuckEventBus eventBus,                        BuildRule rule,                        BuildRuleDurationTracker tracker,                        RuleKeyFactory<RuleKey> ruleKeyFactory)`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        
          `static BuildRuleEvent.StartedRuleKeyCalc`    `ruleKeyCalculationStarted​(BuildRule rule,                          BuildRuleDurationTracker tracker)`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 
          `static BuildRuleEvent.Started`               `started​(BuildRule rule,        BuildRuleDurationTracker tracker)`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     
          `static BuildRuleEvent.Suspended`             `suspended​(BuildRuleEvent.BeginningBuildRuleEvent beginning,          RuleKeyFactory<RuleKey> ruleKeyFactory)`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         
          `static BuildRuleEvent.WillBuildLocally`      `willBuildLocally​(BuildRule rule)`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.event.AbstractBuckEvent}

            ### Methods inherited from class com.facebook.buck.event.[AbstractBuckEvent](../../../event/AbstractBuckEvent.html "class in com.facebook.buck.event")

            `configure, equals, getBuildId, getEventKey, getNanoTime, getThreadId, getThreadUserNanoTime, getTimestampMillis, hashCode, isConfigured, isRelatedTo, toLogMessage, toString`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.event.BuckEvent}

            ### Methods inherited from interface com.facebook.buck.event.[BuckEvent](../../../event/BuckEvent.html "interface in com.facebook.buck.event")

            `configure, getBuildId, getEventKey, getNanoTime, getThreadId, getThreadUserNanoTime, isConfigured, isRelatedTo, toLogMessage`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Methods inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](../../../event/external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `getTimestampMillis, storeLastInstanceAndReplayForNewClients`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#duration}

        -   #### duration

                @Nullable
                protected ClockDuration duration

            ::: block
            Accumulated duration of work spent on this rule up until
            this event occurred.
            :::
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.event.EventKey,com.facebook.buck.core.rules.BuildRule)}

        -   #### BuildRuleEvent

                protected BuildRuleEvent​(EventKey eventKey,
                                         BuildRule rule)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildRule()}

        -   #### getBuildRule

            ``` methodSignature
            public BuildRule getBuildRule()
            ```

        []{#getDuration()}

        -   #### getDuration

            ``` methodSignature
            public ClockDuration getDuration()
            ```

        []{#getValueString()}

        -   #### getValueString

            ``` methodSignature
            public String getValueString()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getValueString` in class `AbstractBuckEvent`

        []{#getEventName()}

        -   #### getEventName

            ``` methodSignature
            public final String getEventName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getEventName` in interface `BuckEventExternalInterface`

            [Returns:]{.returnLabel}
            :   the type of the event.

        []{#isRuleRunningAfterThisEvent()}

        -   #### isRuleRunningAfterThisEvent

            ``` methodSignature
            public abstract boolean isRuleRunningAfterThisEvent()
            ```

        []{#started(com.facebook.buck.core.rules.BuildRule,com.facebook.buck.core.build.stats.BuildRuleDurationTracker)}

        -   #### started

            ``` methodSignature
            public static BuildRuleEvent.Started started​(BuildRule rule,
                                                         BuildRuleDurationTracker tracker)
            ```

        []{#finished(com.facebook.buck.core.build.event.BuildRuleEvent.BeginningBuildRuleEvent,com.facebook.buck.core.rulekey.BuildRuleKeys,com.facebook.buck.core.build.engine.BuildRuleStatus,com.facebook.buck.artifact_cache.CacheResult,java.util.Optional,java.util.Optional,com.facebook.buck.core.build.engine.type.UploadToCacheResultType,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional)}

        -   #### finished

            ``` methodSignature
            public static BuildRuleEvent.Finished finished​(BuildRuleEvent.BeginningBuildRuleEvent beginning,
                                                           BuildRuleKeys ruleKeys,
                                                           BuildRuleStatus status,
                                                           CacheResult cacheResult,
                                                           Optional<BuildId> origin,
                                                           Optional<BuildRuleSuccessType> successType,
                                                           UploadToCacheResultType uploadToCacheResultType,
                                                           Optional<com.google.common.hash.HashCode> outputHash,
                                                           Optional<Long> outputSize,
                                                           Optional<BuildRuleDiagnosticData> diagnosticData,
                                                           Optional<ManifestFetchResult> manifestFetchResult,
                                                           Optional<ManifestStoreResult> manifestStoreResult,
                                                           Optional<Pair<Long,​Long>> ruleKeyCacheCheckTimestamps,
                                                           Optional<Pair<Long,​Long>> inputRuleKeyCacheCheckTimestamps,
                                                           Optional<Pair<Long,​Long>> manifestRuleKeyCacheCheckTimestamps,
                                                           Optional<Pair<Long,​Long>> buildTimestamps,
                                                           Optional<String> strategyResult)
            ```

        []{#ruleKeyCalculationStarted(com.facebook.buck.core.rules.BuildRule,com.facebook.buck.core.build.stats.BuildRuleDurationTracker)}

        -   #### ruleKeyCalculationStarted

            ``` methodSignature
            public static BuildRuleEvent.StartedRuleKeyCalc ruleKeyCalculationStarted​(BuildRule rule,
                                                                                      BuildRuleDurationTracker tracker)
            ```

        []{#ruleKeyCalculationFinished(com.facebook.buck.core.build.event.BuildRuleEvent.StartedRuleKeyCalc,com.facebook.buck.rules.keys.RuleKeyFactory)}

        -   #### ruleKeyCalculationFinished

            ``` methodSignature
            public static BuildRuleEvent.FinishedRuleKeyCalc ruleKeyCalculationFinished​(BuildRuleEvent.StartedRuleKeyCalc started,
                                                                                        RuleKeyFactory<RuleKey> ruleKeyFactory)
            ```

        []{#suspended(com.facebook.buck.core.build.event.BuildRuleEvent.BeginningBuildRuleEvent,com.facebook.buck.rules.keys.RuleKeyFactory)}

        -   #### suspended

            ``` methodSignature
            public static BuildRuleEvent.Suspended suspended​(BuildRuleEvent.BeginningBuildRuleEvent beginning,
                                                             RuleKeyFactory<RuleKey> ruleKeyFactory)
            ```

        []{#resumed(com.facebook.buck.core.rules.BuildRule,com.facebook.buck.core.build.stats.BuildRuleDurationTracker,com.facebook.buck.rules.keys.RuleKeyFactory)}

        -   #### resumed

            ``` methodSignature
            public static BuildRuleEvent.Resumed resumed​(BuildRule rule,
                                                         BuildRuleDurationTracker tracker,
                                                         RuleKeyFactory<RuleKey> ruleKeyFactory)
            ```

        []{#willBuildLocally(com.facebook.buck.core.rules.BuildRule)}

        -   #### willBuildLocally

            ``` methodSignature
            public static BuildRuleEvent.WillBuildLocally willBuildLocally​(BuildRule rule)
            ```

        []{#ruleKeyCalculationScope(com.facebook.buck.event.BuckEventBus,com.facebook.buck.core.rules.BuildRule,com.facebook.buck.core.build.stats.BuildRuleDurationTracker,com.facebook.buck.rules.keys.RuleKeyFactory)}

        -   #### ruleKeyCalculationScope

            ``` methodSignature
            public static Scope ruleKeyCalculationScope​(BuckEventBus eventBus,
                                                        BuildRule rule,
                                                        BuildRuleDurationTracker tracker,
                                                        RuleKeyFactory<RuleKey> ruleKeyFactory)
            ```
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
-   [Nested](#nested.class.summary) \| 
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
