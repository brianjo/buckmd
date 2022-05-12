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
[Package]{.packageLabelInType} [com.facebook.buck.support.bgtasks](package-summary.html)
:::

## Class AsyncBackgroundTaskManager {#class-asyncbackgroundtaskmanager .title title="Class AsyncBackgroundTaskManager"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.support.bgtasks.BackgroundTaskManager](BackgroundTaskManager.html "class in com.facebook.buck.support.bgtasks")

    -   -   com.facebook.buck.support.bgtasks.AsyncBackgroundTaskManager

::: description
-   

    ------------------------------------------------------------------------

        public class AsyncBackgroundTaskManager
        extends BackgroundTaskManager

    ::: block
    Asynchronous-enabled implementation of
    [`BackgroundTaskManager`](BackgroundTaskManager.html "class in com.facebook.buck.support.bgtasks").
    Tasks run in a pool. Takes a blocking flag in constructor; when
    `blocking=true`, manager waits for tasks to complete before
    returning control to client. When `blocking=false`, manager
    schedules on a separate thread and does not wait for task
    completion. Scheduler thread is paused whenever a new command
    begins.
    NOTE: only a manager on buckd should be set/instantiated to
    nonblocking mode, otherwise unexpected behavior might occur
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                  Description
          -------------- -------------------------------------------- -------------
          `protected `   `AsyncBackgroundTaskManager​(int nThreads)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected Map<Class< | `g                    | ::: block             |
        | ?>,​com.facebook.buck. | etCancellableTasks()` | Return map of tasks   |
        | support.bgtasks.Manag |                       | that might be         |
        | edBackgroundTask<?>>` |                       | cancelled (i.e.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected int`       | `                     |                       |
        |                       | getCommandsRunning()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Tas                  | `getNewScope​(Buil     | ::: block             |
        | kManagerCommandScope` | dId buildId,          | Returns a new         |
        |                       |    boolean blocking)` | [`TaskManagerComma    |
        |                       |                       | ndScope`](TaskManager |
        |                       |                       | CommandScope.html "cl |
        |                       |                       | ass in com.facebook.b |
        |                       |                       | uck.support.bgtasks") |
        |                       |                       | for a build on this   |
        |                       |                       | manager.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected Que        | `getScheduledTasks()` | ::: block             |
        | ue<com.facebook.buck. |                       | Return list of        |
        | support.bgtasks.Manag |                       | currently scheduled   |
        | edBackgroundTask<?>>` |                       | (not yet submitted)   |
        |                       |                       | tasks.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected boolean`   | `isShutDown()`        | ::: block             |
        |                       |                       | Check if the manager  |
        |                       |                       | is shut down.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static AsyncB        | `of()`                | ::: block             |
        | ackgroundTaskManager` |                       | Same as               |
        |                       |                       | [`of()`](#of())       |
        |                       |                       | except with the       |
        |                       |                       | default number of     |
        |                       |                       | threads.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static AsyncB        | `of​(int nThreads)`    | ::: block             |
        | ackgroundTaskManager` |                       | Constructs an         |
        |                       |                       | [`As                  |
        |                       |                       | yncBackgroundTaskMana |
        |                       |                       | ger`](AsyncBackground |
        |                       |                       | TaskManager.html "cla |
        |                       |                       | ss in com.facebook.bu |
        |                       |                       | ck.support.bgtasks"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `shutd                | ::: block             |
        |                       | own​(long timeout,     | Shut down manager,    |
        |                       |      TimeUnit units)` | waiting until given   |
        |                       |                       | timeout for tasks to  |
        |                       |                       | finish.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `shutdownNow()`       | ::: block             |
        |                       |                       | Shut down scheduler   |
        |                       |                       | and pool threads.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected void`      | `startScheduling()`   |                       |
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(int)}

        -   #### AsyncBackgroundTaskManager

                protected AsyncBackgroundTaskManager​(int nThreads)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#of(int)}

        -   #### of

            ``` methodSignature
            public static AsyncBackgroundTaskManager of​(int nThreads)
            ```

            ::: block
            Constructs an
            [`AsyncBackgroundTaskManager`](AsyncBackgroundTaskManager.html "class in com.facebook.buck.support.bgtasks").
            If in nonblocking mode, sets up a scheduler thread and pool
            for tasks.
            :::

            [Parameters:]{.paramLabel}
            :   `nThreads` - (optional) number of threads in pool.
                defaults to `DEFAULT_THREADS` if not provided

        []{#of()}

        -   #### of

            ``` methodSignature
            public static AsyncBackgroundTaskManager of()
            ```

            ::: block
            Same as [`of()`](#of()) except with the default number of
            threads.
            :::

        []{#getNewScope(com.facebook.buck.core.model.BuildId,boolean)}

        -   #### getNewScope

            ``` methodSignature
            public TaskManagerCommandScope getNewScope​(BuildId buildId,
                                                       boolean blocking)
            ```

            ::: block
            [Description copied from
            class: `BackgroundTaskManager`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns a new
            [`TaskManagerCommandScope`](TaskManagerCommandScope.html "class in com.facebook.buck.support.bgtasks")
            for a build on this manager. The
            [`TaskManagerCommandScope`](TaskManagerCommandScope.html "class in com.facebook.buck.support.bgtasks")
            lives for the duration of the command such that it\'s
            [`TaskManagerCommandScope.close()`](TaskManagerCommandScope.html#close())
            will trigger the tasks scheduled to be ran.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNewScope` in class `BackgroundTaskManager`

            [Parameters:]{.paramLabel}
            :   `buildId` - unique identifier
                [`BuildId`](../../core/model/BuildId.html "class in com.facebook.buck.core.model")
                of a command that created a scope
            :   `blocking` - whether the current command should wait for
                tasks to finish on exit

        []{#startScheduling()}

        -   #### startScheduling

            ``` methodSignature
            protected void startScheduling()
            ```

        []{#shutdownNow()}

        -   #### shutdownNow

            ``` methodSignature
            public void shutdownNow()
            ```

            ::: block
            Shut down scheduler and pool threads.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `shutdownNow` in class `BackgroundTaskManager`

        []{#shutdown(long,java.util.concurrent.TimeUnit)}

        -   #### shutdown

            ``` methodSignature
            public void shutdown​(long timeout,
                                 TimeUnit units)
                          throws InterruptedException
            ```

            ::: block
            [Description copied from
            class: `BackgroundTaskManager`]{.descfrmTypeLabel}
            :::

            ::: block
            Shut down manager, waiting until given timeout for tasks to
            finish.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `shutdown` in class `BackgroundTaskManager`

            [Parameters:]{.paramLabel}
            :   `timeout` - timeout for tasks to finish
            :   `units` - units of timeout

            [Throws:]{.throwsLabel}
            :   `InterruptedException`

        []{#getScheduledTasks()}

        -   #### getScheduledTasks

            ``` methodSignature
            protected Queue<com.facebook.buck.support.bgtasks.ManagedBackgroundTask<?>> getScheduledTasks()
            ```

            ::: block
            Return list of currently scheduled (not yet submitted)
            tasks. For debugging/testing.
            :::

            [Returns:]{.returnLabel}
            :   list of currently scheduled tasks

        []{#getCancellableTasks()}

        -   #### getCancellableTasks

            ``` methodSignature
            protected Map<Class<?>,​com.facebook.buck.support.bgtasks.ManagedBackgroundTask<?>> getCancellableTasks()
            ```

            ::: block
            Return map of tasks that might be cancelled (i.e. not run)
            if a task with the same action is subsequently scheduled.
            Tasks in this map are currently scheduled, not yet run. For
            debugging/testing.
            :::

            [Returns:]{.returnLabel}
            :   map of cancellable tasks

        []{#isShutDown()}

        -   #### isShutDown

            ``` methodSignature
            protected boolean isShutDown()
            ```

            ::: block
            Check if the manager is shut down. \"Shut down\" means that
            all executors are terminated and manager is no longer
            accepting new task submissions. For debugging/testing.
            :::

            [Returns:]{.returnLabel}
            :   true if manager is shut down, false otherwise

        []{#getCommandsRunning()}

        -   #### getCommandsRunning

            ``` methodSignature
            protected int getCommandsRunning()
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
