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
[Package]{.packageLabelInType} [com.facebook.buck.artifact_cache](package-summary.html)
:::

## Class SQLiteArtifactCacheEvent.SQLiteArtifactCacheEventFactory {#class-sqliteartifactcacheevent.sqliteartifactcacheeventfactory .title title="Class SQLiteArtifactCacheEvent.SQLiteArtifactCacheEventFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.artifact_cache.AbstractArtifactCacheEventFactory](AbstractArtifactCacheEventFactory.html "class in com.facebook.buck.artifact_cache")

    -   -   com.facebook.buck.artifact_cache.SQLiteArtifactCacheEvent.SQLiteArtifactCacheEventFactory

::: description
-   

    All Implemented Interfaces:
    :   `ArtifactCacheEventFactory`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [SQLiteArtifactCacheEvent](SQLiteArtifactCacheEvent.html "class in com.facebook.buck.artifact_cache")

    ------------------------------------------------------------------------

        public static class SQLiteArtifactCacheEvent.SQLiteArtifactCacheEventFactory
        extends AbstractArtifactCacheEventFactory
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                                                                                                                                                                                 Description
          -------------- --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `protected `   `SQLiteArtifactCacheEventFactory​(java.util.function.Function<String,​UnconfiguredBuildTarget> unconfiguredBuildTargetFactory,                                TargetConfigurationSerializer targetConfigurationSerializer)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                     Method                                                                                                                                                                 Description
          ------------------------------------- ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `ArtifactCacheEvent.Finished`         `newContainsFinishedEvent​(ArtifactCacheEvent.Started started,                         Map<RuleKey,​CacheResult> results)`                                                
          `ArtifactCacheEvent.Started`          `newContainsStartedEvent​(com.google.common.collect.ImmutableSet<RuleKey> ruleKeys)`                                                                                     
          `ArtifactCacheEvent.Finished`         `newFetchFinishedEvent​(ArtifactCacheEvent.Started started,                      CacheResult cacheResult)`                                                               
          `ArtifactCacheEvent.Started`          `newFetchStartedEvent​(com.google.common.collect.ImmutableSet<RuleKey> ruleKeys)`                                                                                        
          `SQLiteArtifactCacheEvent.Finished`   `newFinishedEvent​(ArtifactCacheEvent.Started started,                 Optional<CacheResult> cacheResult)`                                                               
          `ArtifactCacheEvent.Finished`         `newStoreFinishedEvent​(ArtifactCacheEvent.Started started)`                                                                                                             
          `ArtifactCacheEvent.Started`          `newStoreStartedEvent​(com.google.common.collect.ImmutableSet<RuleKey> ruleKeys,                     com.google.common.collect.ImmutableMap<String,​String> metadata)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.artifact_cache.AbstractArtifactCacheEventFactory}

            ### Methods inherited from class com.facebook.buck.artifact_cache.[AbstractArtifactCacheEventFactory](AbstractArtifactCacheEventFactory.html "class in com.facebook.buck.artifact_cache")

            `getTarget, getTarget, getTarget`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.util.function.Function,com.facebook.buck.core.model.TargetConfigurationSerializer)}

        -   #### SQLiteArtifactCacheEventFactory

                protected SQLiteArtifactCacheEventFactory​(java.util.function.Function<String,​UnconfiguredBuildTarget> unconfiguredBuildTargetFactory,
                                                          TargetConfigurationSerializer targetConfigurationSerializer)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#newFetchStartedEvent(com.google.common.collect.ImmutableSet)}

        -   #### newFetchStartedEvent

            ``` methodSignature
            public ArtifactCacheEvent.Started newFetchStartedEvent​(com.google.common.collect.ImmutableSet<RuleKey> ruleKeys)
            ```

        []{#newContainsStartedEvent(com.google.common.collect.ImmutableSet)}

        -   #### newContainsStartedEvent

            ``` methodSignature
            public ArtifactCacheEvent.Started newContainsStartedEvent​(com.google.common.collect.ImmutableSet<RuleKey> ruleKeys)
            ```

        []{#newStoreStartedEvent(com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableMap)}

        -   #### newStoreStartedEvent

            ``` methodSignature
            public ArtifactCacheEvent.Started newStoreStartedEvent​(com.google.common.collect.ImmutableSet<RuleKey> ruleKeys,
                                                                   com.google.common.collect.ImmutableMap<String,​String> metadata)
            ```

        []{#newStoreFinishedEvent(com.facebook.buck.artifact_cache.ArtifactCacheEvent.Started)}

        -   #### newStoreFinishedEvent

            ``` methodSignature
            public ArtifactCacheEvent.Finished newStoreFinishedEvent​(ArtifactCacheEvent.Started started)
            ```

        []{#newFetchFinishedEvent(com.facebook.buck.artifact_cache.ArtifactCacheEvent.Started,com.facebook.buck.artifact_cache.CacheResult)}

        -   #### newFetchFinishedEvent

            ``` methodSignature
            public ArtifactCacheEvent.Finished newFetchFinishedEvent​(ArtifactCacheEvent.Started started,
                                                                     CacheResult cacheResult)
            ```

        []{#newContainsFinishedEvent(com.facebook.buck.artifact_cache.ArtifactCacheEvent.Started,java.util.Map)}

        -   #### newContainsFinishedEvent

            ``` methodSignature
            public ArtifactCacheEvent.Finished newContainsFinishedEvent​(ArtifactCacheEvent.Started started,
                                                                        Map<RuleKey,​CacheResult> results)
            ```

        []{#newFinishedEvent(com.facebook.buck.artifact_cache.ArtifactCacheEvent.Started,java.util.Optional)}

        -   #### newFinishedEvent

            ``` methodSignature
            public SQLiteArtifactCacheEvent.Finished newFinishedEvent​(ArtifactCacheEvent.Started started,
                                                                      Optional<CacheResult> cacheResult)
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
