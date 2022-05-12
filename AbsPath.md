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
[Package]{.packageLabelInType} [com.facebook.buck.core.filesystems](package-summary.html)
:::

## Interface AbsPath {#interface-abspath .title title="Interface AbsPath"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `PathWrapper`

    ------------------------------------------------------------------------

        public interface AbsPath
        extends PathWrapper

    ::: block
    Absolute path.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static               | `comparator()`        | ::: block             |
        |  Comparator<AbsPath>` |                       | We cannot implement   |
        |                       |                       | [                     |
        |                       |                       | `Comparable`](http:// |
        |                       |                       | docs.oracle.com/javas |
        |                       |                       | e/7/docs/api/java/lan |
        |                       |                       | g/Comparable.html?is- |
        |                       |                       | external=true "class  |
        |                       |                       | or interface in java. |
        |                       |                       | lang"){.externalLink} |
        |                       |                       | directly.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static AbsPath`      | `get​(String path)`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default AbsPath`     | `getParent()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default AbsPath`     | `getRoot()`           | ::: block             |
        |                       |                       | Get the filesystem    |
        |                       |                       | root of the current   |
        |                       |                       | path.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default AbsPath`     | `normalize()`         | ::: block             |
        |                       |                       | Behaves exactly like  |
        |                       |                       | [                     |
        |                       |                       | `Path.normalize()`](h |
        |                       |                       | ttp://docs.oracle.com |
        |                       |                       | /javase/7/docs/api/ja |
        |                       |                       | va/nio/file/Path.html |
        |                       |                       | ?is-external=true#nor |
        |                       |                       | malize() "class or in |
        |                       |                       | terface in java.nio.f |
        |                       |                       | ile"){.externalLink}. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static AbsPath`      | `of​(Path path)`       | ::: block             |
        |                       |                       | Cosnstruct using      |
        |                       |                       | [`Path`](http://do    |
        |                       |                       | cs.oracle.com/javase/ |
        |                       |                       | 7/docs/api/java/nio/f |
        |                       |                       | ile/Path.html?is-exte |
        |                       |                       | rnal=true "class or i |
        |                       |                       | nterface in java.nio. |
        |                       |                       | file"){.externalLink} |
        |                       |                       | object.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default RelPath`     | `relat                |                       |
        |                       | ivize​(AbsPath other)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default RelPath`     | `re                   |                       |
        |                       | lativize​(Path other)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default AbsPath`     | `re                   |                       |
        |                       | solve​(RelPath other)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default AbsPath`     | `                     |                       |
        |                       | resolve​(String path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default AbsPath`     | `resolve​(Path path)`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `star                 |                       |
        |                       | tsWith​(AbsPath path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default File`        | `toFile()`            |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default AbsPath`     | `toRealPath​(Li        |                       |
        |                       | nkOption... options)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.filesystems.PathWrapper}

            ### Methods inherited from interface com.facebook.buck.core.filesystems.[PathWrapper](PathWrapper.html "interface in com.facebook.buck.core.filesystems")

            `endsWith, endsWith, equals, equals, getFileSystem, getPath, hashCode, startsWith, toString`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#of(java.nio.file.Path)}

        -   #### of

            ``` methodSignature
            static AbsPath of​(Path path)
            ```

            ::: block
            Cosnstruct using
            [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
            object.
            Note this operation is just a cast if the path is
            [`BuckUnixPath`](BuckUnixPath.html "class in com.facebook.buck.core.filesystems").
            :::

            [Throws:]{.throwsLabel}
            :   `RuntimeException` - the path is not absolute.

        []{#get(java.lang.String)}

        -   #### get

            ``` methodSignature
            static AbsPath get​(String path)
            ```

        []{#normalize()}

        -   #### normalize

            ``` methodSignature
            default AbsPath normalize()
            ```

            ::: block
            Behaves exactly like
            [`Path.normalize()`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true#normalize() "class or interface in java.nio.file"){.externalLink}.
            :::

        []{#toRealPath(java.nio.file.LinkOption...)}

        -   #### toRealPath

            ``` methodSignature
            default AbsPath toRealPath​(LinkOption... options)
                                throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#resolve(com.facebook.buck.core.filesystems.RelPath)}

        -   #### resolve

            ``` methodSignature
            default AbsPath resolve​(RelPath other)
            ```

        []{#startsWith(com.facebook.buck.core.filesystems.AbsPath)}

        -   #### startsWith

            ``` methodSignature
            default boolean startsWith​(AbsPath path)
            ```

        []{#resolve(java.nio.file.Path)}

        -   #### resolve

            ``` methodSignature
            default AbsPath resolve​(Path path)
            ```

        []{#resolve(java.lang.String)}

        -   #### resolve

            ``` methodSignature
            default AbsPath resolve​(String path)
            ```

        []{#getParent()}

        -   #### getParent

            ``` methodSignature
            default AbsPath getParent()
            ```

        []{#relativize(java.nio.file.Path)}

        -   #### relativize

            ``` methodSignature
            default RelPath relativize​(Path other)
            ```

        []{#relativize(com.facebook.buck.core.filesystems.AbsPath)}

        -   #### relativize

            ``` methodSignature
            default RelPath relativize​(AbsPath other)
            ```

        []{#getRoot()}

        -   #### getRoot

            ``` methodSignature
            default AbsPath getRoot()
            ```

            ::: block
            Get the filesystem root of the current path. Note unlike
            [`Path.getRoot()`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true#getRoot() "class or interface in java.nio.file"){.externalLink}
            this function never returns `null` because absolute paths
            always have root.
            :::

        []{#toFile()}

        -   #### toFile

            ``` methodSignature
            default File toFile()
            ```

        []{#comparator()}

        -   #### comparator

            ``` methodSignature
            static Comparator<AbsPath> comparator()
            ```

            ::: block
            We cannot implement
            [`Comparable`](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}
            directly.
            :::
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
