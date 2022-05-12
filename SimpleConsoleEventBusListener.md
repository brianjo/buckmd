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
[Package]{.packageLabelInType} [com.facebook.buck.event.listener](package-summary.html)
:::

## Class SimpleConsoleEventBusListener {#class-simpleconsoleeventbuslistener .title title="Class SimpleConsoleEventBusListener"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.event.listener.AbstractConsoleEventBusListener](AbstractConsoleEventBusListener.html "class in com.facebook.buck.event.listener")

    -   -   com.facebook.buck.event.listener.SimpleConsoleEventBusListener

::: description
-   

    All Implemented Interfaces:
    :   `BuckEventListener`, `Closeable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class SimpleConsoleEventBusListener
        extends AbstractConsoleEventBusListener

    ::: block
    Implementation of `AbstractConsoleEventBusListener` for terminals
    that don\'t support ansi.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                                          Field                         Description
          -------------------------------------------------------------------------- ----------------------------- -------------
          `com.google.common.collect.ImmutableList<AdditionalConsoleLineProvider>`   `buildFinishedLineProvider`    

          : Fields[ ]{.tabEnd}

        -   []{#fields.inherited.from.class.com.facebook.buck.event.listener.AbstractConsoleEventBusListener}

            ### Fields inherited from class com.facebook.buck.event.listener.[AbstractConsoleEventBusListener](AbstractConsoleEventBusListener.html "class in com.facebook.buck.event.listener")

            `actionGraphEvents, actionGraphFinished, actionGraphStarted, ansi, buildDetailsCommands, buildFinished, buildRuleThreadTracker, buildStarted, clock, commandFinished, console, installFinished, installStarted, networkStatsTracker, numRulesCompleted, parseStats, progressEstimator, projectGenerationFinished, projectGenerationStarted, publicAnnouncements, ruleCount, UNFINISHED_EVENT_PAIR, verbosity, watchmanFinished, watchmanStarted`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `SimpleConsoleEventBusListener​(RenderingConsole console,                              Clock clock,                              TestResultSummaryVerbosity summaryVerbosity,                              boolean hideSucceededRules,                              int numberOfSlowRulesToShow,                              boolean showSlowRulesInConsole,                              Locale locale,                              Path testLogPath,                              ExecutionEnvironment executionEnvironment,                              BuildId buildId,                              boolean printBuildId,                              Optional<String> buildDetailsTemplate,                              com.google.common.collect.ImmutableSet<String> buildDetailsCommands,                              Optional<String> reSessionIDInfo,                              com.google.common.collect.ImmutableList<AdditionalConsoleLineProvider> buildFinishedLineProvider)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                  Description
          ------------------- ----------------------------------------------------------------------- -------------
          `void`              `actionGraphFinished​(ActionGraphEvent.Finished finished)`                
          `void`              `buildFinished​(BuildEvent.Finished finished)`                            
          `void`              `buildRuleFinished​(BuildRuleEvent.Finished finished)`                    
          `void`              `commandFinished​(CommandEvent.Finished event)`                           
          `boolean`           `displaysEstimatedProgress()`                                            
          `void`              `installFinished​(InstallEvent.Finished finished)`                        
          `void`              `logEvent​(ConsoleEvent event)`                                           
          `void`              `printSevereWarningDirectly​(String line)`                                
          `void`              `testResultsAvailable​(IndividualTestEvent.Finished event)`               
          `void`              `testRunCompleted​(TestRunEvent.Finished event)`                          
          `void`              `testRunStarted​(TestRunEvent.Started event)`                             
          `void`              `testStatusMessageFinished​(TestStatusMessageEvent.Finished finished)`    
          `void`              `testStatusMessageStarted​(TestStatusMessageEvent.Started started)`       

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.event.listener.AbstractConsoleEventBusListener}

            ### Methods inherited from class com.facebook.buck.event.listener.[AbstractConsoleEventBusListener](AbstractConsoleEventBusListener.html "class in com.facebook.buck.event.listener")

            `actionGraphStarted, addLineFromEventInterval, addLineFromEvents, aggregateFinishedEvent, aggregateStartedEvent, buildRuleResumed, buildRuleStarted, buildRuleSuspended, buildStarted, close, commandStartedEvent, convertToAllCapsIfNeeded, formatConsoleEvent, formatElapsedTime, getApproximateBuildProgress, getBuildDetailsLine, getBuildLogLine, getEstimatedProgressOfCreatingActionGraph, getEstimatedProgressOfGeneratingProjectFiles, getEstimatedProgressOfParsingBuckFiles, getEventsBetween, getNetworkStatsLine, getOptionalBuildLineSuffix, getTotalCompletedTimeFromEventIntervals, getWorkingTimeFromLastStartUntilNow, installStarted, logEventInterval, logEventInterval, logHttpCacheUploads, projectGenerationFinished, projectGenerationProcessedTarget, projectGenerationStarted, register, renderRemoteUploads, ruleCountCalculated, ruleCountUpdated, setProgressEstimator, setPublicAnnouncements, testRuleFinished, testRuleStarted, watchmanFinished, watchmanStarted`

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
    -   []{#field.detail}

        ### Field Detail

        []{#buildFinishedLineProvider}

        -   #### buildFinishedLineProvider

                public final com.google.common.collect.ImmutableList<AdditionalConsoleLineProvider> buildFinishedLineProvider
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.event.listener.RenderingConsole,com.facebook.buck.util.timing.Clock,com.facebook.buck.test.config.TestResultSummaryVerbosity,boolean,int,boolean,java.util.Locale,java.nio.file.Path,com.facebook.buck.util.environment.ExecutionEnvironment,com.facebook.buck.core.model.BuildId,boolean,java.util.Optional,com.google.common.collect.ImmutableSet,java.util.Optional,com.google.common.collect.ImmutableList)}

        -   #### SimpleConsoleEventBusListener

                public SimpleConsoleEventBusListener​(RenderingConsole console,
                                                     Clock clock,
                                                     TestResultSummaryVerbosity summaryVerbosity,
                                                     boolean hideSucceededRules,
                                                     int numberOfSlowRulesToShow,
                                                     boolean showSlowRulesInConsole,
                                                     Locale locale,
                                                     Path testLogPath,
                                                     ExecutionEnvironment executionEnvironment,
                                                     BuildId buildId,
                                                     boolean printBuildId,
                                                     Optional<String> buildDetailsTemplate,
                                                     com.google.common.collect.ImmutableSet<String> buildDetailsCommands,
                                                     Optional<String> reSessionIDInfo,
                                                     com.google.common.collect.ImmutableList<AdditionalConsoleLineProvider> buildFinishedLineProvider)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#actionGraphFinished(com.facebook.buck.event.ActionGraphEvent.Finished)}

        -   #### actionGraphFinished

            ``` methodSignature
            public void actionGraphFinished​(ActionGraphEvent.Finished finished)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `actionGraphFinished` in
                class `AbstractConsoleEventBusListener`

        []{#buildFinished(com.facebook.buck.core.build.event.BuildEvent.Finished)}

        -   #### buildFinished

            ``` methodSignature
            public void buildFinished​(BuildEvent.Finished finished)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `buildFinished` in
                class `AbstractConsoleEventBusListener`

        []{#commandFinished(com.facebook.buck.event.CommandEvent.Finished)}

        -   #### commandFinished

            ``` methodSignature
            public void commandFinished​(CommandEvent.Finished event)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `commandFinished` in
                class `AbstractConsoleEventBusListener`

        []{#installFinished(com.facebook.buck.event.InstallEvent.Finished)}

        -   #### installFinished

            ``` methodSignature
            public void installFinished​(InstallEvent.Finished finished)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `installFinished` in
                class `AbstractConsoleEventBusListener`

        []{#logEvent(com.facebook.buck.event.ConsoleEvent)}

        -   #### logEvent

            ``` methodSignature
            public void logEvent​(ConsoleEvent event)
            ```

        []{#printSevereWarningDirectly(java.lang.String)}

        -   #### printSevereWarningDirectly

            ``` methodSignature
            public void printSevereWarningDirectly​(String line)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `printSevereWarningDirectly` in
                class `AbstractConsoleEventBusListener`

        []{#testRunStarted(com.facebook.buck.core.test.event.TestRunEvent.Started)}

        -   #### testRunStarted

            ``` methodSignature
            public void testRunStarted​(TestRunEvent.Started event)
            ```

        []{#testRunCompleted(com.facebook.buck.core.test.event.TestRunEvent.Finished)}

        -   #### testRunCompleted

            ``` methodSignature
            public void testRunCompleted​(TestRunEvent.Finished event)
            ```

        []{#testResultsAvailable(com.facebook.buck.core.test.event.IndividualTestEvent.Finished)}

        -   #### testResultsAvailable

            ``` methodSignature
            public void testResultsAvailable​(IndividualTestEvent.Finished event)
            ```

        []{#buildRuleFinished(com.facebook.buck.core.build.event.BuildRuleEvent.Finished)}

        -   #### buildRuleFinished

            ``` methodSignature
            public void buildRuleFinished​(BuildRuleEvent.Finished finished)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `buildRuleFinished` in
                class `AbstractConsoleEventBusListener`

        []{#testStatusMessageStarted(com.facebook.buck.core.test.event.TestStatusMessageEvent.Started)}

        -   #### testStatusMessageStarted

            ``` methodSignature
            public void testStatusMessageStarted​(TestStatusMessageEvent.Started started)
            ```

        []{#testStatusMessageFinished(com.facebook.buck.core.test.event.TestStatusMessageEvent.Finished)}

        -   #### testStatusMessageFinished

            ``` methodSignature
            public void testStatusMessageFinished​(TestStatusMessageEvent.Finished finished)
            ```

        []{#displaysEstimatedProgress()}

        -   #### displaysEstimatedProgress

            ``` methodSignature
            public boolean displaysEstimatedProgress()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `displaysEstimatedProgress` in
                class `AbstractConsoleEventBusListener`
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
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
