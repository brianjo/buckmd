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
-   [Package](package-summary.html)
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

<div>

-   Summary: 
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.remoteexecution](package-summary.html)
:::

## Interface ContentAddressedStorageClient {#interface-contentaddressedstorageclient .title title="Interface ContentAddressedStorageClient"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `GrpcContentAddressableStorageClient`,
        `LocalContentAddressedStorage`

    ------------------------------------------------------------------------

        public interface ContentAddressedStorageClient

    ::: block
    This is a simple ContentAddressedStorageClient interface used for
    remote execution.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Interface             | Description           |
        +=======================+=======================+=======================+
        | `static interface `   | `Conte                | ::: block             |
        |                       | ntAddressedStorageCli | Interface for         |
        |                       | ent.FileMaterializer` | filesystem operations |
        |                       |                       | required for          |
        |                       |                       | materialization.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
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
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#addMissing(java.util.Collection)}

        -   #### addMissing

            ``` methodSignature
            com.google.common.util.concurrent.ListenableFuture<Unit> addMissing​(Collection<UploadDataSupplier> data)
                                                                         throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#materializeOutputs(java.util.List,java.util.List,com.facebook.buck.remoteexecution.ContentAddressedStorageClient.FileMaterializer)}

        -   #### materializeOutputs

            ``` methodSignature
            com.google.common.util.concurrent.ListenableFuture<Unit> materializeOutputs​(List<Protocol.OutputDirectory> outputDirectories,
                                                                                        List<Protocol.OutputFile> outputFiles,
                                                                                        ContentAddressedStorageClient.FileMaterializer materializer)
                                                                                 throws IOException
            ```

            ::: block
            Materializes the outputFiles and outputDirectories into
            root.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#containsDigest(com.facebook.buck.remoteexecution.interfaces.Protocol.Digest)}

        -   #### containsDigest

            ``` methodSignature
            boolean containsDigest​(Protocol.Digest digest)
            ```

        []{#fetch(com.facebook.buck.remoteexecution.interfaces.Protocol.Digest)}

        -   #### fetch

            ``` methodSignature
            com.google.common.util.concurrent.ListenableFuture<ByteBuffer> fetch​(Protocol.Digest digest)
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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
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

<div>

-   Summary: 
-   [Nested](#nested.class.summary) \| 
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
