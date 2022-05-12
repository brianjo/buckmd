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

## Class ThriftOverHttpServiceImpl\<ThriftRequest extends org.apache.thrift.TBase\<?,​?\>,​ThriftResponse extends org.apache.thrift.TBase\<?,​?\>\> {#class-thriftoverhttpserviceimplthriftrequest-extends-org.apache.thrift.tbasethriftresponse-extends-org.apache.thrift.tbase .title title="Class ThriftOverHttpServiceImpl"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.slb.ThriftOverHttpServiceImpl\<ThriftRequest,​ThriftResponse\>

::: description
-   

    All Implemented Interfaces:
    :   `ThriftOverHttpService<ThriftRequest,​ThriftResponse>`,
        `ThriftService<ThriftRequest,​ThriftResponse>`, `Closeable`,
        `AutoCloseable`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `FrontendService`

    ------------------------------------------------------------------------

        public class ThriftOverHttpServiceImpl<ThriftRequest extends org.apache.thrift.TBase<?,​?>,​ThriftResponse extends org.apache.thrift.TBase<?,​?>>
        extends Object
        implements ThriftOverHttpService<ThriftRequest,​ThriftResponse>

    ::: block
    Implementation of the ThriftOverHttpService.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type            Field                      Description
          ---------------------------- -------------------------- -------------
          `static okhttp3.MediaType`   `THRIFT_CONTENT_TYPE`       
          `static String`              `THRIFT_PROTOCOL_HEADER`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                       Description
          ----------------------------------------------------------------- -------------
          `ThriftOverHttpServiceImpl​(ThriftOverHttpServiceConfig config)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                 Description
          ------------------- -------------------------------------------------------------------------------------- -------------
          `void`              `close()`                                                                               
          `void`              `makeRequest​(ThriftRequest thriftRequest,            ThriftResponse thriftResponse)`    

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
    -   []{#field.detail}

        ### Field Detail

        []{#THRIFT_CONTENT_TYPE}

        -   #### THRIFT_CONTENT_TYPE

                public static final okhttp3.MediaType THRIFT_CONTENT_TYPE

        []{#THRIFT_PROTOCOL_HEADER}

        -   #### THRIFT_PROTOCOL_HEADER

                public static final String THRIFT_PROTOCOL_HEADER

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.slb.ThriftOverHttpServiceImpl.THRIFT_PROTOCOL_HEADER)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.slb.ThriftOverHttpServiceConfig)}

        -   #### ThriftOverHttpServiceImpl

                public ThriftOverHttpServiceImpl​(ThriftOverHttpServiceConfig config)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

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
