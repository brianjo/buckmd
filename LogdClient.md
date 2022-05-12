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
[Package]{.packageLabelInType} [com.facebook.buck.logd.client](package-summary.html)
:::

## Class LogdClient {#class-logdclient .title title="Class LogdClient"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.logd.client.LogdClient

::: description
-   

    All Implemented Interfaces:
    :   `LogDaemonClient`

    ------------------------------------------------------------------------

        public class LogdClient
        extends Object
        implements LogDaemonClient

    ::: block
    Given a host and port number, this client is used to make a
    connection and stream logs to logD server
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `LogdClient​(io.gr                 | ::: block                         |
        | pc.ManagedChannelBuilder<?> chann | Constructs a LogdClient with the  |
        | elBuilder,           StreamObserv | provided channel                  |
        | erFactory streamObserverFactory)` | :::                               |
        +-----------------------------------+-----------------------------------+
        | `LogdClient​(                      | ::: block                         |
        | String host,           int port)` | Constructs a LogdClient with the  |
        |                                   | provided hostname and port        |
        |                                   | number.                           |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `                                 | ::: block                         |
        | LogdClient​(String host,           | Constructs a LogdClient with the  |
        |  int port,           StreamObserv | provided hostname, port number    |
        | erFactory streamObserverFactory)` | and an implementation of          |
        |                                   | StreamObserverFactory.            |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `int`                 | `cr                   | ::: block             |
        |                       | eateLogFile​(String pa | Client calls this     |
        |                       | th,              com. | method to request     |
        |                       | facebook.buck.logd.pr | LogD to create a log  |
        |                       | oto.LogType logType)` | file in file-system   |
        |                       |                       | and/or storage.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `io.grp               | `openLog              | ::: block             |
        | c.stub.StreamObserver | ​(int logFileId,       | Client calls this     |
        | <com.facebook.buck.lo |   String logContent)` | method to acquire a   |
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
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.lang.String,int)}

        -   #### LogdClient

                public LogdClient​(String host,
                                  int port)

            ::: block
            Constructs a LogdClient with the provided hostname and port
            number.
            :::

            [Parameters:]{.paramLabel}
            :   `host` - host name
            :   `port` - port number

        []{#<init>(java.lang.String,int,com.facebook.buck.logd.client.StreamObserverFactory)}

        -   #### LogdClient

                public LogdClient​(String host,
                                  int port,
                                  StreamObserverFactory streamObserverFactory)

            ::: block
            Constructs a LogdClient with the provided hostname, port
            number and an implementation of StreamObserverFactory.
            :::

            [Parameters:]{.paramLabel}
            :   `host` - host name
            :   `port` - port number
            :   `streamObserverFactory` - an implementation of
                StreamObserverFactory

        []{#<init>(io.grpc.ManagedChannelBuilder,com.facebook.buck.logd.client.StreamObserverFactory)}

        -   #### LogdClient

                public LogdClient​(io.grpc.ManagedChannelBuilder<?> channelBuilder,
                                  StreamObserverFactory streamObserverFactory)

            ::: block
            Constructs a LogdClient with the provided channel
            :::

            [Parameters:]{.paramLabel}
            :   `channelBuilder` - a channel to LogD server
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#shutdown()}

        -   #### shutdown

            ``` methodSignature
            public void shutdown()
            ```

            ::: block
            [Description copied from
            interface: `LogDaemonClient`]{.descfrmTypeLabel}
            :::

            ::: block
            close all existing channels to logD server
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `shutdown` in interface `LogDaemonClient`

        []{#createLogFile(java.lang.String,com.facebook.buck.logd.proto.LogType)}

        -   #### createLogFile

            ``` methodSignature
            public int createLogFile​(String path,
                                     com.facebook.buck.logd.proto.LogType logType)
                              throws LogDaemonException
            ```

            ::: block
            [Description copied from
            interface: `LogDaemonClient`]{.descfrmTypeLabel}
            :::

            ::: block
            Client calls this method to request LogD to create a log
            file in file-system and/or storage.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `createLogFile` in interface `LogDaemonClient`

            [Returns:]{.returnLabel}
            :   a file identifier `logFileId` corresponding to the
                created file by LogD server

            [Throws:]{.throwsLabel}
            :   `LogDaemonException`

        []{#openLog(int,java.lang.String)}

        -   #### openLog

            ``` methodSignature
            public io.grpc.stub.StreamObserver<com.facebook.buck.logd.proto.LogMessage> openLog​(int logFileId,
                                                                                                String logContent)
                                                                                         throws LogDaemonException
            ```

            ::: block
            [Description copied from
            interface: `LogDaemonClient`]{.descfrmTypeLabel}
            :::

            ::: block
            Client calls this method to acquire a StreamObserver object
            which listens for incoming logs. Upon receiving the
            StreamObserver, client uses it to stream log messages to
            locations identified by `logFileId`
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `openLog` in interface `LogDaemonClient`

            [Parameters:]{.paramLabel}
            :   `logFileId` - log file identifier generated by LogD
                server
            :   `logContent` - log message to be streamed to LogD

            [Returns:]{.returnLabel}
            :   a StreamObserver which observers and processes incoming
                logs from client

            [Throws:]{.throwsLabel}
            :   `LogDaemonException`
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
