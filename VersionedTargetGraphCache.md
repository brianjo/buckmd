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

## Class VersionedTargetGraphCache {#class-versionedtargetgraphcache .title title="Class VersionedTargetGraphCache"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.versions.VersionedTargetGraphCache

::: description
-   

    ------------------------------------------------------------------------

        public class VersionedTargetGraphCache
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `VersionedTargetG     | ::: block             |
        |                       | raphCache.ResultType` | The possible result   |
        |                       |                       | types using the       |
        |                       |                       | cache.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                     Description
          ------------------------------- -------------
          `VersionedTargetGraphCache()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                        Method                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         Description
          ---------------------------------------------------------------------------------------- ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `com.facebook.buck.versions.VersionedTargetGraphCache.VersionedTargetGraphCacheResult`   `getVersionedTargetGraph​(DepsAwareExecutor<? super ComputeResult,​?> depsAwareExecutor,                        BuckConfig buckConfig,                        TypeCoercerFactory typeCoercerFactory,                        UnconfiguredBuildTargetViewFactory unconfiguredBuildTargetFactory,                        TargetGraphCreationResult targetGraphCreationResult,                        Optional<TargetConfiguration> targetConfiguration,                        CacheStatsTracker statsTracker,                        BuckEventBus eventBus,                        Cells cells)`    
          `com.facebook.buck.versions.VersionedTargetGraphCache.VersionedTargetGraphCacheResult`   `toVersionedTargetGraph​(DepsAwareExecutor<? super ComputeResult,​?> depsAwareExecutor,                       com.google.common.collect.ImmutableMap<String,​VersionUniverse> versionUniverses,                       TypeCoercerFactory typeCoercerFactory,                       UnconfiguredBuildTargetViewFactory unconfiguredBuildTargetFactory,                       TargetGraphCreationResult targetGraphCreationResult,                       CacheStatsTracker statsTracker,                       Cells cells)`                                                                         

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

        []{#<init>()}

        -   #### VersionedTargetGraphCache

                public VersionedTargetGraphCache()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getVersionedTargetGraph(com.facebook.buck.core.graph.transformation.executor.DepsAwareExecutor,com.facebook.buck.core.config.BuckConfig,com.facebook.buck.rules.coercer.TypeCoercerFactory,com.facebook.buck.core.parser.buildtargetparser.UnconfiguredBuildTargetViewFactory,com.facebook.buck.core.model.targetgraph.TargetGraphCreationResult,java.util.Optional,com.facebook.buck.util.cache.CacheStatsTracker,com.facebook.buck.event.BuckEventBus,com.facebook.buck.core.cell.Cells)}

        -   #### getVersionedTargetGraph

            ``` methodSignature
            public com.facebook.buck.versions.VersionedTargetGraphCache.VersionedTargetGraphCacheResult getVersionedTargetGraph​(DepsAwareExecutor<? super ComputeResult,​?> depsAwareExecutor,
                                                                                                                                BuckConfig buckConfig,
                                                                                                                                TypeCoercerFactory typeCoercerFactory,
                                                                                                                                UnconfiguredBuildTargetViewFactory unconfiguredBuildTargetFactory,
                                                                                                                                TargetGraphCreationResult targetGraphCreationResult,
                                                                                                                                Optional<TargetConfiguration> targetConfiguration,
                                                                                                                                CacheStatsTracker statsTracker,
                                                                                                                                BuckEventBus eventBus,
                                                                                                                                Cells cells)
                                                                                                                         throws VersionException,
                                                                                                                                InterruptedException
            ```

            [Returns:]{.returnLabel}
            :   a versioned target graph, either generated from the
                parameters or retrieved from a cache.

            [Throws:]{.throwsLabel}
            :   `VersionException`
            :   `InterruptedException`

        []{#toVersionedTargetGraph(com.facebook.buck.core.graph.transformation.executor.DepsAwareExecutor,com.google.common.collect.ImmutableMap,com.facebook.buck.rules.coercer.TypeCoercerFactory,com.facebook.buck.core.parser.buildtargetparser.UnconfiguredBuildTargetViewFactory,com.facebook.buck.core.model.targetgraph.TargetGraphCreationResult,com.facebook.buck.util.cache.CacheStatsTracker,com.facebook.buck.core.cell.Cells)}

        -   #### toVersionedTargetGraph

            ``` methodSignature
            public com.facebook.buck.versions.VersionedTargetGraphCache.VersionedTargetGraphCacheResult toVersionedTargetGraph​(DepsAwareExecutor<? super ComputeResult,​?> depsAwareExecutor,
                                                                                                                               com.google.common.collect.ImmutableMap<String,​VersionUniverse> versionUniverses,
                                                                                                                               TypeCoercerFactory typeCoercerFactory,
                                                                                                                               UnconfiguredBuildTargetViewFactory unconfiguredBuildTargetFactory,
                                                                                                                               TargetGraphCreationResult targetGraphCreationResult,
                                                                                                                               CacheStatsTracker statsTracker,
                                                                                                                               Cells cells)
                                                                                                                        throws VersionException,
                                                                                                                               InterruptedException,
                                                                                                                               TimeoutException
            ```

            [Throws:]{.throwsLabel}
            :   `VersionException`
            :   `InterruptedException`
            :   `TimeoutException`
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
