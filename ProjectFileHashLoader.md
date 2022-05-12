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
[Package]{.packageLabelInType} [com.facebook.buck.util.hashing](package-summary.html)
:::

## Interface ProjectFileHashLoader {#interface-projectfilehashloader .title title="Interface ProjectFileHashLoader"}
:::

::: contentContainer
::: description
-   

    All Known Subinterfaces:
    :   `ProjectFileHashCache`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `DefaultFileHashCache`, `WatchedFileHashCache`

    ------------------------------------------------------------------------

        public interface ProjectFileHashLoader

    ::: block
    Load hashes of paths under a
    [`ProjectFilesystem`](../../io/filesystem/ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                             Method                                                                                Description
          --------------------------------------------- ------------------------------------------------------------------------------------- -------------
          `com.google.common.hash.HashCode`             `get​(Path path)`                                                                       
          `com.google.common.hash.HashCode`             `getForArchiveMember​(Path relativeArchivePath,                    Path memberPath)`    
          `Optional<com.google.common.hash.HashCode>`   `getIfPresent​(Path path)`                                                              
          `long`                                        `getSize​(Path path)`                                                                   

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
            com.google.common.hash.HashCode getForArchiveMember​(Path relativeArchivePath,
                                                                Path memberPath)
                                                         throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getSize(java.nio.file.Path)}

        -   #### getSize

            ``` methodSignature
            long getSize​(Path path)
                  throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getIfPresent(java.nio.file.Path)}

        -   #### getIfPresent

            ``` methodSignature
            Optional<com.google.common.hash.HashCode> getIfPresent​(Path path)
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
