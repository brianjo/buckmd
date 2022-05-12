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

## Class MoreFutures {#class-morefutures .title title="Class MoreFutures"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.concurrent.MoreFutures

::: description
-   

    ------------------------------------------------------------------------

        public class MoreFutures
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `stati                | `addLi                | ::: block             |
        | c <V> com.google.comm | stenableCallback​(com. | Add a callback to a   |
        | on.util.concurrent.Li | google.common.util.co | listenable future     |
        | stenableFuture<Unit>` | ncurrent.ListenableFu | :::                   |
        |                       | ture<V> future,       |                       |
        |                       |                 com.g |                       |
        |                       | oogle.common.util.con |                       |
        |                       | current.FutureCallbac |                       |
        |                       | k<? super V> callback |                       |
        |                       | ,                     |                       |
        |                       |   Executor executor)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <U,​V          | `combinedFuture       | ::: block             |
        | >com.google.common.ut | s​(com.google.common.u | Combine the {@param   |
        | il.concurrent.Listena | til.concurrent.Listen | first} and {@param    |
        | bleFuture<Pair<U,​V>>` | ableFuture<U> first,  | second} listenable    |
        |                       |                com.go | futures, returning a  |
        |                       | ogle.common.util.conc | listenable future     |
        |                       | urrent.ListenableFutu | that wraps the result |
        |                       | re<V> second,         | of these futures as a |
        |                       |         com.google.co | [`Pair                |
        |                       | mmon.util.concurrent. | `](../types/Pair.html |
        |                       | ListeningExecutorServ |  "class in com.facebo |
        |                       | ice executorService)` | ok.buck.util.types"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `finallyCallbac       |                       |
        | static <V> com.google | k​(Runnable runnable)` |                       |
        | .common.util.concurre |                       |                       |
        | nt.FutureCallback<V>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `fina                 |                       |
        | static <V> com.google | llyCallback​(java.util |                       |
        | .common.util.concurre | .function.Consumer<co |                       |
        | nt.FutureCallback<V>` | m.google.common.util. |                       |
        |                       | concurrent.Listenable |                       |
        |                       | Future<V>> callable)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <V> List<V>`  | `getAll​(com.google    | ::: block             |
        |                       | .common.util.concurre | Invoke multiple       |
        |                       | nt.ListeningExecutorS | callables on the      |
        |                       | ervice executorServic | provided executor and |
        |                       | e,       Iterable<Cal | wait for all to       |
        |                       | lable<V>> callables)` | return successfully.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Throwable`    | `getFailure           | ::: block             |
        |                       | ​(com.google.common.ut | Returns the failure   |
        |                       | il.concurrent.Listena | for a                 |
        |                       | bleFuture<?> future)` | `ListenableFuture`.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static <V> V`        | `ge                   | ::: block             |
        |                       | tUncheckedInterruptib | Waits for the given   |
        |                       | ly​(Future<V> future)` | future to complete    |
        |                       |                       | and returns the       |
        |                       |                       | result.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `isSuccess            | ::: block             |
        |                       | ​(com.google.common.ut | Create a convenience  |
        |                       | il.concurrent.Listena | method for checking   |
        |                       | bleFuture<?> future)` | whether a future      |
        |                       |                       | completed             |
        |                       |                       | successfully because  |
        |                       |                       | this does not appear  |
        |                       |                       | to be possible to do  |
        |                       |                       | in a more direct way: |
        |                       |                       | https://groups.       |
        |                       |                       | google.com/forum/?fro |
        |                       |                       | mgroups=#!topic/guava |
        |                       |                       | -discuss/rofEhagKnOc. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static <X ex         | `propagateCauseIfIn   |                       |
        | tends Throwable>void` | stanceOf​(Throwable e, |                       |
        |                       |                       |                       |
        |                       |       Class<X> type)` |                       |
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

        []{#combinedFutures(com.google.common.util.concurrent.ListenableFuture,com.google.common.util.concurrent.ListenableFuture,com.google.common.util.concurrent.ListeningExecutorService)}

        -   #### combinedFutures

            ``` methodSignature
            public static <U,​V> com.google.common.util.concurrent.ListenableFuture<Pair<U,​V>> combinedFutures​(com.google.common.util.concurrent.ListenableFuture<U> first,
                                                                                                                          com.google.common.util.concurrent.ListenableFuture<V> second,
                                                                                                                          com.google.common.util.concurrent.ListeningExecutorService executorService)
            ```

            ::: block
            Combine the {@param first} and {@param second} listenable
            futures, returning a listenable future that wraps the result
            of these futures as a
            [`Pair`](../types/Pair.html "class in com.facebook.buck.util.types").
            :::

        []{#getAll(com.google.common.util.concurrent.ListeningExecutorService,java.lang.Iterable)}

        -   #### getAll

            ``` methodSignature
            public static <V> List<V> getAll​(com.google.common.util.concurrent.ListeningExecutorService executorService,
                                             Iterable<Callable<V>> callables)
                                      throws ExecutionException,
                                             InterruptedException
            ```

            ::: block
            Invoke multiple callables on the provided executor and wait
            for all to return successfully. An exception is thrown
            (immediately) if any callable fails.
            :::

            [Parameters:]{.paramLabel}
            :   `executorService` - Executor service.
            :   `callables` - Callables to call.

            [Returns:]{.returnLabel}
            :   List of values from each invoked callable in order if
                all callables execute without throwing.

            [Throws:]{.throwsLabel}
            :   `ExecutionException` - If any callable throws an
                exception, the first of such is wrapped in an
                ExecutionException and thrown. Access via
                [`Throwable.getCause()`](http://docs.oracle.com/javase/7/docs/api/java/lang/Throwable.html?is-external=true#getCause() "class or interface in java.lang"){.externalLink}}.
            :   `InterruptedException`

        []{#isSuccess(com.google.common.util.concurrent.ListenableFuture)}

        -   #### isSuccess

            ``` methodSignature
            public static boolean isSuccess​(com.google.common.util.concurrent.ListenableFuture<?> future)
                                     throws InterruptedException
            ```

            ::: block
            Create a convenience method for checking whether a future
            completed successfully because this does not appear to be
            possible to do in a more direct way:
            https://groups.google.com/forum/?fromgroups=#!topic/guava-discuss/rofEhagKnOc.
            :::

            [Returns:]{.returnLabel}
            :   true if the specified future has been resolved without
                throwing an exception or being cancelled.

            [Throws:]{.throwsLabel}
            :   `InterruptedException`

        []{#getFailure(com.google.common.util.concurrent.ListenableFuture)}

        -   #### getFailure

            ``` methodSignature
            public static Throwable getFailure​(com.google.common.util.concurrent.ListenableFuture<?> future)
                                        throws InterruptedException
            ```

            ::: block
            Returns the failure for a `ListenableFuture`.
            :::

            [Parameters:]{.paramLabel}
            :   `future` - Must have completed unsuccessfully.

            [Throws:]{.throwsLabel}
            :   `InterruptedException`

        []{#addListenableCallback(com.google.common.util.concurrent.ListenableFuture,com.google.common.util.concurrent.FutureCallback,java.util.concurrent.Executor)}

        -   #### addListenableCallback

            ``` methodSignature
            public static <V> com.google.common.util.concurrent.ListenableFuture<Unit> addListenableCallback​(com.google.common.util.concurrent.ListenableFuture<V> future,
                                                                                                             com.google.common.util.concurrent.FutureCallback<? super V> callback,
                                                                                                             Executor executor)
            ```

            ::: block
            Add a callback to a listenable future
            :::

        []{#getUncheckedInterruptibly(java.util.concurrent.Future)}

        -   #### getUncheckedInterruptibly

            ``` methodSignature
            public static <V> V getUncheckedInterruptibly​(Future<V> future)
            ```

            ::: block
            Waits for the given future to complete and returns the
            result. On interrupt, this method throws
            [`CancellationException`](http://docs.oracle.com/javase/7/docs/api/java/util/concurrent/CancellationException.html?is-external=true "class or interface in java.util.concurrent"){.externalLink}.
            All exceptions thrown are wrapped with
            [`BuckUncheckedExecutionException`](../../core/exceptions/BuckUncheckedExecutionException.html "class in com.facebook.buck.core.exceptions")
            :::

            [Type Parameters:]{.paramLabel}
            :   `V` - the result type of the
                [`Future`](http://docs.oracle.com/javase/7/docs/api/java/util/concurrent/Future.html?is-external=true "class or interface in java.util.concurrent"){.externalLink}

            [Parameters:]{.paramLabel}
            :   `future` - the
                [`Future`](http://docs.oracle.com/javase/7/docs/api/java/util/concurrent/Future.html?is-external=true "class or interface in java.util.concurrent"){.externalLink}
                to wait for

            [Returns:]{.returnLabel}
            :   the result of the
                [`Future`](http://docs.oracle.com/javase/7/docs/api/java/util/concurrent/Future.html?is-external=true "class or interface in java.util.concurrent"){.externalLink}
                when completed

        []{#propagateCauseIfInstanceOf(java.lang.Throwable,java.lang.Class)}

        -   #### propagateCauseIfInstanceOf

            ``` methodSignature
            public static <X extends Throwable> void propagateCauseIfInstanceOf​(Throwable e,
                                                                                Class<X> type)
            ```

        []{#finallyCallback(java.lang.Runnable)}

        -   #### finallyCallback

            ``` methodSignature
            public static <V> com.google.common.util.concurrent.FutureCallback<V> finallyCallback​(Runnable runnable)
            ```

            [Returns:]{.returnLabel}
            :   a `FutureCallback` which executes the given
                [`Runnable`](http://docs.oracle.com/javase/7/docs/api/java/lang/Runnable.html?is-external=true "class or interface in java.lang"){.externalLink}
                on both success and error.

        []{#finallyCallback(java.util.function.Consumer)}

        -   #### finallyCallback

            ``` methodSignature
            public static <V> com.google.common.util.concurrent.FutureCallback<V> finallyCallback​(java.util.function.Consumer<com.google.common.util.concurrent.ListenableFuture<V>> callable)
            ```

            [Returns:]{.returnLabel}
            :   a `FutureCallback` which executes the given `Consumer`
                on both success and error. This just makes it simpler to
                add unconditional callbacks.
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
