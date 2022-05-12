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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.artifact_cache.config](package-summary.html)
:::

## Class HttpCacheEntry {#class-httpcacheentry .title title="Class HttpCacheEntry"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.artifact_cache.config.HttpCacheEntry

::: description
-   

    ------------------------------------------------------------------------

        public abstract class HttpCacheEntry
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor          Description
          -------------------- -------------
          `HttpCacheEntry()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                     Method                                                                Description
          --------------------------------------------------------------------- --------------------------------------------------------------------- -------------
          `protected abstract com.google.common.collect.ImmutableSet<String>`   `getBlacklistedWifiSsids()`                                            
          `abstract CacheReadMode`                                              `getCacheReadMode()`                                                   
          `abstract int`                                                        `getConnectTimeoutSeconds()`                                           
          `abstract String`                                                     `getErrorMessageFormat()`                                              
          `abstract int`                                                        `getErrorMessageLimit()`                                               
          `abstract Optional<Long>`                                             `getMaxStoreSize()`                                                    
          `abstract com.google.common.collect.ImmutableMap<String,​String>`      `getReadHeaders()`                                                     
          `abstract int`                                                        `getReadTimeoutSeconds()`                                              
          `abstract URI`                                                        `getUrl()`                                                             
          `abstract com.google.common.collect.ImmutableMap<String,​String>`      `getWriteHeaders()`                                                    
          `abstract int`                                                        `getWriteTimeoutSeconds()`                                             
          `boolean`                                                             `isWifiUsableForDistributedCache​(Optional<String> currentWifiSsid)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

        -   #### HttpCacheEntry

                public HttpCacheEntry()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getUrl()}

        -   #### getUrl

            ``` methodSignature
            public abstract URI getUrl()
            ```

        []{#getConnectTimeoutSeconds()}

        -   #### getConnectTimeoutSeconds

            ``` methodSignature
            public abstract int getConnectTimeoutSeconds()
            ```

        []{#getReadTimeoutSeconds()}

        -   #### getReadTimeoutSeconds

            ``` methodSignature
            public abstract int getReadTimeoutSeconds()
            ```

        []{#getWriteTimeoutSeconds()}

        -   #### getWriteTimeoutSeconds

            ``` methodSignature
            public abstract int getWriteTimeoutSeconds()
            ```

        []{#getReadHeaders()}

        -   #### getReadHeaders

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<String,​String> getReadHeaders()
            ```

        []{#getWriteHeaders()}

        -   #### getWriteHeaders

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<String,​String> getWriteHeaders()
            ```

        []{#getCacheReadMode()}

        -   #### getCacheReadMode

            ``` methodSignature
            public abstract CacheReadMode getCacheReadMode()
            ```

        []{#getBlacklistedWifiSsids()}

        -   #### getBlacklistedWifiSsids

            ``` methodSignature
            protected abstract com.google.common.collect.ImmutableSet<String> getBlacklistedWifiSsids()
            ```

        []{#getErrorMessageFormat()}

        -   #### getErrorMessageFormat

            ``` methodSignature
            public abstract String getErrorMessageFormat()
            ```

        []{#getErrorMessageLimit()}

        -   #### getErrorMessageLimit

            ``` methodSignature
            public abstract int getErrorMessageLimit()
            ```

        []{#getMaxStoreSize()}

        -   #### getMaxStoreSize

            ``` methodSignature
            public abstract Optional<Long> getMaxStoreSize()
            ```

        []{#isWifiUsableForDistributedCache(java.util.Optional)}

        -   #### isWifiUsableForDistributedCache

            ``` methodSignature
            public boolean isWifiUsableForDistributedCache​(Optional<String> currentWifiSsid)
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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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
