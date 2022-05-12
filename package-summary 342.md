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
-   Package
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Package com.facebook.buck.log {#package-com.facebook.buck.log .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [CommandIdToIsDaemonMapper](Co    |                                   |
    | mmandIdToIsDaemonMapper.html "int |                                   |
    | erface in com.facebook.buck.log") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CommandIdToIsR                   | ::: block                         |
    | emoteExecutionMapper](CommandIdTo | This tracks where a given command |
    | IsRemoteExecutionMapper.html "int | was run with remote execution.    |
    | erface in com.facebook.buck.log") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CommandIdToIsSuperCons           |                                   |
    | oleEnabledMapper](CommandIdToIsSu |                                   |
    | perConsoleEnabledMapper.html "int |                                   |
    | erface in com.facebook.buck.log") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ConsoleHandlerSta                | ::: block                         |
    | te](ConsoleHandlerState.html "int | How the ConsoleHandler is         |
    | erface in com.facebook.buck.log") | supposed to behave for a          |
    |                                   | particular thread.                |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ConsoleHandlerState.Writer](Con  |                                   |
    | soleHandlerState.Writer.html "int |                                   |
    | erface in com.facebook.buck.log") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Globa                            |                                   |
    | lStateManager.LoggerIsMappedToThr |                                   |
    | eadScope](GlobalStateManager.Logg |                                   |
    | erIsMappedToThreadScope.html "int |                                   |
    | erface in com.facebook.buck.log") |                                   |
    +-----------------------------------+-----------------------------------+
    | [LogFileHandlerSta                |                                   |
    | te](LogFileHandlerState.html "int |                                   |
    | erface in com.facebook.buck.log") |                                   |
    +-----------------------------------+-----------------------------------+
    | [TraceInfoProv                    | ::: block                         |
    | ider](TraceInfoProvider.html "int | Provides any tracing related      |
    | erface in com.facebook.buck.log") | information.                      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [Async                            | ::: block                         |
    | LogHandler](AsyncLogHandler.html  | Wraps a log Handler, e.g.         |
    | "class in com.facebook.buck.log") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CompressingFileHand              |                                   |
    | ler](CompressingFileHandler.html  |                                   |
    | "class in com.facebook.buck.log") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Con                              | ::: block                         |
    | soleHandler](ConsoleHandler.html  | Implementation of Handler which   |
    | "class in com.facebook.buck.log") | writes to the console (System.err |
    |                                   | by default).                      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Err                              |                                   |
    | orLogRecord](ErrorLogRecord.html  |                                   |
    | "class in com.facebook.buck.log") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ErrorLogRecord.Buil              |                                   |
    | der](ErrorLogRecord.Builder.html  |                                   |
    | "class in com.facebook.buck.log") |                                   |
    +-----------------------------------+-----------------------------------+
    | [GlobalState                      |                                   |
    | Manager](GlobalStateManager.html  |                                   |
    | "class in com.facebook.buck.log") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Inv                              |                                   |
    | ocationInfo](InvocationInfo.html  |                                   |
    | "class in com.facebook.buck.log") |                                   |
    +-----------------------------------+-----------------------------------+
    | [LogConfig](LogConfig.html        | ::: block                         |
    | "class in com.facebook.buck.log") | Constructed by                    |
    |                                   | java.util.logging.LogManager via  |
    |                                   | the system property               |
    |                                   | jav                               |
    |                                   | a.util.logging.LogManager.config. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Log                              | ::: block                         |
    | ConfigPaths](LogConfigPaths.html  | Utility class containing          |
    | "class in com.facebook.buck.log") | constants for logging             |
    |                                   | configuration paths.              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Log                              |                                   |
    | ConfigSetup](LogConfigSetup.html  |                                   |
    | "class in com.facebook.buck.log") |                                   |
    +-----------------------------------+-----------------------------------+
    | [LogConfigSetup.Buil              |                                   |
    | der](LogConfigSetup.Builder.html  |                                   |
    | "class in com.facebook.buck.log") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Log                              |                                   |
    | FileHandler](LogFileHandler.html  |                                   |
    | "class in com.facebook.buck.log") |                                   |
    +-----------------------------------+-----------------------------------+
    | [LogFileHandlerDispatche          | ::: block                         |
    | r](LogFileHandlerDispatcher.html  | Switches between synchronous and  |
    | "class in com.facebook.buck.log") | asynchronous LogFileHandler,      |
    |                                   | depending on value returned from  |
    |                                   | LogC                              |
    |                                   | onfig.shouldUseAsyncFileLogging() |
    |                                   | Note: this could potentially      |
    |                                   | change after                      |
    |                                   | LogFileHandlerDispatcher is       |
    |                                   | created                           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [LogFormatter](LogFormatter.html  |                                   |
    | "class in com.facebook.buck.log") |                                   |
    +-----------------------------------+-----------------------------------+
    | [MachineReadableLogConfi          |                                   |
    | g](MachineReadableLogConfig.html  |                                   |
    | "class in com.facebook.buck.log") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Per                              |                                   |
    | fTimesStats](PerfTimesStats.html  |                                   |
    | "class in com.facebook.buck.log") |                                   |
    +-----------------------------------+-----------------------------------+
    | [PerfTimesStats.Buil              |                                   |
    | der](PerfTimesStats.Builder.html  |                                   |
    | "class in com.facebook.buck.log") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ReferenceCountedWri              |                                   |
    | ter](ReferenceCountedWriter.html  |                                   |
    | "class in com.facebook.buck.log") |                                   |
    +-----------------------------------+-----------------------------------+
    | [TimedLogger](TimedLogger.html    | ::: block                         |
    | "class in com.facebook.buck.log") | Records the time that logging     |
    |                                   | calls takes, and alerts if they   |
    |                                   | go over configured threshold.     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../index.html)
-   Package
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

[]{#skip.navbar.bottom}
:::
