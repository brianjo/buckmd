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
[Package]{.packageLabelInType} [com.facebook.buck.event](package-summary.html)
:::

## Interface RuleKeyCalculationEvent {#interface-rulekeycalculationevent .title title="Interface RuleKeyCalculationEvent"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `BuckEvent`, `BuckEventExternalInterface`, `LeafEvent`,
        `WorkAdvanceEvent`

    ```{=html}
    <!-- -->
    ```

    All Known Subinterfaces:
    :   `RuleKeyCalculationEvent.Finished`,
        `RuleKeyCalculationEvent.Started`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `BuildRuleEvent.FinishedRuleKeyCalc`,
        `BuildRuleEvent.StartedRuleKeyCalc`,
        `RuleKeyCalculationEvent.DefaultFinished`,
        `RuleKeyCalculationEvent.DefaultStarted`,
        `RuleKeyCalculationEvent.Event`

    ------------------------------------------------------------------------

        public interface RuleKeyCalculationEvent
        extends LeafEvent, WorkAdvanceEvent

    ::: block
    Events used to track time spent calculating rule keys.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type     Interface                                   Description
          --------------------- ------------------------------------------- -------------
          `static class `       `RuleKeyCalculationEvent.DefaultFinished`    
          `static class `       `RuleKeyCalculationEvent.DefaultStarted`     
          `static class `       `RuleKeyCalculationEvent.Event`              
          `static interface `   `RuleKeyCalculationEvent.Finished`           
          `static interface `   `RuleKeyCalculationEvent.Started`            
          `static class `       `RuleKeyCalculationEvent.Type`               

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Fields inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `BUILD_FINISHED, BUILD_REPORT, BUILD_STARTED, BUILD_STATUS_EVENT, CACHE_RATE_STATS_UPDATE_EVENT, INDIVIDUAL_TEST_AWAITING_RESULTS, INSTALL_STARTED, PARSE_FINISHED, PARSE_STARTED, PROJECT_GENERATION_FINISHED, PROJECT_GENERATION_STARTED, TEST_RUN_STARTED`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                Method                                                                                                Description
          -------------------------------- ----------------------------------------------------------------------------------------------------- -------------
          `default String`                 `getCategory()`                                                                                        
          `BuildTarget`                    `getTarget()`                                                                                          
          `RuleKeyCalculationEvent.Type`   `getType()`                                                                                            
          `static Scope`                   `scope​(BuckEventBus buckEventBus,      RuleKeyCalculationEvent.Type type,      BuildTarget target)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
          .tableTab}[[Default
          Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.event.BuckEvent}

            ### Methods inherited from interface com.facebook.buck.event.[BuckEvent](BuckEvent.html "interface in com.facebook.buck.event")

            `configure, getBuildId, getEventKey, getNanoTime, getThreadId, getThreadUserNanoTime, isConfigured, isRelatedTo, toLogMessage`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Methods inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `getEventName, getTimestampMillis, storeLastInstanceAndReplayForNewClients`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getType()}

        -   #### getType

            ``` methodSignature
            RuleKeyCalculationEvent.Type getType()
            ```

        []{#getTarget()}

        -   #### getTarget

            ``` methodSignature
            BuildTarget getTarget()
            ```

        []{#getCategory()}

        -   #### getCategory

            ``` methodSignature
            default String getCategory()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCategory` in interface `LeafEvent`

            [Returns:]{.returnLabel}
            :   The category time spent in this event should be
                accounted under.

        []{#scope(com.facebook.buck.event.BuckEventBus,com.facebook.buck.event.RuleKeyCalculationEvent.Type,com.facebook.buck.core.model.BuildTarget)}

        -   #### scope

            ``` methodSignature
            static Scope scope​(BuckEventBus buckEventBus,
                               RuleKeyCalculationEvent.Type type,
                               BuildTarget target)
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
