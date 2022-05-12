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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.build.event](package-summary.html)
:::

## Class BuildEvent {#class-buildevent .title title="Class BuildEvent"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.event.AbstractBuckEvent](../../../event/AbstractBuckEvent.html "class in com.facebook.buck.event")

    -   -   com.facebook.buck.core.build.event.BuildEvent

::: description
-   

    All Implemented Interfaces:
    :   `BuckEvent`, `BuckEventExternalInterface`, `WorkAdvanceEvent`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `BuildEvent.BuildReport`, `BuildEvent.Finished`,
        `BuildEvent.RuleCountCalculated`, `BuildEvent.Started`,
        `BuildEvent.UnskippedRuleCountUpdated`

    ------------------------------------------------------------------------

        public abstract class BuildEvent
        extends AbstractBuckEvent
        implements WorkAdvanceEvent

    ::: block
    Base class for events about building.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `Bu                   | ::: block             |
        |                       | ildEvent.BuildReport` | Event used to post    |
        |                       |                       | build reports         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `BuildEvent.Finished` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `BuildEvent           |                       |
        |                       | .RuleCountCalculated` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `BuildEvent.Started`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `BuildEvent.Unski     |                       |
        |                       | ppedRuleCountUpdated` |                       |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Fields inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](../../../event/external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `BUILD_FINISHED, BUILD_REPORT, BUILD_STARTED, BUILD_STATUS_EVENT, CACHE_RATE_STATS_UPDATE_EVENT, INDIVIDUAL_TEST_AWAITING_RESULTS, INSTALL_STARTED, PARSE_FINISHED, PARSE_STARTED, PROJECT_GENERATION_FINISHED, PROJECT_GENERATION_STARTED, TEST_RUN_STARTED`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                       Description
          --------------------------------- -------------
          `BuildEvent​(EventKey eventKey)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                               Method                                                                                                                      Description
          ----------------------------------------------- --------------------------------------------------------------------------------------------------------------------------- -------------
          `static BuildEvent.BuildReport`                 `buildReport​(String buildReportJson)`                                                                                        
          `static BuildEvent.Finished`                    `finished​(BuildEvent.Started started,         ExitCode exitCode)`                                                            
          `static BuildEvent.RuleCountCalculated`         `ruleCountCalculated​(com.google.common.collect.ImmutableSet<BuildTarget> buildTargets,                    int ruleCount)`    
          `static BuildEvent.Started`                     `started​(Iterable<String> buildArgs)`                                                                                        
          `static BuildEvent.UnskippedRuleCountUpdated`   `unskippedRuleCountUpdated​(int ruleCount)`                                                                                   

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.event.AbstractBuckEvent}

            ### Methods inherited from class com.facebook.buck.event.[AbstractBuckEvent](../../../event/AbstractBuckEvent.html "class in com.facebook.buck.event")

            `configure, equals, getBuildId, getEventKey, getNanoTime, getThreadId, getThreadUserNanoTime, getTimestampMillis, getValueString, hashCode, isConfigured, isRelatedTo, toLogMessage, toString`

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

            ### Methods inherited from interface com.facebook.buck.event.[BuckEvent](../../../event/BuckEvent.html "interface in com.facebook.buck.event")

            `configure, getBuildId, getEventKey, getNanoTime, getThreadId, getThreadUserNanoTime, isConfigured, isRelatedTo, toLogMessage`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Methods inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](../../../event/external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `getEventName, getTimestampMillis, storeLastInstanceAndReplayForNewClients`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.event.EventKey)}

        -   #### BuildEvent

                public BuildEvent​(EventKey eventKey)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#started(java.lang.Iterable)}

        -   #### started

            ``` methodSignature
            public static BuildEvent.Started started​(Iterable<String> buildArgs)
            ```

        []{#finished(com.facebook.buck.core.build.event.BuildEvent.Started,com.facebook.buck.util.ExitCode)}

        -   #### finished

            ``` methodSignature
            public static BuildEvent.Finished finished​(BuildEvent.Started started,
                                                       ExitCode exitCode)
            ```

        []{#ruleCountCalculated(com.google.common.collect.ImmutableSet,int)}

        -   #### ruleCountCalculated

            ``` methodSignature
            public static BuildEvent.RuleCountCalculated ruleCountCalculated​(com.google.common.collect.ImmutableSet<BuildTarget> buildTargets,
                                                                             int ruleCount)
            ```

        []{#unskippedRuleCountUpdated(int)}

        -   #### unskippedRuleCountUpdated

            ``` methodSignature
            public static BuildEvent.UnskippedRuleCountUpdated unskippedRuleCountUpdated​(int ruleCount)
            ```

        []{#buildReport(java.lang.String)}

        -   #### buildReport

            ``` methodSignature
            public static BuildEvent.BuildReport buildReport​(String buildReportJson)
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
