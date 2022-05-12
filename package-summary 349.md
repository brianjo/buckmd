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
-   Package
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Package com.facebook.buck.remoteexecution.event {#package-com.facebook.buck.remoteexecution.event .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [                                 | ::: block                         |
    | LocalFallbackStats](LocalFallback | Statistics regarding the          |
    | Stats.html "interface in com.face | LocalFallbackStrategy.            |
    | book.buck.remoteexecution.event") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RemoteExecutionStats             | ::: block                         |
    | Provider](RemoteExecutionStatsPro | Provides statistics about the     |
    | vider.html "interface in com.face | ongoing remote execution flow.    |
    | book.buck.remoteexecution.event") | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [                                 | ::: block                         |
    | CasBlobDownloadEvent](CasBlobDown | Started/Finished event pairs for  |
    | loadEvent.html "class in com.face | CAS blob downloads .              |
    | book.buck.remoteexecution.event") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CasBlobDownloadEve               | ::: block                         |
    | nt.Finished](CasBlobDownloadEvent | Download to the CAS has finished. |
    | .Finished.html "class in com.face | :::                               |
    | book.buck.remoteexecution.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CasBlobDownloadE                 | ::: block                         |
    | vent.Started](CasBlobDownloadEven | Download to the CAS has started.  |
    | t.Started.html "class in com.face | :::                               |
    | book.buck.remoteexecution.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CasBlobUploadEvent](CasBlobUp    | ::: block                         |
    | loadEvent.html "class in com.face | Started/Finished event pairs for  |
    | book.buck.remoteexecution.event") | CAS blob uploads .                |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CasBlobUploadE                   | ::: block                         |
    | vent.Finished](CasBlobUploadEvent | Upload to the CAS has finished.   |
    | .Finished.html "class in com.face | :::                               |
    | book.buck.remoteexecution.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CasBlobUploa                     | ::: block                         |
    | dEvent.Started](CasBlobUploadEven | Upload to the CAS has started.    |
    | t.Started.html "class in com.face | :::                               |
    | book.buck.remoteexecution.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [LocalFallbackEvent](LocalFall    | ::: block                         |
    | backEvent.html "class in com.face | Event containing info about       |
    | book.buck.remoteexecution.event") | single BuildRule executions       |
    |                                   | inside LocalFallbackStrategy.     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [LocalFallbackE                   | ::: block                         |
    | vent.Finished](LocalFallbackEvent | When the LocalFallbackStrategy    |
    | .Finished.html "class in com.face | finished processing a single      |
    | book.buck.remoteexecution.event") | BuildRule.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [LocalFallbac                     | ::: block                         |
    | kEvent.Started](LocalFallbackEven | When the LocalFallbackStrategy    |
    | t.Started.html "class in com.face | starts processing a single        |
    | book.buck.remoteexecution.event") | BuildRule.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [LocalFallbac                     |                                   |
    | kStats.Builder](LocalFallbackStat |                                   |
    | s.Builder.html "class in com.face |                                   |
    | book.buck.remoteexecution.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [RemoteBuildRuleExe               | ::: block                         |
    | cutionEvent](RemoteBuildRuleExecu | Event to signal the end of        |
    | tionEvent.html "class in com.face | building a rule remotely.         |
    | book.buck.remoteexecution.event") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RemoteExecut                     | ::: block                         |
    | ionActionEvent](RemoteExecutionAc | Tracks events related to Remote   |
    | tionEvent.html "class in com.face | Execution Actions.                |
    | book.buck.remoteexecution.event") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RemoteExecutionActionEvent.Fin   | ::: block                         |
    | ished](RemoteExecutionActionEvent | An action just exited from this   |
    | .Finished.html "class in com.face | state.                            |
    | book.buck.remoteexecution.event") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RemoteExe                        | ::: block                         |
    | cutionActionEvent.InputsUploaded] | Describes the event which occurs  |
    | (RemoteExecutionActionEvent.Input | right after inputs were uploaded  |
    | sUploaded.html "class in com.face | to the CAS.                       |
    | book.buck.remoteexecution.event") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RemoteExecutionActionEvent.In    | ::: block                         |
    | putsUploaded.LargeBlob](RemoteExe | Large blob definition             |
    | cutionActionEvent.InputsUploaded. | :::                               |
    | LargeBlob.html "class in com.face |                                   |
    | book.buck.remoteexecution.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [RemoteExecutionActionEvent.Sched | ::: block                         |
    | uled](RemoteExecutionActionEvent. | Indicates that a remote execution |
    | Scheduled.html "class in com.face | event has been scheduled.         |
    | book.buck.remoteexecution.event") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RemoteExecutionActionEvent.S     | ::: block                         |
    | tarted](RemoteExecutionActionEven | An action just moved into this    |
    | t.Started.html "class in com.face | state.                            |
    | book.buck.remoteexecution.event") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RemoteExecutionActionEvent.Ter   | ::: block                         |
    | minal](RemoteExecutionActionEvent | Sends a one off terminal event    |
    | .Terminal.html "class in com.face | for a Remote Execution Action.    |
    | book.buck.remoteexecution.event") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RemoteExecutio                   | ::: block                         |
    | nSessionEvent](RemoteExecutionSes | Base class for events about       |
    | sionEvent.html "class in com.face | building.                         |
    | book.buck.remoteexecution.event") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RemoteExecutionSessionEvent.Fini | ::: block                         |
    | shed](RemoteExecutionSessionEvent | Marks the end of a RE session.    |
    | .Finished.html "class in com.face | :::                               |
    | book.buck.remoteexecution.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [RemoteExecutionSessionEvent.St   | ::: block                         |
    | arted](RemoteExecutionSessionEven | Marks the start of RE session     |
    | t.Started.html "class in com.face | :::                               |
    | book.buck.remoteexecution.event") |                                   |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Enum                              | Description                       |
    +===================================+===================================+
    | [LocalFall                        | ::: block                         |
    | backEvent.Result](LocalFallbackEv | Summary result of an execution.   |
    | ent.Result.html "enum in com.face | :::                               |
    | book.buck.remoteexecution.event") |                                   |
    +-----------------------------------+-----------------------------------+
    | [RemoteExecutionActionEv          | ::: block                         |
    | ent.State](RemoteExecutionActionE | The current state of a Remote     |
    | vent.State.html "enum in com.face | Execution Actions.                |
    | book.buck.remoteexecution.event") | :::                               |
    +-----------------------------------+-----------------------------------+

    : Enum Summary[ ]{.tabEnd}
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../../index.html)
-   Package
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

[]{#skip.navbar.bottom}
:::
