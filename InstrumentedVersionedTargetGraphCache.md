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
[Package]{.packageLabelInType} [com.facebook.buck.versions](package-summary.html)
:::

## Class InstrumentedVersionedTargetGraphCache {#class-instrumentedversionedtargetgraphcache .title title="Class InstrumentedVersionedTargetGraphCache"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.versions.InstrumentedVersionedTargetGraphCache

::: description
-   

    ------------------------------------------------------------------------

        public class InstrumentedVersionedTargetGraphCache
        extends Object

    ::: block
    Wrapper class around VersionedTargetGraphCache containing a command
    specific stats tracker to track performance of the cache
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                     Description
          ----------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `InstrumentedVersionedTargetGraphCache​(VersionedTargetGraphCache cache,                                      CacheStatsTracker statsTracker)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                        Method                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          Description
          ---------------------------------------------------------------------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `CacheStats`                                                                             `getCacheStats()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                
          `com.facebook.buck.versions.VersionedTargetGraphCache.VersionedTargetGraphCacheResult`   `getVersionedTargetGraph​(DepsAwareExecutor<? super ComputeResult,​?> depsAwareExecutor,                        TypeCoercerFactory typeCoercerFactory,                        UnconfiguredBuildTargetViewFactory unconfiguredBuildTargetFactory,                        TargetGraphCreationResult targetGraphCreationResult,                        com.google.common.collect.ImmutableMap<String,​VersionUniverse> versionUniverses,                        Cells cells)`                                                          
          `TargetGraphCreationResult`                                                              `toVersionedTargetGraph​(DepsAwareExecutor<? super ComputeResult,​?> depsAwareExecutor,                       BuckConfig buckConfig,                       TypeCoercerFactory typeCoercerFactory,                       UnconfiguredBuildTargetViewFactory unconfiguredBuildTargetFactory,                       TargetGraphCreationResult targetGraphCreationResult,                       Optional<TargetConfiguration> targetConfiguration,                       BuckEventBus eventBus,                       Cells cells)`    

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

        []{#<init>(com.facebook.buck.versions.VersionedTargetGraphCache,com.facebook.buck.util.cache.CacheStatsTracker)}

        -   #### InstrumentedVersionedTargetGraphCache

                public InstrumentedVersionedTargetGraphCache​(VersionedTargetGraphCache cache,
                                                             CacheStatsTracker statsTracker)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getVersionedTargetGraph(com.facebook.buck.core.graph.transformation.executor.DepsAwareExecutor,com.facebook.buck.rules.coercer.TypeCoercerFactory,com.facebook.buck.core.parser.buildtargetparser.UnconfiguredBuildTargetViewFactory,com.facebook.buck.core.model.targetgraph.TargetGraphCreationResult,com.google.common.collect.ImmutableMap,com.facebook.buck.core.cell.Cells)}

        -   #### getVersionedTargetGraph

            ``` methodSignature
            public com.facebook.buck.versions.VersionedTargetGraphCache.VersionedTargetGraphCacheResult getVersionedTargetGraph​(DepsAwareExecutor<? super ComputeResult,​?> depsAwareExecutor,
                                                                                                                                TypeCoercerFactory typeCoercerFactory,
                                                                                                                                UnconfiguredBuildTargetViewFactory unconfiguredBuildTargetFactory,
                                                                                                                                TargetGraphCreationResult targetGraphCreationResult,
                                                                                                                                com.google.common.collect.ImmutableMap<String,​VersionUniverse> versionUniverses,
                                                                                                                                Cells cells)
                                                                                                                         throws VersionException,
                                                                                                                                InterruptedException,
                                                                                                                                TimeoutException
            ```

            [Returns:]{.returnLabel}
            :   a versioned target graph, either generated from the
                parameters or retrieved from a cache, with the current
                CacheStatsTracker.

            [Throws:]{.throwsLabel}
            :   `VersionException`
            :   `InterruptedException`
            :   `TimeoutException`

        []{#toVersionedTargetGraph(com.facebook.buck.core.graph.transformation.executor.DepsAwareExecutor,com.facebook.buck.core.config.BuckConfig,com.facebook.buck.rules.coercer.TypeCoercerFactory,com.facebook.buck.core.parser.buildtargetparser.UnconfiguredBuildTargetViewFactory,com.facebook.buck.core.model.targetgraph.TargetGraphCreationResult,java.util.Optional,com.facebook.buck.event.BuckEventBus,com.facebook.buck.core.cell.Cells)}

        -   #### toVersionedTargetGraph

            ``` methodSignature
            public TargetGraphCreationResult toVersionedTargetGraph​(DepsAwareExecutor<? super ComputeResult,​?> depsAwareExecutor,
                                                                    BuckConfig buckConfig,
                                                                    TypeCoercerFactory typeCoercerFactory,
                                                                    UnconfiguredBuildTargetViewFactory unconfiguredBuildTargetFactory,
                                                                    TargetGraphCreationResult targetGraphCreationResult,
                                                                    Optional<TargetConfiguration> targetConfiguration,
                                                                    BuckEventBus eventBus,
                                                                    Cells cells)
                                                             throws VersionException,
                                                                    InterruptedException
            ```

            [Returns:]{.returnLabel}
            :   a versioned target graph, either generated from the
                parameters or retrieved from a cache, with the current
                CacheStatsTracker

            [Throws:]{.throwsLabel}
            :   `VersionException`
            :   `InterruptedException`

        []{#getCacheStats()}

        -   #### getCacheStats

            ``` methodSignature
            public CacheStats getCacheStats()
            ```

            [Returns:]{.returnLabel}
            :   a CacheStats object containing the performance data of
                this cache
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
