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
[Package]{.packageLabelInType} [com.facebook.buck.slb](package-summary.html)
:::

## Interface HybridThriftOverHttpService\<ThriftRequest extends org.apache.thrift.TBase\<?,​?\>,​ThriftResponse extends org.apache.thrift.TBase\<?,​?\>\> {#interface-hybridthriftoverhttpservicethriftrequest-extends-org.apache.thrift.tbasethriftresponse-extends-org.apache.thrift.tbase .title title="Interface HybridThriftOverHttpService"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AutoCloseable`, `Closeable`,
        `ThriftOverHttpService<ThriftRequest,​ThriftResponse>`,
        `ThriftService<ThriftRequest,​ThriftResponse>`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `HybridThriftOverHttpServiceImpl`

    ------------------------------------------------------------------------

        public interface HybridThriftOverHttpService<ThriftRequest extends org.apache.thrift.TBase<?,​?>,​ThriftResponse extends org.apache.thrift.TBase<?,​?>>
        extends ThriftOverHttpService<ThriftRequest,​ThriftResponse>

    ::: block
    Sync and async methods to communicate using the Hybrid Thrift
    protocol.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.                 | `makeReque            | ::: block             |
        | google.common.util.co | st​(HybridThriftReques | Asynchronously make a |
        | ncurrent.ListenableFu | tHandler<ThriftReques | request.              |
        | ture<ThriftResponse>` | t> request,           | :::                   |
        |                       |   HybridThriftRespons |                       |
        |                       | eHandler<ThriftRespon |                       |
        |                       | se> responseHandler)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ThriftResponse`      | `makeRequestSync​(H    | ::: block             |
        |                       | ybridThriftRequestHan | Synchronously make a  |
        |                       | dler<ThriftRequest> r | request.              |
        |                       | equest,               | :::                   |
        |                       |   HybridThriftRespons |                       |
        |                       | eHandler<ThriftRespon |                       |
        |                       | se> responseHandler)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.java.io.Closeable}

            ### Methods inherited from interface java.io.[Closeable](http://docs.oracle.com/javase/7/docs/api/java/io/Closeable.html?is-external=true "class or interface in java.io"){.externalLink}

            `close`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.slb.ThriftService}

            ### Methods inherited from interface com.facebook.buck.slb.[ThriftService](ThriftService.html "interface in com.facebook.buck.slb")

            `makeRequest`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#makeRequest(com.facebook.buck.slb.HybridThriftRequestHandler,com.facebook.buck.slb.HybridThriftResponseHandler)}

        -   #### makeRequest

            ``` methodSignature
            com.google.common.util.concurrent.ListenableFuture<ThriftResponse> makeRequest​(HybridThriftRequestHandler<ThriftRequest> request,
                                                                                           HybridThriftResponseHandler<ThriftResponse> responseHandler)
            ```

            ::: block
            Asynchronously make a request.
            :::

        []{#makeRequestSync(com.facebook.buck.slb.HybridThriftRequestHandler,com.facebook.buck.slb.HybridThriftResponseHandler)}

        -   #### makeRequestSync

            ``` methodSignature
            ThriftResponse makeRequestSync​(HybridThriftRequestHandler<ThriftRequest> request,
                                           HybridThriftResponseHandler<ThriftResponse> responseHandler)
                                    throws IOException
            ```

            ::: block
            Synchronously make a request.
            :::

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
