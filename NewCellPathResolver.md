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
[Package]{.packageLabelInType} [com.facebook.buck.core.cell](package-summary.html)
:::

## Interface NewCellPathResolver {#interface-newcellpathresolver .title title="Interface NewCellPathResolver"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `DefaultNewCellPathResolver`

    ------------------------------------------------------------------------

        public interface NewCellPathResolver

    ::: block
    The
    [`NewCellPathResolver`](NewCellPathResolver.html "interface in com.facebook.buck.core.cell")
    maps between
    [`CanonicalCellName`](name/CanonicalCellName.html "class in com.facebook.buck.core.cell.name")s
    and the absolute
    [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
    that they are rooted at.
    The behavior of
    [`NewCellPathResolver`](NewCellPathResolver.html "interface in com.facebook.buck.core.cell")
    is the same for all cells in a build (unlike
    [`CellPathResolver`](CellPathResolver.html "interface in com.facebook.buck.core.cell")).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `CanonicalCellName`   | `getCanonica          |                       |
        |                       | lCellName​(Path path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getCellPath​(Canonic  | ::: block             |
        |                       | alCellName cellName)` | Note: unlike          |
        |                       |                       | [`CellPathRes         |
        |                       |                       | olver.getCellPath(Opt |
        |                       |                       | ional)`](CellPathReso |
        |                       |                       | lver.html#getCellPath |
        |                       |                       | (java.util.Optional)) |
        |                       |                       | this function always  |
        |                       |                       | returns a value.      |
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

        []{#getCellPath(com.facebook.buck.core.cell.name.CanonicalCellName)}

        -   #### getCellPath

            ``` methodSignature
            Path getCellPath​(CanonicalCellName cellName)
            ```

            ::: block
            Note: unlike
            [`CellPathResolver.getCellPath(Optional)`](CellPathResolver.html#getCellPath(java.util.Optional))
            this function always returns a value. Existence/visibility
            of the cell is enforced when the
            [`CanonicalCellName`](name/CanonicalCellName.html "class in com.facebook.buck.core.cell.name")
            is resolved.
            :::

            [Parameters:]{.paramLabel}
            :   `cellName` - Canonical name of the cell.

            [Returns:]{.returnLabel}
            :   Absolute path to the physical root of the cell.

        []{#getCanonicalCellName(java.nio.file.Path)}

        -   #### getCanonicalCellName

            ``` methodSignature
            CanonicalCellName getCanonicalCellName​(Path path)
            ```

            [Parameters:]{.paramLabel}
            :   `path` - Absolute path to the physical root of the cell.

            [Returns:]{.returnLabel}
            :   Canonical name of the cell.
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
