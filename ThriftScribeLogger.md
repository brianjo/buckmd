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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.util.network](package-summary.html)
:::

## Class ThriftScribeLogger {#class-thriftscribelogger .title title="Class ThriftScribeLogger"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.util.network.ScribeLogger](ScribeLogger.html "class in com.facebook.buck.util.network")

    -   -   com.facebook.buck.util.network.ThriftScribeLogger

::: description
-   

    All Implemented Interfaces:
    :   `Closeable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class ThriftScribeLogger
        extends ScribeLogger
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                             Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `ThriftScribeLogger​(ThriftService<com.facebook.buck.frontend.thrift.FrontendRequest,​com.facebook.buck.frontend.thrift.FrontendResponse> thriftService,                   com.google.common.util.concurrent.ListeningExecutorService executorService)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                            Method                                                                           Description
          ------------------------------------------------------------ -------------------------------------------------------------------------------- -------------
          `void`                                                       `close()`                                                                         
          `com.google.common.util.concurrent.ListenableFuture<Unit>`   `log​(String category,    Iterable<String> lines,    Optional<Integer> bucket)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.util.network.ScribeLogger}

            ### Methods inherited from class com.facebook.buck.util.network.[ScribeLogger](ScribeLogger.html "class in com.facebook.buck.util.network")

            `log`

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

        []{#<init>(com.facebook.buck.slb.ThriftService,com.google.common.util.concurrent.ListeningExecutorService)}

        -   #### ThriftScribeLogger

                public ThriftScribeLogger​(ThriftService<com.facebook.buck.frontend.thrift.FrontendRequest,​com.facebook.buck.frontend.thrift.FrontendResponse> thriftService,
                                          com.google.common.util.concurrent.ListeningExecutorService executorService)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#log(java.lang.String,java.lang.Iterable,java.util.Optional)}

        -   #### log

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<Unit> log​(String category,
                                                                                Iterable<String> lines,
                                                                                Optional<Integer> bucket)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `log` in class `ScribeLogger`

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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
