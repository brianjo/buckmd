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
[Package]{.packageLabelInType} [com.facebook.buck.worker](package-summary.html)
:::

## Class WorkerProcessPoolSync.BorrowedWorkerProcess {#class-workerprocesspoolsync.borrowedworkerprocess .title title="Class WorkerProcessPoolSync.BorrowedWorkerProcess"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.worker.WorkerProcessPoolSync.BorrowedWorkerProcess

::: description
-   

    All Implemented Interfaces:
    :   `Closeable`, `AutoCloseable`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [WorkerProcessPoolSync](WorkerProcessPoolSync.html "class in com.facebook.buck.worker")

    ------------------------------------------------------------------------

        public static class WorkerProcessPoolSync.BorrowedWorkerProcess
        extends Object
        implements Closeable

    ::: block
    Represents a
    [`WorkerProcess`](WorkerProcess.html "class in com.facebook.buck.worker")
    borrowed from a
    [`WorkerProcessPoolSync`](WorkerProcessPoolSync.html "class in com.facebook.buck.worker").
    Ownership must be returned to the pool by calling
    [`close()`](#close()) after finishing to use the worker.

    Since BorrowedWorkerProcess implements Closable, it can be used with
    a try-with-resources statement.

    BorrowedWorkerProcess is not threadsafe, and is expected to be used
    by one thread at a time only. Concurrency control is handled by
    [`WorkerProcessPoolSync`](WorkerProcessPoolSync.html "class in com.facebook.buck.worker")
    and `WorkerProcessPoolSync.WorkerLifecycle`.
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
        |                       |                       | Returns ownership of  |
        |                       |                       | the borrowed worker   |
        |                       |                       | process back to the   |
        |                       |                       | pool it was retrieved |
        |                       |                       | from.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.g                | `submitJob​(Str        | ::: block             |
        | oogle.common.util.con | ing expandedJobArgs)` | Submits a job to the  |
        | current.ListenableFut |                       | worker, and returns   |
        | ure<WorkerJobResult>` |                       | the result.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

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
    -   []{#method.detail}

        ### Method Detail

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
            ```

            ::: block
            Returns ownership of the borrowed worker process back to the
            pool it was retrieved from.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `Closeable`

        []{#submitJob(java.lang.String)}

        -   #### submitJob

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<WorkerJobResult> submitJob​(String expandedJobArgs)
                                                                                          throws IOException
            ```

            ::: block
            Submits a job to the worker, and returns the result.
            :::

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
