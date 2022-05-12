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
[Package]{.packageLabelInType} [com.facebook.buck.util.concurrent](package-summary.html)
:::

## Class WorkThreadTrackingTask\<T\> {#class-workthreadtrackingtaskt .title title="Class WorkThreadTrackingTask"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.util.concurrent.ForkJoinTask](http://docs.oracle.com/javase/7/docs/api/java/util/concurrent/ForkJoinTask.html?is-external=true "class or interface in java.util.concurrent"){.externalLink}\<T\>

    -   -   com.facebook.buck.util.concurrent.WorkThreadTrackingTask\<T\>

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`, `Future<T>`

    ------------------------------------------------------------------------

        public class WorkThreadTrackingTask<T>
        extends ForkJoinTask<T>

    ::: block
    A
    [`ForkJoinTask`](http://docs.oracle.com/javase/7/docs/api/java/util/concurrent/ForkJoinTask.html?is-external=true "class or interface in java.util.concurrent"){.externalLink}
    which keeps track of the thread running its computation.
    This task performs [`compute()`](#compute()) in a thread safe
    manner, guaranteeing only one computation will happen even when
    called between multiple threads.
    :::

    [See Also:]{.seeLabel}
    :   [Serialized
        Form](../../../../../serialized-form.html#com.facebook.buck.util.concurrent.WorkThreadTrackingTask)
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type    Field          Description
          -------------------- -------------- -------------
          `protected Thread`   `workThread`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                     Description
          --------------------------------------------------------------- -------------
          `WorkThreadTrackingTask​(java.util.function.Supplier<T> work)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `complete​(T value)`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <T> WorkT     | `completed​(T value)`  |                       |
        | hreadTrackingTask<T>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected T`         | `compute()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected boolean`   | `exec()`              |                       |
        +-----------------------+-----------------------+-----------------------+
        | `T`                   | `externalCompute()`   | ::: block             |
        |                       |                       | computes and          |
        |                       |                       | completes this task,  |
        |                       |                       | which can be called   |
        |                       |                       | outside of the        |
        |                       |                       | forkjoin framework,   |
        |                       |                       | or by threads that    |
        |                       |                       | did not originally    |
        |                       |                       | fork the task.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `T`                   | `getRawResult()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isBeingWorke         |                       |
        |                       | dOnByCurrentThread()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected void`      | `s                    |                       |
        |                       | etRawResult​(T value)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.util.concurrent.ForkJoinTask}

            ### Methods inherited from class java.util.concurrent.[ForkJoinTask](http://docs.oracle.com/javase/7/docs/api/java/util/concurrent/ForkJoinTask.html?is-external=true "class or interface in java.util.concurrent"){.externalLink}

            `adapt, adapt, adapt, cancel, compareAndSetForkJoinTaskTag, completeExceptionally, fork, get, get, getException, getForkJoinTaskTag, getPool, getQueuedTaskCount, getSurplusQueuedTaskCount, helpQuiesce, inForkJoinPool, invoke, invokeAll, invokeAll, invokeAll, isCancelled, isCompletedAbnormally, isCompletedNormally, isDone, join, peekNextLocalTask, pollNextLocalTask, pollSubmission, pollTask, quietlyComplete, quietlyInvoke, quietlyJoin, reinitialize, setForkJoinTaskTag, tryUnfork`

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
    -   []{#field.detail}

        ### Field Detail

        []{#workThread}

        -   #### workThread

                @Nullable
                protected volatile Thread workThread
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.util.function.Supplier)}

        -   #### WorkThreadTrackingTask

                public WorkThreadTrackingTask​(java.util.function.Supplier<T> work)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#externalCompute()}

        -   #### externalCompute

            ``` methodSignature
            @Nullable
            public final T externalCompute()
            ```

            ::: block
            computes and completes this task, which can be called
            outside of the forkjoin framework, or by threads that did
            not originally fork the task.
            Exceptions are propagated via UncheckedExecutionExceptions
            :::

            [Returns:]{.returnLabel}
            :   the result of the task

        []{#compute()}

        -   #### compute

            ``` methodSignature
            @Nullable
            protected final T compute()
            ```

        []{#isBeingWorkedOnByCurrentThread()}

        -   #### isBeingWorkedOnByCurrentThread

            ``` methodSignature
            public final boolean isBeingWorkedOnByCurrentThread()
            ```

        []{#complete(java.lang.Object)} []{#complete(T)}

        -   #### complete

            ``` methodSignature
            public void complete​(T value)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `complete` in class `ForkJoinTask<T>`

        []{#getRawResult()}

        -   #### getRawResult

            ``` methodSignature
            @Nullable
            public T getRawResult()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRawResult` in class `ForkJoinTask<T>`

        []{#setRawResult(java.lang.Object)} []{#setRawResult(T)}

        -   #### setRawResult

            ``` methodSignature
            protected void setRawResult​(T value)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `setRawResult` in class `ForkJoinTask<T>`

        []{#exec()}

        -   #### exec

            ``` methodSignature
            protected boolean exec()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `exec` in class `ForkJoinTask<T>`

        []{#completed(java.lang.Object)} []{#completed(T)}

        -   #### completed

            ``` methodSignature
            public static <T> WorkThreadTrackingTask<T> completed​(T value)
            ```

            [Returns:]{.returnLabel}
            :   an already completed task
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
