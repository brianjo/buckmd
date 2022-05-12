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
[Package]{.packageLabelInType} [com.facebook.buck.remoteexecution](package-summary.html)
:::

## Interface ContentAddressedStorageClient.FileMaterializer {#interface-contentaddressedstorageclient.filematerializer .title title="Interface ContentAddressedStorageClient.FileMaterializer"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `OutputsMaterializer.FilesystemFileMaterializer`

    ```{=html}
    <!-- -->
    ```

    Enclosing interface:
    :   [ContentAddressedStorageClient](ContentAddressedStorageClient.html "interface in com.facebook.buck.remoteexecution")

    ------------------------------------------------------------------------

        public static interface ContentAddressedStorageClient.FileMaterializer

    ::: block
    Interface for filesystem operations required for materialization.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `WritableByteChannel` | `g                    | ::: block             |
        |                       | etOutputChannel​(Path  | Get a writable        |
        |                       | path,                 | channel to the file   |
        |                       |  boolean executable)` | at the provided path, |
        |                       |                       | marking it executable |
        |                       |                       | if appropriate.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `makeDirec            | ::: block             |
        |                       | tories​(Path dirRoot)` | Make the directory    |
        |                       |                       | and all parent        |
        |                       |                       | directories.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

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

        []{#getOutputChannel(java.nio.file.Path,boolean)}

        -   #### getOutputChannel

            ``` methodSignature
            WritableByteChannel getOutputChannel​(Path path,
                                                 boolean executable)
                                          throws IOException
            ```

            ::: block
            Get a writable channel to the file at the provided path,
            marking it executable if appropriate.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#makeDirectories(java.nio.file.Path)}

        -   #### makeDirectories

            ``` methodSignature
            void makeDirectories​(Path dirRoot)
                          throws IOException
            ```

            ::: block
            Make the directory and all parent directories.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`
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
