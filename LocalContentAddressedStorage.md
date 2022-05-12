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
[Package]{.packageLabelInType} [com.facebook.buck.remoteexecution.util](package-summary.html)
:::

## Class LocalContentAddressedStorage {#class-localcontentaddressedstorage .title title="Class LocalContentAddressedStorage"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.remoteexecution.util.LocalContentAddressedStorage

::: description
-   

    All Implemented Interfaces:
    :   `ContentAddressedStorageClient`

    ------------------------------------------------------------------------

        public class LocalContentAddressedStorage
        extends Object
        implements ContentAddressedStorageClient

    ::: block
    A simple, on-disk content addressed storage.
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

          Constructor                                                                                                                                           Description
          ----------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `LocalContentAddressedStorage​(Path cacheDir,                             Protocol protocol,                             BuckEventBus buckEventBus)`    

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
        | `com.goo              | `bat                  | ::: block             |
        | gle.common.collect.Im | chUpdateBlobs​(com.goo | Upload blobs.         |
        | mutableList<CasBlobUp | gle.common.collect.Im | :::                   |
        | loader.UploadResult>` | mutableList<UploadDat |                       |
        |                       | aSupplier> blobData)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `containsDigest​(Pro   |                       |
        |                       | tocol.Digest digest)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `fetch​(Pro            |                       |
        | com.google.common.uti | tocol.Digest digest)` |                       |
        | l.concurrent.Listenab |                       |                       |
        | leFuture<ByteBuffer>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `java.util.stream.Str | `findM                |                       |
        | eam<Protocol.Digest>` | issing​(Iterable<Proto |                       |
        |                       | col.Digest> digests)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `InputStream`         | `getData​(Pro          | ::: block             |
        |                       | tocol.Digest digest)` | Looks up some data.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `FileInputStream`     | `g                    | ::: block             |
        |                       | etFileInputStream​(Pro | Get a file input      |
        |                       | tocol.Digest digest)` | stream to a Digest    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.   | `getTree​(Protoco      | ::: block             |
        | collect.ImmutableList | l.Digest rootDigest)` | Returns a list of all |
        | <Protocol.Directory>` |                       | sub directories.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Protocol.Action`     | `materi               |                       |
        |                       | alizeAction​(Protocol. |                       |
        |                       | Digest actionDigest)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Option               | `materializ           |                       |
        | al<Protocol.Command>` | eInputs​(Path buildDir |                       |
        |                       | ,                  Pr |                       |
        |                       | otocol.Digest rootDig |                       |
        |                       | est,                  |                       |
        |                       |  Optional<Protocol.Di |                       |
        |                       | gest> commandDigest)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.comm      | `materializeOutpu     | ::: block             |
        | on.util.concurrent.Li | ts​(List<Protocol.Outp | Materializes the      |
        | stenableFuture<Unit>` | utDirectory> outputDi | outputs into the      |
        |                       | rectories,            | build root.           |
        |                       |         List<Protocol | :::                   |
        |                       | .OutputFile> outputFi |                       |
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

        []{#<init>(java.nio.file.Path,com.facebook.buck.remoteexecution.interfaces.Protocol,com.facebook.buck.event.BuckEventBus)}

        -   #### LocalContentAddressedStorage

                public LocalContentAddressedStorage​(Path cacheDir,
                                                    Protocol protocol,
                                                    BuckEventBus buckEventBus)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#batchUpdateBlobs(com.google.common.collect.ImmutableList)}

        -   #### batchUpdateBlobs

            ``` methodSignature
            public com.google.common.collect.ImmutableList<CasBlobUploader.UploadResult> batchUpdateBlobs​(com.google.common.collect.ImmutableList<UploadDataSupplier> blobData)
            ```

            ::: block
            Upload blobs.
            :::

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

        []{#materializeOutputs(java.util.List,java.util.List,com.facebook.buck.remoteexecution.ContentAddressedStorageClient.FileMaterializer)}

        -   #### materializeOutputs

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<Unit> materializeOutputs​(List<Protocol.OutputDirectory> outputDirectories,
                                                                                               List<Protocol.OutputFile> outputFiles,
                                                                                               ContentAddressedStorageClient.FileMaterializer materializer)
                                                                                        throws IOException
            ```

            ::: block
            Materializes the outputs into the build root. All required
            data must be present (or inlined).
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `materializeOutputs` in
                interface `ContentAddressedStorageClient`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#materializeAction(com.facebook.buck.remoteexecution.interfaces.Protocol.Digest)}

        -   #### materializeAction

            ``` methodSignature
            public Protocol.Action materializeAction​(Protocol.Digest actionDigest)
                                              throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#materializeInputs(java.nio.file.Path,com.facebook.buck.remoteexecution.interfaces.Protocol.Digest,java.util.Optional)}

        -   #### materializeInputs

            ``` methodSignature
            public Optional<Protocol.Command> materializeInputs​(Path buildDir,
                                                                Protocol.Digest rootDigest,
                                                                Optional<Protocol.Digest> commandDigest)
                                                         throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getTree(com.facebook.buck.remoteexecution.interfaces.Protocol.Digest)}

        -   #### getTree

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Protocol.Directory> getTree​(Protocol.Digest rootDigest)
                                                                                throws IOException
            ```

            ::: block
            Returns a list of all sub directories.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getData(com.facebook.buck.remoteexecution.interfaces.Protocol.Digest)}

        -   #### getData

            ``` methodSignature
            public InputStream getData​(Protocol.Digest digest)
                                throws IOException
            ```

            ::: block
            Looks up some data. Used internally and in tests.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getFileInputStream(com.facebook.buck.remoteexecution.interfaces.Protocol.Digest)}

        -   #### getFileInputStream

            ``` methodSignature
            public FileInputStream getFileInputStream​(Protocol.Digest digest)
                                               throws IOException
            ```

            ::: block
            Get a file input stream to a Digest
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#findMissing(java.lang.Iterable)}

        -   #### findMissing

            ``` methodSignature
            public java.util.stream.Stream<Protocol.Digest> findMissing​(Iterable<Protocol.Digest> digests)
            ```
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
