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
[Package]{.packageLabelInType} [com.facebook.buck.cli](package-summary.html)
:::

## Class AbstractContainerCommand {#class-abstractcontainercommand .title title="Class AbstractContainerCommand"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.cli.CommandWithPluginManager](CommandWithPluginManager.html "class in com.facebook.buck.cli")

    -   -   com.facebook.buck.cli.AbstractContainerCommand

::: description
-   

    All Implemented Interfaces:
    :   `Command`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `AuditCommand`, `AuditMbrCommand`, `BuckCommand`,
        `PerfCasCommand`, `PerfCommand`, `PerfMbrCommand`,
        `ServerCommand`

    ------------------------------------------------------------------------

        public abstract class AbstractContainerCommand
        extends CommandWithPluginManager
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type    Field               Description
          -------------------- ------------------- -------------
          `protected String`   `commandArgsFile`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                    Description
          ------------------------------ -------------
          `AbstractContainerCommand()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `ParsingContext`      | `createParsingCon     | ::: block             |
        |                       | text​(Cell cell,       | Creates a basic       |
        |                       |                com.go | [                     |
        |                       | ogle.common.util.conc | `ParsingContext`](../ |
        |                       | urrent.ListeningExecu | parser/ParsingContext |
        |                       | torService executor)` | .html "class in com.f |
        |                       |                       | acebook.buck.parser") |
        |                       |                       | with some options     |
        |                       |                       | populated from        |
        |                       |                       | command\'s arguments. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CellConfig`          | `getCo                |                       |
        |                       | nfigOverrides​(com.goo |                       |
        |                       | gle.common.collect.Im |                       |
        |                       | mutableMap<CellName,​A |                       |
        |                       | bsPath> cellMapping)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `prote                | `getCont              |                       |
        | cted abstract String` | ainerCommandPrefix()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterabl              | `getEventL            | ::: block             |
        | e<BuckEventListener>` | isteners​(Map<Executor | If any of these       |
        |                       | Pool,​com.google.commo | listeners also        |
        |                       | n.util.concurrent.Lis | extends Closeable, it |
        |                       | teningExecutorService | will be closed by     |
        |                       | > executorPool,       | Main.                 |
        |                       |             Scheduled | :::                   |
        |                       | ExecutorService sched |                       |
        |                       | uledExecutorService)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getHostPlatform()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `LogConfigSetup`      | `getLogConfig()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected abstra     | `getSubcommand()`     |                       |
        | ct Optional<Command>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected String`    | `getSu                |                       |
        |                       | bcommandsFieldName()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `                     |                       |
        | ogle.common.collect.I | getTargetPlatforms()` |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isSourceControlSta   |                       |
        |                       | tsGatheringEnabled()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `performsBuild()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `printUsage           |                       |
        |                       | ​(PrintStream stream)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ExitCode`            | `run​(Command          |                       |
        |                       | RunnerParams params)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<ExitCode>`  | `runHelp              | ::: block             |
        |                       | ​(PrintStream stream)` | If the current        |
        |                       |                       | command is a help     |
        |                       |                       | command, run the      |
        |                       |                       | action to print out   |
        |                       |                       | the appropriate help  |
        |                       |                       | message.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.cli.CommandWithPluginManager}

            ### Methods inherited from class com.facebook.buck.cli.[CommandWithPluginManager](CommandWithPluginManager.html "class in com.facebook.buck.cli")

            `getPluginManager, setPluginManager`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.cli.Command}

            ### Methods inherited from interface com.facebook.buck.cli.[Command](Command.html "interface in com.facebook.buck.cli")

            `getShortDescription, isReadOnly`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#commandArgsFile}

        -   #### commandArgsFile

                @Nullable
                protected String commandArgsFile
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### AbstractContainerCommand

                public AbstractContainerCommand()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getSubcommandsFieldName()}

        -   #### getSubcommandsFieldName

            ``` methodSignature
            protected String getSubcommandsFieldName()
            ```

        []{#getSubcommand()}

        -   #### getSubcommand

            ``` methodSignature
            protected abstract Optional<Command> getSubcommand()
            ```

        []{#getContainerCommandPrefix()}

        -   #### getContainerCommandPrefix

            ``` methodSignature
            protected abstract String getContainerCommandPrefix()
            ```

        []{#runHelp(java.io.PrintStream)}

        -   #### runHelp

            ``` methodSignature
            public Optional<ExitCode> runHelp​(PrintStream stream)
            ```

            ::: block
            [Description copied from
            interface: `Command`]{.descfrmTypeLabel}
            :::

            ::: block
            If the current command is a help command, run the action to
            print out the appropriate help message.
            This is an optimization to avoid initializing everything in
            CommandRunnerParams, in order to return help strings
            quickly.
            :::

            [Parameters:]{.paramLabel}
            :   `stream` - stream to output the help text.

            [Returns:]{.returnLabel}
            :   The exit code of the command, if the command is a help
                request.

        []{#run(com.facebook.buck.cli.CommandRunnerParams)}

        -   #### run

            ``` methodSignature
            public ExitCode run​(CommandRunnerParams params)
                         throws Exception
            ```

            [Returns:]{.returnLabel}
            :   the appropriate exit code for the command

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#printUsage(java.io.PrintStream)}

        -   #### printUsage

            ``` methodSignature
            public void printUsage​(PrintStream stream)
            ```

        []{#getConfigOverrides(com.google.common.collect.ImmutableMap)}

        -   #### getConfigOverrides

            ``` methodSignature
            public CellConfig getConfigOverrides​(com.google.common.collect.ImmutableMap<CellName,​AbsPath> cellMapping)
            ```

        []{#getLogConfig()}

        -   #### getLogConfig

            ``` methodSignature
            public LogConfigSetup getLogConfig()
            ```

            [Returns:]{.returnLabel}
            :   how we want logging to be configured for the the
                command.

        []{#isSourceControlStatsGatheringEnabled()}

        -   #### isSourceControlStatsGatheringEnabled

            ``` methodSignature
            public boolean isSourceControlStatsGatheringEnabled()
            ```

            [Returns:]{.returnLabel}
            :   whether we should gather source control stats while
                executing the command.

        []{#getEventListeners(java.util.Map,java.util.concurrent.ScheduledExecutorService)}

        -   #### getEventListeners

            ``` methodSignature
            public Iterable<BuckEventListener> getEventListeners​(Map<ExecutorPool,​com.google.common.util.concurrent.ListeningExecutorService> executorPool,
                                                                 ScheduledExecutorService scheduledExecutorService)
            ```

            ::: block
            [Description copied from
            interface: `Command`]{.descfrmTypeLabel}
            :::

            ::: block
            If any of these listeners also extends Closeable, it will be
            closed by Main.
            :::

        []{#performsBuild()}

        -   #### performsBuild

            ``` methodSignature
            public boolean performsBuild()
            ```

        []{#getTargetPlatforms()}

        -   #### getTargetPlatforms

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getTargetPlatforms()
            ```

        []{#getHostPlatform()}

        -   #### getHostPlatform

            ``` methodSignature
            public Optional<String> getHostPlatform()
            ```

        []{#createParsingContext(com.facebook.buck.core.cell.Cell,com.google.common.util.concurrent.ListeningExecutorService)}

        -   #### createParsingContext

            ``` methodSignature
            public ParsingContext createParsingContext​(Cell cell,
                                                       com.google.common.util.concurrent.ListeningExecutorService executor)
            ```

            ::: block
            [Description copied from
            interface: `Command`]{.descfrmTypeLabel}
            :::

            ::: block
            Creates a basic
            [`ParsingContext`](../parser/ParsingContext.html "class in com.facebook.buck.parser")
            with some options populated from command\'s arguments.
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
