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
[Package]{.packageLabelInType} [com.facebook.buck.command](package-summary.html)
:::

## Class BuildExecutor {#class-buildexecutor .title title="Class BuildExecutor"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.command.BuildExecutor

::: description
-   

    ------------------------------------------------------------------------

        public class BuildExecutor
        extends Object

    ::: block
    Used to build a given set of targets.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       Description
          --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `BuildExecutor​(BuildExecutorArgs args,              ExecutionContext executionContext,              ActionGraphAndBuilder actionGraphAndBuilder,              CachingBuildEngineDelegate cachingBuildEngineDelegate,              WeightedListeningExecutorService executorService,              boolean keepGoing,              RuleKeyCacheScope<RuleKey> ruleKeyRuleKeyCacheScope,              Optional<BuildType> buildEngineMode,              Optional<ThriftRuleKeyLogger> ruleKeyLogger,              MetadataProvider metadataProvider,              TargetConfigurationSerializer targetConfigurationSerializer,              boolean remoteExecutionAutoEnabled,              boolean forceDisableRemoteExecution)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `ExitCode`            | `buildTargets​(        | ::: block             |
        |                       | Iterable<BuildTarget> | Builds the given      |
        |                       |  targetsToBuild,      | targets               |
        |                       |         Optional<Path | synchronously.        |
        |                       | > pathToBuildReport)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Build`               | `getBuild()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `CachingBuildEngine`  | `get                  |                       |
        |                       | CachingBuildEngine()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `shutdown()`          | ::: block             |
        |                       |                       | Destroy any resources |
        |                       |                       | associated with this  |
        |                       |                       | builder.              |
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

        []{#<init>(com.facebook.buck.command.BuildExecutorArgs,com.facebook.buck.core.build.execution.context.ExecutionContext,com.facebook.buck.core.model.actiongraph.ActionGraphAndBuilder,com.facebook.buck.core.build.engine.delegate.CachingBuildEngineDelegate,com.facebook.buck.util.concurrent.WeightedListeningExecutorService,boolean,com.facebook.buck.rules.keys.RuleKeyCacheScope,java.util.Optional,java.util.Optional,com.facebook.buck.remoteexecution.interfaces.MetadataProvider,com.facebook.buck.core.model.TargetConfigurationSerializer,boolean,boolean)}

        -   #### BuildExecutor

                public BuildExecutor​(BuildExecutorArgs args,
                                     ExecutionContext executionContext,
                                     ActionGraphAndBuilder actionGraphAndBuilder,
                                     CachingBuildEngineDelegate cachingBuildEngineDelegate,
                                     WeightedListeningExecutorService executorService,
                                     boolean keepGoing,
                                     RuleKeyCacheScope<RuleKey> ruleKeyRuleKeyCacheScope,
                                     Optional<BuildType> buildEngineMode,
                                     Optional<ThriftRuleKeyLogger> ruleKeyLogger,
                                     MetadataProvider metadataProvider,
                                     TargetConfigurationSerializer targetConfigurationSerializer,
                                     boolean remoteExecutionAutoEnabled,
                                     boolean forceDisableRemoteExecution)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#buildTargets(java.lang.Iterable,java.util.Optional)}

        -   #### buildTargets

            ``` methodSignature
            public ExitCode buildTargets​(Iterable<BuildTarget> targetsToBuild,
                                         Optional<Path> pathToBuildReport)
                                  throws Exception
            ```

            ::: block
            Builds the given targets synchronously. Failures are printed
            to the EventBus.
            :::

            [Parameters:]{.paramLabel}
            :   `targetsToBuild` -

            [Returns:]{.returnLabel}
            :   exit code.

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#getCachingBuildEngine()}

        -   #### getCachingBuildEngine

            ``` methodSignature
            public CachingBuildEngine getCachingBuildEngine()
            ```

        []{#shutdown()}

        -   #### shutdown

            ``` methodSignature
            public void shutdown()
            ```

            ::: block
            Destroy any resources associated with this builder. Call
            this once only, when all buildLocallyAndReturnExitCode calls
            have finished.
            :::

        []{#getBuild()}

        -   #### getBuild

            ``` methodSignature
            public Build getBuild()
            ```
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
