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
[Package]{.packageLabelInType} [com.facebook.buck.remoteexecution](package-summary.html)
:::

## Interface AsyncBlobFetcher {#interface-asyncblobfetcher .title title="Interface AsyncBlobFetcher"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `GrpcAsyncBlobFetcher`

    ------------------------------------------------------------------------

        public interface AsyncBlobFetcher

    ::: block
    Interface used by OutputsMaterializer to fetch outputs from the CAS.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                  Method                                                                                                                                                                                                                                                               Description
          ------------------------------------------------------------------ -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `com.google.common.util.concurrent.ListenableFuture<Unit>`         `batchFetchBlobs​(com.google.common.collect.ImmutableMultimap<Protocol.Digest,​Callable<WritableByteChannel>> requests,                com.google.common.collect.ImmutableMultimap<Protocol.Digest,​com.google.common.util.concurrent.SettableFuture<Unit>> futures)`    
          `com.google.common.util.concurrent.ListenableFuture<ByteBuffer>`   `fetch​(Protocol.Digest digest)`                                                                                                                                                                                                                                       
          `com.google.common.util.concurrent.ListenableFuture<Unit>`         `fetchToStream​(Protocol.Digest digest,              WritableByteChannel channel)`                                                                                                                                                                                     

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

        []{#fetch(com.facebook.buck.remoteexecution.interfaces.Protocol.Digest)}

        -   #### fetch

            ``` methodSignature
            com.google.common.util.concurrent.ListenableFuture<ByteBuffer> fetch​(Protocol.Digest digest)
            ```

        []{#fetchToStream(com.facebook.buck.remoteexecution.interfaces.Protocol.Digest,java.nio.channels.WritableByteChannel)}

        -   #### fetchToStream

            ``` methodSignature
            com.google.common.util.concurrent.ListenableFuture<Unit> fetchToStream​(Protocol.Digest digest,
                                                                                   WritableByteChannel channel)
            ```

        []{#batchFetchBlobs(com.google.common.collect.ImmutableMultimap,com.google.common.collect.ImmutableMultimap)}

        -   #### batchFetchBlobs

            ``` methodSignature
            com.google.common.util.concurrent.ListenableFuture<Unit> batchFetchBlobs​(com.google.common.collect.ImmutableMultimap<Protocol.Digest,​Callable<WritableByteChannel>> requests,
                                                                                     com.google.common.collect.ImmutableMultimap<Protocol.Digest,​com.google.common.util.concurrent.SettableFuture<Unit>> futures)
                                                                              throws IOException
            ```

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
