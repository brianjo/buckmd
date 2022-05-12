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

-   [Overview](../../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../../index-all.html)
-   [Help](../../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.build.engine.cache.manager](package-summary.html)
:::

## Class BuildCacheArtifactFetcher {#class-buildcacheartifactfetcher .title title="Class BuildCacheArtifactFetcher"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.build.engine.cache.manager.BuildCacheArtifactFetcher

::: description
-   

    ------------------------------------------------------------------------

        public class BuildCacheArtifactFetcher
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type     Class                                             Description
          --------------------- ------------------------------------------------- -------------
          `static interface `   `BuildCacheArtifactFetcher.OnOutputsWillChange`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `BuildCacheArtifactFetcher​(BuildRule rule,                          BuildRuleScopeManager buildRuleScopeManager,                          WeightedListeningExecutorService executorService,                          BuildCacheArtifactFetcher.OnOutputsWillChange onOutputsWillChange,                          BuckEventBus eventBus,                          BuildInfoStoreManager buildInfoStoreManager,                          OnDiskBuildInfo onDiskBuildInfo)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected c          | `convertErr           | ::: block             |
        | om.google.common.util | orToSoftError​(com.goo | Converts a failed     |
        | .concurrent.Listenabl | gle.common.util.concu | `Listenabl            |
        | eFuture<CacheResult>` | rrent.ListenableFutur | eFuture<CacheResult>` |
        |                       | e<CacheResult> cacheR | to a `CacheResult`    |
        |                       | esultListenableFuture | error.                |
        |                       | ,                     | :::                   |
        |                       |     RuleKey ruleKey)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `c                    | `fetch​(ArtifactCache  |                       |
        | om.google.common.util | artifactCache,      R |                       |
        | .concurrent.Listenabl | uleKey ruleKey,       |                       |
        | eFuture<CacheResult>` | LazyPath outputPath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `c                    | `tr                   |                       |
        | om.google.common.util | yToFetchArtifactFromB |                       |
        | .concurrent.Listenabl | uildCacheAndOverlayOn |                       |
        | eFuture<CacheResult>` | TopOfProjectFilesyste |                       |
        |                       | m​(RuleKey ruleKey,    |                       |
        |                       |                       |                       |
        |                       |                       |                       |
        |                       |                       |                       |
        |                       |  ArtifactCache artifa |                       |
        |                       | ctCache,              |                       |
        |                       |                       |                       |
        |                       |                       |                       |
        |                       |             ProjectFi |                       |
        |                       | lesystem filesystem)` |                       |
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

        []{#<init>(com.facebook.buck.core.rules.BuildRule,com.facebook.buck.core.build.engine.cache.manager.BuildRuleScopeManager,com.facebook.buck.util.concurrent.WeightedListeningExecutorService,com.facebook.buck.core.build.engine.cache.manager.BuildCacheArtifactFetcher.OnOutputsWillChange,com.facebook.buck.event.BuckEventBus,com.facebook.buck.core.build.engine.cache.manager.BuildInfoStoreManager,com.facebook.buck.core.build.engine.buildinfo.OnDiskBuildInfo)}

        -   #### BuildCacheArtifactFetcher

                public BuildCacheArtifactFetcher​(BuildRule rule,
                                                 BuildRuleScopeManager buildRuleScopeManager,
                                                 WeightedListeningExecutorService executorService,
                                                 BuildCacheArtifactFetcher.OnOutputsWillChange onOutputsWillChange,
                                                 BuckEventBus eventBus,
                                                 BuildInfoStoreManager buildInfoStoreManager,
                                                 OnDiskBuildInfo onDiskBuildInfo)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#convertErrorToSoftError(com.google.common.util.concurrent.ListenableFuture,com.facebook.buck.core.rulekey.RuleKey)}

        -   #### convertErrorToSoftError

            ``` methodSignature
            protected com.google.common.util.concurrent.ListenableFuture<CacheResult> convertErrorToSoftError​(com.google.common.util.concurrent.ListenableFuture<CacheResult> cacheResultListenableFuture,
                                                                                                              RuleKey ruleKey)
            ```

            ::: block
            Converts a failed `ListenableFuture<CacheResult>` to a
            `CacheResult` error. Then logs all `CacheResult` of type
            `CacheResultType.ERROR`. Returns a
            `  ListenableFuture<CacheResult>` without an Exception.
            :::

            [Parameters:]{.paramLabel}
            :   `cacheResultListenableFuture` - ListenableFuture input
            :   `ruleKey` - rule key associated with that cache result

            [Returns:]{.returnLabel}
            :   a ListenableFuture that holds a CacheResult without
                Exception

        []{#tryToFetchArtifactFromBuildCacheAndOverlayOnTopOfProjectFilesystem(com.facebook.buck.core.rulekey.RuleKey,com.facebook.buck.artifact_cache.ArtifactCache,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### tryToFetchArtifactFromBuildCacheAndOverlayOnTopOfProjectFilesystem

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<CacheResult> tryToFetchArtifactFromBuildCacheAndOverlayOnTopOfProjectFilesystem​(RuleKey ruleKey,
                                                                                                                                                      ArtifactCache artifactCache,
                                                                                                                                                      ProjectFilesystem filesystem)
            ```

        []{#fetch(com.facebook.buck.artifact_cache.ArtifactCache,com.facebook.buck.core.rulekey.RuleKey,com.facebook.buck.io.file.LazyPath)}

        -   #### fetch

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<CacheResult> fetch​(ArtifactCache artifactCache,
                                                                                         RuleKey ruleKey,
                                                                                         LazyPath outputPath)
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

-   [Overview](../../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../../index-all.html)
-   [Help](../../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../../allclasses.html)

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
