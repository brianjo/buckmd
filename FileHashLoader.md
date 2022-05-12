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

## Interface FileHashLoader {#interface-filehashloader .title title="Interface FileHashLoader"}
:::

::: contentContainer
::: description
-   

    All Known Subinterfaces:
    :   `FileHashCache`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `FilePathHashLoader`, `StackedFileHashCache`

    ------------------------------------------------------------------------

        public interface FileHashLoader
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `default com.google.  | `get​(Pr               | ::: block             |
        | common.hash.HashCode` | ojectFilesystem files | Return the `HashCode` |
        |                       | ystem,    Path path)` | for the given         |
        |                       |                       | relative              |
        |                       |                       | [`Path`](http://do    |
        |                       |                       | cs.oracle.com/javase/ |
        |                       |                       | 7/docs/api/java/nio/f |
        |                       |                       | ile/Path.html?is-exte |
        |                       |                       | rnal=true "class or i |
        |                       |                       | nterface in java.nio. |
        |                       |                       | file"){.externalLink} |
        |                       |                       | under the given       |
        |                       |                       | [`Projec              |
        |                       |                       | tFilesystem`](../../i |
        |                       |                       | o/filesystem/ProjectF |
        |                       |                       | ilesystem.html "inter |
        |                       |                       | face in com.facebook. |
        |                       |                       | buck.io.filesystem"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `get​(Path path)`      |                       |
        | common.hash.HashCode` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default com.google.  | `getFo                | ::: block             |
        | common.hash.HashCode` | rArchiveMember​(Projec | Return the `HashCode` |
        |                       | tFilesystem filesyste | for the given         |
        |                       | m,                    | relative              |
        |                       |  Path relativeArchive | [`ArchiveMem          |
        |                       | Path,                 | berPath`](../../core/ |
        |                       |     Path memberPath)` | io/ArchiveMemberPath. |
        |                       |                       | html "class in com.fa |
        |                       |                       | cebook.buck.core.io") |
        |                       |                       | under the given       |
        |                       |                       | [`Projec              |
        |                       |                       | tFilesystem`](../../i |
        |                       |                       | o/filesystem/ProjectF |
        |                       |                       | ilesystem.html "inter |
        |                       |                       | face in com.facebook. |
        |                       |                       | buck.io.filesystem"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getForArchiveMember  |                       |
        | common.hash.HashCode` | ​(Path relativeArchive |                       |
        |                       | Path,                 |                       |
        |                       |     Path memberPath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default long`        | `getSize​(Projec       | ::: block             |
        |                       | tFilesystem filesyste | Return the size of    |
        |                       | m,        Path path)` | the given relative    |
        |                       |                       | [`Path`](http://do    |
        |                       |                       | cs.oracle.com/javase/ |
        |                       |                       | 7/docs/api/java/nio/f |
        |                       |                       | ile/Path.html?is-exte |
        |                       |                       | rnal=true "class or i |
        |                       |                       | nterface in java.nio. |
        |                       |                       | file"){.externalLink} |
        |                       |                       | under the given       |
        |                       |                       | [`Projec              |
        |                       |                       | tFilesystem`](../../i |
        |                       |                       | o/filesystem/ProjectF |
        |                       |                       | ilesystem.html "inter |
        |                       |                       | face in com.facebook. |
        |                       |                       | buck.io.filesystem"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `getSize​(Path path)`  |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}
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

        []{#getSize(java.nio.file.Path)}

        -   #### getSize

            ``` methodSignature
            long getSize​(Path path)
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

        []{#get(com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path)}

        -   #### get

            ``` methodSignature
            default com.google.common.hash.HashCode get​(ProjectFilesystem filesystem,
                                                        Path path)
                                                 throws IOException
            ```

            ::: block
            Return the `HashCode` for the given relative
            [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
            under the given
            [`ProjectFilesystem`](../../io/filesystem/ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem").
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getForArchiveMember(com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path,java.nio.file.Path)}

        -   #### getForArchiveMember

            ``` methodSignature
            default com.google.common.hash.HashCode getForArchiveMember​(ProjectFilesystem filesystem,
                                                                        Path relativeArchivePath,
                                                                        Path memberPath)
                                                                 throws IOException
            ```

            ::: block
            Return the `HashCode` for the given relative
            [`ArchiveMemberPath`](../../core/io/ArchiveMemberPath.html "class in com.facebook.buck.core.io")
            under the given
            [`ProjectFilesystem`](../../io/filesystem/ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem").
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getSize(com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path)}

        -   #### getSize

            ``` methodSignature
            default long getSize​(ProjectFilesystem filesystem,
                                 Path path)
                          throws IOException
            ```

            ::: block
            Return the size of the given relative
            [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
            under the given
            [`ProjectFilesystem`](../../io/filesystem/ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem").
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
