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
[Package]{.packageLabelInType} [com.facebook.buck.remoteexecution.event](package-summary.html)
:::

## Interface RemoteExecutionStatsProvider {#interface-remoteexecutionstatsprovider .title title="Interface RemoteExecutionStatsProvider"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `RemoteExecutionEventListener`

    ------------------------------------------------------------------------

        public interface RemoteExecutionStatsProvider

    ::: block
    Provides statistics about the ongoing remote execution flow.
    :::
:::

::: summary
-   ::: {.section role="region"}
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

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getActionsPerState()}

        -   #### getActionsPerState

            ``` methodSignature
            com.google.common.collect.ImmutableMap<RemoteExecutionActionEvent.State,​Integer> getActionsPerState()
            ```

            ::: block
            Current state of all remote execution Actions.
            :::

        []{#getCasDownloads()}

        -   #### getCasDownloads

            ``` methodSignature
            int getCasDownloads()
            ```

            ::: block
            Total number of downloads.
            :::

        []{#getCasDownloadSizeBytes()}

        -   #### getCasDownloadSizeBytes

            ``` methodSignature
            long getCasDownloadSizeBytes()
            ```

            ::: block
            Total number of downloaded bytes from CAS.
            :::

        []{#getCasUploads()}

        -   #### getCasUploads

            ``` methodSignature
            int getCasUploads()
            ```

            ::: block
            Total number of downloads.
            :::

        []{#getCasUploadSizeBytes()}

        -   #### getCasUploadSizeBytes

            ``` methodSignature
            long getCasUploadSizeBytes()
            ```

            ::: block
            Total of uploaded bytes to CAS.
            :::

        []{#getTotalRulesBuilt()}

        -   #### getTotalRulesBuilt

            ``` methodSignature
            int getTotalRulesBuilt()
            ```

            ::: block
            Get the total number of BuildRules that are finished. (both
            local and remote)
            :::

        []{#getLocalFallbackStats()}

        -   #### getLocalFallbackStats

            ``` methodSignature
            LocalFallbackStats getLocalFallbackStats()
            ```

            ::: block
            Fetches stats regarding the local fallback.
            :::

        []{#getRemoteCpuTimeMs()}

        -   #### getRemoteCpuTimeMs

            ``` methodSignature
            long getRemoteCpuTimeMs()
            ```

            ::: block
            Metadata for total time spent executing actions remotely in
            millis.
            :::

        []{#getRemoteQueueTimeMs()}

        -   #### getRemoteQueueTimeMs

            ``` methodSignature
            long getRemoteQueueTimeMs()
            ```

            ::: block
            Metadata for total time spent queued for executing actions
            in millis.
            :::

        []{#getTotalRemoteTimeMs()}

        -   #### getTotalRemoteTimeMs

            ``` methodSignature
            long getTotalRemoteTimeMs()
            ```

            ::: block
            Metadata for total time spent running actions remotely.
            :::

        []{#exportFieldsToMap()}

        -   #### exportFieldsToMap

            ``` methodSignature
            com.google.common.collect.ImmutableMap<String,​String> exportFieldsToMap()
            ```

            ::: block
            Export all the above metadata in a Map format
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
