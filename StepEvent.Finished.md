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

## Class StepEvent.Finished {#class-stepevent.finished .title title="Class StepEvent.Finished"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.event.AbstractBuckEvent](../event/AbstractBuckEvent.html "class in com.facebook.buck.event")

    -   -   [com.facebook.buck.step.StepEvent](StepEvent.html "class in com.facebook.buck.step")

        -   -   com.facebook.buck.step.StepEvent.Finished

::: description
-   

    All Implemented Interfaces:
    :   `BuckEvent`, `BuckEventExternalInterface`,
        `StepEventExternalInterface`, `LeafEvent`, `WorkAdvanceEvent`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [StepEvent](StepEvent.html "class in com.facebook.buck.step")

    ------------------------------------------------------------------------

        public static class StepEvent.Finished
        extends StepEvent
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.step.StepEvent}

            ### Nested classes/interfaces inherited from class com.facebook.buck.step.[StepEvent](StepEvent.html "class in com.facebook.buck.step")

            `StepEvent.Finished, StepEvent.Started`
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

          Modifier       Constructor                                                   Description
          -------------- ------------------------------------------------------------- -------------
          `protected `   `Finished​(StepEvent.Started started,         int exitCode)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
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
        | `String`              | `getEventName()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getExitCode()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.step.StepEvent}

            ### Methods inherited from class com.facebook.buck.step.[StepEvent](StepEvent.html "class in com.facebook.buck.step")

            `finished, getCategory, getDescription, getShortStepName, getUuid, getValueString, started`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.event.AbstractBuckEvent}

            ### Methods inherited from class com.facebook.buck.event.[AbstractBuckEvent](../event/AbstractBuckEvent.html "class in com.facebook.buck.event")

            `configure, getBuildId, getEventKey, getNanoTime, getThreadId, getThreadUserNanoTime, getTimestampMillis, isConfigured, isRelatedTo, toLogMessage, toString`

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

            `getTimestampMillis, storeLastInstanceAndReplayForNewClients`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.step.StepEvent.Started,int)}

        -   #### Finished

                protected Finished​(StepEvent.Started started,
                                   int exitCode)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getExitCode()}

        -   #### getExitCode

            ``` methodSignature
            public int getExitCode()
            ```

        []{#getEventName()}

        -   #### getEventName

            ``` methodSignature
            public String getEventName()
            ```

            [Returns:]{.returnLabel}
            :   the type of the event.

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object o)
            ```

            ::: block
            [Description copied from
            class: `AbstractBuckEvent`]{.descfrmTypeLabel}
            :::

            ::: block
            The default implementation of equals checks to see if two
            events are related, are on the same thread, and are the same
            concrete class. Subclasses therefore can simply override
            isRelatedTo, and the equals method will work correctly.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `AbstractBuckEvent`

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `AbstractBuckEvent`
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