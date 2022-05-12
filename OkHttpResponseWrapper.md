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

## Class OkHttpResponseWrapper {#class-okhttpresponsewrapper .title title="Class OkHttpResponseWrapper"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.slb.OkHttpResponseWrapper

::: description
-   

    All Implemented Interfaces:
    :   `HttpResponse`, `Closeable`, `AutoCloseable`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `LoadBalancedHttpResponse`

    ------------------------------------------------------------------------

        public class OkHttpResponseWrapper
        extends Object
        implements HttpResponse
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                          Description
          ---------------------------------------------------- -------------
          `OkHttpResponseWrapper​(okhttp3.Response response)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type              Method              Description
          ------------------------------ ------------------- -------------
          `void`                         `close()`            
          `long`                         `contentLength()`    
          `InputStream`                  `getBody()`          
          `protected okhttp3.Response`   `getResponse()`      
          `String`                       `requestUrl()`       
          `int`                          `statusCode()`       
          `String`                       `statusMessage()`    

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

        []{#<init>(okhttp3.Response)}

        -   #### OkHttpResponseWrapper

                public OkHttpResponseWrapper​(okhttp3.Response response)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#statusCode()}

        -   #### statusCode

            ``` methodSignature
            public int statusCode()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `statusCode` in interface `HttpResponse`

            [Returns:]{.returnLabel}
            :   HTTP Response code.

        []{#statusMessage()}

        -   #### statusMessage

            ``` methodSignature
            public String statusMessage()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `statusMessage` in interface `HttpResponse`

            [Returns:]{.returnLabel}
            :   HTTP Response code message.

        []{#contentLength()}

        -   #### contentLength

            ``` methodSignature
            public long contentLength()
                               throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `contentLength` in interface `HttpResponse`

            [Returns:]{.returnLabel}
            :   Number of bytes in the body of this response.

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getBody()}

        -   #### getBody

            ``` methodSignature
            public InputStream getBody()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBody` in interface `HttpResponse`

            [Returns:]{.returnLabel}
            :   Stream with the response body.

        []{#requestUrl()}

        -   #### requestUrl

            ``` methodSignature
            public String requestUrl()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `requestUrl` in interface `HttpResponse`

            [Returns:]{.returnLabel}
            :   The full URL of the request that generated this
                response.

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
                       throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `Closeable`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getResponse()}

        -   #### getResponse

            ``` methodSignature
            protected okhttp3.Response getResponse()
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
