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

## Class BuildCacheArtifactUploader {#class-buildcacheartifactuploader .title title="Class BuildCacheArtifactUploader"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.build.engine.cache.manager.BuildCacheArtifactUploader

::: description
-   

    ------------------------------------------------------------------------

        public class BuildCacheArtifactUploader
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `BuildCacheArtifactUploader​(RuleKey defaultKey,                           java.util.function.Supplier<Optional<RuleKey>> inputBasedKey,                           OnDiskBuildInfo onDiskBuildInfo,                           BuildRule rule,                           ManifestRuleKeyManager manifestRuleKeyManager,                           BuckEventBus eventBus,                           ArtifactCache artifactCache,                           Optional<Long> artifactCacheSizeLimit)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Upl                  | `should               |                       |
        | oadToCacheResultType` | UploadToCache​(BuildRu |                       |
        |                       | leSuccessType success |                       |
        |                       | Type,                 |                       |
        |                       |     long outputSize)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.comm      | `uploadToCach         | ::: block             |
        | on.util.concurrent.Li | e​(BuildRuleSuccessTyp | Perform an actual     |
        | stenableFuture<Unit>` | e success,            | write to a cache      |
        |                       |    long buildTimeMs)` | :::                   |
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

        []{#<init>(com.facebook.buck.core.rulekey.RuleKey,java.util.function.Supplier,com.facebook.buck.core.build.engine.buildinfo.OnDiskBuildInfo,com.facebook.buck.core.rules.BuildRule,com.facebook.buck.core.build.engine.cache.manager.ManifestRuleKeyManager,com.facebook.buck.event.BuckEventBus,com.facebook.buck.artifact_cache.ArtifactCache,java.util.Optional)}

        -   #### BuildCacheArtifactUploader

                public BuildCacheArtifactUploader​(RuleKey defaultKey,
                                                  java.util.function.Supplier<Optional<RuleKey>> inputBasedKey,
                                                  OnDiskBuildInfo onDiskBuildInfo,
                                                  BuildRule rule,
                                                  ManifestRuleKeyManager manifestRuleKeyManager,
                                                  BuckEventBus eventBus,
                                                  ArtifactCache artifactCache,
                                                  Optional<Long> artifactCacheSizeLimit)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#uploadToCache(com.facebook.buck.core.build.engine.BuildRuleSuccessType,long)}

        -   #### uploadToCache

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<Unit> uploadToCache​(BuildRuleSuccessType success,
                                                                                          long buildTimeMs)
                                                                                   throws IOException
            ```

            ::: block
            Perform an actual write to a cache
            :::

            [Parameters:]{.paramLabel}
            :   `success` - outcome of a build rule
            :   `buildTimeMs` - time it took to actually build a rule

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#shouldUploadToCache(com.facebook.buck.core.build.engine.BuildRuleSuccessType,long)}

        -   #### shouldUploadToCache

            ``` methodSignature
            public UploadToCacheResultType shouldUploadToCache​(BuildRuleSuccessType successType,
                                                               long outputSize)
            ```

            [Returns:]{.returnLabel}
            :   whether we should upload the given rules artifacts to
                cache.
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
