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

## Class ClientSideSlb {#class-clientsideslb .title title="Class ClientSideSlb"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.slb.ClientSideSlb

::: description
-   

    All Implemented Interfaces:
    :   `HttpLoadBalancer`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class ClientSideSlb
        extends Object
        implements HttpLoadBalancer
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                        Description
          ------------------- ---------------------------- -------------
          `class `            `ClientSideSlb.ServerPing`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                  Description
          ---------------------------------------------------------------------------------------------------------------------------- -------------
          `ClientSideSlb​(com.facebook.buck.slb.ClientSideSlbConfig config,              okhttp3.OkHttpClient.Builder clientBuilder)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                               Description
          ------------------- -------------------------------------------------------------------- -------------
          `void`              `close()`                                                             
          `URI`               `getBestServer()`                                                     
          `static boolean`    `isSafeToCreate​(com.facebook.buck.slb.ClientSideSlbConfig config)`    
          `void`              `reportRequestException​(URI server)`                                  
          `void`              `reportRequestSuccess​(URI server)`                                    

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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.slb.ClientSideSlbConfig,okhttp3.OkHttpClient.Builder)}

        -   #### ClientSideSlb

                public ClientSideSlb​(com.facebook.buck.slb.ClientSideSlbConfig config,
                                     okhttp3.OkHttpClient.Builder clientBuilder)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#isSafeToCreate(com.facebook.buck.slb.ClientSideSlbConfig)}

        -   #### isSafeToCreate

            ``` methodSignature
            public static boolean isSafeToCreate​(com.facebook.buck.slb.ClientSideSlbConfig config)
            ```

        []{#getBestServer()}

        -   #### getBestServer

            ``` methodSignature
            public URI getBestServer()
                              throws NoHealthyServersException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBestServer` in interface `HttpLoadBalancer`

            [Throws:]{.throwsLabel}
            :   `NoHealthyServersException`

        []{#reportRequestSuccess(java.net.URI)}

        -   #### reportRequestSuccess

            ``` methodSignature
            public void reportRequestSuccess​(URI server)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `reportRequestSuccess` in interface `HttpLoadBalancer`

        []{#reportRequestException(java.net.URI)}

        -   #### reportRequestException

            ``` methodSignature
            public void reportRequestException​(URI server)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `reportRequestException` in interface `HttpLoadBalancer`

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `HttpLoadBalancer`
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
