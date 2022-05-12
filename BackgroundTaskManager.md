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

## Class BackgroundTaskManager {#class-backgroundtaskmanager .title title="Class BackgroundTaskManager"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.support.bgtasks.BackgroundTaskManager

::: description
-   

    Direct Known Subclasses:
    :   `AsyncBackgroundTaskManager`

    ------------------------------------------------------------------------

        public abstract class BackgroundTaskManager
        extends Object

    ::: block
    BackgroundTaskManager schedules and runs background tasks like
    cleanup and logging. A manager should be notified when a new command
    starts and when it finishes so that it can schedule tasks
    appropriately. Tasks should typically be scheduled through a
    [`TaskManagerCommandScope`](TaskManagerCommandScope.html "class in com.facebook.buck.support.bgtasks").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                 Description
          --------------------------- -------------
          `BackgroundTaskManager()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `abstract Tas         | `getNewScope​(Buil     | ::: block             |
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
        | `abstract void`       | `shutd                | ::: block             |
        |                       | own​(long timeout,     | Shut down manager,    |
        |                       |      TimeUnit units)` | waiting until given   |
        |                       |                       | timeout for tasks to  |
        |                       |                       | finish.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract void`       | `shutdownNow()`       | ::: block             |
        |                       |                       | Shut down manager,    |
        |                       |                       | without waiting for   |
        |                       |                       | tasks to finish.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### BackgroundTaskManager

                public BackgroundTaskManager()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getNewScope(com.facebook.buck.core.model.BuildId,boolean)}

        -   #### getNewScope

            ``` methodSignature
            public abstract TaskManagerCommandScope getNewScope​(BuildId buildId,
                                                                boolean blocking)
            ```

            ::: block
            Returns a new
            [`TaskManagerCommandScope`](TaskManagerCommandScope.html "class in com.facebook.buck.support.bgtasks")
            for a build on this manager. The
            [`TaskManagerCommandScope`](TaskManagerCommandScope.html "class in com.facebook.buck.support.bgtasks")
            lives for the duration of the command such that it\'s
            [`TaskManagerCommandScope.close()`](TaskManagerCommandScope.html#close())
            will trigger the tasks scheduled to be ran.
            :::

            [Parameters:]{.paramLabel}
            :   `buildId` - unique identifier
                [`BuildId`](../../core/model/BuildId.html "class in com.facebook.buck.core.model")
                of a command that created a scope
            :   `blocking` - whether the current command should wait for
                tasks to finish on exit

        []{#shutdownNow()}

        -   #### shutdownNow

            ``` methodSignature
            public abstract void shutdownNow()
            ```

            ::: block
            Shut down manager, without waiting for tasks to finish.
            :::

        []{#shutdown(long,java.util.concurrent.TimeUnit)}

        -   #### shutdown

            ``` methodSignature
            public abstract void shutdown​(long timeout,
                                          TimeUnit units)
                                   throws InterruptedException
            ```

            ::: block
            Shut down manager, waiting until given timeout for tasks to
            finish.
            :::

            [Parameters:]{.paramLabel}
            :   `timeout` - timeout for tasks to finish
            :   `units` - units of timeout

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
