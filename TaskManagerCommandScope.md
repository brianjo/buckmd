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

## Class TaskManagerCommandScope {#class-taskmanagercommandscope .title title="Class TaskManagerCommandScope"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.support.bgtasks.TaskManagerCommandScope

::: description
-   

    All Implemented Interfaces:
    :   `Scope`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class TaskManagerCommandScope
        extends Object
        implements Scope

    ::: block
    Scope class for client-side use of
    [`BackgroundTaskManager`](BackgroundTaskManager.html "class in com.facebook.buck.support.bgtasks").
    Scope handles scheduling and start/end notifications for individual
    builds, passing tasks/notifications to the manager for scheduling.
    This lives for the duration of the command, and will schedule the
    tasks to be run on [`close()`](#close()). [`close()`](#close())
    should only occur on command exit.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.util.Scope}

            ### Fields inherited from interface com.facebook.buck.util.[Scope](../../util/Scope.html "interface in com.facebook.buck.util")

            `NOOP`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                                                                                                 Description
          -------------- ------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `protected `   `TaskManagerCommandScope​(BackgroundTaskManager manager,                        BuildId buildId,                        boolean blocking)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `close()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `B                    | `getManager()`        |                       |
        | ackgroundTaskManager` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `schedule​(Bac         | ::: block             |
        |                       | kgroundTask<?> task)` | Schedule a task to be |
        |                       |                       | run by a              |
        |                       |                       | [`BackgroundTas       |
        |                       |                       | kManager`](Background |
        |                       |                       | TaskManager.html "cla |
        |                       |                       | ss in com.facebook.bu |
        |                       |                       | ck.support.bgtasks"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `sche                 | ::: block             |
        |                       | dule​(com.google.commo | Schedule a list of    |
        |                       | n.collect.ImmutableLi | tasks to be run by a  |
        |                       | st<? extends Backgrou | [`BackgroundTas       |
        |                       | ndTask<?>> taskList)` | kManager`](Background |
        |                       |                       | TaskManager.html "cla |
        |                       |                       | ss in com.facebook.bu |
        |                       |                       | ck.support.bgtasks"). |
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.support.bgtasks.BackgroundTaskManager,com.facebook.buck.core.model.BuildId,boolean)}

        -   #### TaskManagerCommandScope

                protected TaskManagerCommandScope​(BackgroundTaskManager manager,
                                                  BuildId buildId,
                                                  boolean blocking)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#schedule(com.facebook.buck.support.bgtasks.BackgroundTask)}

        -   #### schedule

            ``` methodSignature
            public void schedule​(BackgroundTask<?> task)
            ```

            ::: block
            Schedule a task to be run by a
            [`BackgroundTaskManager`](BackgroundTaskManager.html "class in com.facebook.buck.support.bgtasks").
            :::

            [Parameters:]{.paramLabel}
            :   `task` - task to be run

        []{#schedule(com.google.common.collect.ImmutableList)}

        -   #### schedule

            ``` methodSignature
            public void schedule​(com.google.common.collect.ImmutableList<? extends BackgroundTask<?>> taskList)
            ```

            ::: block
            Schedule a list of tasks to be run by a
            [`BackgroundTaskManager`](BackgroundTaskManager.html "class in com.facebook.buck.support.bgtasks").
            :::

            [Parameters:]{.paramLabel}
            :   `taskList` - list of tasks to be run

        []{#getManager()}

        -   #### getManager

            ``` methodSignature
            public BackgroundTaskManager getManager()
            ```

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `Scope`
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
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
