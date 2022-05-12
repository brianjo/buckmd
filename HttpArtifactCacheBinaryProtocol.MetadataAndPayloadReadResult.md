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

## Class HttpArtifactCacheBinaryProtocol.MetadataAndPayloadReadResult {#class-httpartifactcachebinaryprotocol.metadataandpayloadreadresult .title title="Class HttpArtifactCacheBinaryProtocol.MetadataAndPayloadReadResult"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.artifact_cache.HttpArtifactCacheBinaryProtocol.MetadataAndPayloadReadResult

::: description
-   

    Direct Known Subclasses:
    :   `HttpArtifactCacheBinaryProtocol.StoreResponseReadResult`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [HttpArtifactCacheBinaryProtocol](HttpArtifactCacheBinaryProtocol.html "class in com.facebook.buck.artifact_cache")

    ------------------------------------------------------------------------

        public abstract static class HttpArtifactCacheBinaryProtocol.MetadataAndPayloadReadResult
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                        Description
          ---------------------------------- -------------
          `MetadataAndPayloadReadResult()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                  Method                        Description
          ------------------------------------------------------------------ ----------------------------- -------------
          `abstract com.google.common.hash.HashCode`                         `getActualHashCode()`          
          `abstract com.google.common.hash.HashCode`                         `getArtifactOnlyHashCode()`    
          `abstract com.google.common.hash.HashCode`                         `getExpectedHashCode()`        
          `abstract com.google.common.collect.ImmutableMap<String,​String>`   `getMetadata()`                
          `abstract long`                                                    `getResponseSizeBytes()`       
          `abstract com.google.common.collect.ImmutableSet<RuleKey>`         `getRuleKeys()`                

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

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

        -   #### MetadataAndPayloadReadResult

                public MetadataAndPayloadReadResult()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getRuleKeys()}

        -   #### getRuleKeys

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<RuleKey> getRuleKeys()
            ```

        []{#getExpectedHashCode()}

        -   #### getExpectedHashCode

            ``` methodSignature
            public abstract com.google.common.hash.HashCode getExpectedHashCode()
            ```

        []{#getActualHashCode()}

        -   #### getActualHashCode

            ``` methodSignature
            public abstract com.google.common.hash.HashCode getActualHashCode()
            ```

        []{#getArtifactOnlyHashCode()}

        -   #### getArtifactOnlyHashCode

            ``` methodSignature
            public abstract com.google.common.hash.HashCode getArtifactOnlyHashCode()
            ```

        []{#getResponseSizeBytes()}

        -   #### getResponseSizeBytes

            ``` methodSignature
            public abstract long getResponseSizeBytes()
            ```

        []{#getMetadata()}

        -   #### getMetadata

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<String,​String> getMetadata()
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
