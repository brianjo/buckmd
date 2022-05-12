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
-   Nested \| 
-   Field \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.httpserver](package-summary.html)
:::

## Class WebServerBuckEventListener {#class-webserverbuckeventlistener .title title="Class WebServerBuckEventListener"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.httpserver.WebServerBuckEventListener

::: description
-   

    All Implemented Interfaces:
    :   `BuckEventListener`, `Closeable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class WebServerBuckEventListener
        extends Object
        implements BuckEventListener

    ::: block
    [`BuckEventListener`](../event/BuckEventListener.html "interface in com.facebook.buck.event")
    that is responsible for reporting events of interest to the
    [`StreamingWebSocketServlet`](StreamingWebSocketServlet.html "class in com.facebook.buck.httpserver").
    This class passes high-level objects to the servlet, and the servlet
    takes responsibility for serializing the objects as JSON down to the
    client.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `bu                   |                       |
        |                       | ildFinished​(BuildEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `                     |                       |
        |                       | buildProgressUpdated​( |                       |
        |                       | ProgressEvent.BuildPr |                       |
        |                       | ogressUpdated event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `buildRuleF           |                       |
        |                       | inished​(BuildRuleEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `buildStarted​(BuildEv |                       |
        |                       | ent.Started started)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `cacheR               |                       |
        |                       | ateStatsUpdate​(CacheR |                       |
        |                       | ateStatsKeeper.CacheR |                       |
        |                       | ateStatsUpdateEvent c |                       |
        |                       | acheRateStatsUpdate)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `close()`             | ::: block             |
        |                       |                       | Cleanup, output any   |
        |                       |                       | trace data collected  |
        |                       |                       | to the backing store. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `com                  |                       |
        |                       | pilerErrorEvent​(Compi |                       |
        |                       | lerErrorEvent event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `consoleEvent         |                       |
        |                       | ​(ConsoleEvent event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `installE             |                       |
        |                       | ventFinished​(InstallE |                       |
        |                       | vent.Finished event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `pa                   |                       |
        |                       | rseFinished​(ParseEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `parseStarted​(ParseEv |                       |
        |                       | ent.Started started)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `pars                 |                       |
        |                       | ingProgressUpdated​(Pr |                       |
        |                       | ogressEvent.ParsingPr |                       |
        |                       | ogressUpdated event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `pr                   |                       |
        |                       | ojectGenerationFinish |                       |
        |                       | ed​(ProjectGenerationE |                       |
        |                       | vent.Finished event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `pro                  |                       |
        |                       | jectGenerationProgres |                       |
        |                       | sUpdated​(ProgressEven |                       |
        |                       | t.ProjectGenerationPr |                       |
        |                       | ogressUpdated event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `                     |                       |
        |                       | projectGenerationStar |                       |
        |                       | ted​(ProjectGeneration |                       |
        |                       | Event.Started event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `                     |                       |
        |                       | ruleCountCalculated​(B |                       |
        |                       | uildEvent.RuleCountCa |                       |
        |                       | lculated calculated)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `                     |                       |
        |                       | ruleCountUpdated​(Buil |                       |
        |                       | dEvent.UnskippedRuleC |                       |
        |                       | ountUpdated updated)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `testAwaitingR        |                       |
        |                       | esults​(IndividualTest |                       |
        |                       | Event.Started event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `testResultsAvai      |                       |
        |                       | lable​(IndividualTestE |                       |
        |                       | vent.Finished event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `test                 |                       |
        |                       | RunCompleted​(TestRunE |                       |
        |                       | vent.Finished event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `t                    |                       |
        |                       | estRunStarted​(TestRun |                       |
        |                       | Event.Started event)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#parseStarted(com.facebook.buck.parser.ParseEvent.Started)}

        -   #### parseStarted

            ``` methodSignature
            public void parseStarted​(ParseEvent.Started started)
            ```

        []{#parseFinished(com.facebook.buck.parser.ParseEvent.Finished)}

        -   #### parseFinished

            ``` methodSignature
            public void parseFinished​(ParseEvent.Finished finished)
            ```

        []{#buildStarted(com.facebook.buck.core.build.event.BuildEvent.Started)}

        -   #### buildStarted

            ``` methodSignature
            public void buildStarted​(BuildEvent.Started started)
            ```

        []{#cacheRateStatsUpdate(com.facebook.buck.event.listener.stats.cache.CacheRateStatsKeeper.CacheRateStatsUpdateEvent)}

        -   #### cacheRateStatsUpdate

            ``` methodSignature
            public void cacheRateStatsUpdate​(CacheRateStatsKeeper.CacheRateStatsUpdateEvent cacheRateStatsUpdate)
            ```

        []{#buildFinished(com.facebook.buck.core.build.event.BuildEvent.Finished)}

        -   #### buildFinished

            ``` methodSignature
            public void buildFinished​(BuildEvent.Finished finished)
            ```

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

        []{#testAwaitingResults(com.facebook.buck.core.test.event.IndividualTestEvent.Started)}

        -   #### testAwaitingResults

            ``` methodSignature
            public void testAwaitingResults​(IndividualTestEvent.Started event)
            ```

        []{#testResultsAvailable(com.facebook.buck.core.test.event.IndividualTestEvent.Finished)}

        -   #### testResultsAvailable

            ``` methodSignature
            public void testResultsAvailable​(IndividualTestEvent.Finished event)
            ```

        []{#installEventFinished(com.facebook.buck.event.InstallEvent.Finished)}

        -   #### installEventFinished

            ``` methodSignature
            public void installEventFinished​(InstallEvent.Finished event)
            ```

        []{#compilerErrorEvent(com.facebook.buck.event.CompilerErrorEvent)}

        -   #### compilerErrorEvent

            ``` methodSignature
            public void compilerErrorEvent​(CompilerErrorEvent event)
            ```

        []{#consoleEvent(com.facebook.buck.event.ConsoleEvent)}

        -   #### consoleEvent

            ``` methodSignature
            public void consoleEvent​(ConsoleEvent event)
            ```

        []{#buildProgressUpdated(com.facebook.buck.event.ProgressEvent.BuildProgressUpdated)}

        -   #### buildProgressUpdated

            ``` methodSignature
            public void buildProgressUpdated​(ProgressEvent.BuildProgressUpdated event)
            ```

        []{#parsingProgressUpdated(com.facebook.buck.event.ProgressEvent.ParsingProgressUpdated)}

        -   #### parsingProgressUpdated

            ``` methodSignature
            public void parsingProgressUpdated​(ProgressEvent.ParsingProgressUpdated event)
            ```

        []{#projectGenerationProgressUpdated(com.facebook.buck.event.ProgressEvent.ProjectGenerationProgressUpdated)}

        -   #### projectGenerationProgressUpdated

            ``` methodSignature
            public void projectGenerationProgressUpdated​(ProgressEvent.ProjectGenerationProgressUpdated event)
            ```

        []{#projectGenerationStarted(com.facebook.buck.event.ProjectGenerationEvent.Started)}

        -   #### projectGenerationStarted

            ``` methodSignature
            public void projectGenerationStarted​(ProjectGenerationEvent.Started event)
            ```

        []{#projectGenerationFinished(com.facebook.buck.event.ProjectGenerationEvent.Finished)}

        -   #### projectGenerationFinished

            ``` methodSignature
            public void projectGenerationFinished​(ProjectGenerationEvent.Finished event)
            ```

        []{#ruleCountCalculated(com.facebook.buck.core.build.event.BuildEvent.RuleCountCalculated)}

        -   #### ruleCountCalculated

            ``` methodSignature
            public void ruleCountCalculated​(BuildEvent.RuleCountCalculated calculated)
            ```

        []{#ruleCountUpdated(com.facebook.buck.core.build.event.BuildEvent.UnskippedRuleCountUpdated)}

        -   #### ruleCountUpdated

            ``` methodSignature
            public void ruleCountUpdated​(BuildEvent.UnskippedRuleCountUpdated updated)
            ```

        []{#buildRuleFinished(com.facebook.buck.core.build.event.BuildRuleEvent.Finished)}

        -   #### buildRuleFinished

            ``` methodSignature
            public void buildRuleFinished​(BuildRuleEvent.Finished finished)
            ```

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
            ```

            ::: block
            [Description copied from
            interface: `BuckEventListener`]{.descfrmTypeLabel}
            :::

            ::: block
            Cleanup, output any trace data collected to the backing
            store.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `BuckEventListener`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `Closeable`
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
-   Nested \| 
-   Field \| 
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
