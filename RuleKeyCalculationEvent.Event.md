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

## Class RuleKeyCalculationEvent.Event {#class-rulekeycalculationevent.event .title title="Class RuleKeyCalculationEvent.Event"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.event.AbstractBuckEvent](AbstractBuckEvent.html "class in com.facebook.buck.event")

    -   -   com.facebook.buck.event.RuleKeyCalculationEvent.Event

::: description
-   

    All Implemented Interfaces:
    :   `BuckEvent`, `BuckEventExternalInterface`, `LeafEvent`,
        `RuleKeyCalculationEvent`, `WorkAdvanceEvent`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `RuleKeyCalculationEvent.DefaultFinished`,
        `RuleKeyCalculationEvent.DefaultStarted`

    ```{=html}
    <!-- -->
    ```

    Enclosing interface:
    :   [RuleKeyCalculationEvent](RuleKeyCalculationEvent.html "interface in com.facebook.buck.event")

    ------------------------------------------------------------------------

        public static class RuleKeyCalculationEvent.Event
        extends AbstractBuckEvent
        implements RuleKeyCalculationEvent
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.event.RuleKeyCalculationEvent}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.event.[RuleKeyCalculationEvent](RuleKeyCalculationEvent.html "interface in com.facebook.buck.event")

            `RuleKeyCalculationEvent.DefaultFinished, RuleKeyCalculationEvent.DefaultStarted, RuleKeyCalculationEvent.Event, RuleKeyCalculationEvent.Finished, RuleKeyCalculationEvent.Started, RuleKeyCalculationEvent.Type`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Fields inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `BUILD_FINISHED, BUILD_REPORT, BUILD_STARTED, BUILD_STATUS_EVENT, CACHE_RATE_STATS_UPDATE_EVENT, INDIVIDUAL_TEST_AWAITING_RESULTS, INSTALL_STARTED, PARSE_FINISHED, PARSE_STARTED, PROJECT_GENERATION_FINISHED, PROJECT_GENERATION_STARTED, TEST_RUN_STARTED`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                   Description
          --------------------------------------------------------------------------------------------- -------------
          `Event​(EventKey eventKey,      RuleKeyCalculationEvent.Type type,      BuildTarget target)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                Method               Description
          -------------------------------- -------------------- -------------
          `String`                         `getEventName()`      
          `BuildTarget`                    `getTarget()`         
          `RuleKeyCalculationEvent.Type`   `getType()`           
          `protected String`               `getValueString()`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.event.AbstractBuckEvent}

            ### Methods inherited from class com.facebook.buck.event.[AbstractBuckEvent](AbstractBuckEvent.html "class in com.facebook.buck.event")

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

            ### Methods inherited from interface com.facebook.buck.event.[BuckEvent](BuckEvent.html "interface in com.facebook.buck.event")

            `configure, getBuildId, getEventKey, getNanoTime, getThreadId, getThreadUserNanoTime, isConfigured, isRelatedTo, toLogMessage`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Methods inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `getTimestampMillis, storeLastInstanceAndReplayForNewClients`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.event.RuleKeyCalculationEvent}

            ### Methods inherited from interface com.facebook.buck.event.[RuleKeyCalculationEvent](RuleKeyCalculationEvent.html "interface in com.facebook.buck.event")

            `getCategory`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.event.EventKey,com.facebook.buck.event.RuleKeyCalculationEvent.Type,com.facebook.buck.core.model.BuildTarget)}

        -   #### Event

                public Event​(EventKey eventKey,
                             RuleKeyCalculationEvent.Type type,
                             BuildTarget target)
    :::

    ::: {.section role="region"}
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

        []{#getEventName()}

        -   #### getEventName

            ``` methodSignature
            public String getEventName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getEventName` in interface `BuckEventExternalInterface`

            [Returns:]{.returnLabel}
            :   the type of the event.

        []{#getValueString()}

        -   #### getValueString

            ``` methodSignature
            protected String getValueString()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getValueString` in class `AbstractBuckEvent`
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