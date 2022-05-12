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
-   [Nested](#nested.class.summary) \| 
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

## Class RetryingHttpService {#class-retryinghttpservice .title title="Class RetryingHttpService"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.slb.RetryingHttpService

::: description
-   

    All Implemented Interfaces:
    :   `HttpService`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class RetryingHttpService
        extends Object
        implements HttpService
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                                                Description
          ------------------- ---------------------------------------------------- -------------
          `static class `     `RetryingHttpService.RetryingHttpServiceException`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                               Description
          ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `RetryingHttpService​(BuckEventBus eventBus,                    HttpService decoratedService,                    String counterCategory,                    int maxNumberOfRetries)`                                                        
          `RetryingHttpService​(BuckEventBus eventBus,                    HttpService decoratedService,                    String counterCategory,                    int maxNumberOfRetries,                    long retryRequestIntervalMillis)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                   Description
          ------------------- ------------------------------------------------------------------------ -------------
          `void`              `close()`                                                                 
          `HttpResponse`      `makeRequest​(String path,            okhttp3.Request.Builder request)`    

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

        []{#<init>(com.facebook.buck.event.BuckEventBus,com.facebook.buck.slb.HttpService,java.lang.String,int)}

        -   #### RetryingHttpService

                public RetryingHttpService​(BuckEventBus eventBus,
                                           HttpService decoratedService,
                                           String counterCategory,
                                           int maxNumberOfRetries)

        []{#<init>(com.facebook.buck.event.BuckEventBus,com.facebook.buck.slb.HttpService,java.lang.String,int,long)}

        -   #### RetryingHttpService

                public RetryingHttpService​(BuckEventBus eventBus,
                                           HttpService decoratedService,
                                           String counterCategory,
                                           int maxNumberOfRetries,
                                           long retryRequestIntervalMillis)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#makeRequest(java.lang.String,okhttp3.Request.Builder)}

        -   #### makeRequest

            ``` methodSignature
            public HttpResponse makeRequest​(String path,
                                            okhttp3.Request.Builder request)
                                     throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `makeRequest` in interface `HttpService`

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
            :   `close` in interface `HttpService`
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
-   [Nested](#nested.class.summary) \| 
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