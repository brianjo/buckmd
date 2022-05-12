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

## Interface HttpArtifactCacheEvent.HttpArtifactCacheEventStoreData {#interface-httpartifactcacheevent.httpartifactcacheeventstoredata .title title="Interface HttpArtifactCacheEvent.HttpArtifactCacheEventStoreData"}
:::

::: contentContainer
::: description
-   

    Enclosing class:
    :   [HttpArtifactCacheEvent](HttpArtifactCacheEvent.html "class in com.facebook.buck.artifact_cache")

    ------------------------------------------------------------------------

        public static interface HttpArtifactCacheEvent.HttpArtifactCacheEventStoreData
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Interface                                                          Description
          ------------------- ------------------------------------------------------------------ -------------
          `static class `     `HttpArtifactCacheEvent.HttpArtifactCacheEventStoreData.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                         Method                       Description
          ------------------------------------------------------------------------- ---------------------------- -------------
          `static HttpArtifactCacheEvent.HttpArtifactCacheEventStoreData.Builder`   `builder()`                   
          `Optional<String>`                                                        `getArtifactContentHash()`    
          `Optional<Long>`                                                          `getArtifactSizeBytes()`      
          `Optional<String>`                                                        `getErrorMessage()`           
          `Optional<Long>`                                                          `getRequestSizeBytes()`       
          `com.google.common.collect.ImmutableSet<RuleKey>`                         `getRuleKeys()`               
          `ArtifactCacheEvent.StoreType`                                            `getStoreType()`              
          `Optional<Boolean>`                                                       `wasStoreSuccessful()`        

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getRequestSizeBytes()}

        -   #### getRequestSizeBytes

            ``` methodSignature
            Optional<Long> getRequestSizeBytes()
            ```

        []{#wasStoreSuccessful()}

        -   #### wasStoreSuccessful

            ``` methodSignature
            Optional<Boolean> wasStoreSuccessful()
            ```

        []{#getRuleKeys()}

        -   #### getRuleKeys

            ``` methodSignature
            com.google.common.collect.ImmutableSet<RuleKey> getRuleKeys()
            ```

        []{#getArtifactContentHash()}

        -   #### getArtifactContentHash

            ``` methodSignature
            Optional<String> getArtifactContentHash()
            ```

        []{#getArtifactSizeBytes()}

        -   #### getArtifactSizeBytes

            ``` methodSignature
            Optional<Long> getArtifactSizeBytes()
            ```

        []{#getErrorMessage()}

        -   #### getErrorMessage

            ``` methodSignature
            Optional<String> getErrorMessage()
            ```

        []{#getStoreType()}

        -   #### getStoreType

            ``` methodSignature
            ArtifactCacheEvent.StoreType getStoreType()
            ```

        []{#builder()}

        -   #### builder

            ``` methodSignature
            static HttpArtifactCacheEvent.HttpArtifactCacheEventStoreData.Builder builder()
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
-   [Nested](#nested.class.summary) \| 
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
