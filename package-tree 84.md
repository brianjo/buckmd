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
-   Tree
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
# Hierarchy For Package com.facebook.buck.cli {#hierarchy-for-package-com.facebook.buck.cli .title}

[Package Hierarchies:]{.packageHierarchyLabel}

-   [All Packages](../../../../overview-tree.html)
:::

::: contentContainer
::: {.section role="region"}
## Class Hierarchy {#class-hierarchy title="Class Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   com.google.common.util.concurrent.AbstractScheduledService
        (implements com.google.common.util.concurrent.Service)
        -   com.facebook.buck.cli.[[HangMonitor]{.typeNameLink}](HangMonitor.html "class in com.facebook.buck.cli")
    -   com.facebook.buck.cli.[[ActionGraphSerializer]{.typeNameLink}](ActionGraphSerializer.html "class in com.facebook.buck.cli")
    -   com.facebook.buck.cli.[[AdbCommandLineOptions]{.typeNameLink}](AdbCommandLineOptions.html "class in com.facebook.buck.cli")
    -   com.facebook.buck.cli.[[BuckDaemon]{.typeNameLink}](BuckDaemon.html "class in com.facebook.buck.cli")
    -   com.facebook.buck.cli.[[BuckQueryEnvironment]{.typeNameLink}](BuckQueryEnvironment.html "class in com.facebook.buck.cli")
        (implements
        com.facebook.buck.query.[QueryEnvironment](../query/QueryEnvironment.html "interface in com.facebook.buck.query")\<NODE_TYPE\>)
    -   com.facebook.buck.cli.[[CleanCommandBuckConfig]{.typeNameLink}](CleanCommandBuckConfig.html "class in com.facebook.buck.cli")
        (implements
        com.facebook.buck.core.config.[ConfigView](../core/config/ConfigView.html "interface in com.facebook.buck.core.config")\<T\>)
    -   org.kohsuke.args4j.CmdLineParser
        -   com.facebook.buck.cli.[[AdditionalOptionsCmdLineParser]{.typeNameLink}](AdditionalOptionsCmdLineParser.html "class in com.facebook.buck.cli")
    -   com.facebook.buck.cli.[[CommandHelper]{.typeNameLink}](CommandHelper.html "class in com.facebook.buck.cli")
    -   com.facebook.buck.cli.[[CommandLineTargetNodeSpecParser]{.typeNameLink}](CommandLineTargetNodeSpecParser.html "class in com.facebook.buck.cli")
    -   com.facebook.buck.cli.[[CommandRunnerParams]{.typeNameLink}](CommandRunnerParams.html "class in com.facebook.buck.cli")
    -   com.facebook.buck.cli.[[CommandThreadManager]{.typeNameLink}](CommandThreadManager.html "class in com.facebook.buck.cli")
        (implements
        java.lang.[AutoCloseable](http://docs.oracle.com/javase/7/docs/api/java/lang/AutoCloseable.html?is-external=true "class or interface in java.lang"){.externalLink})
    -   com.facebook.buck.cli.[[CommandWithPluginManager]{.typeNameLink}](CommandWithPluginManager.html "class in com.facebook.buck.cli")
        (implements
        com.facebook.buck.cli.[Command](Command.html "interface in com.facebook.buck.cli"))
        -   com.facebook.buck.cli.[[AbstractCommand]{.typeNameLink}](AbstractCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[AbstractPerfCommand]{.typeNameLink}](AbstractPerfCommand.html "class in com.facebook.buck.cli")\<CommandContext\>
                -   com.facebook.buck.cli.[[PerfActionGraphCommand]{.typeNameLink}](PerfActionGraphCommand.html "class in com.facebook.buck.cli")
                -   com.facebook.buck.cli.[[PerfManifestCommand]{.typeNameLink}](PerfManifestCommand.html "class in com.facebook.buck.cli")
                -   com.facebook.buck.cli.[[PerfMbrPrepareRemoteExecutionCommand]{.typeNameLink}](PerfMbrPrepareRemoteExecutionCommand.html "class in com.facebook.buck.cli")
                -   com.facebook.buck.cli.[[PerfMbrSerializationCommand]{.typeNameLink}](PerfMbrSerializationCommand.html "class in com.facebook.buck.cli")
                -   com.facebook.buck.cli.[[PerfRuleKeyCommand]{.typeNameLink}](PerfRuleKeyCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[AbstractQueryCommand]{.typeNameLink}](AbstractQueryCommand.html "class in com.facebook.buck.cli")
                -   com.facebook.buck.cli.[[QueryCommand]{.typeNameLink}](QueryCommand.html "class in com.facebook.buck.cli")
                -   com.facebook.buck.cli.[[UnconfiguredQueryCommand]{.typeNameLink}](UnconfiguredQueryCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[AuditActionGraphCommand]{.typeNameLink}](AuditActionGraphCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[AuditAliasCommand]{.typeNameLink}](AuditAliasCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[AuditBuildInfoCommand]{.typeNameLink}](AuditBuildInfoCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[AuditCellCommand]{.typeNameLink}](AuditCellCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[AuditClasspathCommand]{.typeNameLink}](AuditClasspathCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[AuditConfigCommand]{.typeNameLink}](AuditConfigCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[AuditDependenciesCommand]{.typeNameLink}](AuditDependenciesCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[AuditFlavorsCommand]{.typeNameLink}](AuditFlavorsCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[AuditIncludesCommand]{.typeNameLink}](AuditIncludesCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[AuditInputCommand]{.typeNameLink}](AuditInputCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[AuditMbrIsolationCommand]{.typeNameLink}](AuditMbrIsolationCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[AuditModulesCommand]{.typeNameLink}](AuditModulesCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[AuditOwnerCommand]{.typeNameLink}](AuditOwnerCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[AuditRulesCommand]{.typeNameLink}](AuditRulesCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[AuditRuleTypeCommand]{.typeNameLink}](AuditRuleTypeCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[AuditRuleTypesCommand]{.typeNameLink}](AuditRuleTypesCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[AuditTestsCommand]{.typeNameLink}](AuditTestsCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[BuildCommand]{.typeNameLink}](BuildCommand.html "class in com.facebook.buck.cli")
                -   com.facebook.buck.cli.[[FetchCommand]{.typeNameLink}](FetchCommand.html "class in com.facebook.buck.cli")
                -   com.facebook.buck.cli.[[InstallCommand]{.typeNameLink}](InstallCommand.html "class in com.facebook.buck.cli")
                -   com.facebook.buck.cli.[[PublishCommand]{.typeNameLink}](PublishCommand.html "class in com.facebook.buck.cli")
                -   com.facebook.buck.cli.[[TestCommand]{.typeNameLink}](TestCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[CacheCommand]{.typeNameLink}](CacheCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[CacheDeleteCommand]{.typeNameLink}](CacheDeleteCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[CleanCommand]{.typeNameLink}](CleanCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[DoctorCommand]{.typeNameLink}](DoctorCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[FixCommand]{.typeNameLink}](FixCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[HelpCommand]{.typeNameLink}](HelpCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[KillAllCommand]{.typeNameLink}](KillAllCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[KillCommand]{.typeNameLink}](KillCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[PerfCasDownloadCommand]{.typeNameLink}](PerfCasDownloadCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[PerfCasUploadCommand]{.typeNameLink}](PerfCasUploadCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[PerfStatCommand]{.typeNameLink}](PerfStatCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[ProjectCommand]{.typeNameLink}](ProjectCommand.html "class in com.facebook.buck.cli")
                (implements
                com.facebook.buck.support.cli.args.[PluginBasedCommand](../support/cli/args/PluginBasedCommand.html "interface in com.facebook.buck.support.cli.args"))
            -   com.facebook.buck.cli.[[RootCommand]{.typeNameLink}](RootCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[RunCommand]{.typeNameLink}](RunCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[ServerStatusCommand]{.typeNameLink}](ServerStatusCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[TargetsCommand]{.typeNameLink}](TargetsCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[UninstallCommand]{.typeNameLink}](UninstallCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[VerifyCachesCommand]{.typeNameLink}](VerifyCachesCommand.html "class in com.facebook.buck.cli")
        -   com.facebook.buck.cli.[[AbstractContainerCommand]{.typeNameLink}](AbstractContainerCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[AuditCommand]{.typeNameLink}](AuditCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[AuditMbrCommand]{.typeNameLink}](AuditMbrCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[BuckCommand]{.typeNameLink}](BuckCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[PerfCasCommand]{.typeNameLink}](PerfCasCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[PerfCommand]{.typeNameLink}](PerfCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[PerfMbrCommand]{.typeNameLink}](PerfMbrCommand.html "class in com.facebook.buck.cli")
            -   com.facebook.buck.cli.[[ServerCommand]{.typeNameLink}](ServerCommand.html "class in com.facebook.buck.cli")
    -   com.facebook.buck.cli.[[DdmLibLogRedirector]{.typeNameLink}](DdmLibLogRedirector.html "class in com.facebook.buck.cli")
    -   com.facebook.buck.cli.[[Dot]{.typeNameLink}](Dot.html "class in com.facebook.buck.cli")\<T\>
    -   com.facebook.buck.cli.[[Dot.Builder]{.typeNameLink}](Dot.Builder.html "class in com.facebook.buck.cli")\<T\>
    -   com.facebook.buck.cli.[[FixCommandHandler]{.typeNameLink}](FixCommandHandler.html "class in com.facebook.buck.cli")
    -   com.facebook.buck.cli.[[GraphEngineFactory]{.typeNameLink}](GraphEngineFactory.html "class in com.facebook.buck.cli")
    -   com.facebook.buck.cli.[[HangMonitor.AutoStartInstance]{.typeNameLink}](HangMonitor.AutoStartInstance.html "class in com.facebook.buck.cli")
    -   com.facebook.buck.cli.[[HeapDumper]{.typeNameLink}](HeapDumper.html "class in com.facebook.buck.cli")
    -   com.facebook.buck.cli.[[LabelSelector]{.typeNameLink}](LabelSelector.html "class in com.facebook.buck.cli")
    -   com.facebook.buck.cli.[[MainRunner]{.typeNameLink}](MainRunner.html "class in com.facebook.buck.cli")
    -   com.facebook.buck.cli.[[MainWithNailgun]{.typeNameLink}](MainWithNailgun.html "class in com.facebook.buck.cli")
    -   com.facebook.buck.cli.[[MainWithoutNailgun]{.typeNameLink}](MainWithoutNailgun.html "class in com.facebook.buck.cli")
    -   org.kohsuke.args4j.spi.OptionHandler\<T\>
        -   com.facebook.buck.cli.[[ConsumeAllOptionsHandler]{.typeNameLink}](ConsumeAllOptionsHandler.html "class in com.facebook.buck.cli")
        -   org.kohsuke.args4j.spi.MapOptionHandler
            -   com.facebook.buck.cli.[[EnvironmentOverrideOptionHandler]{.typeNameLink}](EnvironmentOverrideOptionHandler.html "class in com.facebook.buck.cli")
        -   com.facebook.buck.cli.[[PairedStringOptionHandler]{.typeNameLink}](PairedStringOptionHandler.html "class in com.facebook.buck.cli")
        -   com.facebook.buck.cli.[[QueryMultiSetOptionHandler]{.typeNameLink}](QueryMultiSetOptionHandler.html "class in com.facebook.buck.cli")
        -   com.facebook.buck.cli.[[SingleStringSetOptionHandler]{.typeNameLink}](SingleStringSetOptionHandler.html "class in com.facebook.buck.cli")
        -   com.facebook.buck.cli.[[StringSetOptionHandler]{.typeNameLink}](StringSetOptionHandler.html "class in com.facebook.buck.cli")
        -   org.kohsuke.args4j.spi.SubCommandHandler
            -   com.facebook.buck.cli.[[AdditionalOptionsSubCommandHandler]{.typeNameLink}](AdditionalOptionsSubCommandHandler.html "class in com.facebook.buck.cli")
        -   com.facebook.buck.cli.[[TestCommand.CoverageReportFormatsHandler]{.typeNameLink}](TestCommand.CoverageReportFormatsHandler.html "class in com.facebook.buck.cli")
        -   com.facebook.buck.cli.[[TestSelectorOptions.TestSelectorsOptionHandler]{.typeNameLink}](TestSelectorOptions.TestSelectorsOptionHandler.html "class in com.facebook.buck.cli")
    -   com.facebook.buck.cli.[[PathArguments]{.typeNameLink}](PathArguments.html "class in com.facebook.buck.cli")
    -   com.facebook.buck.cli.[[PathUtils]{.typeNameLink}](PathUtils.html "class in com.facebook.buck.cli")
    -   com.facebook.buck.cli.[[PerfManifestCommand.Context]{.typeNameLink}](PerfManifestCommand.Context.html "class in com.facebook.buck.cli")
    -   com.facebook.buck.cli.[[ProjectGeneratorParameters]{.typeNameLink}](ProjectGeneratorParameters.html "class in com.facebook.buck.cli")
    -   com.facebook.buck.cli.[[ProjectSubCommand]{.typeNameLink}](ProjectSubCommand.html "class in com.facebook.buck.cli")
        (implements
        com.facebook.buck.support.cli.args.[PluginBasedSubCommand](../support/cli/args/PluginBasedSubCommand.html "interface in com.facebook.buck.support.cli.args"))
    -   com.facebook.buck.cli.[[ResolveAliasHelper]{.typeNameLink}](ResolveAliasHelper.html "class in com.facebook.buck.cli")
    -   com.facebook.buck.cli.[[SystemInfoLogger]{.typeNameLink}](SystemInfoLogger.html "class in com.facebook.buck.cli")
    -   com.facebook.buck.cli.[[TargetDeviceCommandLineOptions]{.typeNameLink}](TargetDeviceCommandLineOptions.html "class in com.facebook.buck.cli")
    -   com.facebook.buck.cli.[[TestRunning]{.typeNameLink}](TestRunning.html "class in com.facebook.buck.cli")
    -   com.facebook.buck.cli.[[TestSelectorOptions]{.typeNameLink}](TestSelectorOptions.html "class in com.facebook.buck.cli")
    -   com.facebook.buck.cli.[[ThriftOutput]{.typeNameLink}](ThriftOutput.html "class in com.facebook.buck.cli")\<T\>
    -   com.facebook.buck.cli.[[ThriftOutput.Builder]{.typeNameLink}](ThriftOutput.Builder.html "class in com.facebook.buck.cli")\<T\>
    -   java.lang.[[Throwable]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Throwable.html?is-external=true "class or interface in java.lang"){.externalLink}
        (implements
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   java.lang.[[Exception]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Exception.html?is-external=true "class or interface in java.lang"){.externalLink}
            -   com.facebook.buck.cli.[[BuildCommand.ActionGraphCreationException]{.typeNameLink}](BuildCommand.ActionGraphCreationException.html "class in com.facebook.buck.cli")
    -   com.facebook.buck.cli.[[UninstallCommand.UninstallOptions]{.typeNameLink}](UninstallCommand.UninstallOptions.html "class in com.facebook.buck.cli")
    -   com.facebook.buck.cli.[[VerbosityParser]{.typeNameLink}](VerbosityParser.html "class in com.facebook.buck.cli")
:::

::: {.section role="region"}
## Interface Hierarchy {#interface-hierarchy title="Interface Hierarchy"}

-   com.facebook.buck.cli.[[ActionGraphSerializer.ActionGraphData]{.typeNameLink}](ActionGraphSerializer.ActionGraphData.html "interface in com.facebook.buck.cli")
-   com.facebook.buck.cli.[[Command]{.typeNameLink}](Command.html "interface in com.facebook.buck.cli")
-   org.pf4j.ExtensionPoint
    -   com.facebook.buck.support.cli.args.[[PluginBasedSubCommandFactory]{.typeNameLink}](../support/cli/args/PluginBasedSubCommandFactory.html "interface in com.facebook.buck.support.cli.args")\<T\>
        -   com.facebook.buck.cli.[[ProjectSubCommandFactory]{.typeNameLink}](ProjectSubCommandFactory.html "interface in com.facebook.buck.cli")
-   com.facebook.buck.cli.[[MainRunner.KnownRuleTypesFactoryFactory]{.typeNameLink}](MainRunner.KnownRuleTypesFactoryFactory.html "interface in com.facebook.buck.cli")
-   com.facebook.buck.cli.[[MainRunner.ParserAndCaches]{.typeNameLink}](MainRunner.ParserAndCaches.html "interface in com.facebook.buck.cli")
:::

::: {.section role="region"}
## Annotation Type Hierarchy {#annotation-type-hierarchy title="Annotation Type Hierarchy"}

-   com.facebook.buck.cli.[[AdditionalOptions]{.typeNameLink}](AdditionalOptions.html "annotation in com.facebook.buck.cli")
    (implements
    java.lang.annotation.[Annotation](http://docs.oracle.com/javase/7/docs/api/java/lang/annotation/Annotation.html?is-external=true "class or interface in java.lang.annotation"){.externalLink})
:::

::: {.section role="region"}
## Enum Hierarchy {#enum-hierarchy title="Enum Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   java.lang.[[Enum]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<E\>
        (implements
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   com.facebook.buck.cli.[[AbstractQueryCommand.OutputFormat]{.typeNameLink}](AbstractQueryCommand.OutputFormat.html "enum in com.facebook.buck.cli")
        -   com.facebook.buck.cli.[[AbstractQueryCommand.SortOutputFormat]{.typeNameLink}](AbstractQueryCommand.SortOutputFormat.html "enum in com.facebook.buck.cli")
        -   com.facebook.buck.cli.[[AbstractQueryCommand.WhichQueryCommand]{.typeNameLink}](AbstractQueryCommand.WhichQueryCommand.html "enum in com.facebook.buck.cli")
        -   com.facebook.buck.cli.[[Dot.OutputOrder]{.typeNameLink}](Dot.OutputOrder.html "enum in com.facebook.buck.cli")
        -   com.facebook.buck.cli.[[ProjectTestsMode]{.typeNameLink}](ProjectTestsMode.html "enum in com.facebook.buck.cli")
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
-   Tree
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
