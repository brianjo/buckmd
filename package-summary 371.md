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
# Package com.facebook.buck.shell {#package-com.facebook.buck.shell .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [AbstractGenruleDescr             |                                   |
    | iption.CommonArg](AbstractGenrule |                                   |
    | Description.CommonArg.html "inter |                                   |
    | face in com.facebook.buck.shell") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ProvidesWorkerToo                | ::: block                         |
    | l](ProvidesWorkerTool.html "inter | [`Wo                              |
    | face in com.facebook.buck.shell") | rkerTool`](WorkerTool.html "inter |
    |                                   | face in com.facebook.buck.shell") |
    |                                   | provider                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [W                                | ::: block                         |
    | orkerTool](WorkerTool.html "inter | Worker tool definition            |
    | face in com.facebook.buck.shell") | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [AbstractGenruleDescription](Abst |                                   |
    | ractGenruleDescription.html "clas |                                   |
    | s in com.facebook.buck.shell")\<T |                                   |
    | extends                           |                                   |
    | [AbstractGenruleDescrip           |                                   |
    | tion.CommonArg](AbstractGenruleDe |                                   |
    | scription.CommonArg.html "interfa |                                   |
    | ce in com.facebook.buck.shell")\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [AbstractGenrule                  |                                   |
    | Step](AbstractGenruleStep.html "c |                                   |
    | lass in com.facebook.buck.shell") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AbstractGe                       |                                   |
    | nruleStep.CommandString](Abstract |                                   |
    | GenruleStep.CommandString.html "c |                                   |
    | lass in com.facebook.buck.shell") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Ba                               | ::: block                         |
    | seGenrule](BaseGenrule.html "clas | Abstract parent class of all      |
    | s in com.facebook.buck.shell")\<T | Genrules, containing some common  |
    | extends                           | functionality while remaining     |
    | [GenruleBuil                      | generic over the                  |
    | dable](GenruleBuildable.html "cla | [`Buildable`](../rules/mod        |
    | ss in com.facebook.buck.shell")\> | ern/Buildable.html "interface in  |
    |                                   | com.facebook.buck.rules.modern"), |
    |                                   | to be provided by child classes.  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BashStep](BashStep.html "c       | ::: block                         |
    | lass in com.facebook.buck.shell") | Command that makes it possible to |
    |                                   | run an arbitrary command in Bash. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [C                                | ::: block                         |
    | ommandAlias](CommandAlias.html "c | A                                 |
    | lass in com.facebook.buck.shell") | [`BinaryBu                        |
    |                                   | ildRule`](../core/rules/tool/Bina |
    |                                   | ryBuildRule.html "interface in co |
    |                                   | m.facebook.buck.core.rules.tool") |
    |                                   | that wraps other build rules, and |
    |                                   | can optionally add extra          |
    |                                   | arguments, environment variables, |
    |                                   | or run different tools per host   |
    |                                   | [`Platform`](../util/enviro       |
    |                                   | nment/Platform.html "enum in com. |
    |                                   | facebook.buck.util.environment"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CommandAliasDescription          |                                   |
    | ](CommandAliasDescription.html "c |                                   |
    | lass in com.facebook.buck.shell") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CommandAliasDescriptionArg](C    | ::: block                         |
    | ommandAliasDescriptionArg.html "c | Immutable implementation of       |
    | lass in com.facebook.buck.shell") | `CommandAliasDescription.Abs      |
    |                                   | tractCommandAliasDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CommandAlias                     | ::: block                         |
    | DescriptionArg.Builder](CommandAl | Builds instances of type          |
    | iasDescriptionArg.Builder.html "c | [`CommandAliasDescriptionArg`](Co |
    | lass in com.facebook.buck.shell") | mmandAliasDescriptionArg.html "cl |
    |                                   | ass in com.facebook.buck.shell"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DefaultSh                        |                                   |
    | ellStep](DefaultShellStep.html "c |                                   |
    | lass in com.facebook.buck.shell") |                                   |
    +-----------------------------------+-----------------------------------+
    | [DefaultWorkerToolRu              | ::: block                         |
    | le](DefaultWorkerToolRule.html "c | BuildRule for worker_tools.       |
    | lass in com.facebook.buck.shell") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ExportFile](ExportFile.html "c   | ::: block                         |
    | lass in com.facebook.buck.shell") | Export a file so that it can be   |
    |                                   | easily referenced by other        |
    |                                   | [`BuildRule`](../core/r           |
    |                                   | ules/BuildRule.html "interface in |
    |                                   |  com.facebook.buck.core.rules")s. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ExportFileDescripti              |                                   |
    | on](ExportFileDescription.html "c |                                   |
    | lass in com.facebook.buck.shell") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ExportFileDescriptionArg]        | ::: block                         |
    | (ExportFileDescriptionArg.html "c | Immutable implementation of       |
    | lass in com.facebook.buck.shell") | `ExportFileDescription.A          |
    |                                   | bstractExportFileDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ExportFi                         | ::: block                         |
    | leDescriptionArg.Builder](ExportF | Builds instances of type          |
    | ileDescriptionArg.Builder.html "c | [`ExportFileDescriptionArg`](     |
    | lass in com.facebook.buck.shell") | ExportFileDescriptionArg.html "cl |
    |                                   | ass in com.facebook.buck.shell"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Genrule](Genrule.html "c         | ::: block                         |
    | lass in com.facebook.buck.shell") | Build rule for generating a file  |
    |                                   | via a shell command.              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [GenruleAndroidT                  | ::: block                         |
    | ools](GenruleAndroidTools.html "c | Immutable class for holding       |
    | lass in com.facebook.buck.shell") | Android paths and tools, for use  |
    |                                   | in                                |
    |                                   | [`GenruleBuil                     |
    |                                   | dable`](GenruleBuildable.html "cl |
    |                                   | ass in com.facebook.buck.shell"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Gen                              | ::: block                         |
    | ruleBinary](GenruleBinary.html "c | Same as a Genrule, but marked as  |
    | lass in com.facebook.buck.shell") | a binary.                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [GenruleBu                        | ::: block                         |
    | ildable](GenruleBuildable.html "c | Buildable for                     |
    | lass in com.facebook.buck.shell") | [`Genrule`](Genrule.html "c       |
    |                                   | lass in com.facebook.buck.shell") |
    |                                   | suitable for building Genrules    |
    |                                   | directly and also for subclasses  |
    |                                   | extending the functionality of a  |
    |                                   | bare Genrule.                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [GenruleDescri                    |                                   |
    | ption](GenruleDescription.html "c |                                   |
    | lass in com.facebook.buck.shell") |                                   |
    +-----------------------------------+-----------------------------------+
    | [GenruleDescriptionA              | ::: block                         |
    | rg](GenruleDescriptionArg.html "c | Immutable implementation of       |
    | lass in com.facebook.buck.shell") | `GenruleDescriptio                |
    |                                   | n.AbstractGenruleDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Ge                               | ::: block                         |
    | nruleDescriptionArg.Builder](Genr | Builds instances of type          |
    | uleDescriptionArg.Builder.html "c | [`GenruleDescriptionArg           |
    | lass in com.facebook.buck.shell") | `](GenruleDescriptionArg.html "cl |
    |                                   | ass in com.facebook.buck.shell"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | RunShTestAndRecordResultStep](Run | Run an sh_test executable, and    |
    | ShTestAndRecordResultStep.html "c | write its exit code, stdout,      |
    | lass in com.facebook.buck.shell") | stderr to a file to be            |
    |                                   | interpreted later.                |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RunTestAndRecordResultStep](R    | ::: block                         |
    | unTestAndRecordResultStep.html "c | Run a test executable, and write  |
    | lass in com.facebook.buck.shell") | its exit code, stdout, stderr to  |
    |                                   | a file to be interpreted later    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ShBinary](ShBinary.html "c       |                                   |
    | lass in com.facebook.buck.shell") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ShBinaryDescrip                  |                                   |
    | tion](ShBinaryDescription.html "c |                                   |
    | lass in com.facebook.buck.shell") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ShBinaryDescriptionAr            | ::: block                         |
    | g](ShBinaryDescriptionArg.html "c | Immutable implementation of       |
    | lass in com.facebook.buck.shell") | `ShBinaryDescription              |
    |                                   | .AbstractShBinaryDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ShBi                             | ::: block                         |
    | naryDescriptionArg.Builder](ShBin | Builds instances of type          |
    | aryDescriptionArg.Builder.html "c | [`ShBinaryDescriptionArg`         |
    | lass in com.facebook.buck.shell") | ](ShBinaryDescriptionArg.html "cl |
    |                                   | ass in com.facebook.buck.shell"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Shell](Shell.html "c             |                                   |
    | lass in com.facebook.buck.shell") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ShellDescriptionsProvider](      |                                   |
    | ShellDescriptionsProvider.html "c |                                   |
    | lass in com.facebook.buck.shell") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ShellStep](ShellStep.html "c     |                                   |
    | lass in com.facebook.buck.shell") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ShTest](ShTest.html "c           | ::: block                         |
    | lass in com.facebook.buck.shell") | Test whose correctness is         |
    |                                   | determined by running a specified |
    |                                   | shell script.                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ShTestDescr                      |                                   |
    | iption](ShTestDescription.html "c |                                   |
    | lass in com.facebook.buck.shell") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ShTestDescription                | ::: block                         |
    | Arg](ShTestDescriptionArg.html "c | Immutable implementation of       |
    | lass in com.facebook.buck.shell") | `ShTestDescripti                  |
    |                                   | on.AbstractShTestDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | ShTestDescriptionArg.Builder](ShT | Builds instances of type          |
    | estDescriptionArg.Builder.html "c | [`ShTestDescriptionAr             |
    | lass in com.facebook.buck.shell") | g`](ShTestDescriptionArg.html "cl |
    |                                   | ass in com.facebook.buck.shell"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Sy                               | ::: block                         |
    | mlinkFilesIntoDirectoryStep](Syml | [`Step`](../step/Step.html "inte  |
    | inkFilesIntoDirectoryStep.html "c | rface in com.facebook.buck.step") |
    | lass in com.facebook.buck.shell") | that takes a collection of        |
    |                                   | entries in a directory and        |
    |                                   | creates a set of read-only        |
    |                                   | symlinks (with the same           |
    |                                   | structure) to the original        |
    |                                   | entries in a new directory.       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [TestSuite](TestSuite.html "c     | ::: block                         |
    | lass in com.facebook.buck.shell") | Simple rule that logically groups |
    |                                   | tests and propagates dependencies |
    |                                   | on Test rules and makes them      |
    |                                   | available for                     |
    |                                   | [`TestC                           |
    |                                   | ommand`](../cli/TestCommand.html  |
    |                                   | "class in com.facebook.buck.cli") |
    |                                   | to consume.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [TestSuiteDescript                | ::: block                         |
    | ion](TestSuiteDescription.html "c | Produces rules used to logically  |
    | lass in com.facebook.buck.shell") | group tests, allowing \`buck test |
    |                                   | //:some_test_suite\` behavior     |
    |                                   | that invokes all tests that this  |
    |                                   | suite depends on.                 |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [TestSuiteDescriptionArg          | ::: block                         |
    | ](TestSuiteDescriptionArg.html "c | Args for test_suite               |
    | lass in com.facebook.buck.shell") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [TestSu                           | ::: block                         |
    | iteDescriptionArg.Builder](TestSu | Builds instances of type          |
    | iteDescriptionArg.Builder.html "c | [`TestSuiteDescriptionArg`]       |
    | lass in com.facebook.buck.shell") | (TestSuiteDescriptionArg.html "cl |
    |                                   | ass in com.facebook.buck.shell"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [WorkerS                          |                                   |
    | hellStep](WorkerShellStep.html "c |                                   |
    | lass in com.facebook.buck.shell") |                                   |
    +-----------------------------------+-----------------------------------+
    | [WorkerToolDescripti              |                                   |
    | on](WorkerToolDescription.html "c |                                   |
    | lass in com.facebook.buck.shell") |                                   |
    +-----------------------------------+-----------------------------------+
    | [WorkerToolDescriptionArg]        | ::: block                         |
    | (WorkerToolDescriptionArg.html "c | Immutable implementation of       |
    | lass in com.facebook.buck.shell") | `WorkerToolDescription.A          |
    |                                   | bstractWorkerToolDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [WorkerTo                         | ::: block                         |
    | olDescriptionArg.Builder](WorkerT | Builds instances of type          |
    | oolDescriptionArg.Builder.html "c | [`WorkerToolDescriptionArg`](     |
    | lass in com.facebook.buck.shell") | WorkerToolDescriptionArg.html "cl |
    |                                   | ass in com.facebook.buck.shell"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Enum                              | Description                       |
    +===================================+===================================+
    | [ExportFileDescription.Mode](     | ::: block                         |
    | ExportFileDescription.Mode.html " | Controls how \`export_file\`      |
    | enum in com.facebook.buck.shell") | exports it\'s wrapped source.     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ExportFileDirectoryAction]       | ::: block                         |
    | (ExportFileDirectoryAction.html " | An action for a situation when    |
    | enum in com.facebook.buck.shell") | `export_file` is given a          |
    |                                   | directory as input.               |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Enum Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Exception                         | Description                       |
    +===================================+===================================+
    | [CommandAlias.UnsupportedPl       | ::: block                         |
    | atformException](CommandAlias.Uns | Specific runtime exception type   |
    | upportedPlatformException.html "c | that is thrown when trying to run |
    | lass in com.facebook.buck.shell") | a tool via                        |
    |                                   | [`Co                              |
    |                                   | mmandAlias`](CommandAlias.html "c |
    |                                   | lass in com.facebook.buck.shell") |
    |                                   | on a platform that has not been   |
    |                                   | provided.                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Exception Summary[ ]{.tabEnd}
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
