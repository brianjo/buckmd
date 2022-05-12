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

## Class GrpcCasBlobUploader {#class-grpccasblobuploader .title title="Class GrpcCasBlobUploader"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.remoteexecution.grpc.GrpcCasBlobUploader

::: description
-   

    All Implemented Interfaces:
    :   `CasBlobUploader`

    ------------------------------------------------------------------------

        public class GrpcCasBlobUploader
        extends Object
        implements CasBlobUploader

    ::: block
    GRPC implementation of the CasBlobUploader.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.remoteexecution.CasBlobUploader}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.remoteexecution.[CasBlobUploader](../CasBlobUploader.html "interface in com.facebook.buck.remoteexecution")

            `CasBlobUploader.UploadResult`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                      Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `GrpcCasBlobUploader​(String instanceName,                    build.bazel.remote.execution.v2.ContentAddressableStorageGrpc.ContentAddressableStorageFutureStub storageStub,                    com.google.bytestream.ByteStreamGrpc.ByteStreamStub byteStreamStub,                    BuckEventBus buckEventBus,                    com.facebook.buck.remoteexecution.proto.RemoteExecutionMetadata metadata)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                         Method                                                                                  Description
          ------------------------------------------------------------------------- --------------------------------------------------------------------------------------- -------------
          `com.google.common.collect.ImmutableList<CasBlobUploader.UploadResult>`   `batchUpdateBlobs​(com.google.common.collect.ImmutableList<UploadDataSupplier> blobs)`    
          `com.google.common.collect.ImmutableSet<String>`                          `getMissingHashes​(Set<Protocol.Digest> requiredDigests)`                                 
          `CasBlobUploader.UploadResult`                                            `uploadFromStream​(UploadDataSupplier blob)`                                              

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

        []{#<init>(java.lang.String,build.bazel.remote.execution.v2.ContentAddressableStorageGrpc.ContentAddressableStorageFutureStub,com.google.bytestream.ByteStreamGrpc.ByteStreamStub,com.facebook.buck.event.BuckEventBus,com.facebook.buck.remoteexecution.proto.RemoteExecutionMetadata)}

        -   #### GrpcCasBlobUploader

                public GrpcCasBlobUploader​(String instanceName,
                                           build.bazel.remote.execution.v2.ContentAddressableStorageGrpc.ContentAddressableStorageFutureStub storageStub,
                                           com.google.bytestream.ByteStreamGrpc.ByteStreamStub byteStreamStub,
                                           BuckEventBus buckEventBus,
                                           com.facebook.buck.remoteexecution.proto.RemoteExecutionMetadata metadata)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getMissingHashes(java.util.Set)}

        -   #### getMissingHashes

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<String> getMissingHashes​(Set<Protocol.Digest> requiredDigests)
                                                                            throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getMissingHashes` in interface `CasBlobUploader`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#batchUpdateBlobs(com.google.common.collect.ImmutableList)}

        -   #### batchUpdateBlobs

            ``` methodSignature
            public com.google.common.collect.ImmutableList<CasBlobUploader.UploadResult> batchUpdateBlobs​(com.google.common.collect.ImmutableList<UploadDataSupplier> blobs)
                                                                                                   throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `batchUpdateBlobs` in interface `CasBlobUploader`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#uploadFromStream(com.facebook.buck.remoteexecution.UploadDataSupplier)}

        -   #### uploadFromStream

            ``` methodSignature
            public CasBlobUploader.UploadResult uploadFromStream​(UploadDataSupplier blob)
                                                          throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `uploadFromStream` in interface `CasBlobUploader`

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
