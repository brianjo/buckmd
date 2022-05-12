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

## Interface HttpResponse {#interface-httpresponse .title title="Interface HttpResponse"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AutoCloseable`, `Closeable`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `LoadBalancedHttpResponse`, `OkHttpResponseWrapper`

    ------------------------------------------------------------------------

        public interface HttpResponse
        extends Closeable
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method              Description
          ------------------- ------------------- -------------
          `long`              `contentLength()`    
          `InputStream`       `getBody()`          
          `String`            `requestUrl()`       
          `int`               `statusCode()`       
          `String`            `statusMessage()`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.java.io.Closeable}

            ### Methods inherited from interface java.io.[Closeable](http://docs.oracle.com/javase/7/docs/api/java/io/Closeable.html?is-external=true "class or interface in java.io"){.externalLink}

            `close`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#statusCode()}

        -   #### statusCode

            ``` methodSignature
            int statusCode()
            ```

            [Returns:]{.returnLabel}
            :   HTTP Response code.

        []{#statusMessage()}

        -   #### statusMessage

            ``` methodSignature
            String statusMessage()
            ```

            [Returns:]{.returnLabel}
            :   HTTP Response code message.

        []{#contentLength()}

        -   #### contentLength

            ``` methodSignature
            long contentLength()
                        throws IOException
            ```

            [Returns:]{.returnLabel}
            :   Number of bytes in the body of this response.

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getBody()}

        -   #### getBody

            ``` methodSignature
            InputStream getBody()
            ```

            [Returns:]{.returnLabel}
            :   Stream with the response body.

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#requestUrl()}

        -   #### requestUrl

            ``` methodSignature
            String requestUrl()
            ```

            [Returns:]{.returnLabel}
            :   The full URL of the request that generated this
                response.
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
