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
[Package]{.packageLabelInType} [com.facebook.buck.util.concurrent](package-summary.html)
:::

## Class WeightedListeningExecutorService {#class-weightedlisteningexecutorservice .title title="Class WeightedListeningExecutorService"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.util.concurrent.AbstractExecutorService](http://docs.oracle.com/javase/7/docs/api/java/util/concurrent/AbstractExecutorService.html?is-external=true "class or interface in java.util.concurrent"){.externalLink}

    -   -   com.google.common.util.concurrent.AbstractListeningExecutorService

        -   -   com.facebook.buck.util.concurrent.WeightedListeningExecutorService

::: description
-   

    All Implemented Interfaces:
    :   `com.google.common.util.concurrent.ListeningExecutorService`,
        `Executor`, `ExecutorService`

    ------------------------------------------------------------------------

        public class WeightedListeningExecutorService
        extends com.google.common.util.concurrent.AbstractListeningExecutorService

    ::: block
    A `ListeningExecutorService` which gates execution using a
    [`ListeningMultiSemaphore`](ListeningMultiSemaphore.html "class in com.facebook.buck.util.concurrent")
    and allows resources to be assigned to submitted tasks.
    NOTE: If futures for submitted jobs are cancelled while they are
    running, it\'s possible that the semaphore will be released for that
    cancelled job before it is finished, meaning more jobs may be
    scheduled than expected.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                 Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `WeightedListeningExecutorService​(ListeningMultiSemaphore semaphore,                                 ResourceAmounts defaultValues,                                 com.google.common.util.concurrent.ListeningExecutorService delegate)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `awaitTermination​(lon |                       |
        |                       | g timeout,            |                       |
        |                       |       TimeUnit unit)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `execu                |                       |
        |                       | te​(Runnable command)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isShutdown()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isTerminated()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `shutdown()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `List<Runnable>`      | `shutdownNow()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `s                    |                       |
        | ommon.util.concurrent | ubmit​(Runnable task)` |                       |
        | .ListenableFuture<?>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `submit​(Runn          |                       |
        | ommon.util.concurrent | able task,       Reso |                       |
        | .ListenableFuture<?>` | urceAmounts amounts)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `<T> com.google.c     | `submit​(Runnable t    |                       |
        | ommon.util.concurrent | ask,       T result)` |                       |
        | .ListenableFuture<T>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `<T> com.google.c     | `submit               |                       |
        | ommon.util.concurrent | ​(Runnable task,       |                       |
        | .ListenableFuture<T>` |  T result,       Reso |                       |
        |                       | urceAmounts amounts)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `<T> com.google.c     | `subm                 |                       |
        | ommon.util.concurrent | it​(Callable<T> task)` |                       |
        | .ListenableFuture<T>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `<T> com.google.c     | `submit​(Callabl       |                       |
        | ommon.util.concurrent | e<T> task,       Reso |                       |
        | .ListenableFuture<T>` | urceAmounts amounts)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `WeightedList         | `withDefaultA         | ::: block             |
        | eningExecutorService` | mounts​(ResourceAmount | Creates a new service |
        |                       | s newDefaultAmounts)` | that has different    |
        |                       |                       | default resource      |
        |                       |                       | amounts.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.google.common.util.concurrent.AbstractListeningExecutorService}

            ### Methods inherited from class com.google.common.util.concurrent.AbstractListeningExecutorService

            `newTaskFor, newTaskFor`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.util.concurrent.AbstractExecutorService}

            ### Methods inherited from class java.util.concurrent.[AbstractExecutorService](http://docs.oracle.com/javase/7/docs/api/java/util/concurrent/AbstractExecutorService.html?is-external=true "class or interface in java.util.concurrent"){.externalLink}

            `invokeAll, invokeAll, invokeAny, invokeAny`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.util.concurrent.ExecutorService}

            ### Methods inherited from interface java.util.concurrent.[ExecutorService](http://docs.oracle.com/javase/7/docs/api/java/util/concurrent/ExecutorService.html?is-external=true "class or interface in java.util.concurrent"){.externalLink}

            `invokeAny, invokeAny`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.google.common.util.concurrent.ListeningExecutorService}

            ### Methods inherited from interface com.google.common.util.concurrent.ListeningExecutorService

            `invokeAll, invokeAll`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.util.concurrent.ListeningMultiSemaphore,com.facebook.buck.util.concurrent.ResourceAmounts,com.google.common.util.concurrent.ListeningExecutorService)}

        -   #### WeightedListeningExecutorService

                public WeightedListeningExecutorService​(ListeningMultiSemaphore semaphore,
                                                        ResourceAmounts defaultValues,
                                                        com.google.common.util.concurrent.ListeningExecutorService delegate)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#withDefaultAmounts(com.facebook.buck.util.concurrent.ResourceAmounts)}

        -   #### withDefaultAmounts

            ``` methodSignature
            public WeightedListeningExecutorService withDefaultAmounts​(ResourceAmounts newDefaultAmounts)
            ```

            ::: block
            Creates a new service that has different default resource
            amounts. Useful when you need to propagate explicit default
            amounts when you submit the job through execute(),
            Futures.transform() and similar calls.
            :::

            [Parameters:]{.paramLabel}
            :   `newDefaultAmounts` - new default amounts

            [Returns:]{.returnLabel}
            :   Service that uses the same semaphore and delegate but
                with the given default resource amounts.

        []{#submit(java.lang.Runnable,com.facebook.buck.util.concurrent.ResourceAmounts)}

        -   #### submit

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<?> submit​(Runnable task,
                                                                                ResourceAmounts amounts)
            ```

        []{#submit(java.lang.Runnable)}

        -   #### submit

            ``` methodSignature
            @Nonnull
            public com.google.common.util.concurrent.ListenableFuture<?> submit​(Runnable task)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `submit` in interface `ExecutorService`

            [Specified by:]{.overrideSpecifyLabel}
            :   `submit` in
                interface `com.google.common.util.concurrent.ListeningExecutorService`

            [Overrides:]{.overrideSpecifyLabel}
            :   `submit` in
                class `com.google.common.util.concurrent.AbstractListeningExecutorService`

        []{#submit(java.lang.Runnable,java.lang.Object,com.facebook.buck.util.concurrent.ResourceAmounts)}
        []{#submit(java.lang.Runnable,T,com.facebook.buck.util.concurrent.ResourceAmounts)}

        -   #### submit

            ``` methodSignature
            public <T> com.google.common.util.concurrent.ListenableFuture<T> submit​(Runnable task,
                                                                                    @Nullable
                                                                                    T result,
                                                                                    ResourceAmounts amounts)
            ```

        []{#submit(java.lang.Runnable,java.lang.Object)}
        []{#submit(java.lang.Runnable,T)}

        -   #### submit

            ``` methodSignature
            @Nonnull
            public <T> com.google.common.util.concurrent.ListenableFuture<T> submit​(Runnable task,
                                                                                    @Nullable
                                                                                    T result)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `submit` in interface `ExecutorService`

            [Specified by:]{.overrideSpecifyLabel}
            :   `submit` in
                interface `com.google.common.util.concurrent.ListeningExecutorService`

            [Overrides:]{.overrideSpecifyLabel}
            :   `submit` in
                class `com.google.common.util.concurrent.AbstractListeningExecutorService`

        []{#submit(java.util.concurrent.Callable,com.facebook.buck.util.concurrent.ResourceAmounts)}

        -   #### submit

            ``` methodSignature
            public <T> com.google.common.util.concurrent.ListenableFuture<T> submit​(Callable<T> task,
                                                                                    ResourceAmounts amounts)
            ```

        []{#submit(java.util.concurrent.Callable)}

        -   #### submit

            ``` methodSignature
            @Nonnull
            public <T> com.google.common.util.concurrent.ListenableFuture<T> submit​(Callable<T> task)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `submit` in interface `ExecutorService`

            [Specified by:]{.overrideSpecifyLabel}
            :   `submit` in
                interface `com.google.common.util.concurrent.ListeningExecutorService`

            [Overrides:]{.overrideSpecifyLabel}
            :   `submit` in
                class `com.google.common.util.concurrent.AbstractListeningExecutorService`

        []{#awaitTermination(long,java.util.concurrent.TimeUnit)}

        -   #### awaitTermination

            ``` methodSignature
            public final boolean awaitTermination​(long timeout,
                                                  @Nonnull
                                                  TimeUnit unit)
                                           throws InterruptedException
            ```

            [Throws:]{.throwsLabel}
            :   `InterruptedException`

        []{#isShutdown()}

        -   #### isShutdown

            ``` methodSignature
            public final boolean isShutdown()
            ```

        []{#isTerminated()}

        -   #### isTerminated

            ``` methodSignature
            public final boolean isTerminated()
            ```

        []{#shutdown()}

        -   #### shutdown

            ``` methodSignature
            public final void shutdown()
            ```

        []{#shutdownNow()}

        -   #### shutdownNow

            ``` methodSignature
            public final List<Runnable> shutdownNow()
            ```

        []{#execute(java.lang.Runnable)}

        -   #### execute

            ``` methodSignature
            public final void execute​(@Nonnull
                                      Runnable command)
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
