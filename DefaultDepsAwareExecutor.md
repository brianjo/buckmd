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

-   [Overview](../../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../../index-all.html)
-   [Help](../../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../../allclasses.html)

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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.graph.transformation.executor.impl](package-summary.html)
:::

## Class DefaultDepsAwareExecutor\<T\> {#class-defaultdepsawareexecutort .title title="Class DefaultDepsAwareExecutor"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.graph.transformation.executor.impl.DefaultDepsAwareExecutor\<T\>

::: description
-   

    All Implemented Interfaces:
    :   `DepsAwareExecutor<T,​com.facebook.buck.core.graph.transformation.executor.impl.DefaultDepsAwareTask<T>>`,
        `AutoCloseable`

    ------------------------------------------------------------------------

        public class DefaultDepsAwareExecutor<T>
        extends Object

    ::: block
    A specialized Executor that executes
    [`DepsAwareTask`](../DepsAwareTask.html "class in com.facebook.buck.core.graph.transformation.executor").
    This executor will attempt to maintain maximum concurrency, while
    completing dependencies of each supplied work first.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                     Field         Description
          ------------------------------------- ------------- -------------
          `protected Future<?>[]`               `workers`      
          `protected BlockingDeque<TaskType>`   `workQueue`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `close()`             | ::: block             |
        |                       |                       | Shuts down the        |
        |                       |                       | executor workers      |
        |                       |                       | immediately.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.facebook.buck.c  | `createTask​(C         |                       |
        | ore.graph.transformat | allable<T> callable)` |                       |
        | ion.executor.impl.Def |                       |                       |
        | aultDepsAwareTask<T>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.facebook.buck.c  | `createTh             |                       |
        | ore.graph.transformat | rowingTask​(Callable<T |                       |
        | ion.executor.impl.Def | > callable,           |                       |
        | aultDepsAwareTask<T>` |          ThrowingSupp |                       |
        |                       | lier<com.google.commo |                       |
        |                       | n.collect.ImmutableSe |                       |
        |                       | t<com.facebook.buck.c |                       |
        |                       | ore.graph.transformat |                       |
        |                       | ion.executor.impl.Def |                       |
        |                       | aultDepsAwareTask<T>> |                       |
        |                       | ,​Exception> prereqSup |                       |
        |                       | plier,                |                       |
        |                       |     ThrowingSupplier< |                       |
        |                       | com.google.common.col |                       |
        |                       | lect.ImmutableSet<com |                       |
        |                       | .facebook.buck.core.g |                       |
        |                       | raph.transformation.e |                       |
        |                       | xecutor.impl.DefaultD |                       |
        |                       | epsAwareTask<T>>,​Exce |                       |
        |                       | ption> depsSupplier)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isShutdown()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <U> Default   | `of​(                  | ::: block             |
        | DepsAwareExecutor<U>` | int numberOfThreads)` | Creates a             |
        |                       |                       | [`                    |
        |                       |                       | DefaultDepsAwareExecu |
        |                       |                       | tor`](DefaultDepsAwar |
        |                       |                       | eExecutor.html "class |
        |                       |                       |  in com.facebook.buck |
        |                       |                       | .core.graph.transform |
        |                       |                       | ation.executor.impl") |
        |                       |                       | with given            |
        |                       |                       | `numberOfThreads`.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `p                    | `runWorker​(com.faceb  |                       |
        | rotected static void` | ook.buck.core.graph.t |                       |
        |                       | ransformation.executo |                       |
        |                       | r.impl.AbstractDepsAw |                       |
        |                       | areWorker<?> worker)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected            | `startWo              |                       |
        | static <TaskType exte | rkers​(ExecutorService |                       |
        | nds com.facebook.buck |  executorService,     |                       |
        | .core.graph.transform |          int parallel |                       |
        | ation.executor.impl.A | ism,             Link |                       |
        | bstractDepsAwareTask< | edBlockingDeque<TaskT |                       |
        | ?,​TaskType>,​V extends | ype> workQueue,       |                       |
        |  com.facebook.buck.co |        java.util.func |                       |
        | re.graph.transformati | tion.Function<LinkedB |                       |
        | on.executor.impl.Abst | lockingDeque<TaskType |                       |
        | ractDepsAwareWorker<T | >,​V> workerFunction)` |                       |
        | askType>>Future<?>[]` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Future<T>`           | `s                    |                       |
        |                       | ubmit​(TaskType task)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `submitAll​(Collect    | ::: block             |
        | e.common.collect.Immu | ion<TaskType> tasks)` | Same as               |
        | tableList<Future<T>>` |                       | [`D                   |
        |                       |                       | epsAwareExecutor.subm |
        |                       |                       | it(DepsAwareTask)`](. |
        |                       |                       | ./DepsAwareExecutor.h |
        |                       |                       | tml#submit(TaskType)) |
        |                       |                       | except for multiple   |
        |                       |                       | tasks.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

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
    -   []{#field.detail}

        ### Field Detail

        []{#workQueue}

        -   #### workQueue

                protected final BlockingDeque<TaskType extends com.facebook.buck.core.graph.transformation.executor.impl.AbstractDepsAwareTask<T,​TaskType>> workQueue

        []{#workers}

        -   #### workers

                protected final Future<?>[] workers
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#of(int)}

        -   #### of

            ``` methodSignature
            public static <U> DefaultDepsAwareExecutor<U> of​(int numberOfThreads)
            ```

            ::: block
            Creates a
            [`DefaultDepsAwareExecutor`](DefaultDepsAwareExecutor.html "class in com.facebook.buck.core.graph.transformation.executor.impl")
            with given `numberOfThreads`.
            :::

        []{#createThrowingTask(java.util.concurrent.Callable,com.facebook.buck.util.function.ThrowingSupplier,com.facebook.buck.util.function.ThrowingSupplier)}

        -   #### createThrowingTask

            ``` methodSignature
            public com.facebook.buck.core.graph.transformation.executor.impl.DefaultDepsAwareTask<T> createThrowingTask​(Callable<T> callable,
                                                                                                                        ThrowingSupplier<com.google.common.collect.ImmutableSet<com.facebook.buck.core.graph.transformation.executor.impl.DefaultDepsAwareTask<T>>,​Exception> prereqSupplier,
                                                                                                                        ThrowingSupplier<com.google.common.collect.ImmutableSet<com.facebook.buck.core.graph.transformation.executor.impl.DefaultDepsAwareTask<T>>,​Exception> depsSupplier)
            ```

            [Returns:]{.returnLabel}
            :   a new
                [`DepsAwareTask`](../DepsAwareTask.html "class in com.facebook.buck.core.graph.transformation.executor")
                with two stages of dependency computation

        []{#createTask(java.util.concurrent.Callable)}

        -   #### createTask

            ``` methodSignature
            public com.facebook.buck.core.graph.transformation.executor.impl.DefaultDepsAwareTask<T> createTask​(Callable<T> callable)
            ```

            [Returns:]{.returnLabel}
            :   a new
                [`DepsAwareTask`](../DepsAwareTask.html "class in com.facebook.buck.core.graph.transformation.executor")
                that can be executed in this executor

        []{#runWorker(com.facebook.buck.core.graph.transformation.executor.impl.AbstractDepsAwareWorker)}

        -   #### runWorker

            ``` methodSignature
            protected static void runWorker​(com.facebook.buck.core.graph.transformation.executor.impl.AbstractDepsAwareWorker<?> worker)
            ```

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
            ```

            ::: block
            [Description copied from
            interface: `DepsAwareExecutor`]{.descfrmTypeLabel}
            :::

            ::: block
            Shuts down the executor workers immediately. This does not
            shutdown the underlying executor backing the
            [`DepsAwareExecutor`](../DepsAwareExecutor.html "interface in com.facebook.buck.core.graph.transformation.executor")
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in
                interface `DepsAwareExecutor<T,​TaskType extends com.facebook.buck.core.graph.transformation.executor.impl.AbstractDepsAwareTask<T,​TaskType>>`

        []{#isShutdown()}

        -   #### isShutdown

            ``` methodSignature
            public boolean isShutdown()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isShutdown` in
                interface `DepsAwareExecutor<T,​TaskType extends com.facebook.buck.core.graph.transformation.executor.impl.AbstractDepsAwareTask<T,​TaskType>>`

            [Returns:]{.returnLabel}
            :   true iff
                [`DepsAwareExecutor.close()`](../DepsAwareExecutor.html#close())
                has been called

        []{#submit(com.facebook.buck.core.graph.transformation.executor.impl.AbstractDepsAwareTask)}
        []{#submit(TaskType)}

        -   #### submit

            ``` methodSignature
            public Future<T> submit​(TaskType task)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `submit` in
                interface `DepsAwareExecutor<T,​TaskType extends com.facebook.buck.core.graph.transformation.executor.impl.AbstractDepsAwareTask<T,​TaskType>>`

            [Parameters:]{.paramLabel}
            :   `task` - the
                [`DepsAwareTask`](../DepsAwareTask.html "class in com.facebook.buck.core.graph.transformation.executor")
                to run

            [Returns:]{.returnLabel}
            :   a future of the result

        []{#submitAll(java.util.Collection)}

        -   #### submitAll

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Future<T>> submitAll​(Collection<TaskType> tasks)
            ```

            ::: block
            [Description copied from
            interface: `DepsAwareExecutor`]{.descfrmTypeLabel}
            :::

            ::: block
            Same as
            [`DepsAwareExecutor.submit(DepsAwareTask)`](../DepsAwareExecutor.html#submit(TaskType))
            except for multiple tasks.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `submitAll` in
                interface `DepsAwareExecutor<T,​TaskType extends com.facebook.buck.core.graph.transformation.executor.impl.AbstractDepsAwareTask<T,​TaskType>>`

        []{#startWorkers(java.util.concurrent.ExecutorService,int,java.util.concurrent.LinkedBlockingDeque,java.util.function.Function)}

        -   #### startWorkers

            ``` methodSignature
            protected static <TaskType extends com.facebook.buck.core.graph.transformation.executor.impl.AbstractDepsAwareTask<?,​TaskType>,​V extends com.facebook.buck.core.graph.transformation.executor.impl.AbstractDepsAwareWorker<TaskType>> Future<?>[] startWorkers​(ExecutorService executorService,
                                                                                                                                                                                                                                                                                       int parallelism,
                                                                                                                                                                                                                                                                                       LinkedBlockingDeque<TaskType> workQueue,
                                                                                                                                                                                                                                                                                       java.util.function.Function<LinkedBlockingDeque<TaskType>,​V> workerFunction)
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

-   [Overview](../../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../../index-all.html)
-   [Help](../../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   Nested \| 
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
