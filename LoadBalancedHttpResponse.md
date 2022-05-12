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

## Class LoadBalancedHttpResponse {#class-loadbalancedhttpresponse .title title="Class LoadBalancedHttpResponse"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.slb.OkHttpResponseWrapper](OkHttpResponseWrapper.html "class in com.facebook.buck.slb")

    -   -   com.facebook.buck.slb.LoadBalancedHttpResponse

::: description
-   

    All Implemented Interfaces:
    :   `HttpResponse`, `Closeable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class LoadBalancedHttpResponse
        extends OkHttpResponseWrapper
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                   Method                                                                                                                                           Description
          ----------------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `void`                              `close()`                                                                                                                                         
          `long`                              `contentLength()`                                                                                                                                 
          `static LoadBalancedHttpResponse`   `createLoadBalancedResponse​(URI server,                           HttpLoadBalancer loadBalancer,                           okhttp3.Call call)`    
          `InputStream`                       `getBody()`                                                                                                                                       

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.slb.OkHttpResponseWrapper}

            ### Methods inherited from class com.facebook.buck.slb.[OkHttpResponseWrapper](OkHttpResponseWrapper.html "class in com.facebook.buck.slb")

            `getResponse, requestUrl, statusCode, statusMessage`

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
    -   []{#method.detail}

        ### Method Detail

        []{#createLoadBalancedResponse(java.net.URI,com.facebook.buck.slb.HttpLoadBalancer,okhttp3.Call)}

        -   #### createLoadBalancedResponse

            ``` methodSignature
            public static LoadBalancedHttpResponse createLoadBalancedResponse​(URI server,
                                                                              HttpLoadBalancer loadBalancer,
                                                                              okhttp3.Call call)
                                                                       throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#contentLength()}

        -   #### contentLength

            ``` methodSignature
            public long contentLength()
                               throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `contentLength` in interface `HttpResponse`

            [Overrides:]{.overrideSpecifyLabel}
            :   `contentLength` in class `OkHttpResponseWrapper`

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

            [Overrides:]{.overrideSpecifyLabel}
            :   `getBody` in class `OkHttpResponseWrapper`

            [Returns:]{.returnLabel}
            :   Stream with the response body.

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

            [Overrides:]{.overrideSpecifyLabel}
            :   `close` in class `OkHttpResponseWrapper`

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
