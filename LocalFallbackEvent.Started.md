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

## Class LocalFallbackEvent.Started {#class-localfallbackevent.started .title title="Class LocalFallbackEvent.Started"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.event.AbstractBuckEvent](../../event/AbstractBuckEvent.html "class in com.facebook.buck.event")

    -   -   [com.facebook.buck.remoteexecution.event.LocalFallbackEvent](LocalFallbackEvent.html "class in com.facebook.buck.remoteexecution.event")

        -   -   com.facebook.buck.remoteexecution.event.LocalFallbackEvent.Started

::: description
-   

    All Implemented Interfaces:
    :   `BuckEvent`, `BuckEventExternalInterface`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [LocalFallbackEvent](LocalFallbackEvent.html "class in com.facebook.buck.remoteexecution.event")

    ------------------------------------------------------------------------

        public static class LocalFallbackEvent.Started
        extends LocalFallbackEvent

    ::: block
    When the LocalFallbackStrategy starts processing a single BuildRule.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.remoteexecution.event.LocalFallbackEvent}

            ### Nested classes/interfaces inherited from class com.facebook.buck.remoteexecution.event.[LocalFallbackEvent](LocalFallbackEvent.html "class in com.facebook.buck.remoteexecution.event")

            `LocalFallbackEvent.Finished, LocalFallbackEvent.Result, LocalFallbackEvent.Started`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Fields inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](../../event/external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `BUILD_FINISHED, BUILD_REPORT, BUILD_STARTED, BUILD_STATUS_EVENT, CACHE_RATE_STATS_UPDATE_EVENT, INDIVIDUAL_TEST_AWAITING_RESULTS, INSTALL_STARTED, PARSE_FINISHED, PARSE_STARTED, PROJECT_GENERATION_FINISHED, PROJECT_GENERATION_STARTED, TEST_RUN_STARTED`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type               Method                                                                                                                                                                                                                                                                                                                                                                                                                                                                               Description
          ------------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `LocalFallbackEvent.Finished`   `createFinished​(LocalFallbackEvent.Result remoteResult,               LocalFallbackEvent.Result localResult,               long remoteDurationMillis,               Optional<String> remoteErrorMessage,               io.grpc.Status remoteGrpcStatus,               RemoteExecutionActionEvent.State lastNonTerminalState,               OptionalInt exitCode,               Optional<com.facebook.buck.remoteexecution.proto.RemoteExecutionMetadata> remoteExecutionMetadata)`    
          `String`                        `getBuildTarget()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                    
          `protected String`              `getValueString()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.remoteexecution.event.LocalFallbackEvent}

            ### Methods inherited from class com.facebook.buck.remoteexecution.event.[LocalFallbackEvent](LocalFallbackEvent.html "class in com.facebook.buck.remoteexecution.event")

            `createStarted, getEventName`

        ```{=html}
        <!-- -->
        ```
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

        []{#createFinished(com.facebook.buck.remoteexecution.event.LocalFallbackEvent.Result,com.facebook.buck.remoteexecution.event.LocalFallbackEvent.Result,long,java.util.Optional,io.grpc.Status,com.facebook.buck.remoteexecution.event.RemoteExecutionActionEvent.State,java.util.OptionalInt,java.util.Optional)}

        -   #### createFinished

            ``` methodSignature
            public LocalFallbackEvent.Finished createFinished​(LocalFallbackEvent.Result remoteResult,
                                                              LocalFallbackEvent.Result localResult,
                                                              long remoteDurationMillis,
                                                              Optional<String> remoteErrorMessage,
                                                              io.grpc.Status remoteGrpcStatus,
                                                              RemoteExecutionActionEvent.State lastNonTerminalState,
                                                              OptionalInt exitCode,
                                                              Optional<com.facebook.buck.remoteexecution.proto.RemoteExecutionMetadata> remoteExecutionMetadata)
            ```

        []{#getBuildTarget()}

        -   #### getBuildTarget

            ``` methodSignature
            public String getBuildTarget()
            ```

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
