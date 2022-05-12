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
[Package]{.packageLabelInType} [com.facebook.buck.util.cache](package-summary.html)
:::

## Class DelegatingFileHashCacheEngine {#class-delegatingfilehashcacheengine .title title="Class DelegatingFileHashCacheEngine"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.cache.DelegatingFileHashCacheEngine

::: description
-   

    All Implemented Interfaces:
    :   `FileHashCacheEngine`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `StatsTrackingFileHashCacheEngine`

    ------------------------------------------------------------------------

        public class DelegatingFileHashCacheEngine
        extends Object
        implements FileHashCacheEngine
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.util.cache.FileHashCacheEngine}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.util.cache.[FileHashCacheEngine](FileHashCacheEngine.html "interface in com.facebook.buck.util.cache")

            `FileHashCacheEngine.ValueLoader<T>`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                     Description
          --------------------------------------------------------------- -------------
          `DelegatingFileHashCacheEngine​(FileHashCacheEngine delegate)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                           Method                                                                                Description
          ------------------------------------------- ------------------------------------------------------------------------------------- -------------
          `ConcurrentMap<Path,​HashCodeAndFileType>`   `asMap()`                                                                              
          `com.google.common.hash.HashCode`           `get​(Path path)`                                                                       
          `com.google.common.hash.HashCode`           `getForArchiveMember​(Path archiveRelativePath,                    Path memberPath)`    
          `HashCodeAndFileType`                       `getIfPresent​(Path path)`                                                              
          `long`                                      `getSize​(Path relativePath)`                                                           
          `Long`                                      `getSizeIfPresent​(Path path)`                                                          
          `List<AbstractBuckEvent>`                   `getStatsEvents()`                                                                     
          `void`                                      `invalidate​(Path path)`                                                                
          `void`                                      `invalidateAll()`                                                                      
          `void`                                      `invalidateWithParents​(Path path)`                                                     
          `void`                                      `put​(Path path,    HashCodeAndFileType value)`                                         
          `void`                                      `putSize​(Path path,        long value)`                                                

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
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

        []{#<init>(com.facebook.buck.util.cache.FileHashCacheEngine)}

        -   #### DelegatingFileHashCacheEngine

                public DelegatingFileHashCacheEngine​(FileHashCacheEngine delegate)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#put(java.nio.file.Path,com.facebook.buck.util.cache.HashCodeAndFileType)}

        -   #### put

            ``` methodSignature
            public void put​(Path path,
                            HashCodeAndFileType value)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `put` in interface `FileHashCacheEngine`

        []{#putSize(java.nio.file.Path,long)}

        -   #### putSize

            ``` methodSignature
            public void putSize​(Path path,
                                long value)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putSize` in interface `FileHashCacheEngine`

        []{#invalidate(java.nio.file.Path)}

        -   #### invalidate

            ``` methodSignature
            public void invalidate​(Path path)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `invalidate` in interface `FileHashCacheEngine`

        []{#invalidateWithParents(java.nio.file.Path)}

        -   #### invalidateWithParents

            ``` methodSignature
            public void invalidateWithParents​(Path path)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `invalidateWithParents` in
                interface `FileHashCacheEngine`

        []{#get(java.nio.file.Path)}

        -   #### get

            ``` methodSignature
            public com.google.common.hash.HashCode get​(Path path)
                                                throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `get` in interface `FileHashCacheEngine`

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

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getIfPresent(java.nio.file.Path)}

        -   #### getIfPresent

            ``` methodSignature
            @Nullable
            public HashCodeAndFileType getIfPresent​(Path path)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getIfPresent` in interface `FileHashCacheEngine`

        []{#getSizeIfPresent(java.nio.file.Path)}

        -   #### getSizeIfPresent

            ``` methodSignature
            @Nullable
            public Long getSizeIfPresent​(Path path)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSizeIfPresent` in interface `FileHashCacheEngine`

        []{#getSize(java.nio.file.Path)}

        -   #### getSize

            ``` methodSignature
            public long getSize​(Path relativePath)
                         throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSize` in interface `FileHashCacheEngine`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#invalidateAll()}

        -   #### invalidateAll

            ``` methodSignature
            public void invalidateAll()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `invalidateAll` in interface `FileHashCacheEngine`

        []{#asMap()}

        -   #### asMap

            ``` methodSignature
            public ConcurrentMap<Path,​HashCodeAndFileType> asMap()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `asMap` in interface `FileHashCacheEngine`

        []{#getStatsEvents()}

        -   #### getStatsEvents

            ``` methodSignature
            public List<AbstractBuckEvent> getStatsEvents()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getStatsEvents` in interface `FileHashCacheEngine`
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
