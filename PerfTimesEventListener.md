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
-   [Nested](#nested.class.summary) \| 
-   Field \| 
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

## Class PerfTimesEventListener {#class-perftimeseventlistener .title title="Class PerfTimesEventListener"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.event.listener.PerfTimesEventListener

::: description
-   

    All Implemented Interfaces:
    :   `BuckEventListener`, `Closeable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class PerfTimesEventListener
        extends Object
        implements BuckEventListener
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                                     Description
          ------------------- ----------------------------------------- -------------
          `static class `     `PerfTimesEventListener.PerfTimesEvent`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                        Description
          ------------------------------------------------------------------------------------------------------------------ -------------
          `PerfTimesEventListener​(BuckEventBus eventBus,                       ExecutionEnvironment executionEnvironment)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `actionGraphFin       |                       |
        |                       | ished​(ActionGraphEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `bu                   |                       |
        |                       | ildFinished​(BuildEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `bu                   |                       |
        |                       | ildRuleWillBuildLocal |                       |
        |                       | ly​(BuildRuleEvent.Wil |                       |
        |                       | lBuildLocally event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `initializationFinish |                       |
        |                       | ed​(BuckInitialization |                       |
        |                       | DurationEvent event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `instal               |                       |
        |                       | lFinished​(InstallEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `onHttpA              |                       |
        |                       | rtifactCacheStartedEv |                       |
        |                       | ent​(HttpArtifactCache |                       |
        |                       | Event.Started event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `onRuleKe             | ::: block             |
        |                       | yCalculationFinished​( | Records when a        |
        |                       | BuildRuleEvent.Finish | rulekey finished      |
        |                       | edRuleKeyCalc event)` | calculation and it is |
        |                       |                       | time to extract time  |
        |                       |                       | it took.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `onRule               | ::: block             |
        |                       | KeyCalculationStarted | Records when we start |
        |                       | ​(BuildRuleEvent.Start | calculating a         |
        |                       | edRuleKeyCalc event)` | rulekey.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `pa                   |                       |
        |                       | rseFinished​(ParseEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `parseStarted​(ParseEv |                       |
        |                       | ent.Started started)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `proje                |                       |
        |                       | ctGenerationFinished​( |                       |
        |                       | ProjectGenerationEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.event.BuckEventListener}

            ### Methods inherited from interface com.facebook.buck.event.[BuckEventListener](../BuckEventListener.html "interface in com.facebook.buck.event")

            `close`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.event.BuckEventBus,com.facebook.buck.util.environment.ExecutionEnvironment)}

        -   #### PerfTimesEventListener

                public PerfTimesEventListener​(BuckEventBus eventBus,
                                              ExecutionEnvironment executionEnvironment)

            [Parameters:]{.paramLabel}
            :   `eventBus` - When we finish gather all data points, we
                will post the result as event back into event bus.
            :   `executionEnvironment` - We need this in order to get
                Python_init_time, as it is provided by our Python
                wrapper.
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#initializationFinished(com.facebook.buck.event.BuckInitializationDurationEvent)}

        -   #### initializationFinished

            ``` methodSignature
            public void initializationFinished​(BuckInitializationDurationEvent event)
            ```

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

        []{#actionGraphFinished(com.facebook.buck.event.ActionGraphEvent.Finished)}

        -   #### actionGraphFinished

            ``` methodSignature
            public void actionGraphFinished​(ActionGraphEvent.Finished finished)
            ```

        []{#projectGenerationFinished(com.facebook.buck.event.ProjectGenerationEvent.Finished)}

        -   #### projectGenerationFinished

            ``` methodSignature
            public void projectGenerationFinished​(ProjectGenerationEvent.Finished finished)
            ```

        []{#onRuleKeyCalculationStarted(com.facebook.buck.core.build.event.BuildRuleEvent.StartedRuleKeyCalc)}

        -   #### onRuleKeyCalculationStarted

            ``` methodSignature
            public void onRuleKeyCalculationStarted​(BuildRuleEvent.StartedRuleKeyCalc event)
            ```

            ::: block
            Records when we start calculating a rulekey.
            :::

            [Parameters:]{.paramLabel}
            :   `event` - the event that sings the start.

        []{#onRuleKeyCalculationFinished(com.facebook.buck.core.build.event.BuildRuleEvent.FinishedRuleKeyCalc)}

        -   #### onRuleKeyCalculationFinished

            ``` methodSignature
            public void onRuleKeyCalculationFinished​(BuildRuleEvent.FinishedRuleKeyCalc event)
            ```

            ::: block
            Records when a rulekey finished calculation and it is time
            to extract time it took.
            :::

            [Parameters:]{.paramLabel}
            :   `event` - the event that signs the end of calculation.

        []{#onHttpArtifactCacheStartedEvent(com.facebook.buck.artifact_cache.HttpArtifactCacheEvent.Started)}

        -   #### onHttpArtifactCacheStartedEvent

            ``` methodSignature
            public void onHttpArtifactCacheStartedEvent​(HttpArtifactCacheEvent.Started event)
            ```

        []{#buildRuleWillBuildLocally(com.facebook.buck.core.build.event.BuildRuleEvent.WillBuildLocally)}

        -   #### buildRuleWillBuildLocally

            ``` methodSignature
            public void buildRuleWillBuildLocally​(BuildRuleEvent.WillBuildLocally event)
            ```

        []{#buildFinished(com.facebook.buck.core.build.event.BuildEvent.Finished)}

        -   #### buildFinished

            ``` methodSignature
            public void buildFinished​(BuildEvent.Finished finished)
            ```

        []{#installFinished(com.facebook.buck.event.InstallEvent.Finished)}

        -   #### installFinished

            ``` methodSignature
            public void installFinished​(InstallEvent.Finished finished)
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
-   [Nested](#nested.class.summary) \| 
-   Field \| 
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
