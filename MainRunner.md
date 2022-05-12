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

## Class MainRunner {#class-mainrunner .title title="Class MainRunner"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cli.MainRunner

::: description
-   

    ------------------------------------------------------------------------

        public final class MainRunner
        extends Object

    ::: block
    Responsible for running the commands logic of buck after
    [`MainWithNailgun`](MainWithNailgun.html "class in com.facebook.buck.cli")
    and
    [`MainWithoutNailgun`](MainWithoutNailgun.html "class in com.facebook.buck.cli")
    have completed the initial bootstrapping of resources and state.
    One instance of
    [`MainRunner`](MainRunner.html "class in com.facebook.buck.cli")
    exists per command run.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static interface `   | `MainRunner.KnownRul  |                       |
        |                       | eTypesFactoryFactory` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static interface `   | `MainRu               | ::: block             |
        |                       | nner.ParserAndCaches` | Struct for the        |
        |                       |                       | multiple values       |
        |                       |                       | returned by           |
        |                       |                       | [`getPar              |
        |                       |                       | serAndCaches(java.uti |
        |                       |                       | l.Optional<com.facebo |
        |                       |                       | ok.nailgun.NGContext> |
        |                       |                       | , com.facebook.buck.i |
        |                       |                       | o.watchman.WatchmanWa |
        |                       |                       | tcher.FreshInstanceAc |
        |                       |                       | tion, com.facebook.bu |
        |                       |                       | ck.io.filesystem.Proj |
        |                       |                       | ectFilesystem, com.fa |
        |                       |                       | cebook.buck.core.conf |
        |                       |                       | ig.BuckConfig, com.fa |
        |                       |                       | cebook.buck.io.watchm |
        |                       |                       | an.Watchman, com.face |
        |                       |                       | book.buck.core.rules. |
        |                       |                       | knowntypes.provider.K |
        |                       |                       | nownRuleTypesProvider |
        |                       |                       | , com.facebook.buck.c |
        |                       |                       | ore.cell.Cell, com.fa |
        |                       |                       | cebook.buck.support.s |
        |                       |                       | tate.BuckGlobalState, |
        |                       |                       |  com.facebook.buck.ev |
        |                       |                       | ent.BuckEventBus, com |
        |                       |                       | .google.common.collec |
        |                       |                       | t.ImmutableMap<com.fa |
        |                       |                       | cebook.buck.util.conc |
        |                       |                       | urrent.ExecutorPool,  |
        |                       |                       | com.google.common.uti |
        |                       |                       | l.concurrent.Listenin |
        |                       |                       | gExecutorService>, co |
        |                       |                       | m.facebook.buck.rules |
        |                       |                       | .keys.config.RuleKeyC |
        |                       |                       | onfiguration, com.fac |
        |                       |                       | ebook.buck.util.Close |
        |                       |                       | ableMemoizedSupplier< |
        |                       |                       | com.facebook.buck.cor |
        |                       |                       | e.graph.transformatio |
        |                       |                       | n.executor.DepsAwareE |
        |                       |                       | xecutor<? super com.f |
        |                       |                       | acebook.buck.core.gra |
        |                       |                       | ph.transformation.mod |
        |                       |                       | el.ComputeResult, ?>> |
        |                       |                       | , com.facebook.buck.i |
        |                       |                       | o.ExecutableFinder, c |
        |                       |                       | om.facebook.buck.core |
        |                       |                       | .parser.buildtargetpa |
        |                       |                       | rser.UnconfiguredBuil |
        |                       |                       | dTargetViewFactory, c |
        |                       |                       | om.facebook.buck.core |
        |                       |                       | .model.TargetConfigur |
        |                       |                       | ation, com.facebook.b |
        |                       |                       | uck.parser.TargetSpec |
        |                       |                       | Resolver)`](#getParse |
        |                       |                       | rAndCaches(java.util. |
        |                       |                       | Optional,com.facebook |
        |                       |                       | .buck.io.watchman.Wat |
        |                       |                       | chmanWatcher.FreshIns |
        |                       |                       | tanceAction,com.faceb |
        |                       |                       | ook.buck.io.filesyste |
        |                       |                       | m.ProjectFilesystem,c |
        |                       |                       | om.facebook.buck.core |
        |                       |                       | .config.BuckConfig,co |
        |                       |                       | m.facebook.buck.io.wa |
        |                       |                       | tchman.Watchman,com.f |
        |                       |                       | acebook.buck.core.rul |
        |                       |                       | es.knowntypes.provide |
        |                       |                       | r.KnownRuleTypesProvi |
        |                       |                       | der,com.facebook.buck |
        |                       |                       | .core.cell.Cell,com.f |
        |                       |                       | acebook.buck.support. |
        |                       |                       | state.BuckGlobalState |
        |                       |                       | ,com.facebook.buck.ev |
        |                       |                       | ent.BuckEventBus,com. |
        |                       |                       | google.common.collect |
        |                       |                       | .ImmutableMap,com.fac |
        |                       |                       | ebook.buck.rules.keys |
        |                       |                       | .config.RuleKeyConfig |
        |                       |                       | uration,com.facebook. |
        |                       |                       | buck.util.CloseableMe |
        |                       |                       | moizedSupplier,com.fa |
        |                       |                       | cebook.buck.io.Execut |
        |                       |                       | ableFinder,com.facebo |
        |                       |                       | ok.buck.core.parser.b |
        |                       |                       | uildtargetparser.Unco |
        |                       |                       | nfiguredBuildTargetVi |
        |                       |                       | ewFactory,com.faceboo |
        |                       |                       | k.buck.core.model.Tar |
        |                       |                       | getConfiguration,com. |
        |                       |                       | facebook.buck.parser. |
        |                       |                       | TargetSpecResolver)). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `static int`          | `JNA_POINTER_SIZE`    | ::: block             |
        |                       |                       | Force JNA to be       |
        |                       |                       | initialized early to  |
        |                       |                       | avoid deadlock race   |
        |                       |                       | condition.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `MainRunne                        | ::: block                         |
        | r​(Console console,           Inpu | This constructor allows           |
        | tStream stdIn,           MainRunn | integration tests to              |
        | er.KnownRuleTypesFactoryFactory k | add/remove/modify known build     |
        | nownRuleTypesFactoryFactory,      | rules (aka descriptions).         |
        |       BuildId buildId,            | :::                               |
        | com.google.common.collect.Immutab |                                   |
        | leMap<String,​String> clientEnviro |                                   |
        | nment,           Platform platfor |                                   |
        | m,           Path projectRoot,    |                                   |
        |         org.pf4j.PluginManager pl |                                   |
        | uginManager,           BuckModule |                                   |
        | Manager moduleManager,            |                                   |
        | BackgroundTaskManager bgTaskManag |                                   |
        | er,           CommandMode command |                                   |
        | Mode,           Optional<com.face |                                   |
        | book.nailgun.NGContext> context)` |                                   |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                                                                                                                                        Description
          ------------------- ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `ExitCode`          `runMainWithExitCode​(WatchmanWatcher.FreshInstanceAction watchmanFreshInstanceAction,                    long initTimestamp,                    com.google.common.collect.ImmutableList<String> unexpandedCommandLineArgs)`    

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
    -   []{#field.detail}

        ### Field Detail

        []{#JNA_POINTER_SIZE}

        -   #### JNA_POINTER_SIZE

                public static final int JNA_POINTER_SIZE

            ::: block
            Force JNA to be initialized early to avoid deadlock race
            condition.
            See: https://github.com/java-native-access/jna/issues/652
            :::
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.util.Console,java.io.InputStream,com.facebook.buck.cli.MainRunner.KnownRuleTypesFactoryFactory,com.facebook.buck.core.model.BuildId,com.google.common.collect.ImmutableMap,com.facebook.buck.util.environment.Platform,java.nio.file.Path,org.pf4j.PluginManager,com.facebook.buck.core.module.BuckModuleManager,com.facebook.buck.support.bgtasks.BackgroundTaskManager,com.facebook.buck.util.environment.CommandMode,java.util.Optional)}

        -   #### MainRunner

                public MainRunner​(Console console,
                                  InputStream stdIn,
                                  MainRunner.KnownRuleTypesFactoryFactory knownRuleTypesFactoryFactory,
                                  BuildId buildId,
                                  com.google.common.collect.ImmutableMap<String,​String> clientEnvironment,
                                  Platform platform,
                                  Path projectRoot,
                                  org.pf4j.PluginManager pluginManager,
                                  BuckModuleManager moduleManager,
                                  BackgroundTaskManager bgTaskManager,
                                  CommandMode commandMode,
                                  Optional<com.facebook.nailgun.NGContext> context)

            ::: block
            This constructor allows integration tests to
            add/remove/modify known build rules (aka descriptions).
            :::

            [Parameters:]{.paramLabel}
            :   `console` - the
                [`Console`](../util/Console.html "class in com.facebook.buck.util")
                to print to for this command
            :   `stdIn` - the input stream to the command being ran
            :   `knownRuleTypesFactoryFactory` - the known rule types
                for this command
            :   `buildId` - the
                [`BuildId`](../core/model/BuildId.html "class in com.facebook.buck.core.model")
                for this command
            :   `clientEnvironment` - the environment variable map for
                this command
            :   `platform` - the current running
                [`Platform`](../util/environment/Platform.html "enum in com.facebook.buck.util.environment")
            :   `projectRoot` - the project root of the current command
            :   `pluginManager` - the `PluginManager` for this command
            :   `moduleManager` - the
                [`BuckModuleManager`](../core/module/BuckModuleManager.html "interface in com.facebook.buck.core.module")
                for this command
            :   `context` - the `NGContext` from nailgun for this
                command
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#runMainWithExitCode(com.facebook.buck.io.watchman.WatchmanWatcher.FreshInstanceAction,long,com.google.common.collect.ImmutableList)}

        -   #### runMainWithExitCode

            ``` methodSignature
            public ExitCode runMainWithExitCode​(WatchmanWatcher.FreshInstanceAction watchmanFreshInstanceAction,
                                                long initTimestamp,
                                                com.google.common.collect.ImmutableList<String> unexpandedCommandLineArgs)
                                         throws Exception
            ```

            [Parameters:]{.paramLabel}
            :   `initTimestamp` - Value of System.nanoTime() when
                process got main()/nailMain() invoked.
            :   `unexpandedCommandLineArgs` - command line arguments

            [Returns:]{.returnLabel}
            :   an ExitCode representing the result of the command

            [Throws:]{.throwsLabel}
            :   `Exception`
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
