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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.build.engine.impl](package-summary.html)
:::

## Class CachingBuildEngine {#class-cachingbuildengine .title title="Class CachingBuildEngine"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.build.engine.impl.CachingBuildEngine

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngine`, `Closeable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class CachingBuildEngine
        extends Object
        implements BuildEngine, Closeable

    ::: block
    A build engine used to build a
    [`BuildRule`](../../../rules/BuildRule.html "interface in com.facebook.buck.core.rules")
    which also caches the results. If the current
    [`RuleKey`](../../../rulekey/RuleKey.html "class in com.facebook.buck.core.rulekey")
    of the build rules matches the one on disk, it does not do any work.
    It also tries to fetch its output from an
    [`ArtifactCache`](../../../../artifact_cache/ArtifactCache.html "interface in com.facebook.buck.artifact_cache")
    to avoid doing any computation.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                                                  Description
          ------------------- ------------------------------------------------------ -------------
          `static class `     `CachingBuildEngine.DefaultBuildRuleBuilderDelegate`    

          : Nested Classes[ ]{.tabEnd}

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.core.build.engine.BuildEngine}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.core.build.engine.[BuildEngine](../BuildEngine.html "interface in com.facebook.buck.core.build.engine")

            `BuildEngine.BuildEngineResult`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type          Field                                     Description
          -------------------------- ----------------------------------------- -------------
          `static ResourceAmounts`   `CACHE_CHECK_RESOURCE_AMOUNTS`             
          `static ResourceAmounts`   `RULE_KEY_COMPUTATION_RESOURCE_AMOUNTS`    
          `static ResourceAmounts`   `SCHEDULING_MORE_WORK_RESOURCE_AMOUNTS`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 Description
          --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `CachingBuildEngine​(CachingBuildEngineDelegate cachingBuildEngineDelegate,                   Optional<BuildRuleStrategy> customBuildRuleStrategy,                   WeightedListeningExecutorService service,                   BuildType buildMode,                   DepFiles depFiles,                   long maxDepFileCacheEntries,                   Optional<Long> artifactCacheSizeLimit,                   BuildRuleResolver resolver,                   BuildEngineActionToBuildRuleResolver actionToBuildRuleResolver,                   TargetConfigurationSerializer targetConfigurationSerializer,                   BuildInfoStoreManager buildInfoStoreManager,                   ResourceAwareSchedulingInfo resourceAwareSchedulingInfo,                   boolean consoleLogBuildFailuresInline,                   RuleKeyFactories ruleKeyFactories)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `BuildEngi            | `                     | ::: block             |
        | ne.BuildEngineResult` | build​(BuildEngineBuil | Build the given build |
        |                       | dContext buildContext | rule and return a     |
        |                       | ,      ExecutionConte | future to the build   |
        |                       | xt executionContext,  | rule success.         |
        |                       |      BuildRule rule)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `close()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildResult`         | `ge                   | ::: block             |
        |                       | tBuildRuleResult​(Buil | Returns the build     |
        |                       | dTarget buildTarget)` | result of the build   |
        |                       |                       | rule associated with  |
        |                       |                       | the given build       |
        |                       |                       | target.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getN                 | ::: block             |
        |                       | umRulesToBuild​(Iterab | Calculate the total   |
        |                       | le<BuildRule> rules)` | number of transitive  |
        |                       |                       | build rules processed |
        |                       |                       | from the given roots. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ParallelRuleKe       | `ge                   |                       |
        | yCalculator<RuleKey>` | tRuleKeyCalculator()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isRuleBuilt​(Buil     | ::: block             |
        |                       | dTarget buildTarget)` | Returns whether the   |
        |                       |                       | build rule associated |
        |                       |                       | with the build target |
        |                       |                       | has been successfully |
        |                       |                       | built.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `ter                  | ::: block             |
        |                       | minateBuildWithFailur | Marks build as failed |
        |                       | e​(Throwable failure)` | with the given        |
        |                       |                       | Throwable.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `walkRule​(Bui         |                       |
        | ommon.util.concurrent | ldRule rule,          |                       |
        | .ListenableFuture<?>` | Set<BuildRule> seen)` |                       |
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
    -   []{#field.detail}

        ### Field Detail

        []{#CACHE_CHECK_RESOURCE_AMOUNTS}

        -   #### CACHE_CHECK_RESOURCE_AMOUNTS

                public static final ResourceAmounts CACHE_CHECK_RESOURCE_AMOUNTS

        []{#RULE_KEY_COMPUTATION_RESOURCE_AMOUNTS}

        -   #### RULE_KEY_COMPUTATION_RESOURCE_AMOUNTS

                public static final ResourceAmounts RULE_KEY_COMPUTATION_RESOURCE_AMOUNTS

        []{#SCHEDULING_MORE_WORK_RESOURCE_AMOUNTS}

        -   #### SCHEDULING_MORE_WORK_RESOURCE_AMOUNTS

                public static final ResourceAmounts SCHEDULING_MORE_WORK_RESOURCE_AMOUNTS
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.build.engine.delegate.CachingBuildEngineDelegate,java.util.Optional,com.facebook.buck.util.concurrent.WeightedListeningExecutorService,com.facebook.buck.core.build.engine.type.BuildType,com.facebook.buck.core.build.engine.type.DepFiles,long,java.util.Optional,com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.core.build.action.resolver.BuildEngineActionToBuildRuleResolver,com.facebook.buck.core.model.TargetConfigurationSerializer,com.facebook.buck.core.build.engine.cache.manager.BuildInfoStoreManager,com.facebook.buck.core.build.engine.config.ResourceAwareSchedulingInfo,boolean,com.facebook.buck.rules.keys.RuleKeyFactories)}

        -   #### CachingBuildEngine

                public CachingBuildEngine​(CachingBuildEngineDelegate cachingBuildEngineDelegate,
                                          Optional<BuildRuleStrategy> customBuildRuleStrategy,
                                          WeightedListeningExecutorService service,
                                          BuildType buildMode,
                                          DepFiles depFiles,
                                          long maxDepFileCacheEntries,
                                          Optional<Long> artifactCacheSizeLimit,
                                          BuildRuleResolver resolver,
                                          BuildEngineActionToBuildRuleResolver actionToBuildRuleResolver,
                                          TargetConfigurationSerializer targetConfigurationSerializer,
                                          BuildInfoStoreManager buildInfoStoreManager,
                                          ResourceAwareSchedulingInfo resourceAwareSchedulingInfo,
                                          boolean consoleLogBuildFailuresInline,
                                          RuleKeyFactories ruleKeyFactories)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `Closeable`

        []{#getRuleKeyCalculator()}

        -   #### getRuleKeyCalculator

            ``` methodSignature
            public ParallelRuleKeyCalculator<RuleKey> getRuleKeyCalculator()
            ```

        []{#isRuleBuilt(com.facebook.buck.core.model.BuildTarget)}

        -   #### isRuleBuilt

            ``` methodSignature
            public boolean isRuleBuilt​(BuildTarget buildTarget)
                                throws InterruptedException
            ```

            ::: block
            [Description copied from
            interface: `BuildEngine`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns whether the build rule associated with the build
            target has been successfully built.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `isRuleBuilt` in interface `BuildEngine`

            [Throws:]{.throwsLabel}
            :   `InterruptedException`

        []{#terminateBuildWithFailure(java.lang.Throwable)}

        -   #### terminateBuildWithFailure

            ``` methodSignature
            public void terminateBuildWithFailure​(Throwable failure)
            ```

            ::: block
            [Description copied from
            interface: `BuildEngine`]{.descfrmTypeLabel}
            :::

            ::: block
            Marks build as failed with the given Throwable. If keepGoing
            == false, any pending steps will be terminated before
            starting.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `terminateBuildWithFailure` in interface `BuildEngine`

        []{#walkRule(com.facebook.buck.core.rules.BuildRule,java.util.Set)}

        -   #### walkRule

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<?> walkRule​(BuildRule rule,
                                                                                  Set<BuildRule> seen)
            ```

        []{#getNumRulesToBuild(java.lang.Iterable)}

        -   #### getNumRulesToBuild

            ``` methodSignature
            public int getNumRulesToBuild​(Iterable<BuildRule> rules)
            ```

            ::: block
            [Description copied from
            interface: `BuildEngine`]{.descfrmTypeLabel}
            :::

            ::: block
            Calculate the total number of transitive build rules
            processed from the given roots.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNumRulesToBuild` in interface `BuildEngine`

        []{#build(com.facebook.buck.core.build.engine.BuildEngineBuildContext,com.facebook.buck.core.build.execution.context.ExecutionContext,com.facebook.buck.core.rules.BuildRule)}

        -   #### build

            ``` methodSignature
            public BuildEngine.BuildEngineResult build​(BuildEngineBuildContext buildContext,
                                                       ExecutionContext executionContext,
                                                       BuildRule rule)
            ```

            ::: block
            [Description copied from
            interface: `BuildEngine`]{.descfrmTypeLabel}
            :::

            ::: block
            Build the given build rule and return a future to the build
            rule success.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `build` in interface `BuildEngine`

        []{#getBuildRuleResult(com.facebook.buck.core.model.BuildTarget)}

        -   #### getBuildRuleResult

            ``` methodSignature
            @Nullable
            public BuildResult getBuildRuleResult​(BuildTarget buildTarget)
                                           throws ExecutionException,
                                                  InterruptedException
            ```

            ::: block
            [Description copied from
            interface: `BuildEngine`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the build result of the build rule associated with
            the given build target. Returns `null` if the build rule has
            not yet been built.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildRuleResult` in interface `BuildEngine`

            [Throws:]{.throwsLabel}
            :   `ExecutionException`
            :   `InterruptedException`
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
