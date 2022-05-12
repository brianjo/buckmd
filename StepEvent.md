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
[Package]{.packageLabelInType} [com.facebook.buck.step](package-summary.html)
:::

## Class StepEvent {#class-stepevent .title title="Class StepEvent"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.event.AbstractBuckEvent](../event/AbstractBuckEvent.html "class in com.facebook.buck.event")

    -   -   com.facebook.buck.step.StepEvent

::: description
-   

    All Implemented Interfaces:
    :   `BuckEvent`, `BuckEventExternalInterface`,
        `StepEventExternalInterface`, `LeafEvent`, `WorkAdvanceEvent`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `StepEvent.Finished`, `StepEvent.Started`

    ------------------------------------------------------------------------

        public abstract class StepEvent
        extends AbstractBuckEvent
        implements LeafEvent, StepEventExternalInterface, WorkAdvanceEvent

    ::: block
    Base class for events about steps.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                  Description
          ------------------- ---------------------- -------------
          `static class `     `StepEvent.Finished`    
          `static class `     `StepEvent.Started`     

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Fields inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](../event/external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `BUILD_FINISHED, BUILD_REPORT, BUILD_STARTED, BUILD_STATUS_EVENT, CACHE_RATE_STATS_UPDATE_EVENT, INDIVIDUAL_TEST_AWAITING_RESULTS, INSTALL_STARTED, PARSE_FINISHED, PARSE_STARTED, PROJECT_GENERATION_FINISHED, PROJECT_GENERATION_STARTED, TEST_RUN_STARTED`

        ```{=html}
        <!-- -->
        ```
        -   []{#fields.inherited.from.class.com.facebook.buck.event.external.events.StepEventExternalInterface}

            ### Fields inherited from interface com.facebook.buck.event.external.events.[StepEventExternalInterface](../event/external/events/StepEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `STEP_FINISHED, STEP_STARTED`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                                      Description
          -------------- -------------------------------------------------------------------------------- -------------
          `protected `   `StepEvent​(String shortName,          String description,          UUID uuid)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type             Method                                                                     Description
          ----------------------------- -------------------------------------------------------------------------- -------------
          `static StepEvent.Finished`   `finished​(StepEvent.Started started,         int exitCode)`                 
          `String`                      `getCategory()`                                                             
          `String`                      `getDescription()`                                                          
          `String`                      `getShortStepName()`                                                        
          `protected UUID`              `getUuid()`                                                                 
          `protected String`            `getValueString()`                                                          
          `static StepEvent.Started`    `started​(String shortName,        String description,        UUID uuid)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.event.AbstractBuckEvent}

            ### Methods inherited from class com.facebook.buck.event.[AbstractBuckEvent](../event/AbstractBuckEvent.html "class in com.facebook.buck.event")

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

            ### Methods inherited from interface com.facebook.buck.event.[BuckEvent](../event/BuckEvent.html "interface in com.facebook.buck.event")

            `configure, getBuildId, getEventKey, getNanoTime, getThreadId, getThreadUserNanoTime, isConfigured, isRelatedTo, toLogMessage`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Methods inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](../event/external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `getEventName, getTimestampMillis, storeLastInstanceAndReplayForNewClients`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.lang.String,java.lang.String,java.util.UUID)}

        -   #### StepEvent

                protected StepEvent​(String shortName,
                                    String description,
                                    UUID uuid)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getShortStepName()}

        -   #### getShortStepName

            ``` methodSignature
            public String getShortStepName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getShortStepName` in
                interface `StepEventExternalInterface`

            [Returns:]{.returnLabel}
            :   the step name.

        []{#getDescription()}

        -   #### getDescription

            ``` methodSignature
            public String getDescription()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDescription` in
                interface `StepEventExternalInterface`

            [Returns:]{.returnLabel}
            :   the description of the step, usually the command itself.

        []{#getUuid()}

        -   #### getUuid

            ``` methodSignature
            protected UUID getUuid()
            ```

        []{#getCategory()}

        -   #### getCategory

            ``` methodSignature
            public String getCategory()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCategory` in interface `LeafEvent`

            [Returns:]{.returnLabel}
            :   The category time spent in this event should be
                accounted under.

        []{#getValueString()}

        -   #### getValueString

            ``` methodSignature
            protected String getValueString()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getValueString` in class `AbstractBuckEvent`

        []{#started(java.lang.String,java.lang.String,java.util.UUID)}

        -   #### started

            ``` methodSignature
            public static StepEvent.Started started​(String shortName,
                                                    String description,
                                                    UUID uuid)
            ```

        []{#finished(com.facebook.buck.step.StepEvent.Started,int)}

        -   #### finished

            ``` methodSignature
            public static StepEvent.Finished finished​(StepEvent.Started started,
                                                      int exitCode)
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
