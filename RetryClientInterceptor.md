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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.remoteexecution.grpc.retry](package-summary.html)
:::

## Class RetryClientInterceptor {#class-retryclientinterceptor .title title="Class RetryClientInterceptor"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.remoteexecution.grpc.retry.RetryClientInterceptor

::: description
-   

    All Implemented Interfaces:
    :   `io.grpc.ClientInterceptor`

    ------------------------------------------------------------------------

        public class RetryClientInterceptor
        extends Object
        implements io.grpc.ClientInterceptor

    ::: block
    Interceptor for retrying client calls. Only retries in the following
    circumstances:
    -   An UNAVAILABLE error is returned
    -   The client only has a single request (there can be multiple
        responses from the server)
    -   No responses in a stream have been received from the server.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                         Description
          --------------------------------------------------- -------------
          `RetryClientInterceptor​(RetryPolicy retryPolicy)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                              Method                                                                                                                                          Description
          ---------------------------------------------- ----------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `<ReqT,​RespT>io.grpc.ClientCall<ReqT,​RespT>`   `interceptCall​(io.grpc.MethodDescriptor<ReqT,​RespT> method,              io.grpc.CallOptions callOptions,              io.grpc.Channel next)`    

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

        []{#<init>(com.facebook.buck.remoteexecution.grpc.retry.RetryPolicy)}

        -   #### RetryClientInterceptor

                public RetryClientInterceptor​(RetryPolicy retryPolicy)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#interceptCall(io.grpc.MethodDescriptor,io.grpc.CallOptions,io.grpc.Channel)}

        -   #### interceptCall

            ``` methodSignature
            public <ReqT,​RespT> io.grpc.ClientCall<ReqT,​RespT> interceptCall​(io.grpc.MethodDescriptor<ReqT,​RespT> method,
                                                                                         io.grpc.CallOptions callOptions,
                                                                                         io.grpc.Channel next)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `interceptCall` in interface `io.grpc.ClientInterceptor`
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
