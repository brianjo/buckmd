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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.artifact_cache](package-summary.html)
:::

## Interface ArtifactCacheEventFactory {#interface-artifactcacheeventfactory .title title="Interface ArtifactCacheEventFactory"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `AbstractArtifactCacheEventFactory`,
        `DirArtifactCacheEvent.DirArtifactCacheEventFactory`,
        `SQLiteArtifactCacheEvent.SQLiteArtifactCacheEventFactory`

    ------------------------------------------------------------------------

        public interface ArtifactCacheEventFactory
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type               Method                                                                                                                                                                 Description
          ------------------------------- ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `ArtifactCacheEvent.Finished`   `newContainsFinishedEvent​(ArtifactCacheEvent.Started started,                         Map<RuleKey,​CacheResult> results)`                                                
          `ArtifactCacheEvent.Started`    `newContainsStartedEvent​(com.google.common.collect.ImmutableSet<RuleKey> ruleKeys)`                                                                                     
          `ArtifactCacheEvent.Finished`   `newFetchFinishedEvent​(ArtifactCacheEvent.Started started,                      CacheResult cacheResult)`                                                               
          `ArtifactCacheEvent.Started`    `newFetchStartedEvent​(com.google.common.collect.ImmutableSet<RuleKey> ruleKeys)`                                                                                        
          `ArtifactCacheEvent.Finished`   `newStoreFinishedEvent​(ArtifactCacheEvent.Started started)`                                                                                                             
          `ArtifactCacheEvent.Started`    `newStoreStartedEvent​(com.google.common.collect.ImmutableSet<RuleKey> ruleKeys,                     com.google.common.collect.ImmutableMap<String,​String> metadata)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#newFetchStartedEvent(com.google.common.collect.ImmutableSet)}

        -   #### newFetchStartedEvent

            ``` methodSignature
            ArtifactCacheEvent.Started newFetchStartedEvent​(com.google.common.collect.ImmutableSet<RuleKey> ruleKeys)
            ```

        []{#newContainsStartedEvent(com.google.common.collect.ImmutableSet)}

        -   #### newContainsStartedEvent

            ``` methodSignature
            ArtifactCacheEvent.Started newContainsStartedEvent​(com.google.common.collect.ImmutableSet<RuleKey> ruleKeys)
            ```

        []{#newStoreStartedEvent(com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableMap)}

        -   #### newStoreStartedEvent

            ``` methodSignature
            ArtifactCacheEvent.Started newStoreStartedEvent​(com.google.common.collect.ImmutableSet<RuleKey> ruleKeys,
                                                            com.google.common.collect.ImmutableMap<String,​String> metadata)
            ```

        []{#newStoreFinishedEvent(com.facebook.buck.artifact_cache.ArtifactCacheEvent.Started)}

        -   #### newStoreFinishedEvent

            ``` methodSignature
            ArtifactCacheEvent.Finished newStoreFinishedEvent​(ArtifactCacheEvent.Started started)
            ```

        []{#newFetchFinishedEvent(com.facebook.buck.artifact_cache.ArtifactCacheEvent.Started,com.facebook.buck.artifact_cache.CacheResult)}

        -   #### newFetchFinishedEvent

            ``` methodSignature
            ArtifactCacheEvent.Finished newFetchFinishedEvent​(ArtifactCacheEvent.Started started,
                                                              CacheResult cacheResult)
            ```

        []{#newContainsFinishedEvent(com.facebook.buck.artifact_cache.ArtifactCacheEvent.Started,java.util.Map)}

        -   #### newContainsFinishedEvent

            ``` methodSignature
            ArtifactCacheEvent.Finished newContainsFinishedEvent​(ArtifactCacheEvent.Started started,
                                                                 Map<RuleKey,​CacheResult> results)
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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
