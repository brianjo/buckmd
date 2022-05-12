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

## Interface ProjectFileHashCache {#interface-projectfilehashcache .title title="Interface ProjectFileHashCache"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `ProjectFileHashLoader`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `DefaultFileHashCache`, `WatchedFileHashCache`

    ------------------------------------------------------------------------

        public interface ProjectFileHashCache
        extends ProjectFileHashLoader

    ::: block
    A
    [`FileHashLoader`](../hashing/FileHashLoader.html "interface in com.facebook.buck.util.hashing")
    which manages caching file hashes for a given
    [`ProjectFilesystem`](../../io/filesystem/ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                    Method                                                          Description
          ------------------------------------------------------------------------------------ --------------------------------------------------------------- -------------
          `default java.util.stream.Stream<Map.Entry<Path,​com.google.common.hash.HashCode>>`   `debugDump()`                                                    
          `ProjectFilesystem`                                                                  `getFilesystem()`                                                
          `void`                                                                               `invalidate​(Path path)`                                          
          `void`                                                                               `invalidateAll()`                                                
          `boolean`                                                                            `isIgnored​(Path path)`                                           
          `void`                                                                               `set​(Path path,    com.google.common.hash.HashCode hashCode)`    
          `default FileHashCache.FileHashCacheVerificationResult`                              `verify()`                                                       
          `boolean`                                                                            `willGet​(ArchiveMemberPath archiveMemberPath)`                   
          `boolean`                                                                            `willGet​(Path path)`                                             

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
          .tableTab}[[Default
          Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.util.hashing.ProjectFileHashLoader}

            ### Methods inherited from interface com.facebook.buck.util.hashing.[ProjectFileHashLoader](../hashing/ProjectFileHashLoader.html "interface in com.facebook.buck.util.hashing")

            `get, getForArchiveMember, getIfPresent, getSize`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getFilesystem()}

        -   #### getFilesystem

            ``` methodSignature
            ProjectFilesystem getFilesystem()
            ```

        []{#willGet(java.nio.file.Path)}

        -   #### willGet

            ``` methodSignature
            boolean willGet​(Path path)
            ```

        []{#willGet(com.facebook.buck.core.io.ArchiveMemberPath)}

        -   #### willGet

            ``` methodSignature
            boolean willGet​(ArchiveMemberPath archiveMemberPath)
            ```

        []{#isIgnored(java.nio.file.Path)}

        -   #### isIgnored

            ``` methodSignature
            boolean isIgnored​(Path path)
            ```

        []{#invalidate(java.nio.file.Path)}

        -   #### invalidate

            ``` methodSignature
            void invalidate​(Path path)
            ```

        []{#invalidateAll()}

        -   #### invalidateAll

            ``` methodSignature
            void invalidateAll()
            ```

        []{#set(java.nio.file.Path,com.google.common.hash.HashCode)}

        -   #### set

            ``` methodSignature
            void set​(Path path,
                     com.google.common.hash.HashCode hashCode)
              throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#verify()}

        -   #### verify

            ``` methodSignature
            default FileHashCache.FileHashCacheVerificationResult verify()
                                                                  throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#debugDump()}

        -   #### debugDump

            ``` methodSignature
            default java.util.stream.Stream<Map.Entry<Path,​com.google.common.hash.HashCode>> debugDump()
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
