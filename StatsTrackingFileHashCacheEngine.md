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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.util.cache.impl](package-summary.html)
:::

## Class StatsTrackingFileHashCacheEngine {#class-statstrackingfilehashcacheengine .title title="Class StatsTrackingFileHashCacheEngine"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.util.cache.DelegatingFileHashCacheEngine](../DelegatingFileHashCacheEngine.html "class in com.facebook.buck.util.cache")

    -   -   com.facebook.buck.util.cache.impl.StatsTrackingFileHashCacheEngine

::: description
-   

    All Implemented Interfaces:
    :   `FileHashCacheEngine`

    ------------------------------------------------------------------------

        public class StatsTrackingFileHashCacheEngine
        extends DelegatingFileHashCacheEngine
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.util.cache.FileHashCacheEngine}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.util.cache.[FileHashCacheEngine](../FileHashCacheEngine.html "interface in com.facebook.buck.util.cache")

            `FileHashCacheEngine.ValueLoader<T>`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                            Description
          ---------------------------------------------------------------------------------------------------------------------- -------------
          `StatsTrackingFileHashCacheEngine​(FileHashCacheEngine delegate,                                 String subcategory)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                   Method                                                                                Description
          ----------------------------------- ------------------------------------------------------------------------------------- -------------
          `com.google.common.hash.HashCode`   `get​(Path path)`                                                                       
          `com.google.common.hash.HashCode`   `getForArchiveMember​(Path archiveRelativePath,                    Path memberPath)`    
          `List<AbstractBuckEvent>`           `getStatsEvents()`                                                                     
          `void`                              `invalidate​(Path path)`                                                                
          `void`                              `invalidateWithParents​(Path path)`                                                     

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.util.cache.DelegatingFileHashCacheEngine}

            ### Methods inherited from class com.facebook.buck.util.cache.[DelegatingFileHashCacheEngine](../DelegatingFileHashCacheEngine.html "class in com.facebook.buck.util.cache")

            `asMap, getIfPresent, getSize, getSizeIfPresent, invalidateAll, put, putSize`

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

        []{#<init>(com.facebook.buck.util.cache.FileHashCacheEngine,java.lang.String)}

        -   #### StatsTrackingFileHashCacheEngine

                public StatsTrackingFileHashCacheEngine​(FileHashCacheEngine delegate,
                                                        String subcategory)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#invalidate(java.nio.file.Path)}

        -   #### invalidate

            ``` methodSignature
            public void invalidate​(Path path)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `invalidate` in interface `FileHashCacheEngine`

            [Overrides:]{.overrideSpecifyLabel}
            :   `invalidate` in class `DelegatingFileHashCacheEngine`

        []{#invalidateWithParents(java.nio.file.Path)}

        -   #### invalidateWithParents

            ``` methodSignature
            public void invalidateWithParents​(Path path)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `invalidateWithParents` in
                interface `FileHashCacheEngine`

            [Overrides:]{.overrideSpecifyLabel}
            :   `invalidateWithParents` in
                class `DelegatingFileHashCacheEngine`

        []{#get(java.nio.file.Path)}

        -   #### get

            ``` methodSignature
            public com.google.common.hash.HashCode get​(Path path)
                                                throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `get` in interface `FileHashCacheEngine`

            [Overrides:]{.overrideSpecifyLabel}
            :   `get` in class `DelegatingFileHashCacheEngine`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getForArchiveMember(java.nio.file.Path,java.nio.file.Path)}

        -   #### getForArchiveMember

            ``` methodSignature
            public com.google.common.hash.HashCode getForArchiveMember​(Path archiveRelativePath,
                                                                       Path memberPath)
                                                                throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getForArchiveMember` in interface `FileHashCacheEngine`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getForArchiveMember` in
                class `DelegatingFileHashCacheEngine`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getStatsEvents()}

        -   #### getStatsEvents

            ``` methodSignature
            public List<AbstractBuckEvent> getStatsEvents()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getStatsEvents` in interface `FileHashCacheEngine`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getStatsEvents` in
                class `DelegatingFileHashCacheEngine`
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
