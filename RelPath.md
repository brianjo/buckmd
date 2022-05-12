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

## Interface RelPath {#interface-relpath .title title="Interface RelPath"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `PathWrapper`

    ------------------------------------------------------------------------

        public interface RelPath
        extends PathWrapper

    ::: block
    Relative path.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static RelPath`      | `get​(String first     | ::: block             |
        |                       | ,    String... more)` | Construct a path.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default RelPath`     | `getParent()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default RelPath`     | `normalize()`         | ::: block             |
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
        | `static RelPath`      | `of​(Path path)`       | ::: block             |
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
        | `default RelPath`     | `re                   |                       |
        |                       | solve​(RelPath other)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default Path`        | `r                    |                       |
        |                       | esolve​(String other)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default RelPath`     | `reso                 |                       |
        |                       | lveRel​(String other)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default RelPath`     | `sub                  |                       |
        |                       | path​(int beginIndex,  |                       |
        |                       |        int endIndex)` |                       |
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
            static RelPath of​(Path path)
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

        []{#get(java.lang.String,java.lang.String...)}

        -   #### get

            ``` methodSignature
            static RelPath get​(String first,
                               String... more)
            ```

            ::: block
            Construct a path.
            :::

            [Throws:]{.throwsLabel}
            :   `RuntimeException` - if the path is absolute.

        []{#normalize()}

        -   #### normalize

            ``` methodSignature
            default RelPath normalize()
            ```

            ::: block
            Behaves exactly like
            [`Path.normalize()`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true#normalize() "class or interface in java.nio.file"){.externalLink}.
            :::

        []{#getParent()}

        -   #### getParent

            ``` methodSignature
            default RelPath getParent()
            ```

        []{#resolve(java.lang.String)}

        -   #### resolve

            ``` methodSignature
            default Path resolve​(String other)
            ```

        []{#resolveRel(java.lang.String)}

        -   #### resolveRel

            ``` methodSignature
            default RelPath resolveRel​(String other)
            ```

        []{#resolve(com.facebook.buck.core.filesystems.RelPath)}

        -   #### resolve

            ``` methodSignature
            default RelPath resolve​(RelPath other)
            ```

        []{#subpath(int,int)}

        -   #### subpath

            ``` methodSignature
            default RelPath subpath​(int beginIndex,
                                    int endIndex)
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
