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
[Package]{.packageLabelInType} [com.facebook.buck.remoteexecution.event](package-summary.html)
:::

## Class RemoteExecutionActionEvent {#class-remoteexecutionactionevent .title title="Class RemoteExecutionActionEvent"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.event.AbstractBuckEvent](../../event/AbstractBuckEvent.html "class in com.facebook.buck.event")

    -   -   com.facebook.buck.remoteexecution.event.RemoteExecutionActionEvent

::: description
-   

    All Implemented Interfaces:
    :   `BuckEvent`, `BuckEventExternalInterface`, `WorkAdvanceEvent`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `RemoteExecutionActionEvent.Finished`,
        `RemoteExecutionActionEvent.InputsUploaded`,
        `RemoteExecutionActionEvent.Scheduled`,
        `RemoteExecutionActionEvent.Started`,
        `RemoteExecutionActionEvent.Terminal`

    ------------------------------------------------------------------------

        public abstract class RemoteExecutionActionEvent
        extends AbstractBuckEvent
        implements WorkAdvanceEvent

    ::: block
    Tracks events related to Remote Execution Actions.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `RemoteExecution      | ::: block             |
        |                       | ActionEvent.Finished` | An action just exited |
        |                       |                       | from this state.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `                     | ::: block             |
        |                       | RemoteExecutionAction | Describes the event   |
        |                       | Event.InputsUploaded` | which occurs right    |
        |                       |                       | after inputs were     |
        |                       |                       | uploaded to the CAS.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `RemoteExecutionA     | ::: block             |
        |                       | ctionEvent.Scheduled` | Indicates that a      |
        |                       |                       | remote execution      |
        |                       |                       | event has been        |
        |                       |                       | scheduled.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `RemoteExecutio       | ::: block             |
        |                       | nActionEvent.Started` | An action just moved  |
        |                       |                       | into this state.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `RemoteExecut         | ::: block             |
        |                       | ionActionEvent.State` | The current state of  |
        |                       |                       | a Remote Execution    |
        |                       |                       | Actions.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `RemoteExecution      | ::: block             |
        |                       | ActionEvent.Terminal` | Sends a one off       |
        |                       |                       | terminal event for a  |
        |                       |                       | Remote Execution      |
        |                       |                       | Action.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Fields inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](../../event/external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `BUILD_FINISHED, BUILD_REPORT, BUILD_STARTED, BUILD_STATUS_EVENT, CACHE_RATE_STATS_UPDATE_EVENT, INDIVIDUAL_TEST_AWAITING_RESULTS, INSTALL_STARTED, PARSE_FINISHED, PARSE_STARTED, PROJECT_GENERATION_FINISHED, PROJECT_GENERATION_STARTED, TEST_RUN_STARTED`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                       Description
          -------------- ------------------------------------------------- -------------
          `protected `   `RemoteExecutionActionEvent​(EventKey eventKey)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static String`       | `actionDig            |                       |
        |                       | estToString​(Protocol. |                       |
        |                       | Digest actionDigest)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getEventName()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `isTerminalStat       |                       |
        |                       | e​(RemoteExecutionActi |                       |
        |                       | onEvent.State state)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Scope`        | `sendEvent​(Buck       | ::: block             |
        |                       | EventBus eventBus,    | Takes care of sending |
        |                       |        RemoteExecutio | both Started and      |
        |                       | nActionEvent.State st | Finished events       |
        |                       | ate,          BuildRu | within a Scope.       |
        |                       | le buildRule,         | :::                   |
        |                       |   Optional<Protocol.D |                       |
        |                       | igest> actionDigest)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `sendInputsUpl        | ::: block             |
        |                       | oadedEventIfNeed​(Buck | Sending the           |
        |                       | EventBus eventBus,    | InputsUploaded event  |
        |                       |                       | :::                   |
        |                       |       BuildRule build |                       |
        |                       | Rule,                 |                       |
        |                       |               List<Re |                       |
        |                       | moteExecutionActionEv |                       |
        |                       | ent.InputsUploaded.La |                       |
        |                       | rgeBlob> largeBlobs)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `sendScheduledEvent   |                       |
        |                       | ​(BuckEventBus eventBu |                       |
        |                       | s,                    |                       |
        |                       | BuildRule buildRule)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `sendTerminal         | ::: block             |
        |                       | Event​(BuckEventBus ev | Sends the terminal    |
        |                       | entBus,               | event of an action    |
        |                       |     RemoteExecutionAc | \[FAIL\|SUCCESS\].    |
        |                       | tionEvent.State state | :::                   |
        |                       | ,                  Bu |                       |
        |                       | ildRule buildRule,    |                       |
        |                       |                Option |                       |
        |                       | al<Protocol.Digest> a |                       |
        |                       | ctionDigest,          |                       |
        |                       |          Optional<bui |                       |
        |                       | ld.bazel.remote.execu |                       |
        |                       | tion.v2.ExecutedActio |                       |
        |                       | nMetadata> executedAc |                       |
        |                       | tionMetadata,         |                       |
        |                       |           Optional<co |                       |
        |                       | m.facebook.buck.remot |                       |
        |                       | eexecution.proto.Remo |                       |
        |                       | teExecutionMetadata>  |                       |
        |                       | remoteExecutionMetada |                       |
        |                       | ta,                   |                       |
        |                       | Optional<Map<RemoteEx |                       |
        |                       | ecutionActionEvent.St |                       |
        |                       | ate,​Long>> stateMetad |                       |
        |                       | ata,                  |                       |
        |                       |  Optional<Map<RemoteE |                       |
        |                       | xecutionActionEvent.S |                       |
        |                       | tate,​Long>> stateWait |                       |
        |                       | ingMetadata,          |                       |
        |                       |          io.grpc.Stat |                       |
        |                       | us grpcStatus,        |                       |
        |                       |            RemoteExec |                       |
        |                       | utionActionEvent.Stat |                       |
        |                       | e lastNonTerminalStat |                       |
        |                       | e,                  O |                       |
        |                       | ptionalInt exitCode)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.event.AbstractBuckEvent}

            ### Methods inherited from class com.facebook.buck.event.[AbstractBuckEvent](../../event/AbstractBuckEvent.html "class in com.facebook.buck.event")

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

            ### Methods inherited from interface com.facebook.buck.event.[BuckEvent](../../event/BuckEvent.html "interface in com.facebook.buck.event")

            `configure, getBuildId, getEventKey, getNanoTime, getThreadId, getThreadUserNanoTime, isConfigured, isRelatedTo, toLogMessage`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Methods inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](../../event/external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `getTimestampMillis, storeLastInstanceAndReplayForNewClients`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.event.EventKey)}

        -   #### RemoteExecutionActionEvent

                protected RemoteExecutionActionEvent​(EventKey eventKey)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#sendEvent(com.facebook.buck.event.BuckEventBus,com.facebook.buck.remoteexecution.event.RemoteExecutionActionEvent.State,com.facebook.buck.core.rules.BuildRule,java.util.Optional)}

        -   #### sendEvent

            ``` methodSignature
            public static Scope sendEvent​(BuckEventBus eventBus,
                                          RemoteExecutionActionEvent.State state,
                                          BuildRule buildRule,
                                          Optional<Protocol.Digest> actionDigest)
            ```

            ::: block
            Takes care of sending both Started and Finished events
            within a Scope.
            :::

        []{#sendTerminalEvent(com.facebook.buck.event.BuckEventBus,com.facebook.buck.remoteexecution.event.RemoteExecutionActionEvent.State,com.facebook.buck.core.rules.BuildRule,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional,io.grpc.Status,com.facebook.buck.remoteexecution.event.RemoteExecutionActionEvent.State,java.util.OptionalInt)}

        -   #### sendTerminalEvent

            ``` methodSignature
            public static void sendTerminalEvent​(BuckEventBus eventBus,
                                                 RemoteExecutionActionEvent.State state,
                                                 BuildRule buildRule,
                                                 Optional<Protocol.Digest> actionDigest,
                                                 Optional<build.bazel.remote.execution.v2.ExecutedActionMetadata> executedActionMetadata,
                                                 Optional<com.facebook.buck.remoteexecution.proto.RemoteExecutionMetadata> remoteExecutionMetadata,
                                                 Optional<Map<RemoteExecutionActionEvent.State,​Long>> stateMetadata,
                                                 Optional<Map<RemoteExecutionActionEvent.State,​Long>> stateWaitingMetadata,
                                                 io.grpc.Status grpcStatus,
                                                 RemoteExecutionActionEvent.State lastNonTerminalState,
                                                 OptionalInt exitCode)
            ```

            ::: block
            Sends the terminal event of an action \[FAIL\|SUCCESS\].
            :::

        []{#sendScheduledEvent(com.facebook.buck.event.BuckEventBus,com.facebook.buck.core.rules.BuildRule)}

        -   #### sendScheduledEvent

            ``` methodSignature
            public static void sendScheduledEvent​(BuckEventBus eventBus,
                                                  BuildRule buildRule)
            ```

        []{#sendInputsUploadedEventIfNeed(com.facebook.buck.event.BuckEventBus,com.facebook.buck.core.rules.BuildRule,java.util.List)}

        -   #### sendInputsUploadedEventIfNeed

            ``` methodSignature
            public static void sendInputsUploadedEventIfNeed​(BuckEventBus eventBus,
                                                             BuildRule buildRule,
                                                             List<RemoteExecutionActionEvent.InputsUploaded.LargeBlob> largeBlobs)
            ```

            ::: block
            Sending the InputsUploaded event
            :::

        []{#isTerminalState(com.facebook.buck.remoteexecution.event.RemoteExecutionActionEvent.State)}

        -   #### isTerminalState

            ``` methodSignature
            public static boolean isTerminalState​(RemoteExecutionActionEvent.State state)
            ```

        []{#getEventName()}

        -   #### getEventName

            ``` methodSignature
            public String getEventName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getEventName` in interface `BuckEventExternalInterface`

            [Returns:]{.returnLabel}
            :   the type of the event.

        []{#actionDigestToString(com.facebook.buck.remoteexecution.interfaces.Protocol.Digest)}

        -   #### actionDigestToString

            ``` methodSignature
            public static String actionDigestToString​(Protocol.Digest actionDigest)
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