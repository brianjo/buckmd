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

## Class HybridThriftOverHttpServiceImplArgs {#class-hybridthriftoverhttpserviceimplargs .title title="Class HybridThriftOverHttpServiceImplArgs"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.slb.HybridThriftOverHttpServiceImplArgs

::: description
-   

    ------------------------------------------------------------------------

        public abstract class HybridThriftOverHttpServiceImplArgs
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                          Description
          ------------------- ------------------------------ -------------
          `static String`     `DEFAULT_HYBRID_THRIFT_PATH`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                               Description
          ----------------------------------------- -------------
          `HybridThriftOverHttpServiceImplArgs()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                       Method                                                                                                                                                         Description
          ----------------------------------------------------------------------- -------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `abstract com.google.common.util.concurrent.ListeningExecutorService`   `getExecutor()`                                                                                                                                                 
          `abstract String`                                                       `getHybridThriftPath()`                                                                                                                                         
          `abstract HttpService`                                                  `getService()`                                                                                                                                                  
          `abstract ThriftProtocol`                                               `getThriftProtocol()`                                                                                                                                           
          `static HybridThriftOverHttpServiceImplArgs`                            `of​(HttpService service,   com.google.common.util.concurrent.ListeningExecutorService executor)`                                                                
          `static HybridThriftOverHttpServiceImplArgs`                            `of​(HttpService service,   com.google.common.util.concurrent.ListeningExecutorService executor,   ThriftProtocol thriftProtocol,   String hybridThriftPath)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

        []{#DEFAULT_HYBRID_THRIFT_PATH}

        -   #### DEFAULT_HYBRID_THRIFT_PATH

                public static final String DEFAULT_HYBRID_THRIFT_PATH

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.slb.HybridThriftOverHttpServiceImplArgs.DEFAULT_HYBRID_THRIFT_PATH)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### HybridThriftOverHttpServiceImplArgs

                public HybridThriftOverHttpServiceImplArgs()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getService()}

        -   #### getService

            ``` methodSignature
            public abstract HttpService getService()
            ```

        []{#getExecutor()}

        -   #### getExecutor

            ``` methodSignature
            public abstract com.google.common.util.concurrent.ListeningExecutorService getExecutor()
            ```

        []{#getThriftProtocol()}

        -   #### getThriftProtocol

            ``` methodSignature
            public abstract ThriftProtocol getThriftProtocol()
            ```

        []{#getHybridThriftPath()}

        -   #### getHybridThriftPath

            ``` methodSignature
            public abstract String getHybridThriftPath()
            ```

        []{#of(com.facebook.buck.slb.HttpService,com.google.common.util.concurrent.ListeningExecutorService)}

        -   #### of

            ``` methodSignature
            public static HybridThriftOverHttpServiceImplArgs of​(HttpService service,
                                                                 com.google.common.util.concurrent.ListeningExecutorService executor)
            ```

        []{#of(com.facebook.buck.slb.HttpService,com.google.common.util.concurrent.ListeningExecutorService,com.facebook.buck.slb.ThriftProtocol,java.lang.String)}

        -   #### of

            ``` methodSignature
            public static HybridThriftOverHttpServiceImplArgs of​(HttpService service,
                                                                 com.google.common.util.concurrent.ListeningExecutorService executor,
                                                                 ThriftProtocol thriftProtocol,
                                                                 String hybridThriftPath)
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
