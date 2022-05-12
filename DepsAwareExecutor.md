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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.graph.transformation.executor](package-summary.html)
:::

## Interface DepsAwareExecutor\<ResultType,​TaskType extends [DepsAwareTask](DepsAwareTask.html "class in com.facebook.buck.core.graph.transformation.executor")\<ResultType,​TaskType\>\> {#interface-depsawareexecutorresulttypetasktype-extends-depsawaretaskresulttypetasktype .title title="Interface DepsAwareExecutor"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AutoCloseable`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `DefaultDepsAwareExecutor`,
        `DefaultDepsAwareExecutorWithLocalStack`,
        `JavaExecutorBackedDefaultDepsAwareExecutor`,
        `ToposortBasedDepsAwareExecutor`

    ------------------------------------------------------------------------

        public interface DepsAwareExecutor<ResultType,​TaskType extends DepsAwareTask<ResultType,​TaskType>>
        extends AutoCloseable

    ::: block
    A specialized Executor that executes
    [`DepsAwareTask`](DepsAwareTask.html "class in com.facebook.buck.core.graph.transformation.executor").
    This executor will attempt to maintain maximum concurrency, while
    completing dependencies of each supplied work first.
    It is guaranteed that the dependencies from
    [`DepsAwareTask.getDepsSupplier()`](DepsAwareTask.html#getDepsSupplier())
    will be completed before the work itself is executed.

    In terms of thread safety, it is guaranteed that for the same
    [`DepsAwareTask`](DepsAwareTask.html "class in com.facebook.buck.core.graph.transformation.executor"),
    its deps supplier from
    [`DepsAwareTask.getDepsSupplier()`](DepsAwareTask.html#getDepsSupplier())
    will be executed before its callable from
    [`DepsAwareTask.getCallable()`](DepsAwareTask.html#getCallable()) is
    executed. That is, the supplier execution \"happens before\" the
    callable execution, but potentially in different threads, where
    \"happens before\" is the standard event ordering a -\> b. There is
    an at least once guarantee on the number of invocations of the deps
    supplier, and an exactly once guarantee on the callable. There is no
    guarantee of synchronization between different instances of
    [`DepsAwareTask`](DepsAwareTask.html "class in com.facebook.buck.core.graph.transformation.executor")
    other than that its dependencies will be completed before the
    callable is evaluated.
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
        | `TaskType`            | `                     |                       |
        |                       | createTask​(Callable<R |                       |
        |                       | esultType> callable)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `TaskType`            | `createThrowingTask   |                       |
        |                       | ​(Callable<ResultType> |                       |
        |                       |  callable,            |                       |
        |                       |         ThrowingSuppl |                       |
        |                       | ier<com.google.common |                       |
        |                       | .collect.ImmutableSet |                       |
        |                       | <TaskType>,​Exception> |                       |
        |                       |  prereqSupplier,      |                       |
        |                       |               Throwin |                       |
        |                       | gSupplier<com.google. |                       |
        |                       | common.collect.Immuta |                       |
        |                       | bleSet<TaskType>,​Exce |                       |
        |                       | ption> depsSupplier)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isShutdown()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Future<ResultType>`  | `s                    |                       |
        |                       | ubmit​(TaskType task)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.   | `submitAll​(Collect    | ::: block             |
        | collect.ImmutableList | ion<TaskType> tasks)` | Same as               |
        | <Future<ResultType>>` |                       | [`                    |
        |                       |                       | submit(DepsAwareTask) |
        |                       |                       | `](#submit(TaskType)) |
        |                       |                       | except for multiple   |
        |                       |                       | tasks.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#close()}

        -   #### close

            ``` methodSignature
            void close()
            ```

            ::: block
            Shuts down the executor workers immediately. This does not
            shutdown the underlying executor backing the
            [`DepsAwareExecutor`](DepsAwareExecutor.html "interface in com.facebook.buck.core.graph.transformation.executor")
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

        []{#isShutdown()}

        -   #### isShutdown

            ``` methodSignature
            boolean isShutdown()
            ```

            [Returns:]{.returnLabel}
            :   true iff [`close()`](#close()) has been called

        []{#createThrowingTask(java.util.concurrent.Callable,com.facebook.buck.util.function.ThrowingSupplier,com.facebook.buck.util.function.ThrowingSupplier)}

        -   #### createThrowingTask

            ``` methodSignature
            TaskType createThrowingTask​(Callable<ResultType> callable,
                                        ThrowingSupplier<com.google.common.collect.ImmutableSet<TaskType>,​Exception> prereqSupplier,
                                        ThrowingSupplier<com.google.common.collect.ImmutableSet<TaskType>,​Exception> depsSupplier)
            ```

            [Returns:]{.returnLabel}
            :   a new
                [`DepsAwareTask`](DepsAwareTask.html "class in com.facebook.buck.core.graph.transformation.executor")
                with two stages of dependency computation

        []{#createTask(java.util.concurrent.Callable)}

        -   #### createTask

            ``` methodSignature
            TaskType createTask​(Callable<ResultType> callable)
            ```

            [Returns:]{.returnLabel}
            :   a new
                [`DepsAwareTask`](DepsAwareTask.html "class in com.facebook.buck.core.graph.transformation.executor")
                that can be executed in this executor

        []{#submit(com.facebook.buck.core.graph.transformation.executor.DepsAwareTask)}
        []{#submit(TaskType)}

        -   #### submit

            ``` methodSignature
            Future<ResultType> submit​(TaskType task)
            ```

            [Parameters:]{.paramLabel}
            :   `task` - the
                [`DepsAwareTask`](DepsAwareTask.html "class in com.facebook.buck.core.graph.transformation.executor")
                to run

            [Returns:]{.returnLabel}
            :   a future of the result

        []{#submitAll(java.util.Collection)}

        -   #### submitAll

            ``` methodSignature
            com.google.common.collect.ImmutableList<Future<ResultType>> submitAll​(Collection<TaskType> tasks)
            ```

            ::: block
            Same as [`submit(DepsAwareTask)`](#submit(TaskType)) except
            for multiple tasks.
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
