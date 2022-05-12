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
[Package]{.packageLabelInType} [com.facebook.buck.util.cache](package-summary.html)
:::

## Interface FileHashCacheEngine {#interface-filehashcacheengine .title title="Interface FileHashCacheEngine"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `DelegatingFileHashCacheEngine`,
        `StatsTrackingFileHashCacheEngine`

    ------------------------------------------------------------------------

        public interface FileHashCacheEngine

    ::: block
    This interface extracts the methods available to a file hash cache,
    so that the underlying implementation is hidden and can be swapped.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type     Interface                              Description
          --------------------- -------------------------------------- -------------
          `static interface `   `FileHashCacheEngine.ValueLoader<T>`    

          : Nested Classes[ ]{.tabEnd}
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
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#put(java.nio.file.Path,com.facebook.buck.util.cache.HashCodeAndFileType)}

        -   #### put

            ``` methodSignature
            void put​(Path path,
                     HashCodeAndFileType value)
            ```

        []{#putSize(java.nio.file.Path,long)}

        -   #### putSize

            ``` methodSignature
            void putSize​(Path path,
                         long value)
            ```

        []{#invalidate(java.nio.file.Path)}

        -   #### invalidate

            ``` methodSignature
            void invalidate​(Path path)
            ```

        []{#invalidateWithParents(java.nio.file.Path)}

        -   #### invalidateWithParents

            ``` methodSignature
            void invalidateWithParents​(Path path)
            ```

        []{#get(java.nio.file.Path)}

        -   #### get

            ``` methodSignature
            com.google.common.hash.HashCode get​(Path path)
                                         throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getForArchiveMember(java.nio.file.Path,java.nio.file.Path)}

        -   #### getForArchiveMember

            ``` methodSignature
            com.google.common.hash.HashCode getForArchiveMember​(Path archiveRelativePath,
                                                                Path memberPath)
                                                         throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getIfPresent(java.nio.file.Path)}

        -   #### getIfPresent

            ``` methodSignature
            @Nullable
            HashCodeAndFileType getIfPresent​(Path path)
            ```

        []{#getSizeIfPresent(java.nio.file.Path)}

        -   #### getSizeIfPresent

            ``` methodSignature
            @Nullable
            Long getSizeIfPresent​(Path path)
            ```

        []{#getSize(java.nio.file.Path)}

        -   #### getSize

            ``` methodSignature
            long getSize​(Path relativePath)
                  throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#invalidateAll()}

        -   #### invalidateAll

            ``` methodSignature
            void invalidateAll()
            ```

        []{#asMap()}

        -   #### asMap

            ``` methodSignature
            ConcurrentMap<Path,​HashCodeAndFileType> asMap()
            ```

        []{#getStatsEvents()}

        -   #### getStatsEvents

            ``` methodSignature
            List<AbstractBuckEvent> getStatsEvents()
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
