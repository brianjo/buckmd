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
[Package]{.packageLabelInType} [com.facebook.buck.artifact_cache](package-summary.html)
:::

## Class CacheResult {#class-cacheresult .title title="Class CacheResult"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.artifact_cache.CacheResult

::: description
-   

    ------------------------------------------------------------------------

        public abstract class CacheResult
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type      Field              Description
          ---------------------- ------------------ -------------
          `static CacheResult`   `SKIPPED_RESULT`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor       Description
          ----------------- -------------
          `CacheResult()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                            Method                                                                                                                                               Description
          ---------------------------------------------------------------------------- ---------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `abstract Optional<Long>`                                                    `artifactSizeBytes()`                                                                                                                                 
          `abstract Optional<String>`                                                  `cacheError()`                                                                                                                                        
          `abstract Optional<ArtifactCacheMode>`                                       `cacheMode()`                                                                                                                                         
          `protected abstract Optional<String>`                                        `cacheSource()`                                                                                                                                       
          `protected void`                                                             `check()`                                                                                                                                             
          `static CacheResult`                                                         `contains​(String cacheSource,         ArtifactCacheMode cacheMode)`                                                                                   
          `static CacheResult`                                                         `error​(String cacheSource,      ArtifactCacheMode cacheMode,      String cacheError)`                                                                 
          `long`                                                                       `getArtifactSizeBytes()`                                                                                                                              
          `String`                                                                     `getCacheError()`                                                                                                                                     
          `String`                                                                     `getCacheSource()`                                                                                                                                    
          `com.google.common.collect.ImmutableMap<String,​String>`                      `getMetadata()`                                                                                                                                       
          `abstract CacheResultType`                                                   `getType()`                                                                                                                                           
          `static CacheResult`                                                         `hit​(String cacheSource,    ArtifactCacheMode cacheMode)`                                                                                             
          `static CacheResult`                                                         `hit​(String cacheSource,    ArtifactCacheMode cacheMode,    com.google.common.collect.ImmutableMap<String,​String> metadata,    long artifactSize)`    
          `static CacheResult`                                                         `ignored()`                                                                                                                                           
          `static CacheResult`                                                         `localKeyUnchangedHit()`                                                                                                                              
          `abstract Optional<com.google.common.collect.ImmutableMap<String,​String>>`   `metadata()`                                                                                                                                          
          `static CacheResult`                                                         `miss()`                                                                                                                                              
          `static CacheResult`                                                         `miss​(String cacheSource,     ArtifactCacheMode cacheMode)`                                                                                           
          `String`                                                                     `name()`                                                                                                                                              
          `static CacheResult`                                                         `of​(CacheResultType type,   String cacheSource)`                                                                                                      
          `static CacheResult`                                                         `skipped()`                                                                                                                                           
          `static CacheResult`                                                         `softError​(String cacheSource,          ArtifactCacheMode cacheMode,          String cacheError)`                                                     
          `String`                                                                     `toString()`                                                                                                                                          
          `abstract Optional<String>`                                                  `twoLevelContentHashKey()`                                                                                                                            
          `static CacheResult`                                                         `valueOf​(String val)`                                                                                                                                 
          `CacheResult`                                                                `withArtifactSizeBytes​(Optional<Long> artifactSizeBytes)`                                                                                             
          `CacheResult`                                                                `withCacheError​(Optional<String> cacheError)`                                                                                                         
          `CacheResult`                                                                `withMetadata​(Optional<com.google.common.collect.ImmutableMap<String,​String>> metadata)`                                                              
          `CacheResult`                                                                `withTwoLevelContentHashKey​(Optional<String> twoLevelContentHashKey)`                                                                                 

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#SKIPPED_RESULT}

        -   #### SKIPPED_RESULT

                public static final CacheResult SKIPPED_RESULT
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### CacheResult

                public CacheResult()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getType()}

        -   #### getType

            ``` methodSignature
            public abstract CacheResultType getType()
            ```

        []{#cacheSource()}

        -   #### cacheSource

            ``` methodSignature
            protected abstract Optional<String> cacheSource()
            ```

        []{#cacheMode()}

        -   #### cacheMode

            ``` methodSignature
            public abstract Optional<ArtifactCacheMode> cacheMode()
            ```

        []{#cacheError()}

        -   #### cacheError

            ``` methodSignature
            public abstract Optional<String> cacheError()
            ```

        []{#metadata()}

        -   #### metadata

            ``` methodSignature
            public abstract Optional<com.google.common.collect.ImmutableMap<String,​String>> metadata()
            ```

        []{#artifactSizeBytes()}

        -   #### artifactSizeBytes

            ``` methodSignature
            public abstract Optional<Long> artifactSizeBytes()
            ```

        []{#twoLevelContentHashKey()}

        -   #### twoLevelContentHashKey

            ``` methodSignature
            public abstract Optional<String> twoLevelContentHashKey()
            ```

        []{#getCacheSource()}

        -   #### getCacheSource

            ``` methodSignature
            public String getCacheSource()
            ```

        []{#getCacheError()}

        -   #### getCacheError

            ``` methodSignature
            public String getCacheError()
            ```

        []{#getMetadata()}

        -   #### getMetadata

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​String> getMetadata()
            ```

        []{#getArtifactSizeBytes()}

        -   #### getArtifactSizeBytes

            ``` methodSignature
            public long getArtifactSizeBytes()
            ```

        []{#name()}

        -   #### name

            ``` methodSignature
            public String name()
            ```

        []{#hit(java.lang.String,com.facebook.buck.artifact_cache.config.ArtifactCacheMode,com.google.common.collect.ImmutableMap,long)}

        -   #### hit

            ``` methodSignature
            public static CacheResult hit​(String cacheSource,
                                          ArtifactCacheMode cacheMode,
                                          com.google.common.collect.ImmutableMap<String,​String> metadata,
                                          long artifactSize)
            ```

        []{#hit(java.lang.String,com.facebook.buck.artifact_cache.config.ArtifactCacheMode)}

        -   #### hit

            ``` methodSignature
            public static CacheResult hit​(String cacheSource,
                                          ArtifactCacheMode cacheMode)
            ```

        []{#miss(java.lang.String,com.facebook.buck.artifact_cache.config.ArtifactCacheMode)}

        -   #### miss

            ``` methodSignature
            public static CacheResult miss​(String cacheSource,
                                           ArtifactCacheMode cacheMode)
            ```

        []{#error(java.lang.String,com.facebook.buck.artifact_cache.config.ArtifactCacheMode,java.lang.String)}

        -   #### error

            ``` methodSignature
            public static CacheResult error​(String cacheSource,
                                            ArtifactCacheMode cacheMode,
                                            String cacheError)
            ```

        []{#softError(java.lang.String,com.facebook.buck.artifact_cache.config.ArtifactCacheMode,java.lang.String)}

        -   #### softError

            ``` methodSignature
            public static CacheResult softError​(String cacheSource,
                                                ArtifactCacheMode cacheMode,
                                                String cacheError)
            ```

        []{#of(com.facebook.buck.artifact_cache.CacheResultType,java.lang.String)}

        -   #### of

            ``` methodSignature
            public static CacheResult of​(CacheResultType type,
                                         String cacheSource)
            ```

        []{#skipped()}

        -   #### skipped

            ``` methodSignature
            public static CacheResult skipped()
            ```

        []{#miss()}

        -   #### miss

            ``` methodSignature
            public static CacheResult miss()
            ```

        []{#ignored()}

        -   #### ignored

            ``` methodSignature
            public static CacheResult ignored()
            ```

        []{#contains(java.lang.String,com.facebook.buck.artifact_cache.config.ArtifactCacheMode)}

        -   #### contains

            ``` methodSignature
            public static CacheResult contains​(String cacheSource,
                                               ArtifactCacheMode cacheMode)
            ```

        []{#localKeyUnchangedHit()}

        -   #### localKeyUnchangedHit

            ``` methodSignature
            public static CacheResult localKeyUnchangedHit()
            ```

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static CacheResult valueOf​(String val)
            ```

            [Returns:]{.returnLabel}
            :   a
                [`CacheResult`](CacheResult.html "class in com.facebook.buck.artifact_cache")
                constructed from trying to parse the given string
                representation. This is mainly available for backwards
                compatibility for when this class was an enum.

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#check()}

        -   #### check

            ``` methodSignature
            @Check
            protected void check()
            ```

        []{#withCacheError(java.util.Optional)}

        -   #### withCacheError

            ``` methodSignature
            public CacheResult withCacheError​(Optional<String> cacheError)
            ```

        []{#withTwoLevelContentHashKey(java.util.Optional)}

        -   #### withTwoLevelContentHashKey

            ``` methodSignature
            public CacheResult withTwoLevelContentHashKey​(Optional<String> twoLevelContentHashKey)
            ```

        []{#withMetadata(java.util.Optional)}

        -   #### withMetadata

            ``` methodSignature
            public CacheResult withMetadata​(Optional<com.google.common.collect.ImmutableMap<String,​String>> metadata)
            ```

        []{#withArtifactSizeBytes(java.util.Optional)}

        -   #### withArtifactSizeBytes

            ``` methodSignature
            public CacheResult withArtifactSizeBytes​(Optional<Long> artifactSizeBytes)
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
