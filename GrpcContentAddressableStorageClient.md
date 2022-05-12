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
[Package]{.packageLabelInType} [com.facebook.buck.remoteexecution.grpc](package-summary.html)
:::

## Class GrpcContentAddressableStorageClient {#class-grpccontentaddressablestorageclient .title title="Class GrpcContentAddressableStorageClient"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.remoteexecution.grpc.GrpcContentAddressableStorageClient

::: description
-   

    All Implemented Interfaces:
    :   `ContentAddressedStorageClient`

    ------------------------------------------------------------------------

        public class GrpcContentAddressableStorageClient
        extends Object
        implements ContentAddressedStorageClient

    ::: block
    Implementation of a CAS client using GRPC.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.remoteexecution.ContentAddressedStorageClient}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.remoteexecution.[ContentAddressedStorageClient](../ContentAddressedStorageClient.html "interface in com.facebook.buck.remoteexecution")

            `ContentAddressedStorageClient.FileMaterializer`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `GrpcContentAddressableStorageClient​(build.bazel.remote.execution.v2.ContentAddressableStorageGrpc.ContentAddressableStorageFutureStub storageStub,                                    com.google.bytestream.ByteStreamGrpc.ByteStreamStub byteStreamStub,                                    int casDeadline,                                    String instanceName,                                    Protocol protocol,                                    BuckEventBus buckEventBus,                                    com.facebook.buck.remoteexecution.proto.RemoteExecutionMetadata metadata,                                    int outputMaterializationThreads)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.google.comm      | `addMis               |                       |
        | on.util.concurrent.Li | sing​(Collection<Uploa |                       |
        | stenableFuture<Unit>` | dDataSupplier> data)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `containsDigest​(Pro   |                       |
        |                       | tocol.Digest digest)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `fetch​(Pro            |                       |
        | com.google.common.uti | tocol.Digest digest)` |                       |
        | l.concurrent.Listenab |                       |                       |
        | leFuture<ByteBuffer>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.comm      | `materializeOutpu     | ::: block             |
        | on.util.concurrent.Li | ts​(List<Protocol.Outp | Materializes the      |
        | stenableFuture<Unit>` | utDirectory> outputDi | outputFiles and       |
        |                       | rectories,            | outputDirectories     |
        |                       |         List<Protocol | into root.            |
        |                       | .OutputFile> outputFi | :::                   |
        |                       | les,                  |                       |
        |                       |   ContentAddressedSto |                       |
        |                       | rageClient.FileMateri |                       |
        |                       | alizer materializer)` |                       |
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

        []{#<init>(build.bazel.remote.execution.v2.ContentAddressableStorageGrpc.ContentAddressableStorageFutureStub,com.google.bytestream.ByteStreamGrpc.ByteStreamStub,int,java.lang.String,com.facebook.buck.remoteexecution.interfaces.Protocol,com.facebook.buck.event.BuckEventBus,com.facebook.buck.remoteexecution.proto.RemoteExecutionMetadata,int)}

        -   #### GrpcContentAddressableStorageClient

                public GrpcContentAddressableStorageClient​(build.bazel.remote.execution.v2.ContentAddressableStorageGrpc.ContentAddressableStorageFutureStub storageStub,
                                                           com.google.bytestream.ByteStreamGrpc.ByteStreamStub byteStreamStub,
                                                           int casDeadline,
                                                           String instanceName,
                                                           Protocol protocol,
                                                           BuckEventBus buckEventBus,
                                                           com.facebook.buck.remoteexecution.proto.RemoteExecutionMetadata metadata,
                                                           int outputMaterializationThreads)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#addMissing(java.util.Collection)}

        -   #### addMissing

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<Unit> addMissing​(Collection<UploadDataSupplier> data)
                                                                                throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `addMissing` in
                interface `ContentAddressedStorageClient`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#materializeOutputs(java.util.List,java.util.List,com.facebook.buck.remoteexecution.ContentAddressedStorageClient.FileMaterializer)}

        -   #### materializeOutputs

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<Unit> materializeOutputs​(List<Protocol.OutputDirectory> outputDirectories,
                                                                                               List<Protocol.OutputFile> outputFiles,
                                                                                               ContentAddressedStorageClient.FileMaterializer materializer)
                                                                                        throws IOException
            ```

            ::: block
            [Description copied from
            interface: `ContentAddressedStorageClient`]{.descfrmTypeLabel}
            :::

            ::: block
            Materializes the outputFiles and outputDirectories into
            root.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `materializeOutputs` in
                interface `ContentAddressedStorageClient`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#containsDigest(com.facebook.buck.remoteexecution.interfaces.Protocol.Digest)}

        -   #### containsDigest

            ``` methodSignature
            public boolean containsDigest​(Protocol.Digest digest)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `containsDigest` in
                interface `ContentAddressedStorageClient`

        []{#fetch(com.facebook.buck.remoteexecution.interfaces.Protocol.Digest)}

        -   #### fetch

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<ByteBuffer> fetch​(Protocol.Digest digest)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `fetch` in interface `ContentAddressedStorageClient`
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
