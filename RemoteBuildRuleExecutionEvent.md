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
[Package]{.packageLabelInType} [com.facebook.buck.remoteexecution.event](package-summary.html)
:::

## Class RemoteBuildRuleExecutionEvent {#class-remotebuildruleexecutionevent .title title="Class RemoteBuildRuleExecutionEvent"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.event.AbstractBuckEvent](../../event/AbstractBuckEvent.html "class in com.facebook.buck.event")

    -   -   com.facebook.buck.remoteexecution.event.RemoteBuildRuleExecutionEvent

::: description
-   

    All Implemented Interfaces:
    :   `BuckEvent`, `BuckEventExternalInterface`

    ------------------------------------------------------------------------

        public class RemoteBuildRuleExecutionEvent
        extends AbstractBuckEvent

    ::: block
    Event to signal the end of building a rule remotely.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Fields inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](../../event/external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `BUILD_FINISHED, BUILD_REPORT, BUILD_STARTED, BUILD_STATUS_EVENT, CACHE_RATE_STATS_UPDATE_EVENT, INDIVIDUAL_TEST_AWAITING_RESULTS, INSTALL_STARTED, PARSE_FINISHED, PARSE_STARTED, PROJECT_GENERATION_FINISHED, PROJECT_GENERATION_STARTED, TEST_RUN_STARTED`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static RemoteBui     | `createE              |                       |
        | ldRuleExecutionEvent` | vent​(BuildRule buildR |                       |
        |                       | ule,            long  |                       |
        |                       | executionDurationMs)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildRule`           | `getBuildRule()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getEventName()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `getE                 |                       |
        |                       | xecutionDurationMs()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected String`    | `getValueString()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `postEvent​(BuckEven   | ::: block             |
        |                       | tBus buckEventBus,    | Posts event of type   |
        |                       |        BuildRule buil | RemoteBu              |
        |                       | dRule,          long  | ildRuleExecutionEvent |
        |                       | executionDurationMs)` | into                  |
        |                       |                       | [`                    |
        |                       |                       | BuckEventBus`](../../ |
        |                       |                       | event/BuckEventBus.ht |
        |                       |                       | ml "interface in com. |
        |                       |                       | facebook.buck.event") |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.event.AbstractBuckEvent}

            ### Methods inherited from class com.facebook.buck.event.[AbstractBuckEvent](../../event/AbstractBuckEvent.html "class in com.facebook.buck.event")

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
        -   []{#methods.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Methods inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](../../event/external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `storeLastInstanceAndReplayForNewClients`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildRule()}

        -   #### getBuildRule

            ``` methodSignature
            public BuildRule getBuildRule()
            ```

        []{#getExecutionDurationMs()}

        -   #### getExecutionDurationMs

            ``` methodSignature
            public long getExecutionDurationMs()
            ```

        []{#getEventName()}

        -   #### getEventName

            ``` methodSignature
            public String getEventName()
            ```

            [Returns:]{.returnLabel}
            :   the type of the event.

        []{#getValueString()}

        -   #### getValueString

            ``` methodSignature
            protected String getValueString()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getValueString` in class `AbstractBuckEvent`

        []{#postEvent(com.facebook.buck.event.BuckEventBus,com.facebook.buck.core.rules.BuildRule,long)}

        -   #### postEvent

            ``` methodSignature
            public static void postEvent​(BuckEventBus buckEventBus,
                                         BuildRule buildRule,
                                         long executionDurationMs)
            ```

            ::: block
            Posts event of type RemoteBuildRuleExecutionEvent into
            [`BuckEventBus`](../../event/BuckEventBus.html "interface in com.facebook.buck.event")
            :::

        []{#createEvent(com.facebook.buck.core.rules.BuildRule,long)}

        -   #### createEvent

            ``` methodSignature
            public static RemoteBuildRuleExecutionEvent createEvent​(BuildRule buildRule,
                                                                    long executionDurationMs)
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
