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
[Package]{.packageLabelInType} [com.facebook.buck.core.graph.transformation.executor.impl](package-summary.html)
:::

## Class JavaExecutorBackedDefaultDepsAwareExecutor\<T\> {#class-javaexecutorbackeddefaultdepsawareexecutort .title title="Class JavaExecutorBackedDefaultDepsAwareExecutor"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.graph.transformation.executor.impl.JavaExecutorBackedDefaultDepsAwareExecutor\<T\>

::: description
-   

    All Implemented Interfaces:
    :   `DepsAwareExecutor<T,​com.facebook.buck.core.graph.transformation.executor.impl.DefaultDepsAwareTask<T>>`,
        `AutoCloseable`

    ------------------------------------------------------------------------

        public class JavaExecutorBackedDefaultDepsAwareExecutor<T>
        extends Object
        implements DepsAwareExecutor<T,​com.facebook.buck.core.graph.transformation.executor.impl.DefaultDepsAwareTask<T>>

    ::: block
    A specialized Executor that executes
    [`DepsAwareTask`](../DepsAwareTask.html "class in com.facebook.buck.core.graph.transformation.executor").
    This executor will attempt to maintain maximum concurrency, while
    completing dependencies of each supplied work first.
    This implementation submits all tasks to java\'s default executors
    in a queue, without attempting insert dependent work in the front of
    the queue, but rather continuously requeue-ing them until an
    executable work is found. This is how Bazel\'s skyframe works.
    :::
:::

::: summary
-   ::: {.section role="region"}
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
        | `static <U> Java      | `of​(                  | ::: block             |
        | ExecutorBackedDefault | int numberOfThreads)` | Creates a             |
        | DepsAwareExecutor<U>` |                       | [`JavaExecutorBac     |
        |                       |                       | kedDefaultDepsAwareEx |
        |                       |                       | ecutor`](JavaExecutor |
        |                       |                       | BackedDefaultDepsAwar |
        |                       |                       | eExecutor.html "class |
        |                       |                       |  in com.facebook.buck |
        |                       |                       | .core.graph.transform |
        |                       |                       | ation.executor.impl") |
        |                       |                       | with given            |
        |                       |                       | `  numberOfThreads`.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Future<T>`           | `submit​(com.          |                       |
        |                       | facebook.buck.core.gr |                       |
        |                       | aph.transformation.ex |                       |
        |                       | ecutor.impl.DefaultDe |                       |
        |                       | psAwareTask<T> task)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `submit               | ::: block             |
        | e.common.collect.Immu | All​(Collection<com.fa | Same as               |
        | tableList<Future<T>>` | cebook.buck.core.grap | [`D                   |
        |                       | h.transformation.exec | epsAwareExecutor.subm |
        |                       | utor.impl.DefaultDeps | it(DepsAwareTask)`](. |
        |                       | AwareTask<T>> tasks)` | ./DepsAwareExecutor.h |
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
    -   []{#method.detail}

        ### Method Detail

        []{#of(int)}

        -   #### of

            ``` methodSignature
            public static <U> JavaExecutorBackedDefaultDepsAwareExecutor<U> of​(int numberOfThreads)
            ```

            ::: block
            Creates a
            [`JavaExecutorBackedDefaultDepsAwareExecutor`](JavaExecutorBackedDefaultDepsAwareExecutor.html "class in com.facebook.buck.core.graph.transformation.executor.impl")
            with given `  numberOfThreads`.
            :::

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
                interface `DepsAwareExecutor<T,​com.facebook.buck.core.graph.transformation.executor.impl.DefaultDepsAwareTask<T>>`

        []{#isShutdown()}

        -   #### isShutdown

            ``` methodSignature
            public boolean isShutdown()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isShutdown` in
                interface `DepsAwareExecutor<T,​com.facebook.buck.core.graph.transformation.executor.impl.DefaultDepsAwareTask<T>>`

            [Returns:]{.returnLabel}
            :   true iff
                [`DepsAwareExecutor.close()`](../DepsAwareExecutor.html#close())
                has been called

        []{#createThrowingTask(java.util.concurrent.Callable,com.facebook.buck.util.function.ThrowingSupplier,com.facebook.buck.util.function.ThrowingSupplier)}

        -   #### createThrowingTask

            ``` methodSignature
            public com.facebook.buck.core.graph.transformation.executor.impl.DefaultDepsAwareTask<T> createThrowingTask​(Callable<T> callable,
                                                                                                                        ThrowingSupplier<com.google.common.collect.ImmutableSet<com.facebook.buck.core.graph.transformation.executor.impl.DefaultDepsAwareTask<T>>,​Exception> prereqSupplier,
                                                                                                                        ThrowingSupplier<com.google.common.collect.ImmutableSet<com.facebook.buck.core.graph.transformation.executor.impl.DefaultDepsAwareTask<T>>,​Exception> depsSupplier)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createThrowingTask` in
                interface `DepsAwareExecutor<T,​com.facebook.buck.core.graph.transformation.executor.impl.DefaultDepsAwareTask<T>>`

            [Returns:]{.returnLabel}
            :   a new
                [`DepsAwareTask`](../DepsAwareTask.html "class in com.facebook.buck.core.graph.transformation.executor")
                with two stages of dependency computation

        []{#createTask(java.util.concurrent.Callable)}

        -   #### createTask

            ``` methodSignature
            public com.facebook.buck.core.graph.transformation.executor.impl.DefaultDepsAwareTask<T> createTask​(Callable<T> callable)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createTask` in
                interface `DepsAwareExecutor<T,​com.facebook.buck.core.graph.transformation.executor.impl.DefaultDepsAwareTask<T>>`

            [Returns:]{.returnLabel}
            :   a new
                [`DepsAwareTask`](../DepsAwareTask.html "class in com.facebook.buck.core.graph.transformation.executor")
                that can be executed in this executor

        []{#submit(com.facebook.buck.core.graph.transformation.executor.impl.DefaultDepsAwareTask)}

        -   #### submit

            ``` methodSignature
            public Future<T> submit​(com.facebook.buck.core.graph.transformation.executor.impl.DefaultDepsAwareTask<T> task)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `submit` in
                interface `DepsAwareExecutor<T,​com.facebook.buck.core.graph.transformation.executor.impl.DefaultDepsAwareTask<T>>`

            [Parameters:]{.paramLabel}
            :   `task` - the
                [`DepsAwareTask`](../DepsAwareTask.html "class in com.facebook.buck.core.graph.transformation.executor")
                to run

            [Returns:]{.returnLabel}
            :   a future of the result

        []{#submitAll(java.util.Collection)}

        -   #### submitAll

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Future<T>> submitAll​(Collection<com.facebook.buck.core.graph.transformation.executor.impl.DefaultDepsAwareTask<T>> tasks)
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
                interface `DepsAwareExecutor<T,​com.facebook.buck.core.graph.transformation.executor.impl.DefaultDepsAwareTask<T>>`
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
