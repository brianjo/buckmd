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
[Package]{.packageLabelInType} [com.facebook.buck.frontend](package-summary.html)
:::

## Class FrontendService {#class-frontendservice .title title="Class FrontendService"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.slb.ThriftOverHttpServiceImpl](../slb/ThriftOverHttpServiceImpl.html "class in com.facebook.buck.slb")\<com.facebook.buck.frontend.thrift.FrontendRequest,​com.facebook.buck.frontend.thrift.FrontendResponse\>

    -   -   com.facebook.buck.frontend.FrontendService

::: description
-   

    All Implemented Interfaces:
    :   `ThriftOverHttpService<com.facebook.buck.frontend.thrift.FrontendRequest,​com.facebook.buck.frontend.thrift.FrontendResponse>`,
        `ThriftService<com.facebook.buck.frontend.thrift.FrontendRequest,​com.facebook.buck.frontend.thrift.FrontendResponse>`,
        `Closeable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class FrontendService
        extends ThriftOverHttpServiceImpl<com.facebook.buck.frontend.thrift.FrontendRequest,​com.facebook.buck.frontend.thrift.FrontendResponse>

    ::: block
    Extension of ThriftOverHttpServiceImpl to get rid of the template
    arguments and make it easymock-able
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.slb.ThriftOverHttpServiceImpl}

            ### Fields inherited from class com.facebook.buck.slb.[ThriftOverHttpServiceImpl](../slb/ThriftOverHttpServiceImpl.html "class in com.facebook.buck.slb")

            `THRIFT_CONTENT_TYPE, THRIFT_PROTOCOL_HEADER`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                             Description
          ------------------------------------------------------- -------------
          `FrontendService​(ThriftOverHttpServiceConfig config)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                      Method                                                                     Description
          ------------------------------------------------------ -------------------------------------------------------------------------- -------------
          `com.facebook.buck.frontend.thrift.FrontendResponse`   `makeRequest​(com.facebook.buck.frontend.thrift.FrontendRequest request)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.slb.ThriftOverHttpServiceImpl}

            ### Methods inherited from class com.facebook.buck.slb.[ThriftOverHttpServiceImpl](../slb/ThriftOverHttpServiceImpl.html "class in com.facebook.buck.slb")

            `close, makeRequest`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.slb.ThriftOverHttpServiceConfig)}

        -   #### FrontendService

                public FrontendService​(ThriftOverHttpServiceConfig config)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#makeRequest(com.facebook.buck.frontend.thrift.FrontendRequest)}

        -   #### makeRequest

            ``` methodSignature
            public com.facebook.buck.frontend.thrift.FrontendResponse makeRequest​(com.facebook.buck.frontend.thrift.FrontendRequest request)
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
-   [Field](#field.summary) \| 
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
