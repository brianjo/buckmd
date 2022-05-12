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
[Package]{.packageLabelInType} [com.facebook.buck.cli](package-summary.html)
:::

## Interface Command {#interface-command .title title="Interface Command"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `AbstractCommand`, `AbstractContainerCommand`,
        `AbstractPerfCommand`, `AbstractQueryCommand`,
        `AuditActionGraphCommand`, `AuditAliasCommand`,
        `AuditBuildInfoCommand`, `AuditCellCommand`,
        `AuditClasspathCommand`, `AuditCommand`, `AuditConfigCommand`,
        `AuditDependenciesCommand`, `AuditFlavorsCommand`,
        `AuditIncludesCommand`, `AuditInputCommand`, `AuditMbrCommand`,
        `AuditMbrIsolationCommand`, `AuditModulesCommand`,
        `AuditOwnerCommand`, `AuditRulesCommand`,
        `AuditRuleTypeCommand`, `AuditRuleTypesCommand`,
        `AuditTestsCommand`, `BuckCommand`, `BuildCommand`,
        `CacheCommand`, `CacheDeleteCommand`, `CleanCommand`,
        `CommandWithPluginManager`, `DoctorCommand`, `FetchCommand`,
        `FixCommand`, `HelpCommand`, `InstallCommand`, `KillAllCommand`,
        `KillCommand`, `PerfActionGraphCommand`, `PerfCasCommand`,
        `PerfCasDownloadCommand`, `PerfCasUploadCommand`, `PerfCommand`,
        `PerfManifestCommand`, `PerfMbrCommand`,
        `PerfMbrPrepareRemoteExecutionCommand`,
        `PerfMbrSerializationCommand`, `PerfRuleKeyCommand`,
        `PerfStatCommand`, `ProjectCommand`, `PublishCommand`,
        `QueryCommand`, `RootCommand`, `RunCommand`, `ServerCommand`,
        `ServerStatusCommand`, `TargetsCommand`, `TestCommand`,
        `UnconfiguredQueryCommand`, `UninstallCommand`,
        `VerifyCachesCommand`

    ------------------------------------------------------------------------

        public interface Command
:::

::: summary
-   ::: {.section role="region"}
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
        | `or                   | `getPluginManager()`  |                       |
        | g.pf4j.PluginManager` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `g                    |                       |
        |                       | etShortDescription()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `                     |                       |
        | ogle.common.collect.I | getTargetPlatforms()` |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isReadOnly()`        |                       |
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
        | `void`                | `setPluginMana        |                       |
        |                       | ger​(org.pf4j.PluginMa |                       |
        |                       | nager pluginManager)` |                       |
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

        []{#run(com.facebook.buck.cli.CommandRunnerParams)}

        -   #### run

            ``` methodSignature
            ExitCode run​(CommandRunnerParams params)
                  throws Exception
            ```

            [Returns:]{.returnLabel}
            :   the appropriate exit code for the command

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#runHelp(java.io.PrintStream)}

        -   #### runHelp

            ``` methodSignature
            Optional<ExitCode> runHelp​(PrintStream stream)
            ```

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

        []{#isReadOnly()}

        -   #### isReadOnly

            ``` methodSignature
            boolean isReadOnly()
            ```

            [Returns:]{.returnLabel}
            :   whether the command doesn\'t modify the state of the
                filesystem

        []{#isSourceControlStatsGatheringEnabled()}

        -   #### isSourceControlStatsGatheringEnabled

            ``` methodSignature
            boolean isSourceControlStatsGatheringEnabled()
            ```

            [Returns:]{.returnLabel}
            :   whether we should gather source control stats while
                executing the command.

        []{#getShortDescription()}

        -   #### getShortDescription

            ``` methodSignature
            String getShortDescription()
            ```

        []{#getConfigOverrides(com.google.common.collect.ImmutableMap)}

        -   #### getConfigOverrides

            ``` methodSignature
            CellConfig getConfigOverrides​(com.google.common.collect.ImmutableMap<CellName,​AbsPath> cellMapping)
            ```

        []{#getLogConfig()}

        -   #### getLogConfig

            ``` methodSignature
            LogConfigSetup getLogConfig()
            ```

            [Returns:]{.returnLabel}
            :   how we want logging to be configured for the the
                command.

        []{#getEventListeners(java.util.Map,java.util.concurrent.ScheduledExecutorService)}

        -   #### getEventListeners

            ``` methodSignature
            Iterable<BuckEventListener> getEventListeners​(Map<ExecutorPool,​com.google.common.util.concurrent.ListeningExecutorService> executorPool,
                                                          ScheduledExecutorService scheduledExecutorService)
            ```

            ::: block
            If any of these listeners also extends Closeable, it will be
            closed by Main.
            :::

        []{#printUsage(java.io.PrintStream)}

        -   #### printUsage

            ``` methodSignature
            void printUsage​(PrintStream stream)
            ```

        []{#performsBuild()}

        -   #### performsBuild

            ``` methodSignature
            boolean performsBuild()
            ```

        []{#setPluginManager(org.pf4j.PluginManager)}

        -   #### setPluginManager

            ``` methodSignature
            void setPluginManager​(org.pf4j.PluginManager pluginManager)
            ```

        []{#getPluginManager()}

        -   #### getPluginManager

            ``` methodSignature
            org.pf4j.PluginManager getPluginManager()
            ```

        []{#getTargetPlatforms()}

        -   #### getTargetPlatforms

            ``` methodSignature
            com.google.common.collect.ImmutableList<String> getTargetPlatforms()
            ```

        []{#getHostPlatform()}

        -   #### getHostPlatform

            ``` methodSignature
            Optional<String> getHostPlatform()
            ```

        []{#createParsingContext(com.facebook.buck.core.cell.Cell,com.google.common.util.concurrent.ListeningExecutorService)}

        -   #### createParsingContext

            ``` methodSignature
            ParsingContext createParsingContext​(Cell cell,
                                                com.google.common.util.concurrent.ListeningExecutorService executor)
            ```

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
