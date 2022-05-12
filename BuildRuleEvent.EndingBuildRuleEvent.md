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
[Package]{.packageLabelInType} [com.facebook.buck.core.build.event](package-summary.html)
:::

## Class BuildRuleEvent.EndingBuildRuleEvent {#class-buildruleevent.endingbuildruleevent .title title="Class BuildRuleEvent.EndingBuildRuleEvent"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.event.AbstractBuckEvent](../../../event/AbstractBuckEvent.html "class in com.facebook.buck.event")

    -   -   [com.facebook.buck.core.build.event.BuildRuleEvent](BuildRuleEvent.html "class in com.facebook.buck.core.build.event")

        -   -   com.facebook.buck.core.build.event.BuildRuleEvent.EndingBuildRuleEvent

::: description
-   

    All Implemented Interfaces:
    :   `BuckEvent`, `BuckEventExternalInterface`, `WorkAdvanceEvent`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `BuildRuleEvent.Finished`, `BuildRuleEvent.Suspended`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [BuildRuleEvent](BuildRuleEvent.html "class in com.facebook.buck.core.build.event")

    ------------------------------------------------------------------------

        public abstract static class BuildRuleEvent.EndingBuildRuleEvent
        extends BuildRuleEvent

    ::: block
    A
    [`BuildRuleEvent`](BuildRuleEvent.html "class in com.facebook.buck.core.build.event")
    that denotes ending of computation for a particular
    [`BuildRule`](../../rules/BuildRule.html "interface in com.facebook.buck.core.rules").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.core.build.event.BuildRuleEvent}

            ### Nested classes/interfaces inherited from class com.facebook.buck.core.build.event.[BuildRuleEvent](BuildRuleEvent.html "class in com.facebook.buck.core.build.event")

            `BuildRuleEvent.BeginningBuildRuleEvent, BuildRuleEvent.EndingBuildRuleEvent, BuildRuleEvent.Finished, BuildRuleEvent.FinishedRuleKeyCalc, BuildRuleEvent.Resumed, BuildRuleEvent.Started, BuildRuleEvent.StartedRuleKeyCalc, BuildRuleEvent.Suspended, BuildRuleEvent.WillBuildLocally`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.core.build.event.BuildRuleEvent}

            ### Fields inherited from class com.facebook.buck.core.build.event.[BuildRuleEvent](BuildRuleEvent.html "class in com.facebook.buck.core.build.event")

            `duration`

        ```{=html}
        <!-- -->
        ```
        -   []{#fields.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Fields inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](../../../event/external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `BUILD_FINISHED, BUILD_REPORT, BUILD_STARTED, BUILD_STATUS_EVENT, CACHE_RATE_STATS_UPDATE_EVENT, INDIVIDUAL_TEST_AWAITING_RESULTS, INSTALL_STARTED, PARSE_FINISHED, PARSE_STARTED, PROJECT_GENERATION_FINISHED, PROJECT_GENERATION_STARTED, TEST_RUN_STARTED`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                Description
          -------------------------------------------------------------------------- -------------
          `EndingBuildRuleEvent​(BuildRuleEvent.BeginningBuildRuleEvent beginning)`    

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
        |                       | serNanoTime,          | [`Buck                |
        |                       |  long threadId,       | EventBus`](../../../e |
        |                       |     BuildId buildId)` | vent/BuckEventBus.htm |
        |                       |                       | l "interface in com.f |
        |                       |                       | acebook.buck.event"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `BuildRuleEvent.Beg   | `getBeginningEvent()` |                       |
        | inningBuildRuleEvent` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isRuleRun            |                       |
        |                       | ningAfterThisEvent()` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.build.event.BuildRuleEvent}

            ### Methods inherited from class com.facebook.buck.core.build.event.[BuildRuleEvent](BuildRuleEvent.html "class in com.facebook.buck.core.build.event")

            `finished, getBuildRule, getDuration, getEventName, getValueString, resumed, ruleKeyCalculationFinished, ruleKeyCalculationScope, ruleKeyCalculationStarted, started, suspended, willBuildLocally`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.event.AbstractBuckEvent}

            ### Methods inherited from class com.facebook.buck.event.[AbstractBuckEvent](../../../event/AbstractBuckEvent.html "class in com.facebook.buck.event")

            `equals, getBuildId, getEventKey, getNanoTime, getThreadId, getThreadUserNanoTime, getTimestampMillis, hashCode, isConfigured, isRelatedTo, toLogMessage, toString`

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

            `getBuildId, getEventKey, getNanoTime, getThreadId, getThreadUserNanoTime, isConfigured, isRelatedTo, toLogMessage`

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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.build.event.BuildRuleEvent.BeginningBuildRuleEvent)}

        -   #### EndingBuildRuleEvent

                public EndingBuildRuleEvent​(BuildRuleEvent.BeginningBuildRuleEvent beginning)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBeginningEvent()}

        -   #### getBeginningEvent

            ``` methodSignature
            public BuildRuleEvent.BeginningBuildRuleEvent getBeginningEvent()
            ```

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
            [Description copied from
            class: `AbstractBuckEvent`]{.descfrmTypeLabel}
            :::

            ::: block
            Method to configure an event before posting it to the
            [`BuckEventBus`](../../../event/BuckEventBus.html "interface in com.facebook.buck.event").
            This method should only be invoked once per event, and only
            by the
            [`BuckEventBus`](../../../event/BuckEventBus.html "interface in com.facebook.buck.event")
            in production code.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `configure` in interface `BuckEvent`

            [Overrides:]{.overrideSpecifyLabel}
            :   `configure` in class `AbstractBuckEvent`

        []{#isRuleRunningAfterThisEvent()}

        -   #### isRuleRunningAfterThisEvent

            ``` methodSignature
            public final boolean isRuleRunningAfterThisEvent()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isRuleRunningAfterThisEvent` in class `BuildRuleEvent`
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
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
