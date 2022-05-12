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
[Package]{.packageLabelInType} [com.facebook.buck.slb](package-summary.html)
:::

## Class HybridThriftResponseHandler\<ThriftResponse extends org.apache.thrift.TBase\<?,​?\>\> {#class-hybridthriftresponsehandlerthriftresponse-extends-org.apache.thrift.tbase .title title="Class HybridThriftResponseHandler"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.slb.HybridThriftResponseHandler\<ThriftResponse\>

::: description
-   

    ------------------------------------------------------------------------

        public abstract class HybridThriftResponseHandler<ThriftResponse extends org.apache.thrift.TBase<?,​?>>
        extends Object

    ::: block
    Control struct to receive a hybrid thrift response.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                   Description
          -------------- ------------------------------------------------------------- -------------
          `protected `   `HybridThriftResponseHandler​(ThriftResponse emptyResponse)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static <ThriftRespon | `create               | ::: block             |
        | se extends org.apache | NoPayloadHandler​(Thri | Encodes a response    |
        | .thrift.TBase<?,​?>>Hy | ftResponse response)` | without out-of-band   |
        | bridThriftResponseHan |                       | payloads.             |
        | dler<ThriftResponse>` |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static <ThriftRespon | `                     | ::: block             |
        | se extends org.apache | createNoPayloadHandle | Encodes a response    |
        | .thrift.TBase<?,​?>>Hy | r​(ThriftResponse resp | without out-of-band   |
        | bridThriftResponseHan | onse,                 | payloads.             |
        | dler<ThriftResponse>` |        ThrowingConsum | :::                   |
        |                       | er<ThriftResponse,​IOE |                       |
        |                       | xception> validator)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract long`       | `getPayload           | ::: block             |
        |                       | SizeBytes​(int index)` | Size bytes of the nth |
        |                       |                       | payload.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ThriftResponse`      | `getResponse()`       | ::: block             |
        |                       |                       | The thrift response.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `a                    | `getStreamF           | ::: block             |
        | bstract OutputStream` | orPayload​(int index)` | Where to write the    |
        |                       |                       | nth payload bytes to. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract int`        | `getTotalPayloads()`  | ::: block             |
        |                       |                       | Total number of       |
        |                       |                       | payloads expected for |
        |                       |                       | the current thrift    |
        |                       |                       | response.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `onResponseParsed()`  | ::: block             |
        |                       |                       | Called as soon as the |
        |                       |                       | thrift metadata       |
        |                       |                       | section of the        |
        |                       |                       | response is parsed.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

        []{#<init>(org.apache.thrift.TBase)} []{#<init>(ThriftResponse)}

        -   #### HybridThriftResponseHandler

                protected HybridThriftResponseHandler​(ThriftResponse emptyResponse)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createNoPayloadHandler(org.apache.thrift.TBase)}
        []{#createNoPayloadHandler(ThriftResponse)}

        -   #### createNoPayloadHandler

            ``` methodSignature
            public static <ThriftResponse extends org.apache.thrift.TBase<?,​?>> HybridThriftResponseHandler<ThriftResponse> createNoPayloadHandler​(ThriftResponse response)
            ```

            ::: block
            Encodes a response without out-of-band payloads.
            :::

        []{#createNoPayloadHandler(org.apache.thrift.TBase,com.facebook.buck.util.function.ThrowingConsumer)}
        []{#createNoPayloadHandler(ThriftResponse,com.facebook.buck.util.function.ThrowingConsumer)}

        -   #### createNoPayloadHandler

            ``` methodSignature
            public static <ThriftResponse extends org.apache.thrift.TBase<?,​?>> HybridThriftResponseHandler<ThriftResponse> createNoPayloadHandler​(ThriftResponse response,
                                                                                                                                                         ThrowingConsumer<ThriftResponse,​IOException> validator)
            ```

            ::: block
            Encodes a response without out-of-band payloads.
            :::

        []{#getResponse()}

        -   #### getResponse

            ``` methodSignature
            public ThriftResponse getResponse()
            ```

            ::: block
            The thrift response.
            :::

        []{#onResponseParsed()}

        -   #### onResponseParsed

            ``` methodSignature
            public void onResponseParsed()
                                  throws IOException
            ```

            ::: block
            Called as soon as the thrift metadata section of the
            response is parsed.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getTotalPayloads()}

        -   #### getTotalPayloads

            ``` methodSignature
            public abstract int getTotalPayloads()
            ```

            ::: block
            Total number of payloads expected for the current thrift
            response.
            :::

        []{#getPayloadSizeBytes(int)}

        -   #### getPayloadSizeBytes

            ``` methodSignature
            public abstract long getPayloadSizeBytes​(int index)
            ```

            ::: block
            Size bytes of the nth payload. Must be positive.
            :::

        []{#getStreamForPayload(int)}

        -   #### getStreamForPayload

            ``` methodSignature
            public abstract OutputStream getStreamForPayload​(int index)
            ```

            ::: block
            Where to write the nth payload bytes to.
            :::
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
