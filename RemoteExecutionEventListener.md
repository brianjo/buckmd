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
-   Nested \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.remoteexecution.event.listener](package-summary.html)
:::

## Class RemoteExecutionEventListener {#class-remoteexecutioneventlistener .title title="Class RemoteExecutionEventListener"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.remoteexecution.event.listener.RemoteExecutionEventListener

::: description
-   

    All Implemented Interfaces:
    :   `BuckEventListener`, `RemoteExecutionStatsProvider`,
        `Closeable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class RemoteExecutionEventListener
        extends Object
        implements BuckEventListener, RemoteExecutionStatsProvider

    ::: block
    Remote execution events sent to the event bus.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                        Description
          ---------------------------------- -------------
          `RemoteExecutionEventListener()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.google.c         | `exportFieldsToMap()` | ::: block             |
        | ommon.collect.Immutab |                       | Export all the above  |
        | leMap<String,​String>` |                       | metadata in a Map     |
        |                       |                       | format                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.   | `                     | ::: block             |
        | collect.ImmutableMap< | getActionsPerState()` | Current state of all  |
        | RemoteExecutionAction |                       | remote execution      |
        | Event.State,​Integer>` |                       | Actions.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getCasDownloads()`   | ::: block             |
        |                       |                       | Total number of       |
        |                       |                       | downloads.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `getCa                | ::: block             |
        |                       | sDownloadSizeBytes()` | Total number of       |
        |                       |                       | downloaded bytes from |
        |                       |                       | CAS.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getCasUploads()`     | ::: block             |
        |                       |                       | Total number of       |
        |                       |                       | downloads.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `get                  | ::: block             |
        |                       | CasUploadSizeBytes()` | Total of uploaded     |
        |                       |                       | bytes to CAS.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `LocalFallbackStats`  | `get                  | ::: block             |
        |                       | LocalFallbackStats()` | Fetches stats         |
        |                       |                       | regarding the local   |
        |                       |                       | fallback.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `                     | ::: block             |
        |                       | getRemoteCpuTimeMs()` | Metadata for total    |
        |                       |                       | time spent executing  |
        |                       |                       | actions remotely in   |
        |                       |                       | millis.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `ge                   | ::: block             |
        |                       | tRemoteQueueTimeMs()` | Metadata for total    |
        |                       |                       | time spent queued for |
        |                       |                       | executing actions in  |
        |                       |                       | millis.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `LongAdder`           | `getStateCount​(       |                       |
        |                       | RemoteExecutionAction |                       |
        |                       | Event.State waiting)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `ge                   | ::: block             |
        |                       | tTotalRemoteTimeMs()` | Metadata for total    |
        |                       |                       | time spent running    |
        |                       |                       | actions remotely.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `                     | ::: block             |
        |                       | getTotalRulesBuilt()` | Get the total number  |
        |                       |                       | of BuildRules that    |
        |                       |                       | are finished.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `on                   | ::: block             |
        |                       | ActionEventFinished​(R | Event specific        |
        |                       | emoteExecutionActionE | subscriber method.    |
        |                       | vent.Finished event)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `                     | ::: block             |
        |                       | onActionEventStarted​( | Event specific        |
        |                       | RemoteExecutionAction | subscriber method.    |
        |                       | Event.Started event)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `on                   | ::: block             |
        |                       | ActionEventTerminal​(R | Event specific        |
        |                       | emoteExecutionActionE | subscriber method.    |
        |                       | vent.Terminal event)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `onActionScheduled​(Re | ::: block             |
        |                       | moteExecutionActionEv | Event specific        |
        |                       | ent.Scheduled event)` | subscriber method.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `onBuil               | ::: block             |
        |                       | dRuleEvent​(BuildRuleE | Event specific        |
        |                       | vent.Finished event)` | subscriber method.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `onCasDownloadE       | ::: block             |
        |                       | vent​(CasBlobDownloadE | Event specific        |
        |                       | vent.Finished event)` | subscriber method.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `onCasUploa           | ::: block             |
        |                       | dEvent​(CasBlobUploadE | Event specific        |
        |                       | vent.Finished event)` | subscriber method.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `o                    | ::: block             |
        |                       | nLocalFallbackEventFi | Events from the       |
        |                       | nished​(LocalFallbackE | LocalFallback stats.  |
        |                       | vent.Finished event)` | :::                   |
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

            ### Methods inherited from interface com.facebook.buck.event.[BuckEventListener](../../../event/BuckEventListener.html "interface in com.facebook.buck.event")

            `close`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### RemoteExecutionEventListener

                public RemoteExecutionEventListener()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#onBuildRuleEvent(com.facebook.buck.core.build.event.BuildRuleEvent.Finished)}

        -   #### onBuildRuleEvent

            ``` methodSignature
            public void onBuildRuleEvent​(BuildRuleEvent.Finished event)
            ```

            ::: block
            Event specific subscriber method.
            :::

        []{#onCasUploadEvent(com.facebook.buck.remoteexecution.event.CasBlobUploadEvent.Finished)}

        -   #### onCasUploadEvent

            ``` methodSignature
            public void onCasUploadEvent​(CasBlobUploadEvent.Finished event)
            ```

            ::: block
            Event specific subscriber method.
            :::

        []{#onCasDownloadEvent(com.facebook.buck.remoteexecution.event.CasBlobDownloadEvent.Finished)}

        -   #### onCasDownloadEvent

            ``` methodSignature
            public void onCasDownloadEvent​(CasBlobDownloadEvent.Finished event)
            ```

            ::: block
            Event specific subscriber method.
            :::

        []{#onActionScheduled(com.facebook.buck.remoteexecution.event.RemoteExecutionActionEvent.Scheduled)}

        -   #### onActionScheduled

            ``` methodSignature
            public void onActionScheduled​(RemoteExecutionActionEvent.Scheduled event)
            ```

            ::: block
            Event specific subscriber method.
            :::

        []{#onActionEventTerminal(com.facebook.buck.remoteexecution.event.RemoteExecutionActionEvent.Terminal)}

        -   #### onActionEventTerminal

            ``` methodSignature
            public void onActionEventTerminal​(RemoteExecutionActionEvent.Terminal event)
            ```

            ::: block
            Event specific subscriber method.
            :::

        []{#onActionEventStarted(com.facebook.buck.remoteexecution.event.RemoteExecutionActionEvent.Started)}

        -   #### onActionEventStarted

            ``` methodSignature
            public void onActionEventStarted​(RemoteExecutionActionEvent.Started event)
            ```

            ::: block
            Event specific subscriber method.
            :::

        []{#getStateCount(com.facebook.buck.remoteexecution.event.RemoteExecutionActionEvent.State)}

        -   #### getStateCount

            ``` methodSignature
            public LongAdder getStateCount​(RemoteExecutionActionEvent.State waiting)
            ```

        []{#onActionEventFinished(com.facebook.buck.remoteexecution.event.RemoteExecutionActionEvent.Finished)}

        -   #### onActionEventFinished

            ``` methodSignature
            public void onActionEventFinished​(RemoteExecutionActionEvent.Finished event)
            ```

            ::: block
            Event specific subscriber method.
            :::

        []{#onLocalFallbackEventFinished(com.facebook.buck.remoteexecution.event.LocalFallbackEvent.Finished)}

        -   #### onLocalFallbackEventFinished

            ``` methodSignature
            public void onLocalFallbackEventFinished​(LocalFallbackEvent.Finished event)
            ```

            ::: block
            Events from the LocalFallback stats.
            :::

        []{#getActionsPerState()}

        -   #### getActionsPerState

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<RemoteExecutionActionEvent.State,​Integer> getActionsPerState()
            ```

            ::: block
            [Description copied from
            interface: `RemoteExecutionStatsProvider`]{.descfrmTypeLabel}
            :::

            ::: block
            Current state of all remote execution Actions.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getActionsPerState` in
                interface `RemoteExecutionStatsProvider`

        []{#getCasDownloads()}

        -   #### getCasDownloads

            ``` methodSignature
            public int getCasDownloads()
            ```

            ::: block
            [Description copied from
            interface: `RemoteExecutionStatsProvider`]{.descfrmTypeLabel}
            :::

            ::: block
            Total number of downloads.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCasDownloads` in
                interface `RemoteExecutionStatsProvider`

        []{#getCasDownloadSizeBytes()}

        -   #### getCasDownloadSizeBytes

            ``` methodSignature
            public long getCasDownloadSizeBytes()
            ```

            ::: block
            [Description copied from
            interface: `RemoteExecutionStatsProvider`]{.descfrmTypeLabel}
            :::

            ::: block
            Total number of downloaded bytes from CAS.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCasDownloadSizeBytes` in
                interface `RemoteExecutionStatsProvider`

        []{#getCasUploads()}

        -   #### getCasUploads

            ``` methodSignature
            public int getCasUploads()
            ```

            ::: block
            [Description copied from
            interface: `RemoteExecutionStatsProvider`]{.descfrmTypeLabel}
            :::

            ::: block
            Total number of downloads.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCasUploads` in
                interface `RemoteExecutionStatsProvider`

        []{#getCasUploadSizeBytes()}

        -   #### getCasUploadSizeBytes

            ``` methodSignature
            public long getCasUploadSizeBytes()
            ```

            ::: block
            [Description copied from
            interface: `RemoteExecutionStatsProvider`]{.descfrmTypeLabel}
            :::

            ::: block
            Total of uploaded bytes to CAS.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCasUploadSizeBytes` in
                interface `RemoteExecutionStatsProvider`

        []{#getTotalRulesBuilt()}

        -   #### getTotalRulesBuilt

            ``` methodSignature
            public int getTotalRulesBuilt()
            ```

            ::: block
            [Description copied from
            interface: `RemoteExecutionStatsProvider`]{.descfrmTypeLabel}
            :::

            ::: block
            Get the total number of BuildRules that are finished. (both
            local and remote)
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTotalRulesBuilt` in
                interface `RemoteExecutionStatsProvider`

        []{#getLocalFallbackStats()}

        -   #### getLocalFallbackStats

            ``` methodSignature
            public LocalFallbackStats getLocalFallbackStats()
            ```

            ::: block
            [Description copied from
            interface: `RemoteExecutionStatsProvider`]{.descfrmTypeLabel}
            :::

            ::: block
            Fetches stats regarding the local fallback.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLocalFallbackStats` in
                interface `RemoteExecutionStatsProvider`

        []{#getRemoteCpuTimeMs()}

        -   #### getRemoteCpuTimeMs

            ``` methodSignature
            public long getRemoteCpuTimeMs()
            ```

            ::: block
            [Description copied from
            interface: `RemoteExecutionStatsProvider`]{.descfrmTypeLabel}
            :::

            ::: block
            Metadata for total time spent executing actions remotely in
            millis.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRemoteCpuTimeMs` in
                interface `RemoteExecutionStatsProvider`

        []{#getRemoteQueueTimeMs()}

        -   #### getRemoteQueueTimeMs

            ``` methodSignature
            public long getRemoteQueueTimeMs()
            ```

            ::: block
            [Description copied from
            interface: `RemoteExecutionStatsProvider`]{.descfrmTypeLabel}
            :::

            ::: block
            Metadata for total time spent queued for executing actions
            in millis.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRemoteQueueTimeMs` in
                interface `RemoteExecutionStatsProvider`

        []{#getTotalRemoteTimeMs()}

        -   #### getTotalRemoteTimeMs

            ``` methodSignature
            public long getTotalRemoteTimeMs()
            ```

            ::: block
            [Description copied from
            interface: `RemoteExecutionStatsProvider`]{.descfrmTypeLabel}
            :::

            ::: block
            Metadata for total time spent running actions remotely.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTotalRemoteTimeMs` in
                interface `RemoteExecutionStatsProvider`

        []{#exportFieldsToMap()}

        -   #### exportFieldsToMap

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​String> exportFieldsToMap()
            ```

            ::: block
            [Description copied from
            interface: `RemoteExecutionStatsProvider`]{.descfrmTypeLabel}
            :::

            ::: block
            Export all the above metadata in a Map format
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `exportFieldsToMap` in
                interface `RemoteExecutionStatsProvider`
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
-   Nested \| 
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
