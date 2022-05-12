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
[Package]{.packageLabelInType} [com.facebook.buck.util](package-summary.html)
:::

## Interface ProcessExecutor {#interface-processexecutor .title title="Interface ProcessExecutor"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `ContextualProcessExecutor`, `DefaultProcessExecutor`

    ------------------------------------------------------------------------

        public interface ProcessExecutor
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Interface             | Description           |
        +=======================+=======================+=======================+
        | `static interface `   | `ProcessExec          | ::: block             |
        |                       | utor.LaunchedProcess` | Represents a running  |
        |                       |                       | process returned by   |
        |                       |                       | [`launchProcess(Pro   |
        |                       |                       | cessExecutorParams)`] |
        |                       |                       | (#launchProcess(com.f |
        |                       |                       | acebook.buck.util.Pro |
        |                       |                       | cessExecutorParams)). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `ProcessExecutor      | ::: block             |
        |                       | .LaunchedProcessImpl` | Wraps a               |
        |                       |                       | [`Process`](http      |
        |                       |                       | ://docs.oracle.com/ja |
        |                       |                       | vase/7/docs/api/java/ |
        |                       |                       | lang/Process.html?is- |
        |                       |                       | external=true "class  |
        |                       |                       | or interface in java. |
        |                       |                       | lang"){.externalLink} |
        |                       |                       | and exposes only its  |
        |                       |                       | I/O streams, so       |
        |                       |                       | callers have to pass  |
        |                       |                       | it back to this       |
        |                       |                       | class.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `Pr                   | ::: block             |
        |                       | ocessExecutor.Option` | Options for           |
        |                       |                       | [`laun                |
        |                       |                       | chAndExecute(ProcessE |
        |                       |                       | xecutorParams, Set, O |
        |                       |                       | ptional,  Optional, O |
        |                       |                       | ptional)`](#launchAnd |
        |                       |                       | Execute(com.facebook. |
        |                       |                       | buck.util.ProcessExec |
        |                       |                       | utorParams,java.util. |
        |                       |                       | Set,java.util.Optiona |
        |                       |                       | l,java.util.Optional, |
        |                       |                       | java.util.Optional)). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `Pr                   | ::: block             |
        |                       | ocessExecutor.Result` | Values from the       |
        |                       |                       | result of             |
        |                       |                       | [`laun                |
        |                       |                       | chAndExecute(ProcessE |
        |                       |                       | xecutorParams, Set,   |
        |                       |                       | Optional, Optional, O |
        |                       |                       | ptional)`](#launchAnd |
        |                       |                       | Execute(com.facebook. |
        |                       |                       | buck.util.ProcessExec |
        |                       |                       | utorParams,java.util. |
        |                       |                       | Set,java.util.Optiona |
        |                       |                       | l,java.util.Optional, |
        |                       |                       | java.util.Optional)). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `ProcessExecutor`     | `cloneWithOutp        | ::: block             |
        |                       | utStreams​(PrintStream | Makes a clone of this |
        |                       |  stdOutStream,        | process executor with |
        |                       |                 Print | the stdout and stderr |
        |                       | Stream stdErrStream)` | streams overridden.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `destroyLa            | ::: block             |
        |                       | unchedProcess​(Process | Terminates a process  |
        |                       | Executor.LaunchedProc | previously returned   |
        |                       | ess launchedProcess)` | by                    |
        |                       |                       | [`launchProcess(Pro   |
        |                       |                       | cessExecutorParams)`] |
        |                       |                       | (#launchProcess(com.f |
        |                       |                       | acebook.buck.util.Pro |
        |                       |                       | cessExecutorParams)). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `launc                | ::: block             |
        | ocessExecutor.Result` | hAndExecute​(ProcessEx | Convenience method    |
        |                       | ecutorParams params)` | for                   |
        |                       |                       | [`lau                 |
        |                       |                       | nchAndExecute(Process |
        |                       |                       | ExecutorParams, Set,  |
        |                       |                       | Optional, Optional,   |
        |                       |                       | Optional)`](#launchAn |
        |                       |                       | dExecute(com.facebook |
        |                       |                       | .buck.util.ProcessExe |
        |                       |                       | cutorParams,java.util |
        |                       |                       | .Set,java.util.Option |
        |                       |                       | al,java.util.Optional |
        |                       |                       | ,java.util.Optional)) |
        |                       |                       | with boolean values   |
        |                       |                       | set to `false` and    |
        |                       |                       | optional values set   |
        |                       |                       | to absent.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `                     |                       |
        | ocessExecutor.Result` | launchAndExecute​(Proc |                       |
        |                       | essExecutorParams par |                       |
        |                       | ams,                  |                       |
        |                       | com.google.common.col |                       |
        |                       | lect.ImmutableMap<Str |                       |
        |                       | ing,​String> context)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `laun                 |                       |
        | ocessExecutor.Result` | chAndExecute​(ProcessE |                       |
        |                       | xecutorParams params, |                       |
        |                       |                  com. |                       |
        |                       | google.common.collect |                       |
        |                       | .ImmutableMap<String, |                       |
        |                       | ​String> context,      |                       |
        |                       |             Set<Proce |                       |
        |                       | ssExecutor.Option> op |                       |
        |                       | tions,                |                       |
        |                       |   Optional<String> st |                       |
        |                       | din,                  |                       |
        |                       | Optional<Long> timeOu |                       |
        |                       | tMs,                  |                       |
        |                       | Optional<java.util.fu |                       |
        |                       | nction.Consumer<Proce |                       |
        |                       | ss>> timeOutHandler)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `launchAnd            | ::: block             |
        | ocessExecutor.Result` | Execute​(ProcessExecut | Launches then         |
        |                       | orParams params,      | executes a process    |
        |                       |             Set<Proce | with the specified    |
        |                       | ssExecutor.Option> op | `params`.             |
        |                       | tions,                | :::                   |
        |                       |   Optional<String> st |                       |
        |                       | din,                  |                       |
        |                       | Optional<Long> timeOu |                       |
        |                       | tMs,                  |                       |
        |                       | Optional<java.util.fu |                       |
        |                       | nction.Consumer<Proce |                       |
        |                       | ss>> timeOutHandler)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ProcessExec          | `la                   | ::: block             |
        | utor.LaunchedProcess` | unchProcess​(ProcessEx | Launches a            |
        |                       | ecutorParams params)` | [`Process`](http      |
        |                       |                       | ://docs.oracle.com/ja |
        |                       |                       | vase/7/docs/api/java/ |
        |                       |                       | lang/Process.html?is- |
        |                       |                       | external=true "class  |
        |                       |                       | or interface in java. |
        |                       |                       | lang"){.externalLink} |
        |                       |                       | given                 |
        |                       |                       | [`Pr                  |
        |                       |                       | ocessExecutorParams`] |
        |                       |                       | (ProcessExecutorParam |
        |                       |                       | s.html "class in com. |
        |                       |                       | facebook.buck.util"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ProcessExec          | `launchProcess​(P      |                       |
        | utor.LaunchedProcess` | rocessExecutorParams  |                       |
        |                       | params,               |                       |
        |                       | com.google.common.col |                       |
        |                       | lect.ImmutableMap<Str |                       |
        |                       | ing,​String> context)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `waitForLa            | ::: block             |
        | ocessExecutor.Result` | unchedProcess​(Process | Blocks while waiting  |
        |                       | Executor.LaunchedProc | for a process         |
        |                       | ess launchedProcess)` | previously returned   |
        |                       |                       | by                    |
        |                       |                       | [`launchProcess(Pr    |
        |                       |                       | ocessExecutorParams)` |
        |                       |                       | ](#launchProcess(com. |
        |                       |                       | facebook.buck.util.Pr |
        |                       |                       | ocessExecutorParams)) |
        |                       |                       | to exit, then returns |
        |                       |                       | the exit code of the  |
        |                       |                       | process.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `waitForLaunched      | ::: block             |
        | ocessExecutor.Result` | ProcessWithTimeout​(Pr | As                    |
        |                       | ocessExecutor.Launche | [`waitForLaunchedPr   |
        |                       | dProcess launchedProc | ocess(LaunchedProcess |
        |                       | ess,                  | )`](#waitForLaunchedP |
        |                       |                  long | rocess(com.facebook.b |
        |                       |  millis,              | uck.util.ProcessExecu |
        |                       |                       | tor.LaunchedProcess)) |
        |                       | Optional<java.util.fu | but with a timeout in |
        |                       | nction.Consumer<Proce | milliseconds.         |
        |                       | ss>> timeOutHandler)` | :::                   |
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

        []{#launchAndExecute(com.facebook.buck.util.ProcessExecutorParams)}

        -   #### launchAndExecute

            ``` methodSignature
            ProcessExecutor.Result launchAndExecute​(ProcessExecutorParams params)
                                             throws InterruptedException,
                                                    IOException
            ```

            ::: block
            Convenience method for
            [`launchAndExecute(ProcessExecutorParams, Set, Optional, Optional,  Optional)`](#launchAndExecute(com.facebook.buck.util.ProcessExecutorParams,java.util.Set,java.util.Optional,java.util.Optional,java.util.Optional))
            with boolean values set to `false` and optional values set
            to absent.
            :::

            [Throws:]{.throwsLabel}
            :   `InterruptedException`
            :   `IOException`

        []{#launchAndExecute(com.facebook.buck.util.ProcessExecutorParams,com.google.common.collect.ImmutableMap)}

        -   #### launchAndExecute

            ``` methodSignature
            ProcessExecutor.Result launchAndExecute​(ProcessExecutorParams params,
                                                    com.google.common.collect.ImmutableMap<String,​String> context)
                                             throws InterruptedException,
                                                    IOException
            ```

            [Throws:]{.throwsLabel}
            :   `InterruptedException`
            :   `IOException`

        []{#launchAndExecute(com.facebook.buck.util.ProcessExecutorParams,java.util.Set,java.util.Optional,java.util.Optional,java.util.Optional)}

        -   #### launchAndExecute

            ``` methodSignature
            ProcessExecutor.Result launchAndExecute​(ProcessExecutorParams params,
                                                    Set<ProcessExecutor.Option> options,
                                                    Optional<String> stdin,
                                                    Optional<Long> timeOutMs,
                                                    Optional<java.util.function.Consumer<Process>> timeOutHandler)
                                             throws InterruptedException,
                                                    IOException
            ```

            ::: block
            Launches then executes a process with the specified
            `params`.
            If `options` contains
            [`ProcessExecutor.Option.PRINT_STD_OUT`](ProcessExecutor.Option.html#PRINT_STD_OUT),
            then the stdout of the process will be written directly to
            the stdout passed to the constructor of this executor.
            Otherwise, the stdout of the process will be made available
            via
            [`ProcessExecutor.Result.getStdout()`](ProcessExecutor.Result.html#getStdout()).

            If `options` contains
            [`ProcessExecutor.Option.PRINT_STD_ERR`](ProcessExecutor.Option.html#PRINT_STD_ERR),
            then the stderr of the process will be written directly to
            the stderr passed to the constructor of this executor.
            Otherwise, the stderr of the process will be made available
            via
            [`ProcessExecutor.Result.getStderr()`](ProcessExecutor.Result.html#getStderr()).
            :::

            [Throws:]{.throwsLabel}
            :   `InterruptedException`
            :   `IOException`

        []{#launchAndExecute(com.facebook.buck.util.ProcessExecutorParams,com.google.common.collect.ImmutableMap,java.util.Set,java.util.Optional,java.util.Optional,java.util.Optional)}

        -   #### launchAndExecute

            ``` methodSignature
            ProcessExecutor.Result launchAndExecute​(ProcessExecutorParams params,
                                                    com.google.common.collect.ImmutableMap<String,​String> context,
                                                    Set<ProcessExecutor.Option> options,
                                                    Optional<String> stdin,
                                                    Optional<Long> timeOutMs,
                                                    Optional<java.util.function.Consumer<Process>> timeOutHandler)
                                             throws InterruptedException,
                                                    IOException
            ```

            [Throws:]{.throwsLabel}
            :   `InterruptedException`
            :   `IOException`

        []{#launchProcess(com.facebook.buck.util.ProcessExecutorParams)}

        -   #### launchProcess

            ``` methodSignature
            ProcessExecutor.LaunchedProcess launchProcess​(ProcessExecutorParams params)
                                                   throws IOException
            ```

            ::: block
            Launches a
            [`Process`](http://docs.oracle.com/javase/7/docs/api/java/lang/Process.html?is-external=true "class or interface in java.lang"){.externalLink}
            given
            [`ProcessExecutorParams`](ProcessExecutorParams.html "class in com.facebook.buck.util").
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#launchProcess(com.facebook.buck.util.ProcessExecutorParams,com.google.common.collect.ImmutableMap)}

        -   #### launchProcess

            ``` methodSignature
            ProcessExecutor.LaunchedProcess launchProcess​(ProcessExecutorParams params,
                                                          com.google.common.collect.ImmutableMap<String,​String> context)
                                                   throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#destroyLaunchedProcess(com.facebook.buck.util.ProcessExecutor.LaunchedProcess)}

        -   #### destroyLaunchedProcess

            ``` methodSignature
            void destroyLaunchedProcess​(ProcessExecutor.LaunchedProcess launchedProcess)
            ```

            ::: block
            Terminates a process previously returned by
            [`launchProcess(ProcessExecutorParams)`](#launchProcess(com.facebook.buck.util.ProcessExecutorParams)).
            :::

        []{#waitForLaunchedProcess(com.facebook.buck.util.ProcessExecutor.LaunchedProcess)}

        -   #### waitForLaunchedProcess

            ``` methodSignature
            ProcessExecutor.Result waitForLaunchedProcess​(ProcessExecutor.LaunchedProcess launchedProcess)
                                                   throws InterruptedException
            ```

            ::: block
            Blocks while waiting for a process previously returned by
            [`launchProcess(ProcessExecutorParams)`](#launchProcess(com.facebook.buck.util.ProcessExecutorParams))
            to exit, then returns the exit code of the process.
            After this method returns, the `launchedProcess` can no
            longer be passed to any methods of this object.
            :::

            [Throws:]{.throwsLabel}
            :   `InterruptedException`

        []{#waitForLaunchedProcessWithTimeout(com.facebook.buck.util.ProcessExecutor.LaunchedProcess,long,java.util.Optional)}

        -   #### waitForLaunchedProcessWithTimeout

            ``` methodSignature
            ProcessExecutor.Result waitForLaunchedProcessWithTimeout​(ProcessExecutor.LaunchedProcess launchedProcess,
                                                                     long millis,
                                                                     Optional<java.util.function.Consumer<Process>> timeOutHandler)
                                                              throws InterruptedException
            ```

            ::: block
            As
            [`waitForLaunchedProcess(LaunchedProcess)`](#waitForLaunchedProcess(com.facebook.buck.util.ProcessExecutor.LaunchedProcess))
            but with a timeout in milliseconds.
            :::

            [Throws:]{.throwsLabel}
            :   `InterruptedException`

        []{#cloneWithOutputStreams(java.io.PrintStream,java.io.PrintStream)}

        -   #### cloneWithOutputStreams

            ``` methodSignature
            ProcessExecutor cloneWithOutputStreams​(PrintStream stdOutStream,
                                                   PrintStream stdErrStream)
            ```

            ::: block
            Makes a clone of this process executor with the stdout and
            stderr streams overridden.
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
