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
[Package]{.packageLabelInType} [com.facebook.buck.cli](package-summary.html)
:::

## Class BuildCommand {#class-buildcommand .title title="Class BuildCommand"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.cli.CommandWithPluginManager](CommandWithPluginManager.html "class in com.facebook.buck.cli")

    -   -   [com.facebook.buck.cli.AbstractCommand](AbstractCommand.html "class in com.facebook.buck.cli")

        -   -   com.facebook.buck.cli.BuildCommand

::: description
-   

    All Implemented Interfaces:
    :   `Command`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `FetchCommand`, `InstallCommand`, `PublishCommand`,
        `TestCommand`

    ------------------------------------------------------------------------

        public class BuildCommand
        extends AbstractCommand
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                                         Description
          ------------------- --------------------------------------------- -------------
          `static class `     `BuildCommand.ActionGraphCreationException`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.cli.AbstractCommand}

            ### Fields inherited from class com.facebook.buck.cli.[AbstractCommand](AbstractCommand.html "class in com.facebook.buck.cli")

            `commandArgsFile`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                              Description
          ---------------------------------------- -------------
          `BuildCommand()`                          
          `BuildCommand​(List<String> arguments)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected void`      | `as                   |                       |
        |                       | sertArguments​(Command |                       |
        |                       | RunnerParams params)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected ExitCode`  | `execute              |                       |
        |                       | LocalBuild​(CommandRun |                       |
        |                       | nerParams params,     |                       |
        |                       |               com.fac |                       |
        |                       | ebook.buck.cli.BuildC |                       |
        |                       | ommand.GraphsAndBuild |                       |
        |                       | Targets graphsAndBuil |                       |
        |                       | dTargets,             |                       |
        |                       |       WeightedListeni |                       |
        |                       | ngExecutorService exe |                       |
        |                       | cutor,                |                       |
        |                       |    Optional<ThriftRul |                       |
        |                       | eKeyLogger> ruleKeyLo |                       |
        |                       | gger,                 |                       |
        |                       |   Optional<CountDownL |                       |
        |                       | atch> initializeBuild |                       |
        |                       | Latch,                |                       |
        |                       |    RuleKeyCacheScope< |                       |
        |                       | RuleKey> ruleKeyCache |                       |
        |                       | Scope,                |                       |
        |                       |    AtomicReference<Bu |                       |
        |                       | ild> buildReference)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected I          | `get                  |                       |
        | terable<BuildTarget>` | AdditionalTargetsToBu |                       |
        |                       | ild​(com.facebook.buck |                       |
        |                       | .cli.BuildCommand.Gra |                       |
        |                       | phsAndBuildTargets gr |                       |
        |                       | aphsAndBuildTargets)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `List<String>`        | `getArguments()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<BuildType>` | `                     |                       |
        |                       | getBuildEngineMode()` |                       |
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
        | `protected Exec       | `getExecutionC        |                       |
        | utionContext.Builder` | ontextBuilder​(Command |                       |
        |                       | RunnerParams params)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Path>`      | `ge                   |                       |
        |                       | tPathToBuildReport​(Bu |                       |
        |                       | ckConfig buckConfig)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `g                    |                       |
        |                       | etShortDescription()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isC                  |                       |
        |                       | odeCoverageEnabled()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isDebugEnabled()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isKeepGoing()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isReadOnly()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isRemoteExec         |                       |
        |                       | utionForceDisabled()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isSourceControlSta   |                       |
        |                       | tsGatheringEnabled()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `performsBuild()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected com.face   | `                     |                       |
        | book.buck.cli.BuildCo | run​(CommandRunnerPara |                       |
        | mmand.BuildRunResult` | ms params,    Command |                       |
        |                       | ThreadManager command |                       |
        |                       | ThreadManager,    jav |                       |
        |                       | a.util.function.Funct |                       |
        |                       | ion<com.google.common |                       |
        |                       | .collect.ImmutableLis |                       |
        |                       | t<TargetNodeSpec>,​com |                       |
        |                       | .google.common.collec |                       |
        |                       | t.ImmutableList<Targe |                       |
        |                       | tNodeSpec>> targetNod |                       |
        |                       | eSpecEnhancer,    com |                       |
        |                       | .google.common.collec |                       |
        |                       | t.ImmutableSet<String |                       |
        |                       | > additionalTargets)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ExitCode`            | `r                    |                       |
        |                       | unWithoutHelp​(Command |                       |
        |                       | RunnerParams params)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `setKeepGoin          |                       |
        |                       | g​(boolean keepGoing)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected boolean`   | `shouldR              |                       |
        |                       | eportAbsolutePaths()` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.cli.AbstractCommand}

            ### Methods inherited from class com.facebook.buck.cli.[AbstractCommand](AbstractCommand.html "class in com.facebook.buck.cli")

            `addCommandSpecificConfigOverrides, convertArgumentsToBuildTargets, createParsingContext, getCommandArgsFile, getCommandLineBuildTargetNormalizer, getConcurrencyLimit, getConfigOverrides, getEnableParserProfiling, getEventsOutputPath, getExcludeIncompatibleTargets, getExecutionContext, getHostPlatform, getLogConfig, getTargetPlatforms, handleException, handleException, isNoCache, isReuseCurrentConfig, matchBuildTargetsWithLabelsFromSpecs, prepareExecutionContext, printUsage, printWarning, printWarning, run, runHelp`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.cli.CommandWithPluginManager}

            ### Methods inherited from class com.facebook.buck.cli.[CommandWithPluginManager](CommandWithPluginManager.html "class in com.facebook.buck.cli")

            `getPluginManager, setPluginManager`

        ```{=html}
        <!-- -->
        ```
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

        -   #### BuildCommand

                public BuildCommand()

        []{#<init>(java.util.List)}

        -   #### BuildCommand

                public BuildCommand​(List<String> arguments)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getArguments()}

        -   #### getArguments

            ``` methodSignature
            public List<String> getArguments()
            ```

        []{#isCodeCoverageEnabled()}

        -   #### isCodeCoverageEnabled

            ``` methodSignature
            public boolean isCodeCoverageEnabled()
            ```

        []{#isDebugEnabled()}

        -   #### isDebugEnabled

            ``` methodSignature
            public boolean isDebugEnabled()
            ```

        []{#getBuildEngineMode()}

        -   #### getBuildEngineMode

            ``` methodSignature
            public Optional<BuildType> getBuildEngineMode()
            ```

        []{#isKeepGoing()}

        -   #### isKeepGoing

            ``` methodSignature
            public boolean isKeepGoing()
            ```

        []{#shouldReportAbsolutePaths()}

        -   #### shouldReportAbsolutePaths

            ``` methodSignature
            protected boolean shouldReportAbsolutePaths()
            ```

        []{#setKeepGoing(boolean)}

        -   #### setKeepGoing

            ``` methodSignature
            public void setKeepGoing​(boolean keepGoing)
            ```

        []{#isRemoteExecutionForceDisabled()}

        -   #### isRemoteExecutionForceDisabled

            ``` methodSignature
            public boolean isRemoteExecutionForceDisabled()
            ```

        []{#getPathToBuildReport(com.facebook.buck.core.config.BuckConfig)}

        -   #### getPathToBuildReport

            ``` methodSignature
            public Optional<Path> getPathToBuildReport​(BuckConfig buckConfig)
            ```

            [Returns:]{.returnLabel}
            :   an absolute path or
                [`Optional.empty()`](http://docs.oracle.com/javase/7/docs/api/java/util/Optional.html?is-external=true#empty() "class or interface in java.util"){.externalLink}.

        []{#runWithoutHelp(com.facebook.buck.cli.CommandRunnerParams)}

        -   #### runWithoutHelp

            ``` methodSignature
            public ExitCode runWithoutHelp​(CommandRunnerParams params)
                                    throws Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `runWithoutHelp` in class `AbstractCommand`

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#assertArguments(com.facebook.buck.cli.CommandRunnerParams)}

        -   #### assertArguments

            ``` methodSignature
            protected void assertArguments​(CommandRunnerParams params)
            ```

            [Throws:]{.throwsLabel}
            :   `CommandLineException` - if arguments provided are
                incorrect

        []{#run(com.facebook.buck.cli.CommandRunnerParams,com.facebook.buck.cli.CommandThreadManager,java.util.function.Function,com.google.common.collect.ImmutableSet)}

        -   #### run

            ``` methodSignature
            protected com.facebook.buck.cli.BuildCommand.BuildRunResult run​(CommandRunnerParams params,
                                                                            CommandThreadManager commandThreadManager,
                                                                            java.util.function.Function<com.google.common.collect.ImmutableList<TargetNodeSpec>,​com.google.common.collect.ImmutableList<TargetNodeSpec>> targetNodeSpecEnhancer,
                                                                            com.google.common.collect.ImmutableSet<String> additionalTargets)
                                                                     throws Exception
            ```

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#executeLocalBuild(com.facebook.buck.cli.CommandRunnerParams,com.facebook.buck.cli.BuildCommand.GraphsAndBuildTargets,com.facebook.buck.util.concurrent.WeightedListeningExecutorService,java.util.Optional,java.util.Optional,com.facebook.buck.rules.keys.RuleKeyCacheScope,java.util.concurrent.atomic.AtomicReference)}

        -   #### executeLocalBuild

            ``` methodSignature
            protected ExitCode executeLocalBuild​(CommandRunnerParams params,
                                                 com.facebook.buck.cli.BuildCommand.GraphsAndBuildTargets graphsAndBuildTargets,
                                                 WeightedListeningExecutorService executor,
                                                 Optional<ThriftRuleKeyLogger> ruleKeyLogger,
                                                 Optional<CountDownLatch> initializeBuildLatch,
                                                 RuleKeyCacheScope<RuleKey> ruleKeyCacheScope,
                                                 AtomicReference<Build> buildReference)
                                          throws Exception
            ```

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#getExecutionContextBuilder(com.facebook.buck.cli.CommandRunnerParams)}

        -   #### getExecutionContextBuilder

            ``` methodSignature
            protected ExecutionContext.Builder getExecutionContextBuilder​(CommandRunnerParams params)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `getExecutionContextBuilder` in class `AbstractCommand`

        []{#getAdditionalTargetsToBuild(com.facebook.buck.cli.BuildCommand.GraphsAndBuildTargets)}

        -   #### getAdditionalTargetsToBuild

            ``` methodSignature
            protected Iterable<BuildTarget> getAdditionalTargetsToBuild​(com.facebook.buck.cli.BuildCommand.GraphsAndBuildTargets graphsAndBuildTargets)
            ```

        []{#isReadOnly()}

        -   #### isReadOnly

            ``` methodSignature
            public boolean isReadOnly()
            ```

            [Returns:]{.returnLabel}
            :   whether the command doesn\'t modify the state of the
                filesystem

        []{#isSourceControlStatsGatheringEnabled()}

        -   #### isSourceControlStatsGatheringEnabled

            ``` methodSignature
            public boolean isSourceControlStatsGatheringEnabled()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isSourceControlStatsGatheringEnabled` in
                interface `Command`

            [Overrides:]{.overrideSpecifyLabel}
            :   `isSourceControlStatsGatheringEnabled` in
                class `AbstractCommand`

            [Returns:]{.returnLabel}
            :   whether we should gather source control stats while
                executing the command.

        []{#getShortDescription()}

        -   #### getShortDescription

            ``` methodSignature
            public String getShortDescription()
            ```

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

            [Specified by:]{.overrideSpecifyLabel}
            :   `getEventListeners` in interface `Command`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getEventListeners` in class `AbstractCommand`

        []{#performsBuild()}

        -   #### performsBuild

            ``` methodSignature
            public boolean performsBuild()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `performsBuild` in interface `Command`

            [Overrides:]{.overrideSpecifyLabel}
            :   `performsBuild` in class `AbstractCommand`
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
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
