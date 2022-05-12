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

## Interface FileHashCache {#interface-filehashcache .title title="Interface FileHashCache"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `FileHashLoader`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `StackedFileHashCache`

    ------------------------------------------------------------------------

        public interface FileHashCache
        extends FileHashLoader

    ::: block
    A cache which maps Paths to cached hashes of their contents, based
    on a simplified subset of the java.util.Map\<Path, HashCode\>
    interface.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type     Interface                                         Description
          --------------------- ------------------------------------------------- -------------
          `static interface `   `FileHashCache.FileHashCacheVerificationResult`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `default java.util.   | `debugDump()`         |                       |
        | stream.Stream<Map.Ent |                       |                       |
        | ry<Path,​com.google.co |                       |                       |
        | mmon.hash.HashCode>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `i                    |                       |
        |                       | nvalidate​(Path path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `invalidateAll()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default void`        | `set​(Proje            | ::: block             |
        |                       | ctFilesystem filesyst | Set the `HashCode`    |
        |                       | em,    Path path,     | for the given         |
        |                       | com.google.common.has | relative              |
        |                       | h.HashCode hashCode)` | [`Path`](http://do    |
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
        | `void`                | `set​(Path path,       |                       |
        |                       | com.google.common.has |                       |
        |                       | h.HashCode hashCode)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default File         | `verify()`            |                       |
        | HashCache.FileHashCac |                       |                       |
        | heVerificationResult` |                       |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.util.hashing.FileHashLoader}

            ### Methods inherited from interface com.facebook.buck.util.hashing.[FileHashLoader](../hashing/FileHashLoader.html "interface in com.facebook.buck.util.hashing")

            `get, get, getForArchiveMember, getForArchiveMember, getSize, getSize`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

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

        []{#set(com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path,com.google.common.hash.HashCode)}

        -   #### set

            ``` methodSignature
            default void set​(ProjectFilesystem filesystem,
                             Path path,
                             com.google.common.hash.HashCode hashCode)
                      throws IOException
            ```

            ::: block
            Set the `HashCode` for the given relative
            [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
            under the given
            [`ProjectFilesystem`](../../io/filesystem/ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem").
            :::

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
