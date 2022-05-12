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

## Class ActionGraphPerfStatEvent {#class-actiongraphperfstatevent .title title="Class ActionGraphPerfStatEvent"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.event.AbstractBuckEvent](AbstractBuckEvent.html "class in com.facebook.buck.event")

    -   -   com.facebook.buck.event.ActionGraphPerfStatEvent

::: description
-   

    All Implemented Interfaces:
    :   `BuckEvent`, `BuckEventExternalInterface`

    ------------------------------------------------------------------------

        public class ActionGraphPerfStatEvent
        extends AbstractBuckEvent

    ::: block
    Event Class containing the perf data regarding action graph building
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `ActionGrap           | ::: block             |
        |                       | hPerfStatEvent.Start` | Class representing    |
        |                       |                       | the start of timing   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

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

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `String`              | `                     |                       |
        |                       | getBuildTargetName()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `getElapsedTime()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getEventName()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getNu                |                       |
        |                       | mberNodesGenerated()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `getNum               |                       |
        |                       | NoopNodesGenerated()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getTargetN           |                       |
        |                       | odeDescriptionName()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected String`    | `getValueString()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Scope`        | `start​(               | ::: block             |
        |                       | Clock clock,      Buc | Creates a Scope for   |
        |                       | kEventBus eventBus,   | the timing event      |
        |                       |     java.util.functio | :::                   |
        |                       | n.Supplier<Integer> g |                       |
        |                       | etRuleSize,      java |                       |
        |                       | .util.function.Suppli |                       |
        |                       | er<Long> getNoOpRuleS |                       |
        |                       | ize,      String desc |                       |
        |                       | riptionName,      Str |                       |
        |                       | ing buildTargetName)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
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
        -   []{#methods.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Methods inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `storeLastInstanceAndReplayForNewClients`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#start(com.facebook.buck.util.timing.Clock,com.facebook.buck.event.BuckEventBus,java.util.function.Supplier,java.util.function.Supplier,java.lang.String,java.lang.String)}

        -   #### start

            ``` methodSignature
            public static Scope start​(Clock clock,
                                      BuckEventBus eventBus,
                                      java.util.function.Supplier<Integer> getRuleSize,
                                      java.util.function.Supplier<Long> getNoOpRuleSize,
                                      String descriptionName,
                                      String buildTargetName)
            ```

            ::: block
            Creates a Scope for the timing event
            :::

            [Parameters:]{.paramLabel}

            `clock` -

            `eventBus` -

            `getRuleSize` -

            `descriptionName` -

            `buildTargetName` -

            [Returns:]{.returnLabel}

        []{#getValueString()}

        -   #### getValueString

            ``` methodSignature
            protected String getValueString()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getValueString` in class `AbstractBuckEvent`

        []{#getEventName()}

        -   #### getEventName

            ``` methodSignature
            public String getEventName()
            ```

            [Returns:]{.returnLabel}
            :   the type of the event.

        []{#getElapsedTime()}

        -   #### getElapsedTime

            ``` methodSignature
            public long getElapsedTime()
            ```

        []{#getNumberNodesGenerated()}

        -   #### getNumberNodesGenerated

            ``` methodSignature
            public int getNumberNodesGenerated()
            ```

        []{#getNumNoopNodesGenerated()}

        -   #### getNumNoopNodesGenerated

            ``` methodSignature
            public long getNumNoopNodesGenerated()
            ```

        []{#getBuildTargetName()}

        -   #### getBuildTargetName

            ``` methodSignature
            public String getBuildTargetName()
            ```

        []{#getTargetNodeDescriptionName()}

        -   #### getTargetNodeDescriptionName

            ``` methodSignature
            public String getTargetNodeDescriptionName()
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
