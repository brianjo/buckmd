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

## Interface HttpArtifactCacheEvent.HttpArtifactCacheEventFetchData {#interface-httpartifactcacheevent.httpartifactcacheeventfetchdata .title title="Interface HttpArtifactCacheEvent.HttpArtifactCacheEventFetchData"}
:::

::: contentContainer
::: description
-   

    Enclosing class:
    :   [HttpArtifactCacheEvent](HttpArtifactCacheEvent.html "class in com.facebook.buck.artifact_cache")

    ------------------------------------------------------------------------

        public static interface HttpArtifactCacheEvent.HttpArtifactCacheEventFetchData
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Interface                                                          Description
          ------------------- ------------------------------------------------------------------ -------------
          `static class `     `HttpArtifactCacheEvent.HttpArtifactCacheEventFetchData.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                         Method                       Description
          ------------------------------------------------------------------------- ---------------------------- -------------
          `static HttpArtifactCacheEvent.HttpArtifactCacheEventFetchData.Builder`   `builder()`                   
          `Optional<String>`                                                        `getArtifactContentHash()`    
          `Optional<Long>`                                                          `getArtifactSizeBytes()`      
          `com.google.common.collect.ImmutableSet<RuleKey>`                         `getAssociatedRuleKeys()`     
          `Optional<String>`                                                        `getErrorMessage()`           
          `Optional<CacheResult>`                                                   `getFetchResult()`            
          `RuleKey`                                                                 `getRequestedRuleKey()`       
          `Optional<Long>`                                                          `getResponseSizeBytes()`      

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

        []{#getResponseSizeBytes()}

        -   #### getResponseSizeBytes

            ``` methodSignature
            Optional<Long> getResponseSizeBytes()
            ```

        []{#getFetchResult()}

        -   #### getFetchResult

            ``` methodSignature
            Optional<CacheResult> getFetchResult()
            ```

        []{#getRequestedRuleKey()}

        -   #### getRequestedRuleKey

            ``` methodSignature
            RuleKey getRequestedRuleKey()
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

        []{#getAssociatedRuleKeys()}

        -   #### getAssociatedRuleKeys

            ``` methodSignature
            com.google.common.collect.ImmutableSet<RuleKey> getAssociatedRuleKeys()
            ```

        []{#builder()}

        -   #### builder

            ``` methodSignature
            static HttpArtifactCacheEvent.HttpArtifactCacheEventFetchData.Builder builder()
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
