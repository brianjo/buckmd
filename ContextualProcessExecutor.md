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

## Class ContextualProcessExecutor {#class-contextualprocessexecutor .title title="Class ContextualProcessExecutor"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.ContextualProcessExecutor

::: description
-   

    All Implemented Interfaces:
    :   `ProcessExecutor`

    ------------------------------------------------------------------------

        public class ContextualProcessExecutor
        extends Object
        implements ProcessExecutor
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.util.ProcessExecutor}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.util.[ProcessExecutor](ProcessExecutor.html "interface in com.facebook.buck.util")

            `ProcessExecutor.LaunchedProcess, ProcessExecutor.LaunchedProcessImpl, ProcessExecutor.Option, ProcessExecutor.Result`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                     Description
          ----------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `ContextualProcessExecutor​(ProcessExecutor delegate,                          com.google.common.collect.ImmutableMap<String,​String> context)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `ProcessExecutor`     | `cloneWithOutputStre  | ::: block             |
        |                       | ams​(PrintStream newSt | Makes a clone of this |
        |                       | dOutStream,           | process executor with |
        |                       |              PrintStr | the stdout and stderr |
        |                       | eam newStdErrStream)` | streams overridden.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `destroyLa            | ::: block             |
        |                       | unchedProcess​(Process | Terminates a process  |
        |                       | Executor.LaunchedProc | previously returned   |
        |                       | ess launchedProcess)` | by                    |
        |                       |                       | [`ProcessExec         |
        |                       |                       | utor.launchProcess(Pr |
        |                       |                       | ocessExecutorParams)` |
        |                       |                       | ](ProcessExecutor.htm |
        |                       |                       | l#launchProcess(com.f |
        |                       |                       | acebook.buck.util.Pro |
        |                       |                       | cessExecutorParams)). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `getContext()`        |                       |
        | ommon.collect.Immutab |                       |                       |
        | leMap<String,​String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ProcessExecutor`     | `getDelegate()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `launc                | ::: block             |
        | ocessExecutor.Result` | hAndExecute​(ProcessEx | Convenience method    |
        |                       | ecutorParams params)` | for                   |
        |                       |                       | [`ProcessExecutor.la  |
        |                       |                       | unchAndExecute(Proces |
        |                       |                       | sExecutorParams, Set, |
        |                       |                       |  Optional, Optional,  |
        |                       |                       |  Optional)`](ProcessE |
        |                       |                       | xecutor.html#launchAn |
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
        |                       |                       | [`ProcessExe          |
        |                       |                       | cutor.launchProcess(P |
        |                       |                       | rocessExecutorParams) |
        |                       |                       | `](ProcessExecutor.ht |
        |                       |                       | ml#launchProcess(com. |
        |                       |                       | facebook.buck.util.Pr |
        |                       |                       | ocessExecutorParams)) |
        |                       |                       | to exit, then returns |
        |                       |                       | the exit code of the  |
        |                       |                       | process.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `waitForLaunched      | ::: block             |
        | ocessExecutor.Result` | ProcessWithTimeout​(Pr | As                    |
        |                       | ocessExecutor.Launche | [`ProcessExec         |
        |                       | dProcess launchedProc | utor.waitForLaunchedP |
        |                       | ess,                  | rocess(LaunchedProces |
        |                       |                  long | s)`](ProcessExecutor. |
        |                       |  millis,              | html#waitForLaunchedP |
        |                       |                       | rocess(com.facebook.b |
        |                       | Optional<java.util.fu | uck.util.ProcessExecu |
        |                       | nction.Consumer<Proce | tor.LaunchedProcess)) |
        |                       | ss>> timeOutHandler)` | but with a timeout in |
        |                       |                       | milliseconds.         |
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

        []{#<init>(com.facebook.buck.util.ProcessExecutor,com.google.common.collect.ImmutableMap)}

        -   #### ContextualProcessExecutor

                public ContextualProcessExecutor​(ProcessExecutor delegate,
                                                 com.google.common.collect.ImmutableMap<String,​String> context)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getContext()}

        -   #### getContext

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​String> getContext()
            ```

        []{#getDelegate()}

        -   #### getDelegate

            ``` methodSignature
            public ProcessExecutor getDelegate()
            ```

        []{#launchProcess(com.facebook.buck.util.ProcessExecutorParams)}

        -   #### launchProcess

            ``` methodSignature
            public ProcessExecutor.LaunchedProcess launchProcess​(ProcessExecutorParams params)
                                                          throws IOException
            ```

            ::: block
            [Description copied from
            interface: `ProcessExecutor`]{.descfrmTypeLabel}
            :::

            ::: block
            Launches a
            [`Process`](http://docs.oracle.com/javase/7/docs/api/java/lang/Process.html?is-external=true "class or interface in java.lang"){.externalLink}
            given
            [`ProcessExecutorParams`](ProcessExecutorParams.html "class in com.facebook.buck.util").
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `launchProcess` in interface `ProcessExecutor`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#launchProcess(com.facebook.buck.util.ProcessExecutorParams,com.google.common.collect.ImmutableMap)}

        -   #### launchProcess

            ``` methodSignature
            public ProcessExecutor.LaunchedProcess launchProcess​(ProcessExecutorParams params,
                                                                 com.google.common.collect.ImmutableMap<String,​String> context)
                                                          throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `launchProcess` in interface `ProcessExecutor`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#launchAndExecute(com.facebook.buck.util.ProcessExecutorParams)}

        -   #### launchAndExecute

            ``` methodSignature
            public ProcessExecutor.Result launchAndExecute​(ProcessExecutorParams params)
                                                    throws InterruptedException,
                                                           IOException
            ```

            ::: block
            [Description copied from
            interface: `ProcessExecutor`]{.descfrmTypeLabel}
            :::

            ::: block
            Convenience method for
            [`ProcessExecutor.launchAndExecute(ProcessExecutorParams, Set, Optional, Optional,  Optional)`](ProcessExecutor.html#launchAndExecute(com.facebook.buck.util.ProcessExecutorParams,java.util.Set,java.util.Optional,java.util.Optional,java.util.Optional))
            with boolean values set to `false` and optional values set
            to absent.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `launchAndExecute` in interface `ProcessExecutor`

            [Throws:]{.throwsLabel}
            :   `InterruptedException`
            :   `IOException`

        []{#launchAndExecute(com.facebook.buck.util.ProcessExecutorParams,com.google.common.collect.ImmutableMap)}

        -   #### launchAndExecute

            ``` methodSignature
            public ProcessExecutor.Result launchAndExecute​(ProcessExecutorParams params,
                                                           com.google.common.collect.ImmutableMap<String,​String> context)
                                                    throws InterruptedException,
                                                           IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `launchAndExecute` in interface `ProcessExecutor`

            [Throws:]{.throwsLabel}
            :   `InterruptedException`
            :   `IOException`

        []{#launchAndExecute(com.facebook.buck.util.ProcessExecutorParams,java.util.Set,java.util.Optional,java.util.Optional,java.util.Optional)}

        -   #### launchAndExecute

            ``` methodSignature
            public ProcessExecutor.Result launchAndExecute​(ProcessExecutorParams params,
                                                           Set<ProcessExecutor.Option> options,
                                                           Optional<String> stdin,
                                                           Optional<Long> timeOutMs,
                                                           Optional<java.util.function.Consumer<Process>> timeOutHandler)
                                                    throws InterruptedException,
                                                           IOException
            ```

            ::: block
            [Description copied from
            interface: `ProcessExecutor`]{.descfrmTypeLabel}
            :::

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

            [Specified by:]{.overrideSpecifyLabel}
            :   `launchAndExecute` in interface `ProcessExecutor`

            [Throws:]{.throwsLabel}
            :   `InterruptedException`
            :   `IOException`

        []{#launchAndExecute(com.facebook.buck.util.ProcessExecutorParams,com.google.common.collect.ImmutableMap,java.util.Set,java.util.Optional,java.util.Optional,java.util.Optional)}

        -   #### launchAndExecute

            ``` methodSignature
            public ProcessExecutor.Result launchAndExecute​(ProcessExecutorParams params,
                                                           com.google.common.collect.ImmutableMap<String,​String> context,
                                                           Set<ProcessExecutor.Option> options,
                                                           Optional<String> stdin,
                                                           Optional<Long> timeOutMs,
                                                           Optional<java.util.function.Consumer<Process>> timeOutHandler)
                                                    throws InterruptedException,
                                                           IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `launchAndExecute` in interface `ProcessExecutor`

            [Throws:]{.throwsLabel}
            :   `InterruptedException`
            :   `IOException`

        []{#waitForLaunchedProcess(com.facebook.buck.util.ProcessExecutor.LaunchedProcess)}

        -   #### waitForLaunchedProcess

            ``` methodSignature
            public ProcessExecutor.Result waitForLaunchedProcess​(ProcessExecutor.LaunchedProcess launchedProcess)
                                                          throws InterruptedException
            ```

            ::: block
            [Description copied from
            interface: `ProcessExecutor`]{.descfrmTypeLabel}
            :::

            ::: block
            Blocks while waiting for a process previously returned by
            [`ProcessExecutor.launchProcess(ProcessExecutorParams)`](ProcessExecutor.html#launchProcess(com.facebook.buck.util.ProcessExecutorParams))
            to exit, then returns the exit code of the process.
            After this method returns, the `launchedProcess` can no
            longer be passed to any methods of this object.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `waitForLaunchedProcess` in interface `ProcessExecutor`

            [Throws:]{.throwsLabel}
            :   `InterruptedException`

        []{#waitForLaunchedProcessWithTimeout(com.facebook.buck.util.ProcessExecutor.LaunchedProcess,long,java.util.Optional)}

        -   #### waitForLaunchedProcessWithTimeout

            ``` methodSignature
            public ProcessExecutor.Result waitForLaunchedProcessWithTimeout​(ProcessExecutor.LaunchedProcess launchedProcess,
                                                                            long millis,
                                                                            Optional<java.util.function.Consumer<Process>> timeOutHandler)
                                                                     throws InterruptedException
            ```

            ::: block
            [Description copied from
            interface: `ProcessExecutor`]{.descfrmTypeLabel}
            :::

            ::: block
            As
            [`ProcessExecutor.waitForLaunchedProcess(LaunchedProcess)`](ProcessExecutor.html#waitForLaunchedProcess(com.facebook.buck.util.ProcessExecutor.LaunchedProcess))
            but with a timeout in milliseconds.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `waitForLaunchedProcessWithTimeout` in
                interface `ProcessExecutor`

            [Throws:]{.throwsLabel}
            :   `InterruptedException`

        []{#destroyLaunchedProcess(com.facebook.buck.util.ProcessExecutor.LaunchedProcess)}

        -   #### destroyLaunchedProcess

            ``` methodSignature
            public void destroyLaunchedProcess​(ProcessExecutor.LaunchedProcess launchedProcess)
            ```

            ::: block
            [Description copied from
            interface: `ProcessExecutor`]{.descfrmTypeLabel}
            :::

            ::: block
            Terminates a process previously returned by
            [`ProcessExecutor.launchProcess(ProcessExecutorParams)`](ProcessExecutor.html#launchProcess(com.facebook.buck.util.ProcessExecutorParams)).
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `destroyLaunchedProcess` in interface `ProcessExecutor`

        []{#cloneWithOutputStreams(java.io.PrintStream,java.io.PrintStream)}

        -   #### cloneWithOutputStreams

            ``` methodSignature
            public ProcessExecutor cloneWithOutputStreams​(PrintStream newStdOutStream,
                                                          PrintStream newStdErrStream)
            ```

            ::: block
            [Description copied from
            interface: `ProcessExecutor`]{.descfrmTypeLabel}
            :::

            ::: block
            Makes a clone of this process executor with the stdout and
            stderr streams overridden.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `cloneWithOutputStreams` in interface `ProcessExecutor`
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
