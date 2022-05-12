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
[Package]{.packageLabelInType} [com.facebook.buck.slb](package-summary.html)
:::

## Class HybridThriftOverHttpServiceImpl\<ThriftRequest extends org.apache.thrift.TBase\<?,​?\>,​ThriftResponse extends org.apache.thrift.TBase\<?,​?\>\> {#class-hybridthriftoverhttpserviceimplthriftrequest-extends-org.apache.thrift.tbasethriftresponse-extends-org.apache.thrift.tbase .title title="Class HybridThriftOverHttpServiceImpl"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.slb.HybridThriftOverHttpServiceImpl\<ThriftRequest,​ThriftResponse\>

::: description
-   

    All Implemented Interfaces:
    :   `HybridThriftOverHttpService<ThriftRequest,​ThriftResponse>`,
        `ThriftOverHttpService<ThriftRequest,​ThriftResponse>`,
        `ThriftService<ThriftRequest,​ThriftResponse>`, `Closeable`,
        `AutoCloseable`

    ------------------------------------------------------------------------

        public class HybridThriftOverHttpServiceImpl<ThriftRequest extends org.apache.thrift.TBase<?,​?>,​ThriftResponse extends org.apache.thrift.TBase<?,​?>>
        extends Object
        implements HybridThriftOverHttpService<ThriftRequest,​ThriftResponse>

    ::: block
    The HTTP body contains: - 4 bytes big endian byte size of the thrift
    serialised message. - N bytes of the thrift serialised message. -
    Remaining bytes correspond to the out-of-band payload(s).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type            Field                                 Description
          ---------------------------- ------------------------------------- -------------
          `static okhttp3.MediaType`   `HYBRID_THRIFT_STREAM_CONTENT_TYPE`    
          `static String`              `PROTOCOL_HEADER`                      

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `HybridTh                         | ::: block                         |
        | riftOverHttpServiceImpl​(HybridThr | New instances.                    |
        | iftOverHttpServiceImplArgs args)` | :::                               |
        +-----------------------------------+-----------------------------------+

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
        | `com.                 | `makeReque            | ::: block             |
        | google.common.util.co | st​(HybridThriftReques | Asynchronously make a |
        | ncurrent.ListenableFu | tHandler<ThriftReques | request.              |
        | ture<ThriftResponse>` | t> request,           | :::                   |
        |                       |   HybridThriftRespons |                       |
        |                       | eHandler<ThriftRespon |                       |
        |                       | se> responseHandler)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `makeRequest​(ThriftRe |                       |
        |                       | quest thriftRequest,  |                       |
        |                       |            ThriftResp |                       |
        |                       | onse thriftResponse)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ThriftResponse`      | `makeRequestSync​(H    | ::: block             |
        |                       | ybridThriftRequestHan | Synchronously make a  |
        |                       | dler<ThriftRequest> r | request.              |
        |                       | equest,               | :::                   |
        |                       |   HybridThriftRespons |                       |
        |                       | eHandler<ThriftRespon |                       |
        |                       | se> responseHandler)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <Thri         | `readFromStrea        | ::: block             |
        | ftResponse extends or | m​(DataInputStream raw | Reads a HTTP body     |
        | g.apache.thrift.TBase | BodyStream,           | stream in Hybrid      |
        | <?,​?>>ThriftResponse` |      ThriftProtocol p | Thrift over HTTP      |
        |                       | rotocol,              | format.               |
        |                       |   HybridThriftRespons | :::                   |
        |                       | eHandler<ThriftRespon |                       |
        |                       | se> responseHandler)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `s                    | `writ                 | ::: block             |
        | tatic <ThriftRequest  | eToStream​(DataOutputS | Writes the HTTP body  |
        | extends org.apache.th | tream outputStream,   | into a stream in      |
        | rift.TBase<?,​?>>void` |             byte[] se | Hybrid Thrift over    |
        |                       | rializedThriftData,   | HTTP format.          |
        |                       |             HybridThr | :::                   |
        |                       | iftRequestHandler<Thr |                       |
        |                       | iftRequest> request)` |                       |
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

        []{#HYBRID_THRIFT_STREAM_CONTENT_TYPE}

        -   #### HYBRID_THRIFT_STREAM_CONTENT_TYPE

                public static final okhttp3.MediaType HYBRID_THRIFT_STREAM_CONTENT_TYPE

        []{#PROTOCOL_HEADER}

        -   #### PROTOCOL_HEADER

                public static final String PROTOCOL_HEADER

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.slb.HybridThriftOverHttpServiceImpl.PROTOCOL_HEADER)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.slb.HybridThriftOverHttpServiceImplArgs)}

        -   #### HybridThriftOverHttpServiceImpl

                public HybridThriftOverHttpServiceImpl​(HybridThriftOverHttpServiceImplArgs args)

            ::: block
            New instances.
            :::
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#makeRequest(com.facebook.buck.slb.HybridThriftRequestHandler,com.facebook.buck.slb.HybridThriftResponseHandler)}

        -   #### makeRequest

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<ThriftResponse> makeRequest​(HybridThriftRequestHandler<ThriftRequest> request,
                                                                                                  HybridThriftResponseHandler<ThriftResponse> responseHandler)
            ```

            ::: block
            [Description copied from
            interface: `HybridThriftOverHttpService`]{.descfrmTypeLabel}
            :::

            ::: block
            Asynchronously make a request.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `makeRequest` in
                interface `HybridThriftOverHttpService<ThriftRequest extends org.apache.thrift.TBase<?,​?>,​ThriftResponse extends org.apache.thrift.TBase<?,​?>>`

        []{#makeRequestSync(com.facebook.buck.slb.HybridThriftRequestHandler,com.facebook.buck.slb.HybridThriftResponseHandler)}

        -   #### makeRequestSync

            ``` methodSignature
            public ThriftResponse makeRequestSync​(HybridThriftRequestHandler<ThriftRequest> request,
                                                  HybridThriftResponseHandler<ThriftResponse> responseHandler)
                                           throws IOException
            ```

            ::: block
            [Description copied from
            interface: `HybridThriftOverHttpService`]{.descfrmTypeLabel}
            :::

            ::: block
            Synchronously make a request.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `makeRequestSync` in
                interface `HybridThriftOverHttpService<ThriftRequest extends org.apache.thrift.TBase<?,​?>,​ThriftResponse extends org.apache.thrift.TBase<?,​?>>`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#writeToStream(java.io.DataOutputStream,byte[],com.facebook.buck.slb.HybridThriftRequestHandler)}

        -   #### writeToStream

            ``` methodSignature
            public static <ThriftRequest extends org.apache.thrift.TBase<?,​?>> void writeToStream​(DataOutputStream outputStream,
                                                                                                        byte[] serializedThriftData,
                                                                                                        HybridThriftRequestHandler<ThriftRequest> request)
                                                                                                 throws IOException
            ```

            ::: block
            Writes the HTTP body into a stream in Hybrid Thrift over
            HTTP format.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#readFromStream(java.io.DataInputStream,com.facebook.buck.slb.ThriftProtocol,com.facebook.buck.slb.HybridThriftResponseHandler)}

        -   #### readFromStream

            ``` methodSignature
            public static <ThriftResponse extends org.apache.thrift.TBase<?,​?>> ThriftResponse readFromStream​(DataInputStream rawBodyStream,
                                                                                                                    ThriftProtocol protocol,
                                                                                                                    HybridThriftResponseHandler<ThriftResponse> responseHandler)
                                                                                                             throws IOException
            ```

            ::: block
            Reads a HTTP body stream in Hybrid Thrift over HTTP format.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#makeRequest(org.apache.thrift.TBase,org.apache.thrift.TBase)}
        []{#makeRequest(ThriftRequest,ThriftResponse)}

        -   #### makeRequest

            ``` methodSignature
            public void makeRequest​(ThriftRequest thriftRequest,
                                    ThriftResponse thriftResponse)
                             throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `makeRequest` in
                interface `ThriftService<ThriftRequest extends org.apache.thrift.TBase<?,​?>,​ThriftResponse extends org.apache.thrift.TBase<?,​?>>`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `Closeable`
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
