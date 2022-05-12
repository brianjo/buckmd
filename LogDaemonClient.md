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
[Package]{.packageLabelInType} [com.facebook.buck.logd.client](package-summary.html)
:::

## Interface LogDaemonClient {#interface-logdaemonclient .title title="Interface LogDaemonClient"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `LogdClient`

    ------------------------------------------------------------------------

        public interface LogDaemonClient

    ::: block
    Interface for LogD Client.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `int`                 | `createLog            | ::: block             |
        |                       | File​(String logFilePa | Client calls this     |
        |                       | th,              com. | method to request     |
        |                       | facebook.buck.logd.pr | LogD to create a log  |
        |                       | oto.LogType logType)` | file in file-system   |
        |                       |                       | and/or storage.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `io.grp               | `openLog              | ::: block             |
        | c.stub.StreamObserver | ​(int logFileId,       | Client calls this     |
        | <com.facebook.buck.lo |   String logMessage)` | method to acquire a   |
        | gd.proto.LogMessage>` |                       | StreamObserver object |
        |                       |                       | which listens for     |
        |                       |                       | incoming logs.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `shutdown()`          | ::: block             |
        |                       |                       | close all existing    |
        |                       |                       | channels to logD      |
        |                       |                       | server                |
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

        []{#createLogFile(java.lang.String,com.facebook.buck.logd.proto.LogType)}

        -   #### createLogFile

            ``` methodSignature
            int createLogFile​(String logFilePath,
                              com.facebook.buck.logd.proto.LogType logType)
                       throws LogDaemonException
            ```

            ::: block
            Client calls this method to request LogD to create a log
            file in file-system and/or storage.
            :::

            [Returns:]{.returnLabel}
            :   a file identifier `logFileId` corresponding to the
                created file by LogD server

            [Throws:]{.throwsLabel}
            :   `LogDaemonException`

        []{#openLog(int,java.lang.String)}

        -   #### openLog

            ``` methodSignature
            io.grpc.stub.StreamObserver<com.facebook.buck.logd.proto.LogMessage> openLog​(int logFileId,
                                                                                         String logMessage)
                                                                                  throws LogDaemonException
            ```

            ::: block
            Client calls this method to acquire a StreamObserver object
            which listens for incoming logs. Upon receiving the
            StreamObserver, client uses it to stream log messages to
            locations identified by `logFileId`
            :::

            [Parameters:]{.paramLabel}
            :   `logFileId` - log file identifier generated by LogD
                server
            :   `logMessage` - log message to be streamed to LogD

            [Returns:]{.returnLabel}
            :   a StreamObserver which observers and processes incoming
                logs from client

            [Throws:]{.throwsLabel}
            :   `LogDaemonException`

        []{#shutdown()}

        -   #### shutdown

            ``` methodSignature
            void shutdown()
            ```

            ::: block
            close all existing channels to logD server
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
