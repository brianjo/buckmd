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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.remoteexecution.grpc](package-summary.html)
:::

## Class GrpcRemoteExecutionClients {#class-grpcremoteexecutionclients .title title="Class GrpcRemoteExecutionClients"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.remoteexecution.grpc.GrpcRemoteExecutionClients

::: description
-   

    All Implemented Interfaces:
    :   `RemoteExecutionClients`, `Closeable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class GrpcRemoteExecutionClients
        extends Object
        implements RemoteExecutionClients

    ::: block
    A RemoteExecution that sends jobs to a grpc-based remote execution
    service.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field        Description
          ------------------- ------------ -------------
          `static Protocol`   `PROTOCOL`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                    Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `GrpcRemoteExecutionClients​(String instanceName,                           io.grpc.ManagedChannel executionEngineChannel,                           io.grpc.ManagedChannel casChannel,                           int casDeadline,                           MetadataProvider metadataProvider,                           BuckEventBus buckEventBus,                           RemoteExecutionStrategyConfig strategyConfig)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `close()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ContentAd            | `getConte             |                       |
        | dressedStorageClient` | ntAddressedStorage()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Protocol`            | `getProtocol()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `RemoteEx             | `getRemo              |                       |
        | ecutionServiceClient` | teExecutionService()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `getResourceNa        |                       |
        |                       | me​(String instanceNam |                       |
        |                       | e,                Pro |                       |
        |                       | tocol.Digest digest)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `s                    | `rea                  | ::: block             |
        | tatic com.google.comm | dByteStream​(String in | Reads a ByteStream    |
        | on.util.concurrent.Li | stanceName,           | onto the arg          |
        | stenableFuture<Unit>` |      Protocol.Digest  | consumer.             |
        |                       | digest,               | :::                   |
        |                       |  com.google.bytestrea |                       |
        |                       | m.ByteStreamGrpc.Byte |                       |
        |                       | StreamStub byteStream |                       |
        |                       | Stub,               T |                       |
        |                       | hrowingConsumer<com.g |                       |
        |                       | oogle.protobuf.ByteSt |                       |
        |                       | ring,​IOException> dat |                       |
        |                       | aConsumer,            |                       |
        |                       |     int casDeadline)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
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
    -   []{#field.detail}

        ### Field Detail

        []{#PROTOCOL}

        -   #### PROTOCOL

                public static final Protocol PROTOCOL
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.lang.String,io.grpc.ManagedChannel,io.grpc.ManagedChannel,int,com.facebook.buck.remoteexecution.interfaces.MetadataProvider,com.facebook.buck.event.BuckEventBus,com.facebook.buck.remoteexecution.config.RemoteExecutionStrategyConfig)}

        -   #### GrpcRemoteExecutionClients

                public GrpcRemoteExecutionClients​(String instanceName,
                                                  io.grpc.ManagedChannel executionEngineChannel,
                                                  io.grpc.ManagedChannel casChannel,
                                                  int casDeadline,
                                                  MetadataProvider metadataProvider,
                                                  BuckEventBus buckEventBus,
                                                  RemoteExecutionStrategyConfig strategyConfig)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getResourceName(java.lang.String,com.facebook.buck.remoteexecution.interfaces.Protocol.Digest)}

        -   #### getResourceName

            ``` methodSignature
            public static String getResourceName​(String instanceName,
                                                 Protocol.Digest digest)
            ```

        []{#readByteStream(java.lang.String,com.facebook.buck.remoteexecution.interfaces.Protocol.Digest,com.google.bytestream.ByteStreamGrpc.ByteStreamStub,com.facebook.buck.util.function.ThrowingConsumer,int)}

        -   #### readByteStream

            ``` methodSignature
            public static com.google.common.util.concurrent.ListenableFuture<Unit> readByteStream​(String instanceName,
                                                                                                  Protocol.Digest digest,
                                                                                                  com.google.bytestream.ByteStreamGrpc.ByteStreamStub byteStreamStub,
                                                                                                  ThrowingConsumer<com.google.protobuf.ByteString,​IOException> dataConsumer,
                                                                                                  int casDeadline)
            ```

            ::: block
            Reads a ByteStream onto the arg consumer.
            :::

        []{#getRemoteExecutionService()}

        -   #### getRemoteExecutionService

            ``` methodSignature
            public RemoteExecutionServiceClient getRemoteExecutionService()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRemoteExecutionService` in
                interface `RemoteExecutionClients`

        []{#getContentAddressedStorage()}

        -   #### getContentAddressedStorage

            ``` methodSignature
            public ContentAddressedStorageClient getContentAddressedStorage()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getContentAddressedStorage` in
                interface `RemoteExecutionClients`

        []{#getProtocol()}

        -   #### getProtocol

            ``` methodSignature
            public Protocol getProtocol()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getProtocol` in interface `RemoteExecutionClients`

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
                       throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `Closeable`

            [Throws:]{.throwsLabel}
            :   `IOException`
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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
