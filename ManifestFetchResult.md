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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.build.engine.manifest](package-summary.html)
:::

## Class ManifestFetchResult {#class-manifestfetchresult .title title="Class ManifestFetchResult"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.build.engine.manifest.ManifestFetchResult

::: description
-   

    ------------------------------------------------------------------------

        public abstract class ManifestFetchResult
        extends Object

    ::: block
    Provides a results summary of a manifest-based cache fetch process.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                           Description
          ------------------- ------------------------------- -------------
          `static class `     `ManifestFetchResult.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor               Description
          ------------------------- -------------
          `ManifestFetchResult()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                      Method                       Description
          -------------------------------------- ---------------------------- -------------
          `static ManifestFetchResult.Builder`   `builder()`                   
          `abstract CacheResult`                 `getManifestCacheResult()`    
          `abstract Optional<String>`            `getManifestLoadError()`      
          `abstract Optional<ManifestStats>`     `getManifestStats()`          
          `abstract Optional<CacheResult>`       `getRuleCacheResult()`        

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

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### ManifestFetchResult

                public ManifestFetchResult()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getManifestCacheResult()}

        -   #### getManifestCacheResult

            ``` methodSignature
            public abstract CacheResult getManifestCacheResult()
            ```

            [Returns:]{.returnLabel}
            :   the result of fetching the manifest from cache.

        []{#getManifestLoadError()}

        -   #### getManifestLoadError

            ``` methodSignature
            public abstract Optional<String> getManifestLoadError()
            ```

            [Returns:]{.returnLabel}
            :   the error generated when trying to load the manifest.

        []{#getManifestStats()}

        -   #### getManifestStats

            ``` methodSignature
            public abstract Optional<ManifestStats> getManifestStats()
            ```

            [Returns:]{.returnLabel}
            :   stats for the fetched manifest.

        []{#getRuleCacheResult()}

        -   #### getRuleCacheResult

            ``` methodSignature
            public abstract Optional<CacheResult> getRuleCacheResult()
            ```

            [Returns:]{.returnLabel}
            :   the result from fetching the rule outputs via the found
                dep file rule key.

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static ManifestFetchResult.Builder builder()
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
