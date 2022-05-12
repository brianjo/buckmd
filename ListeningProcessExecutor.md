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
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.util](package-summary.html)
:::

## Class ListeningProcessExecutor {#class-listeningprocessexecutor .title title="Class ListeningProcessExecutor"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.ListeningProcessExecutor

::: description
-   

    ------------------------------------------------------------------------

        public class ListeningProcessExecutor
        extends Object

    ::: block
    Replacement for
    [`ProcessBuilder`](http://docs.oracle.com/javase/7/docs/api/java/lang/ProcessBuilder.html?is-external=true "class or interface in java.lang"){.externalLink}
    which provides an asynchronous callback interface to notify the
    caller on a background thread when a process starts, performs I/O,
    or exits.
    Unlike
    [`ProcessExecutor`](ProcessExecutor.html "interface in com.facebook.buck.util"),
    this does not automatically forward output to
    [`Console`](Console.html "class in com.facebook.buck.util")
    formatted with ANSI escapes.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static interface `   | `ListeningProcessExec | ::: block             |
        |                       | utor.LaunchedProcess` | Represents a process  |
        |                       |                       | which was launched by |
        |                       |                       | a                     |
        |                       |                       | [`Listenin            |
        |                       |                       | gProcessExecutor`](Li |
        |                       |                       | steningProcessExecuto |
        |                       |                       | r.html "class in com. |
        |                       |                       | facebook.buck.util"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static interface `   | `ListeningProcessExec | ::: block             |
        |                       | utor.ProcessListener` | Callback API to       |
        |                       |                       | notify the caller on  |
        |                       |                       | a background thread   |
        |                       |                       | when a process        |
        |                       |                       | starts, exits, has    |
        |                       |                       | stdout or stderr      |
        |                       |                       | bytes to read, or is  |
        |                       |                       | ready to receive      |
        |                       |                       | bytes on stdin.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                    Description
          ------------------------------ -------------
          `ListeningProcessExecutor()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `destroyPro           | ::: block             |
        |                       | cess​(ListeningProcess | Destroys a process.   |
        |                       | Executor.LaunchedProc | :::                   |
        |                       | ess process,          |                       |
        |                       |       boolean force)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ListeningProcessExec | `lau                  | ::: block             |
        | utor.LaunchedProcess` | nchProcess​(ProcessExe | Launches a process    |
        |                       | cutorParams params,   | and asynchronously    |
        |                       |             Listening | sends notifications   |
        |                       | ProcessExecutor.Proce | to `listener` on a    |
        |                       | ssListener listener)` | background thread     |
        |                       |                       | when the process      |
        |                       |                       | starts, has I/O, or   |
        |                       |                       | exits.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `wa                   | ::: block             |
        |                       | itForProcess​(Listenin | Blocks the calling    |
        |                       | gProcessExecutor.Laun | thread until the      |
        |                       | chedProcess process)` | process exits.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `                     | ::: block             |
        |                       | waitForProcess​(Listen | Blocks the calling    |
        |                       | ingProcessExecutor.La | thread until either   |
        |                       | unchedProcess process | the process exits or  |
        |                       | ,               long  | the timeout expires,  |
        |                       | timeout,              | whichever is first.   |
        |                       |   TimeUnit timeUnit)` | :::                   |
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

        []{#<init>()}

        -   #### ListeningProcessExecutor

                public ListeningProcessExecutor()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#launchProcess(com.facebook.buck.util.ProcessExecutorParams,com.facebook.buck.util.ListeningProcessExecutor.ProcessListener)}

        -   #### launchProcess

            ``` methodSignature
            public ListeningProcessExecutor.LaunchedProcess launchProcess​(ProcessExecutorParams params,
                                                                          ListeningProcessExecutor.ProcessListener listener)
                                                                   throws IOException
            ```

            ::: block
            Launches a process and asynchronously sends notifications to
            `listener` on a background thread when the process starts,
            has I/O, or exits.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#waitForProcess(com.facebook.buck.util.ListeningProcessExecutor.LaunchedProcess,long,java.util.concurrent.TimeUnit)}

        -   #### waitForProcess

            ``` methodSignature
            public int waitForProcess​(ListeningProcessExecutor.LaunchedProcess process,
                                      long timeout,
                                      TimeUnit timeUnit)
                               throws InterruptedException
            ```

            ::: block
            Blocks the calling thread until either the process exits or
            the timeout expires, whichever is first.
            :::

            [Returns:]{.returnLabel}
            :   `Integer.MIN_VALUE` if the timeout expired or the
                process failed to start, or the exit code of the process
                otherwise.

            [Throws:]{.throwsLabel}
            :   `InterruptedException`

        []{#waitForProcess(com.facebook.buck.util.ListeningProcessExecutor.LaunchedProcess)}

        -   #### waitForProcess

            ``` methodSignature
            public int waitForProcess​(ListeningProcessExecutor.LaunchedProcess process)
                               throws InterruptedException,
                                      IOException
            ```

            ::: block
            Blocks the calling thread until the process exits.
            :::

            [Returns:]{.returnLabel}
            :   the exit code of the process.

            [Throws:]{.throwsLabel}
            :   `IOException` - if the process failed to start.
            :   `InterruptedException`

        []{#destroyProcess(com.facebook.buck.util.ListeningProcessExecutor.LaunchedProcess,boolean)}

        -   #### destroyProcess

            ``` methodSignature
            public void destroyProcess​(ListeningProcessExecutor.LaunchedProcess process,
                                       boolean force)
            ```

            ::: block
            Destroys a process. If `force` is `true`, then forcibly
            destroys the process in a way it cannot ignore.
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
-   [Nested](#nested.class.summary) \| 
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
