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

## Interface PathWrapper {#interface-pathwrapper .title title="Interface PathWrapper"}
:::

::: contentContainer
::: description
-   

    All Known Subinterfaces:
    :   `AbsPath`, `RelPath`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `BuckUnixPath`

    ------------------------------------------------------------------------

        public interface PathWrapper

    ::: block
    [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
    wrapper object, either absolute or relative.
    Note this object is implemented directly for
    [`BuckUnixPath`](BuckUnixPath.html "class in com.facebook.buck.core.filesystems").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `default boolean`     | `en                   |                       |
        |                       | dsWith​(String other)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `endsWith​(Path path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `equals​(Object that)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `equals​(Path that)`   | ::: block             |
        |                       |                       | [Deprecate            |
        |                       |                       | d.]{.deprecatedLabel} |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default FileSystem`  | `getFileSystem()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getPath()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `st                   |                       |
        |                       | artsWith​(Path other)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5
        .tableTab}[[Deprecated
        Methods](javascript:show(32);)[ ]{.tabEnd}]{#t6 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getPath()}

        -   #### getPath

            ``` methodSignature
            Path getPath()
            ```

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            boolean equals​(Object that)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

        []{#equals(java.nio.file.Path)}

        -   #### equals

            ``` methodSignature
            @Deprecated
            default boolean equals​(Path that)
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            ::: block
            This overload should not be used.
            This code is incorrect:
            `  AbsPath p1 = ...  Path p2 = ...  p1.equals(p2);  `
            because `AbsPath` and
            [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
            are different \"types\" and should not be equal according to
            [`Object.equals(Object)`](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true#equals(java.lang.Object) "class or interface in java.lang"){.externalLink}
            contract.

            This overload helps to catch this error.
            :::

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`

        []{#toString()}

        -   #### toString

            ``` methodSignature
            String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#endsWith(java.lang.String)}

        -   #### endsWith

            ``` methodSignature
            default boolean endsWith​(String other)
            ```

        []{#endsWith(java.nio.file.Path)}

        -   #### endsWith

            ``` methodSignature
            default boolean endsWith​(Path path)
            ```

        []{#getFileSystem()}

        -   #### getFileSystem

            ``` methodSignature
            default FileSystem getFileSystem()
            ```

        []{#startsWith(java.nio.file.Path)}

        -   #### startsWith

            ``` methodSignature
            default boolean startsWith​(Path other)
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
