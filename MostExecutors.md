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
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.util.concurrent](package-summary.html)
:::

## Class MostExecutors {#class-mostexecutors .title title="Class MostExecutors"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.concurrent.MostExecutors

::: description
-   

    ------------------------------------------------------------------------

        public class MostExecutors
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `MostExecutor         | ::: block             |
        |                       | s.NamedThreadFactory` | A ThreadFactory which |
        |                       |                       | gives each thread a   |
        |                       |                       | meaningful and        |
        |                       |                       | distinct name.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static ForkJoinPool` | `                     | ::: block             |
        |                       | forkJoinPoolWithThrea | Construct a           |
        |                       | dLimit​(int parallelis | ForkJoinPool with a   |
        |                       | m,                    | stricter thread       |
        |                       |          int spares)` | limit.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `newMultiThre         | ::: block             |
        | atic ExecutorService` | adExecutor​(String thr | Creates a             |
        |                       | eadName,              | multi-threaded        |
        |                       |           int count)` | executor with         |
        |                       |                       | meaningfully named    |
        |                       |                       | threads.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `n                    |                       |
        | atic ExecutorService` | ewMultiThreadExecutor |                       |
        |                       | ​(ThreadFactory thread |                       |
        |                       | Factory,              |                       |
        |                       |           int count)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `n                    | ::: block             |
        | atic ExecutorService` | ewSingleThreadExecuto | Creates a single      |
        |                       | r​(String threadName)` | threaded executor     |
        |                       |                       | that silently         |
        |                       |                       | discards rejected     |
        |                       |                       | tasks.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `newSingleTh          |                       |
        | atic ExecutorService` | readExecutor​(ThreadFa |                       |
        |                       | ctory threadFactory)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `shutdown​(Executo     | ::: block             |
        |                       | rService service,     | Shutdown `service`    |
        |                       |      long timeout,    | and wait for all      |
        |                       |       TimeUnit unit)` | it\'s tasks to        |
        |                       |                       | terminate.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `shutdownOrThrow​(E    | ::: block             |
        |                       | xecutorService servic | Cancel the processing |
        |                       | e,                lon | being carried out by  |
        |                       | g timeout,            | the given service and |
        |                       |      TimeUnit unit,   | waits for the         |
        |                       |               Runtime | processing to         |
        |                       | Exception exception)` | complete.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
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

        []{#newSingleThreadExecutor(java.lang.String)}

        -   #### newSingleThreadExecutor

            ``` methodSignature
            public static ExecutorService newSingleThreadExecutor​(String threadName)
            ```

            ::: block
            Creates a single threaded executor that silently discards
            rejected tasks. The problem with
            [`Executors.newSingleThreadExecutor()`](http://docs.oracle.com/javase/7/docs/api/java/util/concurrent/Executors.html?is-external=true#newSingleThreadExecutor() "class or interface in java.util.concurrent"){.externalLink}
            is that it does not let us specify a
            RejectedExecutionHandler, which we need to ensure that
            garbage is not spewed to the user\'s console if the build
            fails.
            :::

            [Parameters:]{.paramLabel}
            :   `threadName` - a thread name prefix used to easily
                identify threads when debugging.

            [Returns:]{.returnLabel}
            :   A single-threaded executor that silently discards
                rejected tasks.

        []{#newSingleThreadExecutor(java.util.concurrent.ThreadFactory)}

        -   #### newSingleThreadExecutor

            ``` methodSignature
            public static ExecutorService newSingleThreadExecutor​(ThreadFactory threadFactory)
            ```

        []{#newMultiThreadExecutor(java.lang.String,int)}

        -   #### newMultiThreadExecutor

            ``` methodSignature
            public static ExecutorService newMultiThreadExecutor​(String threadName,
                                                                 int count)
            ```

            ::: block
            Creates a multi-threaded executor with meaningfully named
            threads.
            :::

            [Parameters:]{.paramLabel}
            :   `threadName` - a thread name prefix used to easily
                identify threads when debugging.
            :   `count` - the number of threads that should be created
                in the pool.

            [Returns:]{.returnLabel}
            :   A multi-threaded executor.

        []{#newMultiThreadExecutor(java.util.concurrent.ThreadFactory,int)}

        -   #### newMultiThreadExecutor

            ``` methodSignature
            public static ExecutorService newMultiThreadExecutor​(ThreadFactory threadFactory,
                                                                 int count)
            ```

        []{#shutdown(java.util.concurrent.ExecutorService,long,java.util.concurrent.TimeUnit)}

        -   #### shutdown

            ``` methodSignature
            public static boolean shutdown​(ExecutorService service,
                                           long timeout,
                                           TimeUnit unit)
                                    throws InterruptedException
            ```

            ::: block
            Shutdown `service` and wait for all it\'s tasks to
            terminate. In the event of
            [`InterruptedException`](http://docs.oracle.com/javase/7/docs/api/java/lang/InterruptedException.html?is-external=true "class or interface in java.lang"){.externalLink},
            propagate the interrupt to all tasks, wait for them to
            finish, then re-throw the exception.
            :::

            [Throws:]{.throwsLabel}
            :   `InterruptedException`

        []{#shutdownOrThrow(java.util.concurrent.ExecutorService,long,java.util.concurrent.TimeUnit,java.lang.RuntimeException)}

        -   #### shutdownOrThrow

            ``` methodSignature
            public static void shutdownOrThrow​(ExecutorService service,
                                               long timeout,
                                               TimeUnit unit,
                                               RuntimeException exception)
            ```

            ::: block
            Cancel the processing being carried out by the given service
            and waits for the processing to complete. If processing has
            still not terminated the method throws the given exception.
            :::

        []{#forkJoinPoolWithThreadLimit(int,int)}

        -   #### forkJoinPoolWithThreadLimit

            ``` methodSignature
            public static ForkJoinPool forkJoinPoolWithThreadLimit​(int parallelism,
                                                                   int spares)
            ```

            ::: block
            Construct a ForkJoinPool with a stricter thread limit.
            ForkJoinPool by default will create a new thread to handle
            pending work whenever an existing thread becomes blocked on
            a task and cannot work steal. In cases when many tasks would
            block on a slow running dependency, it can trigger thread
            creation for all those tasks.

            Note that limiting the maximum threads will impact the
            ability for ManagedBlockers to cause the pool to create new
            worker threads, leading to potential deadlock if many
            ManagedBlockers are used.
            :::
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
-   [Nested](#nested.class.summary) \| 
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
