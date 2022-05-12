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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
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

## Class BuildRuleEvent.FinishedRuleKeyCalc {#class-buildruleevent.finishedrulekeycalc .title title="Class BuildRuleEvent.FinishedRuleKeyCalc"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.event.AbstractBuckEvent](../../../event/AbstractBuckEvent.html "class in com.facebook.buck.event")

    -   -   [com.facebook.buck.core.build.event.BuildRuleEvent](BuildRuleEvent.html "class in com.facebook.buck.core.build.event")

        -   -   [com.facebook.buck.core.build.event.BuildRuleEvent.EndingBuildRuleEvent](BuildRuleEvent.EndingBuildRuleEvent.html "class in com.facebook.buck.core.build.event")

            -   -   [com.facebook.buck.core.build.event.BuildRuleEvent.Suspended](BuildRuleEvent.Suspended.html "class in com.facebook.buck.core.build.event")

                -   -   com.facebook.buck.core.build.event.BuildRuleEvent.FinishedRuleKeyCalc

::: description
-   

    All Implemented Interfaces:
    :   `BuckEvent`, `BuckEventExternalInterface`, `LeafEvent`,
        `RuleKeyCalculationEvent`, `RuleKeyCalculationEvent.Finished`,
        `WorkAdvanceEvent`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [BuildRuleEvent](BuildRuleEvent.html "class in com.facebook.buck.core.build.event")

    ------------------------------------------------------------------------

        public static class BuildRuleEvent.FinishedRuleKeyCalc
        extends BuildRuleEvent.Suspended
        implements RuleKeyCalculationEvent.Finished

    ::: block
    Marks the completion of processing a rule to calculate its rule key.
    We overload this as both a rule suspend and rule key calc finish
    event to generate less events and be more efficient.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.core.build.event.BuildRuleEvent}

            ### Nested classes/interfaces inherited from class com.facebook.buck.core.build.event.[BuildRuleEvent](BuildRuleEvent.html "class in com.facebook.buck.core.build.event")

            `BuildRuleEvent.BeginningBuildRuleEvent, BuildRuleEvent.EndingBuildRuleEvent, BuildRuleEvent.Finished, BuildRuleEvent.FinishedRuleKeyCalc, BuildRuleEvent.Resumed, BuildRuleEvent.Started, BuildRuleEvent.StartedRuleKeyCalc, BuildRuleEvent.Suspended, BuildRuleEvent.WillBuildLocally`

        ```{=html}
        <!-- -->
        ```
        -   []{#nested.classes.inherited.from.class.com.facebook.buck.event.RuleKeyCalculationEvent}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.event.[RuleKeyCalculationEvent](../../../event/RuleKeyCalculationEvent.html "interface in com.facebook.buck.event")

            `RuleKeyCalculationEvent.DefaultFinished, RuleKeyCalculationEvent.DefaultStarted, RuleKeyCalculationEvent.Event, RuleKeyCalculationEvent.Finished, RuleKeyCalculationEvent.Started, RuleKeyCalculationEvent.Type`
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
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                Method          Description
          -------------------------------- --------------- -------------
          `BuildTarget`                    `getTarget()`    
          `RuleKeyCalculationEvent.Type`   `getType()`      

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.build.event.BuildRuleEvent.Suspended}

            ### Methods inherited from class com.facebook.buck.core.build.event.[BuildRuleEvent.Suspended](BuildRuleEvent.Suspended.html "class in com.facebook.buck.core.build.event")

            `getRuleKey`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.build.event.BuildRuleEvent.EndingBuildRuleEvent}

            ### Methods inherited from class com.facebook.buck.core.build.event.[BuildRuleEvent.EndingBuildRuleEvent](BuildRuleEvent.EndingBuildRuleEvent.html "class in com.facebook.buck.core.build.event")

            `configure, getBeginningEvent, isRuleRunningAfterThisEvent`

        ```{=html}
        <!-- -->
        ```
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

            `configure, getBuildId, getEventKey, getNanoTime, getThreadId, getThreadUserNanoTime, isConfigured, isRelatedTo, toLogMessage`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Methods inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](../../../event/external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `getEventName, getTimestampMillis, storeLastInstanceAndReplayForNewClients`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.event.RuleKeyCalculationEvent}

            ### Methods inherited from interface com.facebook.buck.event.[RuleKeyCalculationEvent](../../../event/RuleKeyCalculationEvent.html "interface in com.facebook.buck.event")

            `getCategory`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getType()}

        -   #### getType

            ``` methodSignature
            public RuleKeyCalculationEvent.Type getType()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getType` in interface `RuleKeyCalculationEvent`

        []{#getTarget()}

        -   #### getTarget

            ``` methodSignature
            public BuildTarget getTarget()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTarget` in interface `RuleKeyCalculationEvent`
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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
