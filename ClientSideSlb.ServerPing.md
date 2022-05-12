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

## Class ClientSideSlb.ServerPing {#class-clientsideslb.serverping .title title="Class ClientSideSlb.ServerPing"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.slb.ClientSideSlb.ServerPing

::: description
-   

    All Implemented Interfaces:
    :   `okhttp3.Callback`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [ClientSideSlb](ClientSideSlb.html "class in com.facebook.buck.slb")

    ------------------------------------------------------------------------

        public class ClientSideSlb.ServerPing
        extends Object
        implements okhttp3.Callback
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                               Method                                                                 Description
          ----------------------------------------------------------------------------------------------- ---------------------------------------------------------------------- -------------
          `com.google.common.util.concurrent.ListenableFuture<LoadBalancerPingEvent.PerServerPingData>`   `getFuture()`                                                           
          `void`                                                                                          `onFailure​(okhttp3.Call call,          IOException e)`                  
          `void`                                                                                          `onResponse​(okhttp3.Call call,           okhttp3.Response response)`    

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
    -   []{#method.detail}

        ### Method Detail

        []{#getFuture()}

        -   #### getFuture

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<LoadBalancerPingEvent.PerServerPingData> getFuture()
            ```

        []{#onResponse(okhttp3.Call,okhttp3.Response)}

        -   #### onResponse

            ``` methodSignature
            public void onResponse​(okhttp3.Call call,
                                   okhttp3.Response response)
                            throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `onResponse` in interface `okhttp3.Callback`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#onFailure(okhttp3.Call,java.io.IOException)}

        -   #### onFailure

            ``` methodSignature
            public void onFailure​(okhttp3.Call call,
                                  IOException e)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `onFailure` in interface `okhttp3.Callback`
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
