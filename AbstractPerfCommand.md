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

## Class AbstractPerfCommand\<CommandContext\> {#class-abstractperfcommandcommandcontext .title title="Class AbstractPerfCommand"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.cli.CommandWithPluginManager](CommandWithPluginManager.html "class in com.facebook.buck.cli")

    -   -   [com.facebook.buck.cli.AbstractCommand](AbstractCommand.html "class in com.facebook.buck.cli")

        -   -   com.facebook.buck.cli.AbstractPerfCommand\<CommandContext\>

::: description
-   

    All Implemented Interfaces:
    :   `Command`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `PerfActionGraphCommand`, `PerfManifestCommand`,
        `PerfMbrPrepareRemoteExecutionCommand`,
        `PerfMbrSerializationCommand`, `PerfRuleKeyCommand`

    ------------------------------------------------------------------------

        public abstract class AbstractPerfCommand<CommandContext>
        extends AbstractCommand

    ::: block
    This is the core of our perf commands, it handles the outer
    prepare + loop and statistics gathering.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.cli.AbstractCommand}

            ### Fields inherited from class com.facebook.buck.cli.[AbstractCommand](AbstractCommand.html "class in com.facebook.buck.cli")

            `commandArgsFile`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor               Description
          ------------------------- -------------
          `AbstractPerfCommand()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected            | `createStacked        | ::: block             |
        | StackedFileHashCache` | FileHashCache​(Command | Creates a             |
        |                       | RunnerParams params)` | [`StackedF            |
        |                       |                       | ileHashCache`](../uti |
        |                       |                       | l/cache/impl/StackedF |
        |                       |                       | ileHashCache.html "cl |
        |                       |                       | ass in com.facebook.b |
        |                       |                       | uck.util.cache.impl") |
        |                       |                       | similar to a real     |
        |                       |                       | command but that uses |
        |                       |                       | our hash-faking       |
        |                       |                       | delegate.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `prote                | `                     |                       |
        | cted abstract String` | getComputationName()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `prote                | `getRulesInG          | ::: block             |
        | cted static com.googl | raph​(ActionGraphBuild | Gets a list of the    |
        | e.common.collect.Immu | er graphBuilder,      | rules in the graph    |
        | tableList<BuildRule>` |            Iterable<B | reachable from the    |
        |                       | uildTarget> targets)` | provided targets.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected Targe      | `getTargetGrap        | ::: block             |
        | tGraphCreationResult` | h​(CommandRunnerParams | Most of our perf      |
        |                       |  params,              | tests require a       |
        |                       |   com.google.common.c | target graph, this    |
        |                       | ollect.ImmutableSet<B | helps them get it     |
        |                       | uildTarget> targets)` | concisely.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `p                    | `initializeRulesFrom  | ::: block             |
        | rotected static void` | Disk​(ActionGraphBuild | Calls                 |
        |                       | er graphBuilder,      | initializeFromDisk()  |
        |                       |                    co | on all the            |
        |                       | m.google.common.colle | initializable rules   |
        |                       | ct.ImmutableList<Buil | in the graph.         |
        |                       | dRule> rulesInGraph)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isReadOnly()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ExitCode`            | `r                    |                       |
        |                       | unWithoutHelp​(Command |                       |
        |                       | RunnerParams params)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.cli.AbstractCommand}

            ### Methods inherited from class com.facebook.buck.cli.[AbstractCommand](AbstractCommand.html "class in com.facebook.buck.cli")

            `addCommandSpecificConfigOverrides, convertArgumentsToBuildTargets, createParsingContext, getCommandArgsFile, getCommandLineBuildTargetNormalizer, getConcurrencyLimit, getConfigOverrides, getEnableParserProfiling, getEventListeners, getEventsOutputPath, getExcludeIncompatibleTargets, getExecutionContext, getExecutionContextBuilder, getHostPlatform, getLogConfig, getTargetPlatforms, handleException, handleException, isNoCache, isReuseCurrentConfig, isSourceControlStatsGatheringEnabled, matchBuildTargetsWithLabelsFromSpecs, performsBuild, prepareExecutionContext, printUsage, printWarning, printWarning, run, runHelp`

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

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.cli.Command}

            ### Methods inherited from interface com.facebook.buck.cli.[Command](Command.html "interface in com.facebook.buck.cli")

            `getShortDescription`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### AbstractPerfCommand

                public AbstractPerfCommand()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getComputationName()}

        -   #### getComputationName

            ``` methodSignature
            protected abstract String getComputationName()
            ```

        []{#runWithoutHelp(com.facebook.buck.cli.CommandRunnerParams)}

        -   #### runWithoutHelp

            ``` methodSignature
            public final ExitCode runWithoutHelp​(CommandRunnerParams params)
                                          throws Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `runWithoutHelp` in class `AbstractCommand`

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#getTargetGraph(com.facebook.buck.cli.CommandRunnerParams,com.google.common.collect.ImmutableSet)}

        -   #### getTargetGraph

            ``` methodSignature
            protected TargetGraphCreationResult getTargetGraph​(CommandRunnerParams params,
                                                               com.google.common.collect.ImmutableSet<BuildTarget> targets)
                                                        throws InterruptedException,
                                                               IOException,
                                                               VersionException
            ```

            ::: block
            Most of our perf tests require a target graph, this helps
            them get it concisely.
            :::

            [Throws:]{.throwsLabel}
            :   `InterruptedException`
            :   `IOException`
            :   `VersionException`

        []{#initializeRulesFromDisk(com.facebook.buck.core.rules.ActionGraphBuilder,com.google.common.collect.ImmutableList)}

        -   #### initializeRulesFromDisk

            ``` methodSignature
            protected static void initializeRulesFromDisk​(ActionGraphBuilder graphBuilder,
                                                          com.google.common.collect.ImmutableList<BuildRule> rulesInGraph)
                                                   throws IOException
            ```

            ::: block
            Calls initializeFromDisk() on all the initializable rules in
            the graph. This is unsafe.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getRulesInGraph(com.facebook.buck.core.rules.ActionGraphBuilder,java.lang.Iterable)}

        -   #### getRulesInGraph

            ``` methodSignature
            protected static com.google.common.collect.ImmutableList<BuildRule> getRulesInGraph​(ActionGraphBuilder graphBuilder,
                                                                                                Iterable<BuildTarget> targets)
                                                                                         throws CycleException
            ```

            ::: block
            Gets a list of the rules in the graph reachable from the
            provided targets.
            :::

            [Throws:]{.throwsLabel}
            :   `CycleException`

        []{#createStackedFileHashCache(com.facebook.buck.cli.CommandRunnerParams)}

        -   #### createStackedFileHashCache

            ``` methodSignature
            protected StackedFileHashCache createStackedFileHashCache​(CommandRunnerParams params)
                                                               throws InterruptedException
            ```

            ::: block
            Creates a
            [`StackedFileHashCache`](../util/cache/impl/StackedFileHashCache.html "class in com.facebook.buck.util.cache.impl")
            similar to a real command but that uses our hash-faking
            delegate.
            :::

            [Throws:]{.throwsLabel}
            :   `InterruptedException`

        []{#isReadOnly()}

        -   #### isReadOnly

            ``` methodSignature
            public final boolean isReadOnly()
            ```

            [Returns:]{.returnLabel}
            :   whether the command doesn\'t modify the state of the
                filesystem
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
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
