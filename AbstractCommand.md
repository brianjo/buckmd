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

## Class AbstractCommand {#class-abstractcommand .title title="Class AbstractCommand"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.cli.CommandWithPluginManager](CommandWithPluginManager.html "class in com.facebook.buck.cli")

    -   -   com.facebook.buck.cli.AbstractCommand

::: description
-   

    All Implemented Interfaces:
    :   `Command`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `AbstractPerfCommand`, `AbstractQueryCommand`,
        `AuditActionGraphCommand`, `AuditAliasCommand`,
        `AuditBuildInfoCommand`, `AuditCellCommand`,
        `AuditClasspathCommand`, `AuditConfigCommand`,
        `AuditDependenciesCommand`, `AuditFlavorsCommand`,
        `AuditIncludesCommand`, `AuditInputCommand`,
        `AuditMbrIsolationCommand`, `AuditModulesCommand`,
        `AuditOwnerCommand`, `AuditRulesCommand`,
        `AuditRuleTypeCommand`, `AuditRuleTypesCommand`,
        `AuditTestsCommand`, `BuildCommand`, `CacheCommand`,
        `CacheDeleteCommand`, `CleanCommand`, `DoctorCommand`,
        `FixCommand`, `HelpCommand`, `KillAllCommand`, `KillCommand`,
        `PerfCasDownloadCommand`, `PerfCasUploadCommand`,
        `PerfStatCommand`, `ProjectCommand`, `RootCommand`,
        `RunCommand`, `ServerStatusCommand`, `TargetsCommand`,
        `UninstallCommand`, `VerifyCachesCommand`

    ------------------------------------------------------------------------

        public abstract class AbstractCommand
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

          Constructor           Description
          --------------------- -------------
          `AbstractCommand()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected void`      | `addCommandSpecificCo | ::: block             |
        |                       | nfigOverrides​(CellCon | Injection point for   |
        |                       | fig.Builder builder)` | commands to add       |
        |                       |                       | config overrides.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected com.google | `convertA             | ::: block             |
        | .common.collect.Immut | rgumentsToBuildTarget | Converts target       |
        | ableSet<BuildTarget>` | s​(CommandRunnerParams | arguments to fully    |
        |                       |  params,              | qualified form        |
        |                       |                   Lis | (including resolving  |
        |                       | t<String> arguments)` | aliases, resolving    |
        |                       |                       | the implicit package  |
        |                       |                       | target, etc).         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
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
        | `String`              | `                     |                       |
        |                       | getCommandArgsFile()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `pr                   | `getCo                |                       |
        | otected com.facebook. | mmandLineBuildTargetN |                       |
        | buck.cli.CommandLineB | ormalizer​(Cell rootCe |                       |
        | uildTargetNormalizer` | ll,                   |                       |
        |                       |                   Pat |                       |
        |                       | h clientWorkingDirect |                       |
        |                       | ory,                  |                       |
        |                       |                    Bu |                       |
        |                       | ckConfig buckConfig)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ConcurrencyLimit`    | `g                    |                       |
        |                       | etConcurrencyLimit​(Bu |                       |
        |                       | ckConfig buckConfig)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `CellConfig`          | `getCo                |                       |
        |                       | nfigOverrides​(com.goo |                       |
        |                       | gle.common.collect.Im |                       |
        |                       | mutableMap<CellName,​A |                       |
        |                       | bsPath> cellMapping)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getEna               |                       |
        |                       | bleParserProfiling()` |                       |
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
        | `Optional<Path>`      | `g                    |                       |
        |                       | etEventsOutputPath()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getExcludeI          |                       |
        |                       | ncompatibleTargets()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protec               | `g                    |                       |
        | ted ExecutionContext` | etExecutionContext()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected Exec       | `getExecutionC        |                       |
        | utionContext.Builder` | ontextBuilder​(Command |                       |
        |                       | RunnerParams params)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getHostPlatform()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `LogConfigSetup`      | `getLogConfig()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `                     |                       |
        | ogle.common.collect.I | getTargetPlatforms()` |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `handleExcepti        | ::: block             |
        |                       | on​(org.kohsuke.args4j | Handle                |
        |                       | .CmdLineException e)` | CmdLineException when |
        |                       |                       | calling               |
        |                       |                       | parseArguments()      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected void`      | `handleExceptio       | ::: block             |
        |                       | n​(org.kohsuke.args4j. | Print error message   |
        |                       | CmdLineException e,   | when there are        |
        |                       |               String  | unknown options       |
        |                       | printedErrorMessage)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isNoCache()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `is                   |                       |
        |                       | ReuseCurrentConfig()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isSourceControlSta   |                       |
        |                       | tsGatheringEnabled()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected            | `matchBuildTargetsWit | ::: block             |
        | com.google.common.col | hLabelsFromSpecs​(com. | Returns a set of      |
        | lect.ImmutableSet<Bui | google.common.collect | [`Bu                  |
        | ldTargetWithOutputs>` | .ImmutableList<Target | ildTargetWithOutputs` |
        |                       | NodeSpec> specs,      | ](../core/model/Build |
        |                       |                       | TargetWithOutputs.htm |
        |                       |            Set<BuildT | l "class in com.faceb |
        |                       | arget> buildTargets)` | ook.buck.core.model") |
        |                       |                       | instances by matching |
        |                       |                       | the given             |
        |                       |                       | [`B                   |
        |                       |                       | uildTarget`](../core/ |
        |                       |                       | model/BuildTarget.htm |
        |                       |                       | l "class in com.faceb |
        |                       |                       | ook.buck.core.model") |
        |                       |                       | instances with the    |
        |                       |                       | given                 |
        |                       |                       | [`TargetNodeSpe       |
        |                       |                       | c`](../parser/spec/Ta |
        |                       |                       | rgetNodeSpec.html "in |
        |                       |                       | terface in com.facebo |
        |                       |                       | ok.buck.parser.spec") |
        |                       |                       | instances, and        |
        |                       |                       | applying any          |
        |                       |                       | [`O                   |
        |                       |                       | utputLabel`](../core/ |
        |                       |                       | model/OutputLabel.htm |
        |                       |                       | l "class in com.faceb |
        |                       |                       | ook.buck.core.model") |
        |                       |                       | instances to the      |
        |                       |                       | matching              |
        |                       |                       | [`B                   |
        |                       |                       | uildTarget`](../core/ |
        |                       |                       | model/BuildTarget.htm |
        |                       |                       | l "class in com.faceb |
        |                       |                       | ook.buck.core.model") |
        |                       |                       | instances.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `performsBuild()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected Closeable` | `prepareExe           |                       |
        |                       | cutionContext​(Command |                       |
        |                       | RunnerParams params)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `printUsage           |                       |
        |                       | ​(PrintStream stream)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected void`      | `                     | ::: block             |
        |                       | printWarning​(CommandR | Helper for printing   |
        |                       | unnerParams params,   | warnings to the       |
        |                       |            String s)` | console.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected void`      | `printWarning         | ::: block             |
        |                       | ​(CommandRunnerParams  | Helper for printing   |
        |                       | params,             S | warnings to the       |
        |                       | tring format,         | console.              |
        |                       |      Object... args)` | :::                   |
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
        | `abstract ExitCode`   | `r                    |                       |
        |                       | unWithoutHelp​(Command |                       |
        |                       | RunnerParams params)` |                       |
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

        -   #### AbstractCommand

                public AbstractCommand()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getLogConfig()}

        -   #### getLogConfig

            ``` methodSignature
            public LogConfigSetup getLogConfig()
            ```

            [Returns:]{.returnLabel}
            :   how we want logging to be configured for the the
                command.

        []{#isNoCache()}

        -   #### isNoCache

            ``` methodSignature
            public boolean isNoCache()
            ```

            [Returns:]{.returnLabel}
            :   {code true} if the `[cache]` in `.buckconfig` should be
                ignored.

        []{#isReuseCurrentConfig()}

        -   #### isReuseCurrentConfig

            ``` methodSignature
            public boolean isReuseCurrentConfig()
            ```

        []{#getCommandArgsFile()}

        -   #### getCommandArgsFile

            ``` methodSignature
            @Nullable
            public String getCommandArgsFile()
            ```

        []{#getEventsOutputPath()}

        -   #### getEventsOutputPath

            ``` methodSignature
            public Optional<Path> getEventsOutputPath()
            ```

        []{#handleException(org.kohsuke.args4j.CmdLineException)}

        -   #### handleException

            ``` methodSignature
            public void handleException​(org.kohsuke.args4j.CmdLineException e)
                                 throws org.kohsuke.args4j.CmdLineException
            ```

            ::: block
            Handle CmdLineException when calling parseArguments()
            :::

            [Throws:]{.throwsLabel}
            :   `org.kohsuke.args4j.CmdLineException`

        []{#handleException(org.kohsuke.args4j.CmdLineException,java.lang.String)}

        -   #### handleException

            ``` methodSignature
            protected void handleException​(org.kohsuke.args4j.CmdLineException e,
                                           String printedErrorMessage)
                                    throws org.kohsuke.args4j.CmdLineException
            ```

            ::: block
            Print error message when there are unknown options
            :::

            [Throws:]{.throwsLabel}
            :   `org.kohsuke.args4j.CmdLineException`

        []{#printUsage(java.io.PrintStream)}

        -   #### printUsage

            ``` methodSignature
            public void printUsage​(PrintStream stream)
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
            public final ExitCode run​(CommandRunnerParams params)
                               throws Exception
            ```

            [Returns:]{.returnLabel}
            :   the appropriate exit code for the command

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#prepareExecutionContext(com.facebook.buck.cli.CommandRunnerParams)}

        -   #### prepareExecutionContext

            ``` methodSignature
            protected Closeable prepareExecutionContext​(CommandRunnerParams params)
            ```

        []{#printWarning(com.facebook.buck.cli.CommandRunnerParams,java.lang.String,java.lang.Object...)}

        -   #### printWarning

            ``` methodSignature
            protected void printWarning​(CommandRunnerParams params,
                                        String format,
                                        Object... args)
            ```

            ::: block
            Helper for printing warnings to the console.
            :::

        []{#printWarning(com.facebook.buck.cli.CommandRunnerParams,java.lang.String)}

        -   #### printWarning

            ``` methodSignature
            protected void printWarning​(CommandRunnerParams params,
                                        String s)
            ```

            ::: block
            Helper for printing warnings to the console.
            :::

        []{#runWithoutHelp(com.facebook.buck.cli.CommandRunnerParams)}

        -   #### runWithoutHelp

            ``` methodSignature
            public abstract ExitCode runWithoutHelp​(CommandRunnerParams params)
                                             throws Exception
            ```

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#getCommandLineBuildTargetNormalizer(com.facebook.buck.core.cell.Cell,java.nio.file.Path,com.facebook.buck.core.config.BuckConfig)}

        -   #### getCommandLineBuildTargetNormalizer

            ``` methodSignature
            protected com.facebook.buck.cli.CommandLineBuildTargetNormalizer getCommandLineBuildTargetNormalizer​(Cell rootCell,
                                                                                                                 Path clientWorkingDirectory,
                                                                                                                 BuckConfig buckConfig)
            ```

        []{#getEnableParserProfiling()}

        -   #### getEnableParserProfiling

            ``` methodSignature
            public boolean getEnableParserProfiling()
            ```

        []{#matchBuildTargetsWithLabelsFromSpecs(com.google.common.collect.ImmutableList,java.util.Set)}

        -   #### matchBuildTargetsWithLabelsFromSpecs

            ``` methodSignature
            protected com.google.common.collect.ImmutableSet<BuildTargetWithOutputs> matchBuildTargetsWithLabelsFromSpecs​(com.google.common.collect.ImmutableList<TargetNodeSpec> specs,
                                                                                                                          Set<BuildTarget> buildTargets)
            ```

            ::: block
            Returns a set of
            [`BuildTargetWithOutputs`](../core/model/BuildTargetWithOutputs.html "class in com.facebook.buck.core.model")
            instances by matching the given
            [`BuildTarget`](../core/model/BuildTarget.html "class in com.facebook.buck.core.model")
            instances with the given
            [`TargetNodeSpec`](../parser/spec/TargetNodeSpec.html "interface in com.facebook.buck.parser.spec")
            instances, and applying any
            [`OutputLabel`](../core/model/OutputLabel.html "class in com.facebook.buck.core.model")
            instances to the matching
            [`BuildTarget`](../core/model/BuildTarget.html "class in com.facebook.buck.core.model")
            instances. Applies the default label if a given build target
            cannot find a matching spec.
            :::

        []{#getExecutionContext()}

        -   #### getExecutionContext

            ``` methodSignature
            protected ExecutionContext getExecutionContext()
            ```

        []{#getExecutionContextBuilder(com.facebook.buck.cli.CommandRunnerParams)}

        -   #### getExecutionContextBuilder

            ``` methodSignature
            protected ExecutionContext.Builder getExecutionContextBuilder​(CommandRunnerParams params)
            ```

        []{#getConcurrencyLimit(com.facebook.buck.core.config.BuckConfig)}

        -   #### getConcurrencyLimit

            ``` methodSignature
            public ConcurrencyLimit getConcurrencyLimit​(BuckConfig buckConfig)
            ```

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

        []{#getExcludeIncompatibleTargets()}

        -   #### getExcludeIncompatibleTargets

            ``` methodSignature
            public boolean getExcludeIncompatibleTargets()
            ```

        []{#convertArgumentsToBuildTargets(com.facebook.buck.cli.CommandRunnerParams,java.util.List)}

        -   #### convertArgumentsToBuildTargets

            ``` methodSignature
            protected com.google.common.collect.ImmutableSet<BuildTarget> convertArgumentsToBuildTargets​(CommandRunnerParams params,
                                                                                                         List<String> arguments)
            ```

            ::: block
            Converts target arguments to fully qualified form (including
            resolving aliases, resolving the implicit package target,
            etc).
            :::

        []{#getConfigOverrides(com.google.common.collect.ImmutableMap)}

        -   #### getConfigOverrides

            ``` methodSignature
            public CellConfig getConfigOverrides​(com.google.common.collect.ImmutableMap<CellName,​AbsPath> cellMapping)
            ```

        []{#addCommandSpecificConfigOverrides(com.facebook.buck.core.cell.CellConfig.Builder)}

        -   #### addCommandSpecificConfigOverrides

            ``` methodSignature
            protected void addCommandSpecificConfigOverrides​(CellConfig.Builder builder)
            ```

            ::: block
            Injection point for commands to add config overrides. Adding
            anything here will likely invalidate the \@{link
            BuckGlobalState} and so it should be used extremely
            sparingly.
            :::

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
