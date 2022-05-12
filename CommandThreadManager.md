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
[Package]{.packageLabelInType} [com.facebook.buck.cli](package-summary.html)
:::

## Class CommandThreadManager {#class-commandthreadmanager .title title="Class CommandThreadManager"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cli.CommandThreadManager

::: description
-   

    All Implemented Interfaces:
    :   `AutoCloseable`

    ------------------------------------------------------------------------

        public class CommandThreadManager
        extends Object
        implements AutoCloseable

    ::: block
    Encapsulates a group of threads which operate a
    `ListeningExecutorService`, providing an
    [`AutoCloseable`](http://docs.oracle.com/javase/7/docs/api/java/lang/AutoCloseable.html?is-external=true "class or interface in java.lang"){.externalLink}
    interface which waits for and kills the threads on close.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                              Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `CommandThreadManager​(String name,                     ConcurrencyLimit concurrencyLimit)`                                                                                                                                                                                                
          `CommandThreadManager​(String name,                     ConcurrencyLimit concurrencyLimit,                     long shutdownTimeout,                     TimeUnit shutdownTimeoutUnit)`                                                                                                    
          `CommandThreadManager​(String name,                     ListeningMultiSemaphore semaphore,                     ResourceAmounts defaultAmounts,                     int managedThreadCount)`                                                                                                
          `CommandThreadManager​(String name,                     ListeningMultiSemaphore semaphore,                     ResourceAmounts defaultAmounts,                     int managedThreadCount,                     long shutdownTimeout,                     TimeUnit shutdownTimeoutUnit)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                              Method                                    Description
          -------------------------------------------------------------- ----------------------------------------- -------------
          `void`                                                         `close()`                                  
          `ExecutorService`                                              `getExecutorService()`                     
          `com.google.common.util.concurrent.ListeningExecutorService`   `getListeningExecutorService()`            
          `WeightedListeningExecutorService`                             `getWeightedListeningExecutorService()`    

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

        []{#<init>(java.lang.String,com.facebook.buck.util.concurrent.ListeningMultiSemaphore,com.facebook.buck.util.concurrent.ResourceAmounts,int,long,java.util.concurrent.TimeUnit)}

        -   #### CommandThreadManager

                public CommandThreadManager​(String name,
                                            ListeningMultiSemaphore semaphore,
                                            ResourceAmounts defaultAmounts,
                                            int managedThreadCount,
                                            long shutdownTimeout,
                                            TimeUnit shutdownTimeoutUnit)

        []{#<init>(java.lang.String,com.facebook.buck.util.concurrent.ListeningMultiSemaphore,com.facebook.buck.util.concurrent.ResourceAmounts,int)}

        -   #### CommandThreadManager

                public CommandThreadManager​(String name,
                                            ListeningMultiSemaphore semaphore,
                                            ResourceAmounts defaultAmounts,
                                            int managedThreadCount)

        []{#<init>(java.lang.String,com.facebook.buck.util.concurrent.ConcurrencyLimit,long,java.util.concurrent.TimeUnit)}

        -   #### CommandThreadManager

                public CommandThreadManager​(String name,
                                            ConcurrencyLimit concurrencyLimit,
                                            long shutdownTimeout,
                                            TimeUnit shutdownTimeoutUnit)

        []{#<init>(java.lang.String,com.facebook.buck.util.concurrent.ConcurrencyLimit)}

        -   #### CommandThreadManager

                public CommandThreadManager​(String name,
                                            ConcurrencyLimit concurrencyLimit)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getExecutorService()}

        -   #### getExecutorService

            ``` methodSignature
            public ExecutorService getExecutorService()
            ```

        []{#getListeningExecutorService()}

        -   #### getListeningExecutorService

            ``` methodSignature
            public com.google.common.util.concurrent.ListeningExecutorService getListeningExecutorService()
            ```

        []{#getWeightedListeningExecutorService()}

        -   #### getWeightedListeningExecutorService

            ``` methodSignature
            public WeightedListeningExecutorService getWeightedListeningExecutorService()
            ```

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
                       throws InterruptedException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

            [Throws:]{.throwsLabel}
            :   `InterruptedException`
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
