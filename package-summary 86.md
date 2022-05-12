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
-   Package
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Package com.facebook.buck.cli {#package-com.facebook.buck.cli .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [ActionGraphSerialize             | ::: block                         |
    | r.ActionGraphData](ActionGraphSer | Data object that is used to       |
    | ializer.ActionGraphData.html "int | serialize action graph            |
    | erface in com.facebook.buck.cli") | information into a file           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Command](Command.html "int       |                                   |
    | erface in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [MainRunner.KnownRuleType         |                                   |
    | sFactoryFactory](MainRunner.Known |                                   |
    | RuleTypesFactoryFactory.html "int |                                   |
    | erface in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [MainRunner.ParserAndCaches](Mai  | ::: block                         |
    | nRunner.ParserAndCaches.html "int | Struct for the multiple values    |
    | erface in com.facebook.buck.cli") | returned by                       |
    |                                   | [`MainRunner.getParser            |
    |                                   | AndCaches(java.util.Optional<com. |
    |                                   | facebook.nailgun.NGContext>, com. |
    |                                   | facebook.buck.io.watchman.Watchma |
    |                                   | nWatcher.FreshInstanceAction, com |
    |                                   | .facebook.buck.io.filesystem.Proj |
    |                                   | ectFilesystem, com.facebook.buck. |
    |                                   | core.config.BuckConfig, com.faceb |
    |                                   | ook.buck.io.watchman.Watchman, co |
    |                                   | m.facebook.buck.core.rules.knownt |
    |                                   | ypes.provider.KnownRuleTypesProvi |
    |                                   | der, com.facebook.buck.core.cell. |
    |                                   | Cell, com.facebook.buck.support.s |
    |                                   | tate.BuckGlobalState, com.faceboo |
    |                                   | k.buck.event.BuckEventBus, com.go |
    |                                   | ogle.common.collect.ImmutableMap< |
    |                                   | com.facebook.buck.util.concurrent |
    |                                   | .ExecutorPool, com.google.common. |
    |                                   | util.concurrent.ListeningExecutor |
    |                                   | Service>, com.facebook.buck.rules |
    |                                   | .keys.config.RuleKeyConfiguration |
    |                                   | , com.facebook.buck.util.Closeabl |
    |                                   | eMemoizedSupplier<com.facebook.bu |
    |                                   | ck.core.graph.transformation.exec |
    |                                   | utor.DepsAwareExecutor<? super co |
    |                                   | m.facebook.buck.core.graph.transf |
    |                                   | ormation.model.ComputeResult, ?>> |
    |                                   | , com.facebook.buck.io.Executable |
    |                                   | Finder, com.facebook.buck.core.pa |
    |                                   | rser.buildtargetparser.Unconfigur |
    |                                   | edBuildTargetViewFactory, com.fac |
    |                                   | ebook.buck.core.model.TargetConfi |
    |                                   | guration, com.facebook.buck.parse |
    |                                   | r.TargetSpecResolver)`](MainRunne |
    |                                   | r.html#getParserAndCaches(java.ut |
    |                                   | il.Optional,com.facebook.buck.io. |
    |                                   | watchman.WatchmanWatcher.FreshIns |
    |                                   | tanceAction,com.facebook.buck.io. |
    |                                   | filesystem.ProjectFilesystem,com. |
    |                                   | facebook.buck.core.config.BuckCon |
    |                                   | fig,com.facebook.buck.io.watchman |
    |                                   | .Watchman,com.facebook.buck.core. |
    |                                   | rules.knowntypes.provider.KnownRu |
    |                                   | leTypesProvider,com.facebook.buck |
    |                                   | .core.cell.Cell,com.facebook.buck |
    |                                   | .support.state.BuckGlobalState,co |
    |                                   | m.facebook.buck.event.BuckEventBu |
    |                                   | s,com.google.common.collect.Immut |
    |                                   | ableMap,com.facebook.buck.rules.k |
    |                                   | eys.config.RuleKeyConfiguration,c |
    |                                   | om.facebook.buck.util.CloseableMe |
    |                                   | moizedSupplier,com.facebook.buck. |
    |                                   | io.ExecutableFinder,com.facebook. |
    |                                   | buck.core.parser.buildtargetparse |
    |                                   | r.UnconfiguredBuildTargetViewFact |
    |                                   | ory,com.facebook.buck.core.model. |
    |                                   | TargetConfiguration,com.facebook. |
    |                                   | buck.parser.TargetSpecResolver)). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ProjectSubCommandFactory](P      |                                   |
    | rojectSubCommandFactory.html "int |                                   |
    | erface in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [Abstr                            |                                   |
    | actCommand](AbstractCommand.html  |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AbstractContainerComman          |                                   |
    | d](AbstractContainerCommand.html  |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AbstractPerfCommand](AbstractPe  | ::: block                         |
    | rfCommand.html "class in com.face | This is the core of our perf      |
    | book.buck.cli")\<CommandContext\> | commands, it handles the outer    |
    |                                   | prepare + loop and statistics     |
    |                                   | gathering.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AbstractQueryCo                  | ::: block                         |
    | mmand](AbstractQueryCommand.html  | Provides base functionality for   |
    | "class in com.facebook.buck.cli") | query commands.                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ActionGraphSerial                | ::: block                         |
    | izer](ActionGraphSerializer.html  | Serializer for ActionGraph.       |
    | "class in com.facebook.buck.cli") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AdbCommandLineOpt                |                                   |
    | ions](AdbCommandLineOptions.html  |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Ad                               | ::: block                         |
    | ditionalOptionsCmdLineParser](Add | `CmdLineParser` with nested       |
    | itionalOptionsCmdLineParser.html  | options via the                   |
    | "class in com.facebook.buck.cli") | [`AdditionalOptio                 |
    |                                   | ns`](AdditionalOptions.html "anno |
    |                                   | tation in com.facebook.buck.cli") |
    |                                   | annotation.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Additional                       |                                   |
    | OptionsSubCommandHandler](Additio |                                   |
    | nalOptionsSubCommandHandler.html  |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AuditActionGraphComma            | ::: block                         |
    | nd](AuditActionGraphCommand.html  | Command that dumps basic          |
    | "class in com.facebook.buck.cli") | information about the action      |
    |                                   | graph.                            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AuditAlia                        |                                   |
    | sCommand](AuditAliasCommand.html  |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AuditBuildInfoCom                | ::: block                         |
    | mand](AuditBuildInfoCommand.html  | A subcommand in \`buck audit\`    |
    | "class in com.facebook.buck.cli") | that shows information about Buck |
    |                                   | build.                            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AuditCe                          |                                   |
    | llCommand](AuditCellCommand.html  |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AuditClasspathCom                |                                   |
    | mand](AuditClasspathCommand.html  |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AuditCommand](AuditCommand.html  |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AuditConfig                      |                                   |
    | Command](AuditConfigCommand.html  |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AuditDependenciesComman          |                                   |
    | d](AuditDependenciesCommand.html  |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AuditFlavorsC                    | ::: block                         |
    | ommand](AuditFlavorsCommand.html  | List flavor domains for build     |
    | "class in com.facebook.buck.cli") | targets.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AuditIncludesCo                  | ::: block                         |
    | mmand](AuditIncludesCommand.html  | Evaluates a build file and prints |
    | "class in com.facebook.buck.cli") | out a list of build file          |
    |                                   | extensions included at parse      |
    |                                   | time.                             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AuditInpu                        |                                   |
    | tCommand](AuditInputCommand.html  |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Audit                            | ::: block                         |
    | MbrCommand](AuditMbrCommand.html  | Provides utilities for debugging  |
    | "class in com.facebook.buck.cli") | implementation of                 |
    |                                   | ModernBuildRule.                  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AuditMbrIsolationComman          | ::: block                         |
    | d](AuditMbrIsolationCommand.html  | Generates an isolation report.    |
    | "class in com.facebook.buck.cli") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AuditModulesC                    | ::: block                         |
    | ommand](AuditModulesCommand.html  | Prints the following information  |
    | "class in com.facebook.buck.cli") | about all modules: id, hash,      |
    |                                   | dependencies.                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AuditOwne                        |                                   |
    | rCommand](AuditOwnerCommand.html  |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AuditRule                        | ::: block                         |
    | sCommand](AuditRulesCommand.html  | Evaluates a build file and prints |
    | "class in com.facebook.buck.cli") | out an equivalent build file with |
    |                                   | all includes/macros expanded.     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AuditRuleTypeCo                  | ::: block                         |
    | mmand](AuditRuleTypeCommand.html  | Prints a requested rule type as a |
    | "class in com.facebook.buck.cli") | Python function with all          |
    |                                   | supported attributes.             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AuditRuleTypesCom                |                                   |
    | mand](AuditRuleTypesCommand.html  |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AuditTest                        |                                   |
    | sCommand](AuditTestsCommand.html  |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [BuckCommand](BuckCommand.html    |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [BuckDaemon](BuckDaemon.html      | ::: block                         |
    | "class in com.facebook.buck.cli") | The buckd process, which is the   |
    |                                   | long running nailgun server.      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuckQueryEnviro                  | ::: block                         |
    | nment](BuckQueryEnvironment.html  | The environment of a Buck query   |
    | "class in com.facebook.buck.cli") | that can evaluate queries to      |
    |                                   | produce a result.                 |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildCommand](BuildCommand.html  |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CacheCommand](CacheCommand.html  | ::: block                         |
    | "class in com.facebook.buck.cli") | A command for inspecting the      |
    |                                   | artifact cache.                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CacheDelete                      | ::: block                         |
    | Command](CacheDeleteCommand.html  | A command for deleting artifacts  |
    | "class in com.facebook.buck.cli") | from cache.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CleanCommand](CleanCommand.html  |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CleanCommandBuckCon              | ::: block                         |
    | fig](CleanCommandBuckConfig.html  | Configuration options used by     |
    | "class in com.facebook.buck.cli") | `buck clean` command.             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [C                                | ::: block                         |
    | ommandHelper](CommandHelper.html  | Utility class with print methods  |
    | "class in com.facebook.buck.cli") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Comm                             | ::: block                         |
    | andLineTargetNodeSpecParser](Comm | A helper wrapper over             |
    | andLineTargetNodeSpecParser.html  | [`B                               |
    | "class in com.facebook.buck.cli") | uildTargetMatcherTargetNodeParser |
    |                                   | `](../parser/spec/BuildTargetMatc |
    |                                   | herTargetNodeParser.html "class i |
    |                                   | n com.facebook.buck.parser.spec") |
    |                                   | to normalize user input before    |
    |                                   | parsing, resolve aliases and      |
    |                                   | validate that base path exists    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CommandRunner                    |                                   |
    | Params](CommandRunnerParams.html  |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CommandThreadMa                  | ::: block                         |
    | nager](CommandThreadManager.html  | Encapsulates a group of threads   |
    | "class in com.facebook.buck.cli") | which operate a                   |
    |                                   | `ListeningExecutorService`,       |
    |                                   | providing an                      |
    |                                   | [`AutoCloseable`](http            |
    |                                   | ://docs.oracle.com/javase/7/docs/ |
    |                                   | api/java/lang/AutoCloseable.html? |
    |                                   | is-external=true "class or interf |
    |                                   | ace in java.lang"){.externalLink} |
    |                                   | interface which waits for and     |
    |                                   | kills the threads on close.       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CommandWithPluginManage          | ::: block                         |
    | r](CommandWithPluginManager.html  | An implementation of              |
    | "class in com.facebook.buck.cli") | [`Command`](Command.html "int     |
    |                                   | erface in com.facebook.buck.cli") |
    |                                   | that allows keeping               |
    |                                   | `PluginManager`.                  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ConsumeAllOptionsHandle          |                                   |
    | r](ConsumeAllOptionsHandler.html  |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [DdmLibLogRedi                    | ::: block                         |
    | rector](DdmLibLogRedirector.html  | This is used to convert ddmlib\'s |
    | "class in com.facebook.buck.cli") | logging to ConsoleEvents to       |
    |                                   | interact correctly with           |
    |                                   | SuperConsole.                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [D                                |                                   |
    | octorCommand](DoctorCommand.html  |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Dot](Dot.html "clas              |                                   |
    | s in com.facebook.buck.cli")\<T\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [Do                               | ::: block                         |
    | t.Builder](Dot.Builder.html "clas | Builder class for Dot output      |
    | s in com.facebook.buck.cli")\<T\> | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Enviro                           | ::: block                         |
    | nmentOverrideOptionHandler](Envir | OptionHandler used for specifying |
    | onmentOverrideOptionHandler.html  | environment overrides.            |
    | "class in com.facebook.buck.cli") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [FetchCommand](FetchCommand.html  |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [FixCommand](FixCommand.html      | ::: block                         |
    | "class in com.facebook.buck.cli") | Attempts to fix errors            |
    |                                   | encountered in previous builds    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [FixComman                        | ::: block                         |
    | dHandler](FixCommandHandler.html  | Encapsulates the logic around     |
    | "class in com.facebook.buck.cli") | running \`buck fix\`.             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [GraphEngine                      | ::: block                         |
    | Factory](GraphEngineFactory.html  | Factory that creates              |
    | "class in com.facebook.buck.cli") | [`GraphTransforma                 |
    |                                   | tionEngine`](../core/graph/transf |
    |                                   | ormation/GraphTransformationEngin |
    |                                   | e.html "interface in com.facebook |
    |                                   | .buck.core.graph.transformation") |
    |                                   | for given parameters              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HangMonitor](HangMonitor.html    |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [                                 |                                   |
    | HangMonitor.AutoStartInstance](Ha |                                   |
    | ngMonitor.AutoStartInstance.html  |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [HeapDumper](HeapDumper.html      | ::: block                         |
    | "class in com.facebook.buck.cli") | Lightweight utility for capturing |
    |                                   | a heap dump programmatically.     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HelpCommand](HelpCommand.html    |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Ins                              | ::: block                         |
    | tallCommand](InstallCommand.html  | Command so a user can build and   |
    | "class in com.facebook.buck.cli") | install an APK.                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Kil                              | ::: block                         |
    | lAllCommand](KillAllCommand.html  | Buck subcommand to kill all buck  |
    | "class in com.facebook.buck.cli") | processes.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [KillCommand](KillCommand.html    |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [L                                |                                   |
    | abelSelector](LabelSelector.html  |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [MainRunner](MainRunner.html      | ::: block                         |
    | "class in com.facebook.buck.cli") | Responsible for running the       |
    |                                   | commands logic of buck after      |
    |                                   | [`MainWi                          |
    |                                   | thNailgun`](MainWithNailgun.html  |
    |                                   | "class in com.facebook.buck.cli") |
    |                                   | and                               |
    |                                   | [`MainWithoutN                    |
    |                                   | ailgun`](MainWithoutNailgun.html  |
    |                                   | "class in com.facebook.buck.cli") |
    |                                   | have completed the initial        |
    |                                   | bootstrapping of resources and    |
    |                                   | state.                            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [MainW                            | ::: block                         |
    | ithNailgun](MainWithNailgun.html  | The Main entry point for Nailgun  |
    | "class in com.facebook.buck.cli") | calls.                            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [MainWithout                      | ::: block                         |
    | Nailgun](MainWithoutNailgun.html  | This is the main entry point for  |
    | "class in com.facebook.buck.cli") | running buck without buckd.       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PairedStringOptionHandler        | ::: block                         |
    | ](PairedStringOptionHandler.html  | OptionHandler which takes exactly |
    | "class in com.facebook.buck.cli") | two strings next to each other,   |
    |                                   | and returns them as a Pair.       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [P                                |                                   |
    | athArguments](PathArguments.html  |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [PathUtils](PathUtils.html        | ::: block                         |
    | "class in com.facebook.buck.cli") | Path-related utility methods for  |
    |                                   | the command-line interface.       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PerfActionGraphComm              | ::: block                         |
    | and](PerfActionGraphCommand.html  | Tests performance of creating the |
    | "class in com.facebook.buck.cli") | action graph.                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Per                              | ::: block                         |
    | fCasCommand](PerfCasCommand.html  | Commands to test the performance  |
    | "class in com.facebook.buck.cli") | of cas upload and download.       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PerfCasDownloadComm              | ::: block                         |
    | and](PerfCasDownloadCommand.html  | Command to measure performance of |
    | "class in com.facebook.buck.cli") | cas downloads.                    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PerfCasUploadCo                  | ::: block                         |
    | mmand](PerfCasUploadCommand.html  | Command to measure performance of |
    | "class in com.facebook.buck.cli") | cas uploads.                      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PerfCommand](PerfCommand.html    | ::: block                         |
    | "class in com.facebook.buck.cli") | The PerfCommand is for targeted   |
    |                                   | tests of the performance of buck  |
    |                                   | components.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PerfManifestC                    | ::: block                         |
    | ommand](PerfManifestCommand.html  | Tests performance of creating and |
    | "class in com.facebook.buck.cli") | manipulating                      |
    |                                   | [`Manifest`](.                    |
    |                                   | ./core/build/engine/manifest/Mani |
    |                                   | fest.html "class in com.facebook. |
    |                                   | buck.core.build.engine.manifest") |
    |                                   | objects.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PerfManifestCommand.Context](    | ::: block                         |
    | PerfManifestCommand.Context.html  | Our test context.                 |
    | "class in com.facebook.buck.cli") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Per                              | ::: block                         |
    | fMbrCommand](PerfMbrCommand.html  | Container for                     |
    | "class in com.facebook.buck.cli") | [`Modern                          |
    |                                   | BuildRule`](../rules/modern/Moder |
    |                                   | nBuildRule.html "class in com.fac |
    |                                   | ebook.buck.rules.modern")-related |
    |                                   | perf tests.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PerfMbrPrepare                   | ::: block                         |
    | RemoteExecutionCommand](PerfMbrPr | Tests performance of preparing    |
    | epareRemoteExecutionCommand.html  | MBR rules for remote execution    |
    | "class in com.facebook.buck.cli") | (primarily merkle tree node       |
    |                                   | computations).                    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PerfMbrSerializationCommand](    | ::: block                         |
    | PerfMbrSerializationCommand.html  | Tests performance of serializing  |
    | "class in com.facebook.buck.cli") | MBR rules.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PerfRuleKey                      | ::: block                         |
    | Command](PerfRuleKeyCommand.html  | Tests performance of computing    |
    | "class in com.facebook.buck.cli") | the various rulekeys.             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PerfS                            | ::: block                         |
    | tatCommand](PerfStatCommand.html  | Some human readable statistics of |
    | "class in com.facebook.buck.cli") | running buck process.             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Pro                              |                                   |
    | jectCommand](ProjectCommand.html  |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ProjectGeneratorParameters]      |                                   |
    | (ProjectGeneratorParameters.html  |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ProjectSu                        |                                   |
    | bCommand](ProjectSubCommand.html  |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Pub                              |                                   |
    | lishCommand](PublishCommand.html  |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [QueryCommand](QueryCommand.html  | ::: block                         |
    | "class in com.facebook.buck.cli") | Buck subcommand which relies on   |
    |                                   | the configured target graph,      |
    |                                   | whose nodes\' selects are         |
    |                                   | evaluated                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [QueryMultiSetOptionHandler]      | ::: block                         |
    | (QueryMultiSetOptionHandler.html  | A simple option handler whose     |
    | "class in com.facebook.buck.cli") | main job is to not freak out when |
    |                                   | it sees \`\--\`, which is used by |
    |                                   | QueryCommand as a separator       |
    |                                   | between different sets.           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ResolveAlia                      | ::: block                         |
    | sHelper](ResolveAliasHelper.html  | Helper class with functionality   |
    | "class in com.facebook.buck.cli") | to resolve alias in \`targets\`   |
    |                                   | command.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RootCommand](RootCommand.html    |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [RunCommand](RunCommand.html      |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [S                                |                                   |
    | erverCommand](ServerCommand.html  |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ServerStatusC                    |                                   |
    | ommand](ServerStatusCommand.html  |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [SingleStringSetOptionHandler](S  | ::: block                         |
    | ingleStringSetOptionHandler.html  | An option handler that allows an  |
    | "class in com.facebook.buck.cli") | option to be specified multiple   |
    |                                   | times and coaleced into a set of  |
    |                                   | strings, but only allows one      |
    |                                   | value for each specification of   |
    |                                   | the option.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [StringSetOptionHand              | ::: block                         |
    | ler](StringSetOptionHandler.html  | `OptionHandler` that collects     |
    | "class in com.facebook.buck.cli") | multiple arguments passed to an   |
    |                                   | option in a                       |
    |                                   | [`S                               |
    |                                   | et`](http://docs.oracle.com/javas |
    |                                   | e/7/docs/api/java/util/Set.html?i |
    |                                   | s-external=true "class or interfa |
    |                                   | ce in java.util"){.externalLink}. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [SystemI                          | ::: block                         |
    | nfoLogger](SystemInfoLogger.html  | Utility class for logging useful  |
    | "class in com.facebook.buck.cli") | system information.               |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Ta                               |                                   |
    | rgetDeviceCommandLineOptions](Tar |                                   |
    | getDeviceCommandLineOptions.html  |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Tar                              |                                   |
    | getsCommand](TargetsCommand.html  |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [TestCommand](TestCommand.html    |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [TestCommand.CoverageRe           | ::: block                         |
    | portFormatsHandler](TestCommand.C | args4j does not support parsing   |
    | overageReportFormatsHandler.html  | repeated (or delimiter separated) |
    | "class in com.facebook.buck.cli") | Enums by default.                 |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [TestRunning](TestRunning.html    | ::: block                         |
    | "class in com.facebook.buck.cli") | Utility class for running tests   |
    |                                   | from                              |
    |                                   | [`TestRule`](../core/test/ru      |
    |                                   | le/TestRule.html "interface in co |
    |                                   | m.facebook.buck.core.test.rule")s |
    |                                   | which have been built.            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [TestSelectorO                    |                                   |
    | ptions](TestSelectorOptions.html  |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [T                                |                                   |
    | estSelectorOptions.TestSelectorsO |                                   |
    | ptionHandler](TestSelectorOptions |                                   |
    | .TestSelectorsOptionHandler.html  |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Thri                             | ::: block                         |
    | ftOutput](ThriftOutput.html "clas | Class responsible for             |
    | s in com.facebook.buck.cli")\<T\> | serialization of                  |
    |                                   | DirectedAcyclicGraph into Thrift  |
    |                                   | output format                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ThriftOutput.Builder             | ::: block                         |
    | ](ThriftOutput.Builder.html "clas | Builder class for Thrift output   |
    | s in com.facebook.buck.cli")\<T\> | :::                               |
    +-----------------------------------+-----------------------------------+
    | [UnconfiguredQueryComman          | ::: block                         |
    | d](UnconfiguredQueryCommand.html  | Buck subcommand which relies on   |
    | "class in com.facebook.buck.cli") | the unconfigured target graph,    |
    |                                   | whose nodes contain all the       |
    |                                   | information inside selects        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Uninsta                          |                                   |
    | llCommand](UninstallCommand.html  |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Uninstal                         |                                   |
    | lCommand.UninstallOptions](Uninst |                                   |
    | allCommand.UninstallOptions.html  |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Verbo                            |                                   |
    | sityParser](VerbosityParser.html  |                                   |
    | "class in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [VerifyCachesC                    | ::: block                         |
    | ommand](VerifyCachesCommand.html  | Verify the contents of our        |
    | "class in com.facebook.buck.cli") | FileHashCache.                    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Enum                              | Description                       |
    +===================================+===================================+
    | [Abstrac                          | ::: block                         |
    | tQueryCommand.OutputFormat](Abstr | Enum with values for              |
    | actQueryCommand.OutputFormat.html | \`\--output-format\` CLI          |
    |  "enum in com.facebook.buck.cli") | parameter                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AbstractQueryCo                  | ::: block                         |
    | mmand.SortOutputFormat](AbstractQ | Sort Output format.               |
    | ueryCommand.SortOutputFormat.html | :::                               |
    |  "enum in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AbstractQueryComm                | ::: block                         |
    | and.WhichQueryCommand](AbstractQu | Which of \*query commands was     |
    | eryCommand.WhichQueryCommand.html | invoked                           |
    |  "enum in com.facebook.buck.cli") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Dot.                             | ::: block                         |
    | OutputOrder](Dot.OutputOrder.html | How to print the dot graph.       |
    |  "enum in com.facebook.buck.cli") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Projec                           |                                   |
    | tTestsMode](ProjectTestsMode.html |                                   |
    |  "enum in com.facebook.buck.cli") |                                   |
    +-----------------------------------+-----------------------------------+

    : Enum Summary[ ]{.tabEnd}

-   
      Exception                                                                                                                      Description
      ------------------------------------------------------------------------------------------------------------------------------ -------------
      [BuildCommand.ActionGraphCreationException](BuildCommand.ActionGraphCreationException.html "class in com.facebook.buck.cli")    

      : Exception Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Annotation Type                   | Description                       |
    +===================================+===================================+
    | [AdditionalOpti                   | ::: block                         |
    | ons](AdditionalOptions.html "anno | If this annotation is used on a   |
    | tation in com.facebook.buck.cli") | field in one of the `..Options`   |
    |                                   | classes (e.g.                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Annotation Types Summary[ ]{.tabEnd}
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../index.html)
-   Package
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

[]{#skip.navbar.bottom}
:::
