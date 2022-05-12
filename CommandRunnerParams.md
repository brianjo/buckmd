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
[Package]{.packageLabelInType} [com.facebook.buck.cli](package-summary.html)
:::

## Class CommandRunnerParams {#class-commandrunnerparams .title title="Class CommandRunnerParams"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cli.CommandRunnerParams

::: description
-   

    ------------------------------------------------------------------------

        public abstract class CommandRunnerParams
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor               Description
          ------------------------- -------------
          `CommandRunnerParams()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `BuildExecutorArgs`   | `createBuilderArgs()` | ::: block             |
        |                       |                       | Create                |
        |                       |                       | [`BuildEx             |
        |                       |                       | ecutorArgs`](../comma |
        |                       |                       | nd/BuildExecutorArgs. |
        |                       |                       | html "class in com.fa |
        |                       |                       | cebook.buck.command") |
        |                       |                       | using this            |
        |                       |                       | [`CommandRunnerParam  |
        |                       |                       | s`](CommandRunnerPara |
        |                       |                       | ms.html "class in com |
        |                       |                       | .facebook.buck.cli"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract             | `getA                 |                       |
        |  ActionGraphProvider` | ctionGraphProvider()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract             | `getAr                |                       |
        | ArtifactCacheFactory` | tifactCacheFactory()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract BuckConfig` | `getBuckConfig()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `a                    | `getBuckEventBus()`   |                       |
        | bstract BuckEventBus` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstra               | `ge                   |                       |
        | ct BuckModuleManager` | tBuckModuleManager()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract BuildEn     | `getBuildEnvi         |                       |
        | vironmentDescription` | ronmentDescription()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract B           | `getBui               |                       |
        | uildInfoStoreManager` | ldInfoStoreManager()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Cells`      | `getCells()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Path`       | `g                    |                       |
        |                       | etClientWorkingDir()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Clock`      | `getClock()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Console`    | `getConsole()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstrac              | `getDefaultRuleKeyFa  |                       |
        | t Optional<RuleKeyCac | ctoryCacheRecycler()` |                       |
        | heRecycler<RuleKey>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Closeab     | `getDepsAwa           |                       |
        | leMemoizedSupplier<De | reExecutorSupplier()` |                       |
        | psAwareExecutor<? sup |                       |                       |
        | er ComputeResult,​?>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getEnvironment()`    |                       |
        | abstract com.google.c |                       |                       |
        | ommon.collect.Immutab |                       |                       |
        | leMap<String,​String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstr                | `g                    |                       |
        | act ExecutableFinder` | etExecutableFinder()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com.goo     | `getExecutors()`      |                       |
        | gle.common.collect.Im |                       |                       |
        | mutableMap<ExecutorPo |                       |                       |
        | ol,​com.google.common. |                       |                       |
        | util.concurrent.Liste |                       |                       |
        | ningExecutorService>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract             | `getFileHashCache()`  |                       |
        | StackedFileHashCache` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abst                 | `getGlobalState()`    |                       |
        | ract BuckGlobalState` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Optional<   | `ge                   |                       |
        | TargetConfiguration>` | tHostConfiguration()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Opti        | `getInvocationInfo()` |                       |
        | onal<InvocationInfo>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstra               | `ge                   |                       |
        | ct JavaPackageFinder` | tJavaPackageFinder()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Kn          | `getKnow              |                       |
        | ownRuleTypesProvider` | nRuleTypesProvider()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstr                | `g                    |                       |
        | act MetadataProvider` | etMetadataProvider()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Parser`     | `getParser()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstrac              | `getPer               |                       |
        | t ConcurrentMap<Strin | sistentWorkerPools()` |                       |
        | g,​WorkerProcessPool>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Platform`   | `getPlatform()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract or          | `getPluginManager()`  |                       |
        | g.pf4j.PluginManager` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abst                 | `                     |                       |
        | ract ProcessExecutor` | getProcessExecutor()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Opti        | `getProcessManager()` |                       |
        | onal<ProcessManager>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Proj        | `getProjec            |                       |
        | ectFilesystemFactory` | tFilesystemFactory()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract             | `getRu                |                       |
        | RuleKeyConfiguration` | leKeyConfiguration()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Sche        | `ge                   |                       |
        | duledExecutorService` | tScheduledExecutor()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getStdIn()`          |                       |
        | abstract InputStream` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Optional<   | `getT                 |                       |
        | TargetConfiguration>` | argetConfiguration()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract TargetCon   | `getTargetConfi       |                       |
        | figurationSerializer` | gurationSerializer()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstrac              | `get                  |                       |
        | t TypeCoercerFactory` | TypeCoercerFactory()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ab                   | `getUnconfigured      |                       |
        | stract UnconfiguredBu | BuildTargetFactory()` |                       |
        | ildTargetViewFactory` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract VersionC    | `getVersionCon        |                       |
        | ontrolStatsGenerator` | trolStatsGenerator()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstr                | `getVersion           |                       |
        | act InstrumentedVersi | edTargetGraphCache()` |                       |
        | onedTargetGraphCache` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Watchman`   | `getWatchman()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract             | `getWebServer()`      |                       |
        |  Optional<WebServer>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `CommandRunnerParams` | `withA                |                       |
        |                       | rtifactCacheFactory​(A |                       |
        |                       | rtifactCacheFactory a |                       |
        |                       | rtifactCacheFactory)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `CommandRunnerParams` | `withBuckConfig​(Bu    |                       |
        |                       | ckConfig buckConfig)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

        []{#<init>()}

        -   #### CommandRunnerParams

                public CommandRunnerParams()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getConsole()}

        -   #### getConsole

            ``` methodSignature
            public abstract Console getConsole()
            ```

        []{#getStdIn()}

        -   #### getStdIn

            ``` methodSignature
            public abstract InputStream getStdIn()
            ```

        []{#getCells()}

        -   #### getCells

            ``` methodSignature
            public abstract Cells getCells()
            ```

        []{#getWatchman()}

        -   #### getWatchman

            ``` methodSignature
            public abstract Watchman getWatchman()
            ```

        []{#getVersionedTargetGraphCache()}

        -   #### getVersionedTargetGraphCache

            ``` methodSignature
            public abstract InstrumentedVersionedTargetGraphCache getVersionedTargetGraphCache()
            ```

        []{#getArtifactCacheFactory()}

        -   #### getArtifactCacheFactory

            ``` methodSignature
            public abstract ArtifactCacheFactory getArtifactCacheFactory()
            ```

        []{#getTypeCoercerFactory()}

        -   #### getTypeCoercerFactory

            ``` methodSignature
            public abstract TypeCoercerFactory getTypeCoercerFactory()
            ```

        []{#getUnconfiguredBuildTargetFactory()}

        -   #### getUnconfiguredBuildTargetFactory

            ``` methodSignature
            public abstract UnconfiguredBuildTargetViewFactory getUnconfiguredBuildTargetFactory()
            ```

        []{#getTargetConfiguration()}

        -   #### getTargetConfiguration

            ``` methodSignature
            public abstract Optional<TargetConfiguration> getTargetConfiguration()
            ```

        []{#getHostConfiguration()}

        -   #### getHostConfiguration

            ``` methodSignature
            public abstract Optional<TargetConfiguration> getHostConfiguration()
            ```

        []{#getTargetConfigurationSerializer()}

        -   #### getTargetConfigurationSerializer

            ``` methodSignature
            public abstract TargetConfigurationSerializer getTargetConfigurationSerializer()
            ```

        []{#getParser()}

        -   #### getParser

            ``` methodSignature
            public abstract Parser getParser()
            ```

        []{#getBuckEventBus()}

        -   #### getBuckEventBus

            ``` methodSignature
            public abstract BuckEventBus getBuckEventBus()
            ```

        []{#getPlatform()}

        -   #### getPlatform

            ``` methodSignature
            public abstract Platform getPlatform()
            ```

        []{#getEnvironment()}

        -   #### getEnvironment

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<String,​String> getEnvironment()
            ```

        []{#getJavaPackageFinder()}

        -   #### getJavaPackageFinder

            ``` methodSignature
            public abstract JavaPackageFinder getJavaPackageFinder()
            ```

        []{#getClock()}

        -   #### getClock

            ``` methodSignature
            public abstract Clock getClock()
            ```

        []{#getVersionControlStatsGenerator()}

        -   #### getVersionControlStatsGenerator

            ``` methodSignature
            public abstract VersionControlStatsGenerator getVersionControlStatsGenerator()
            ```

        []{#getProcessManager()}

        -   #### getProcessManager

            ``` methodSignature
            public abstract Optional<ProcessManager> getProcessManager()
            ```

        []{#getWebServer()}

        -   #### getWebServer

            ``` methodSignature
            public abstract Optional<WebServer> getWebServer()
            ```

        []{#getPersistentWorkerPools()}

        -   #### getPersistentWorkerPools

            ``` methodSignature
            public abstract ConcurrentMap<String,​WorkerProcessPool> getPersistentWorkerPools()
            ```

        []{#getBuckConfig()}

        -   #### getBuckConfig

            ``` methodSignature
            public abstract BuckConfig getBuckConfig()
            ```

        []{#getFileHashCache()}

        -   #### getFileHashCache

            ``` methodSignature
            public abstract StackedFileHashCache getFileHashCache()
            ```

        []{#getExecutors()}

        -   #### getExecutors

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<ExecutorPool,​com.google.common.util.concurrent.ListeningExecutorService> getExecutors()
            ```

        []{#getScheduledExecutor()}

        -   #### getScheduledExecutor

            ``` methodSignature
            public abstract ScheduledExecutorService getScheduledExecutor()
            ```

        []{#getBuildEnvironmentDescription()}

        -   #### getBuildEnvironmentDescription

            ``` methodSignature
            public abstract BuildEnvironmentDescription getBuildEnvironmentDescription()
            ```

        []{#getActionGraphProvider()}

        -   #### getActionGraphProvider

            ``` methodSignature
            public abstract ActionGraphProvider getActionGraphProvider()
            ```

        []{#getKnownRuleTypesProvider()}

        -   #### getKnownRuleTypesProvider

            ``` methodSignature
            public abstract KnownRuleTypesProvider getKnownRuleTypesProvider()
            ```

        []{#getBuildInfoStoreManager()}

        -   #### getBuildInfoStoreManager

            ``` methodSignature
            public abstract BuildInfoStoreManager getBuildInfoStoreManager()
            ```

        []{#getInvocationInfo()}

        -   #### getInvocationInfo

            ``` methodSignature
            public abstract Optional<InvocationInfo> getInvocationInfo()
            ```

        []{#getDefaultRuleKeyFactoryCacheRecycler()}

        -   #### getDefaultRuleKeyFactoryCacheRecycler

            ``` methodSignature
            public abstract Optional<RuleKeyCacheRecycler<RuleKey>> getDefaultRuleKeyFactoryCacheRecycler()
            ```

        []{#getProjectFilesystemFactory()}

        -   #### getProjectFilesystemFactory

            ``` methodSignature
            public abstract ProjectFilesystemFactory getProjectFilesystemFactory()
            ```

        []{#getRuleKeyConfiguration()}

        -   #### getRuleKeyConfiguration

            ``` methodSignature
            public abstract RuleKeyConfiguration getRuleKeyConfiguration()
            ```

        []{#getProcessExecutor()}

        -   #### getProcessExecutor

            ``` methodSignature
            public abstract ProcessExecutor getProcessExecutor()
            ```

        []{#getExecutableFinder()}

        -   #### getExecutableFinder

            ``` methodSignature
            public abstract ExecutableFinder getExecutableFinder()
            ```

        []{#getPluginManager()}

        -   #### getPluginManager

            ``` methodSignature
            public abstract org.pf4j.PluginManager getPluginManager()
            ```

        []{#getBuckModuleManager()}

        -   #### getBuckModuleManager

            ``` methodSignature
            public abstract BuckModuleManager getBuckModuleManager()
            ```

        []{#getDepsAwareExecutorSupplier()}

        -   #### getDepsAwareExecutorSupplier

            ``` methodSignature
            public abstract CloseableMemoizedSupplier<DepsAwareExecutor<? super ComputeResult,​?>> getDepsAwareExecutorSupplier()
            ```

        []{#getMetadataProvider()}

        -   #### getMetadataProvider

            ``` methodSignature
            public abstract MetadataProvider getMetadataProvider()
            ```

        []{#getGlobalState()}

        -   #### getGlobalState

            ``` methodSignature
            public abstract BuckGlobalState getGlobalState()
            ```

            [Returns:]{.returnLabel}
            :   [`BuckGlobalState`](../support/state/BuckGlobalState.html "class in com.facebook.buck.support.state")
                object which is a set of objects bearing the data
                reflecting filesystem state and thus shared between
                commands

        []{#getClientWorkingDir()}

        -   #### getClientWorkingDir

            ``` methodSignature
            public abstract Path getClientWorkingDir()
            ```

            [Returns:]{.returnLabel}

            :   the original absolute PWD for the client

                NOTE: This is the path the the user was in when they
                invoked buck. The buck wrapper executes buck from the
                project root, so this is not the same as most `getCwd()`
                style functions.

        []{#createBuilderArgs()}

        -   #### createBuilderArgs

            ``` methodSignature
            public BuildExecutorArgs createBuilderArgs()
            ```

            ::: block
            Create
            [`BuildExecutorArgs`](../command/BuildExecutorArgs.html "class in com.facebook.buck.command")
            using this
            [`CommandRunnerParams`](CommandRunnerParams.html "class in com.facebook.buck.cli").
            :::

            [Returns:]{.returnLabel}
            :   New instance of
                [`BuildExecutorArgs`](../command/BuildExecutorArgs.html "class in com.facebook.buck.command").

        []{#withArtifactCacheFactory(com.facebook.buck.artifact_cache.ArtifactCacheFactory)}

        -   #### withArtifactCacheFactory

            ``` methodSignature
            public CommandRunnerParams withArtifactCacheFactory​(ArtifactCacheFactory artifactCacheFactory)
            ```

        []{#withBuckConfig(com.facebook.buck.core.config.BuckConfig)}

        -   #### withBuckConfig

            ``` methodSignature
            public CommandRunnerParams withBuckConfig​(BuckConfig buckConfig)
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
