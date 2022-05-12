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
[Package]{.packageLabelInType} [com.facebook.buck.event.listener](package-summary.html)
:::

## Class SilentConsoleEventBusListener {#class-silentconsoleeventbuslistener .title title="Class SilentConsoleEventBusListener"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.event.listener.AbstractConsoleEventBusListener](AbstractConsoleEventBusListener.html "class in com.facebook.buck.event.listener")

    -   -   com.facebook.buck.event.listener.SilentConsoleEventBusListener

::: description
-   

    All Implemented Interfaces:
    :   `BuckEventListener`, `Closeable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class SilentConsoleEventBusListener
        extends AbstractConsoleEventBusListener

    ::: block
    A special console event listener for the silent case. Almost nothing
    should be printed in that case, and it\'s easier to get it correct
    when we handle it explicitly.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.event.listener.AbstractConsoleEventBusListener}

            ### Fields inherited from class com.facebook.buck.event.listener.[AbstractConsoleEventBusListener](AbstractConsoleEventBusListener.html "class in com.facebook.buck.event.listener")

            `actionGraphEvents, actionGraphFinished, actionGraphStarted, ansi, buildDetailsCommands, buildFinished, buildRuleThreadTracker, buildStarted, clock, commandFinished, console, installFinished, installStarted, networkStatsTracker, numRulesCompleted, parseStats, progressEstimator, projectGenerationFinished, projectGenerationStarted, publicAnnouncements, ruleCount, UNFINISHED_EVENT_PAIR, verbosity, watchmanFinished, watchmanStarted`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                    Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `SilentConsoleEventBusListener​(RenderingConsole superConsole,                              Clock clock,                              Locale locale,                              ExecutionEnvironment executionEnvironment)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `logEvent             | ::: block             |
        |                       | ​(ConsoleEvent event)` | Logs only SEVERE      |
        |                       |                       | events.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `printSevereWarningD  |                       |
        |                       | irectly​(String line)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.event.listener.AbstractConsoleEventBusListener}

            ### Methods inherited from class com.facebook.buck.event.listener.[AbstractConsoleEventBusListener](AbstractConsoleEventBusListener.html "class in com.facebook.buck.event.listener")

            `actionGraphFinished, actionGraphStarted, addLineFromEventInterval, addLineFromEvents, aggregateFinishedEvent, aggregateStartedEvent, buildFinished, buildRuleFinished, buildRuleResumed, buildRuleStarted, buildRuleSuspended, buildStarted, close, commandFinished, commandStartedEvent, convertToAllCapsIfNeeded, displaysEstimatedProgress, formatConsoleEvent, formatElapsedTime, getApproximateBuildProgress, getBuildDetailsLine, getBuildLogLine, getEstimatedProgressOfCreatingActionGraph, getEstimatedProgressOfGeneratingProjectFiles, getEstimatedProgressOfParsingBuckFiles, getEventsBetween, getNetworkStatsLine, getOptionalBuildLineSuffix, getTotalCompletedTimeFromEventIntervals, getWorkingTimeFromLastStartUntilNow, installFinished, installStarted, logEventInterval, logEventInterval, logHttpCacheUploads, projectGenerationFinished, projectGenerationProcessedTarget, projectGenerationStarted, register, renderRemoteUploads, ruleCountCalculated, ruleCountUpdated, setProgressEstimator, setPublicAnnouncements, testRuleFinished, testRuleStarted, watchmanFinished, watchmanStarted`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.event.listener.RenderingConsole,com.facebook.buck.util.timing.Clock,java.util.Locale,com.facebook.buck.util.environment.ExecutionEnvironment)}

        -   #### SilentConsoleEventBusListener

                public SilentConsoleEventBusListener​(RenderingConsole superConsole,
                                                     Clock clock,
                                                     Locale locale,
                                                     ExecutionEnvironment executionEnvironment)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#printSevereWarningDirectly(java.lang.String)}

        -   #### printSevereWarningDirectly

            ``` methodSignature
            public void printSevereWarningDirectly​(String line)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `printSevereWarningDirectly` in
                class `AbstractConsoleEventBusListener`

        []{#logEvent(com.facebook.buck.event.ConsoleEvent)}

        -   #### logEvent

            ``` methodSignature
            public void logEvent​(ConsoleEvent event)
            ```

            ::: block
            Logs only SEVERE events.
            :::
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
