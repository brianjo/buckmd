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
[Package]{.packageLabelInType} [com.facebook.buck.core.build.engine.cache.manager](package-summary.html)
:::

## Class ManifestRuleKeyManager {#class-manifestrulekeymanager .title title="Class ManifestRuleKeyManager"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.build.engine.cache.manager.ManifestRuleKeyManager

::: description
-   

    ------------------------------------------------------------------------

        public class ManifestRuleKeyManager
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `ManifestRuleKeyManager​(DepFiles depFiles,                       BuildRule rule,                       FileHashLoader fileHashLoader,                       long maxDepFileCacheEntries,                       SourcePathResolverAdapter pathResolver,                       RuleKeyFactories ruleKeyFactories,                       BuildCacheArtifactFetcher buildCacheArtifactFetcher,                       ArtifactCache artifactCache,                       java.util.function.Supplier<Optional<DependencyFileRuleKeyFactory.RuleKeyAndInputs>> manifestBasedKeySupplier,                       ManifestRuleKeyService manifestRuleKeyService)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                           Method                                                                                                                                                                                                                                                    Description
          --------------------------------------------------------------------------- --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `Optional<DependencyFileRuleKeyFactory.RuleKeyAndInputs>`                   `calculateManifestKey​(BuckEventBus eventBus)`                                                                                                                                                                                                              
          `com.google.common.util.concurrent.ListenableFuture<CacheResult>`           `fetchManifest​(RuleKey key)`                                                                                                                                                                                                                               
          `static Path`                                                               `getManifestPath​(BuildRule rule)`                                                                                                                                                                                                                          
          `ManifestLoadResult`                                                        `loadManifest​(RuleKey key)`                                                                                                                                                                                                                                
          `com.google.common.util.concurrent.ListenableFuture<ManifestFetchResult>`   `performManifestBasedCacheFetch​(DependencyFileRuleKeyFactory.RuleKeyAndInputs originalRuleKeyAndInputs)`                                                                                                                                                   
          `ManifestStoreResult`                                                       `updateAndStoreManifest​(RuleKey key,                       com.google.common.collect.ImmutableSet<SourcePath> inputs,                       DependencyFileRuleKeyFactory.RuleKeyAndInputs manifestKey,                       long artifactBuildTimeMs)`    
          `boolean`                                                                   `useManifestCaching()`                                                                                                                                                                                                                                     

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
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

        []{#<init>(com.facebook.buck.core.build.engine.type.DepFiles,com.facebook.buck.core.rules.BuildRule,com.facebook.buck.util.hashing.FileHashLoader,long,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.facebook.buck.rules.keys.RuleKeyFactories,com.facebook.buck.core.build.engine.cache.manager.BuildCacheArtifactFetcher,com.facebook.buck.artifact_cache.ArtifactCache,java.util.function.Supplier,com.facebook.buck.core.build.engine.cache.manager.ManifestRuleKeyService)}

        -   #### ManifestRuleKeyManager

                public ManifestRuleKeyManager​(DepFiles depFiles,
                                              BuildRule rule,
                                              FileHashLoader fileHashLoader,
                                              long maxDepFileCacheEntries,
                                              SourcePathResolverAdapter pathResolver,
                                              RuleKeyFactories ruleKeyFactories,
                                              BuildCacheArtifactFetcher buildCacheArtifactFetcher,
                                              ArtifactCache artifactCache,
                                              java.util.function.Supplier<Optional<DependencyFileRuleKeyFactory.RuleKeyAndInputs>> manifestBasedKeySupplier,
                                              ManifestRuleKeyService manifestRuleKeyService)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#useManifestCaching()}

        -   #### useManifestCaching

            ``` methodSignature
            public boolean useManifestCaching()
            ```

        []{#getManifestPath(com.facebook.buck.core.rules.BuildRule)}

        -   #### getManifestPath

            ``` methodSignature
            public static Path getManifestPath​(BuildRule rule)
            ```

        []{#updateAndStoreManifest(com.facebook.buck.core.rulekey.RuleKey,com.google.common.collect.ImmutableSet,com.facebook.buck.rules.keys.DependencyFileRuleKeyFactory.RuleKeyAndInputs,long)}

        -   #### updateAndStoreManifest

            ``` methodSignature
            public ManifestStoreResult updateAndStoreManifest​(RuleKey key,
                                                              com.google.common.collect.ImmutableSet<SourcePath> inputs,
                                                              DependencyFileRuleKeyFactory.RuleKeyAndInputs manifestKey,
                                                              long artifactBuildTimeMs)
                                                       throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#calculateManifestKey(com.facebook.buck.event.BuckEventBus)}

        -   #### calculateManifestKey

            ``` methodSignature
            public Optional<DependencyFileRuleKeyFactory.RuleKeyAndInputs> calculateManifestKey​(BuckEventBus eventBus)
                                                                                         throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#fetchManifest(com.facebook.buck.core.rulekey.RuleKey)}

        -   #### fetchManifest

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<CacheResult> fetchManifest​(RuleKey key)
            ```

        []{#loadManifest(com.facebook.buck.core.rulekey.RuleKey)}

        -   #### loadManifest

            ``` methodSignature
            public ManifestLoadResult loadManifest​(RuleKey key)
            ```

        []{#performManifestBasedCacheFetch(com.facebook.buck.rules.keys.DependencyFileRuleKeyFactory.RuleKeyAndInputs)}

        -   #### performManifestBasedCacheFetch

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<ManifestFetchResult> performManifestBasedCacheFetch​(DependencyFileRuleKeyFactory.RuleKeyAndInputs originalRuleKeyAndInputs)
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
