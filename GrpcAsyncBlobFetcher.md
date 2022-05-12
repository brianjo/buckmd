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
[Package]{.packageLabelInType} [com.facebook.buck.remoteexecution.grpc](package-summary.html)
:::

## Class GrpcAsyncBlobFetcher {#class-grpcasyncblobfetcher .title title="Class GrpcAsyncBlobFetcher"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.remoteexecution.grpc.GrpcAsyncBlobFetcher

::: description
-   

    All Implemented Interfaces:
    :   `AsyncBlobFetcher`

    ------------------------------------------------------------------------

        public class GrpcAsyncBlobFetcher
        extends Object
        implements AsyncBlobFetcher

    ::: block
    GRPC implementation of the AsyncBlobFetcher.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `GrpcAsyncBlobFetcher​(String instanceName,                     build.bazel.remote.execution.v2.ContentAddressableStorageGrpc.ContentAddressableStorageFutureStub storageStub,                     com.google.bytestream.ByteStreamGrpc.ByteStreamStub byteStreamStub,                     BuckEventBus buckEventBus,                     com.facebook.buck.remoteexecution.proto.RemoteExecutionMetadata metadata,                     Protocol protocol,                     int casDeadline)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                  Method                                                                                                                                                                                                                                                               Description
          ------------------------------------------------------------------ -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `com.google.common.util.concurrent.ListenableFuture<Unit>`         `batchFetchBlobs​(com.google.common.collect.ImmutableMultimap<Protocol.Digest,​Callable<WritableByteChannel>> requests,                com.google.common.collect.ImmutableMultimap<Protocol.Digest,​com.google.common.util.concurrent.SettableFuture<Unit>> futures)`    
          `com.google.common.util.concurrent.ListenableFuture<ByteBuffer>`   `fetch​(Protocol.Digest digest)`                                                                                                                                                                                                                                       
          `com.google.common.util.concurrent.ListenableFuture<Unit>`         `fetchToStream​(Protocol.Digest digest,              WritableByteChannel channel)`                                                                                                                                                                                     

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

        []{#<init>(java.lang.String,build.bazel.remote.execution.v2.ContentAddressableStorageGrpc.ContentAddressableStorageFutureStub,com.google.bytestream.ByteStreamGrpc.ByteStreamStub,com.facebook.buck.event.BuckEventBus,com.facebook.buck.remoteexecution.proto.RemoteExecutionMetadata,com.facebook.buck.remoteexecution.interfaces.Protocol,int)}

        -   #### GrpcAsyncBlobFetcher

                public GrpcAsyncBlobFetcher​(String instanceName,
                                            build.bazel.remote.execution.v2.ContentAddressableStorageGrpc.ContentAddressableStorageFutureStub storageStub,
                                            com.google.bytestream.ByteStreamGrpc.ByteStreamStub byteStreamStub,
                                            BuckEventBus buckEventBus,
                                            com.facebook.buck.remoteexecution.proto.RemoteExecutionMetadata metadata,
                                            Protocol protocol,
                                            int casDeadline)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#fetch(com.facebook.buck.remoteexecution.interfaces.Protocol.Digest)}

        -   #### fetch

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<ByteBuffer> fetch​(Protocol.Digest digest)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `fetch` in interface `AsyncBlobFetcher`

        []{#fetchToStream(com.facebook.buck.remoteexecution.interfaces.Protocol.Digest,java.nio.channels.WritableByteChannel)}

        -   #### fetchToStream

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<Unit> fetchToStream​(Protocol.Digest digest,
                                                                                          WritableByteChannel channel)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `fetchToStream` in interface `AsyncBlobFetcher`

        []{#batchFetchBlobs(com.google.common.collect.ImmutableMultimap,com.google.common.collect.ImmutableMultimap)}

        -   #### batchFetchBlobs

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<Unit> batchFetchBlobs​(com.google.common.collect.ImmutableMultimap<Protocol.Digest,​Callable<WritableByteChannel>> requests,
                                                                                            com.google.common.collect.ImmutableMultimap<Protocol.Digest,​com.google.common.util.concurrent.SettableFuture<Unit>> futures)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `batchFetchBlobs` in interface `AsyncBlobFetcher`
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
