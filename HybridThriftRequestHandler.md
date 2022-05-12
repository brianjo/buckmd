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

## Class HybridThriftRequestHandler\<ThriftRequest extends org.apache.thrift.TBase\<?,​?\>\> {#class-hybridthriftrequesthandlerthriftrequest-extends-org.apache.thrift.tbase .title title="Class HybridThriftRequestHandler"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.slb.HybridThriftRequestHandler\<ThriftRequest\>

::: description
-   

    ------------------------------------------------------------------------

        public abstract class HybridThriftRequestHandler<ThriftRequest extends org.apache.thrift.TBase<?,​?>>
        extends Object

    ::: block
    Handles the contents of a hybrid thrift request.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                           Description
          -------------- ----------------------------------------------------- -------------
          `protected `   `HybridThriftRequestHandler​(ThriftRequest request)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static <ThriftReq    | `cre                  | ::: block             |
        | uest extends org.apac | ateWithoutPayloads​(Th | Create request that   |
        | he.thrift.TBase<?,​?>> | riftRequest request)` | sends no out-of-band  |
        | HybridThriftRequestHa |                       | payloads.             |
        | ndler<ThriftRequest>` |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract int`        | `g                    | ::: block             |
        |                       | etNumberOfPayloads()` | Total number of       |
        |                       |                       | payloads.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getPayl              | ::: block             |
        | abstract InputStream` | oadStream​(int index)` | Fetches the data for  |
        |                       |                       | one specific payload. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ThriftRequest`       | `getRequest()`        | ::: block             |
        |                       |                       | Get thrift request.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract long`       | `getTota              | ::: block             |
        |                       | lPayloadsSizeBytes()` | The sum bytes of all  |
        |                       |                       | out-of-band payloads. |
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

        []{#<init>(org.apache.thrift.TBase)} []{#<init>(ThriftRequest)}

        -   #### HybridThriftRequestHandler

                protected HybridThriftRequestHandler​(ThriftRequest request)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createWithoutPayloads(org.apache.thrift.TBase)}
        []{#createWithoutPayloads(ThriftRequest)}

        -   #### createWithoutPayloads

            ``` methodSignature
            public static <ThriftRequest extends org.apache.thrift.TBase<?,​?>> HybridThriftRequestHandler<ThriftRequest> createWithoutPayloads​(ThriftRequest request)
            ```

            ::: block
            Create request that sends no out-of-band payloads.
            :::

        []{#getRequest()}

        -   #### getRequest

            ``` methodSignature
            public ThriftRequest getRequest()
            ```

            ::: block
            Get thrift request.
            :::

        []{#getTotalPayloadsSizeBytes()}

        -   #### getTotalPayloadsSizeBytes

            ``` methodSignature
            public abstract long getTotalPayloadsSizeBytes()
            ```

            ::: block
            The sum bytes of all out-of-band payloads.
            :::

        []{#getNumberOfPayloads()}

        -   #### getNumberOfPayloads

            ``` methodSignature
            public abstract int getNumberOfPayloads()
            ```

            ::: block
            Total number of payloads.
            :::

        []{#getPayloadStream(int)}

        -   #### getPayloadStream

            ``` methodSignature
            public abstract InputStream getPayloadStream​(int index)
                                                  throws IOException
            ```

            ::: block
            Fetches the data for one specific payload.
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
