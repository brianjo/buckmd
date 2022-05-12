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

## Class DirCacheEntry {#class-dircacheentry .title title="Class DirCacheEntry"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.artifact_cache.config.DirCacheEntry

::: description
-   

    ------------------------------------------------------------------------

        public abstract class DirCacheEntry
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor         Description
          ------------------- -------------
          `DirCacheEntry()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type             Method                                                                                                       Description
          ----------------------------- ------------------------------------------------------------------------------------------------------------ -------------
          `abstract Path`               `getCacheDir()`                                                                                               
          `abstract CacheReadMode`      `getCacheReadMode()`                                                                                          
          `abstract Optional<Long>`     `getMaxSizeBytes()`                                                                                           
          `abstract Optional<String>`   `getName()`                                                                                                   
          `static DirCacheEntry`        `of​(Path cacheDir,   Optional<Long> maxSizeBytes,   CacheReadMode cacheReadMode)`                             
          `static DirCacheEntry`        `of​(Optional<String> name,   Path cacheDir,   Optional<Long> maxSizeBytes,   CacheReadMode cacheReadMode)`    
          `DirCacheEntry`               `withCacheReadMode​(CacheReadMode cacheReadMode)`                                                              

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

        -   #### DirCacheEntry

                public DirCacheEntry()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getName()}

        -   #### getName

            ``` methodSignature
            public abstract Optional<String> getName()
            ```

        []{#getCacheDir()}

        -   #### getCacheDir

            ``` methodSignature
            public abstract Path getCacheDir()
            ```

        []{#getMaxSizeBytes()}

        -   #### getMaxSizeBytes

            ``` methodSignature
            public abstract Optional<Long> getMaxSizeBytes()
            ```

        []{#getCacheReadMode()}

        -   #### getCacheReadMode

            ``` methodSignature
            public abstract CacheReadMode getCacheReadMode()
            ```

        []{#of(java.nio.file.Path,java.util.Optional,com.facebook.buck.artifact_cache.config.CacheReadMode)}

        -   #### of

            ``` methodSignature
            public static DirCacheEntry of​(Path cacheDir,
                                           Optional<Long> maxSizeBytes,
                                           CacheReadMode cacheReadMode)
            ```

        []{#of(java.util.Optional,java.nio.file.Path,java.util.Optional,com.facebook.buck.artifact_cache.config.CacheReadMode)}

        -   #### of

            ``` methodSignature
            public static DirCacheEntry of​(Optional<String> name,
                                           Path cacheDir,
                                           Optional<Long> maxSizeBytes,
                                           CacheReadMode cacheReadMode)
            ```

        []{#withCacheReadMode(com.facebook.buck.artifact_cache.config.CacheReadMode)}

        -   #### withCacheReadMode

            ``` methodSignature
            public DirCacheEntry withCacheReadMode​(CacheReadMode cacheReadMode)
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
