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

## Interface CellPathResolver {#interface-cellpathresolver .title title="Interface CellPathResolver"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `AbstractCellPathResolver`, `CellPathResolverView`,
        `DefaultCellPathResolver`

    ------------------------------------------------------------------------

        public interface CellPathResolver
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `defa                 | `getCanonicalCellNa   | ::: block             |
        | ult Optional<String>` | me​(AbsPath cellPath)` | Abs-path version of   |
        |                       |                       | [`getCanoni           |
        |                       |                       | calCellName(Path)`](# |
        |                       |                       | getCanonicalCellName( |
        |                       |                       | java.nio.file.Path)). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getCanonicalCel      | ::: block             |
        |                       | lName​(Path cellPath)` | Returns a cell name   |
        |                       |                       | that can be used to   |
        |                       |                       | refer to the cell at  |
        |                       |                       | the given path.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CellNameResolver`    | `g                    | ::: block             |
        |                       | etCellNameResolver()` | Provides access to    |
        |                       |                       | the                   |
        |                       |                       | [`CellN               |
        |                       |                       | ameResolver`](nameres |
        |                       |                       | olver/CellNameResolve |
        |                       |                       | r.html "interface in  |
        |                       |                       | com.facebook.buck.cor |
        |                       |                       | e.cell.nameresolver") |
        |                       |                       | for this cell.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Path>`      | `getCellPath​(Option   |                       |
        |                       | al<String> cellName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getCe                |                       |
        |                       | llPathOrThrow​(Canonic |                       |
        |                       | alCellName cellName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getC                 |                       |
        |                       | ellPathOrThrow​(Option |                       |
        |                       | al<String> cellName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.co        | `getCellPathsByRo     |                       |
        | mmon.collect.Immutabl | otCellExternalName()` |                       |
        | eMap<String,​AbsPath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `defau                | `                     | ::: block             |
        | lt CanonicalCellName` | getCurrentCellName()` | Cell name resolver    |
        |                       |                       | works in context of   |
        |                       |                       | some cell.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `getKnownRoots()`     |                       |
        | ommon.collect.Immutab |                       |                       |
        | leSortedSet<AbsPath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `NewCellPathResolver` | `getN                 | ::: block             |
        |                       | ewCellPathResolver()` | Provides access to    |
        |                       |                       | the                   |
        |                       |                       | [`NewCell             |
        |                       |                       | PathResolver`](NewCel |
        |                       |                       | lPathResolver.html "i |
        |                       |                       | nterface in com.faceb |
        |                       |                       | ook.buck.core.cell"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `resolveCellRelati    | ::: block             |
        |                       | vePath​(CellRelativePa | Resolve a             |
        |                       | th cellRelativePath)` | cell-relative path to |
        |                       |                       | an absolute path.     |
        |                       |                       | :::                   |
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

        []{#getCurrentCellName()}

        -   #### getCurrentCellName

            ``` methodSignature
            default CanonicalCellName getCurrentCellName()
            ```

            ::: block
            Cell name resolver works in context of some cell. This
            function returns current cell.
            :::

        []{#getCellNameResolver()}

        -   #### getCellNameResolver

            ``` methodSignature
            CellNameResolver getCellNameResolver()
            ```

            ::: block
            Provides access to the
            [`CellNameResolver`](nameresolver/CellNameResolver.html "interface in com.facebook.buck.core.cell.nameresolver")
            for this cell. This is to assist in migration to the new
            name/path resolvers.
            :::

        []{#getNewCellPathResolver()}

        -   #### getNewCellPathResolver

            ``` methodSignature
            NewCellPathResolver getNewCellPathResolver()
            ```

            ::: block
            Provides access to the
            [`NewCellPathResolver`](NewCellPathResolver.html "interface in com.facebook.buck.core.cell").
            This is to assist in migration to the new name/path
            resolvers.
            :::

        []{#getCellPath(java.util.Optional)}

        -   #### getCellPath

            ``` methodSignature
            Optional<Path> getCellPath​(Optional<String> cellName)
            ```

            [Parameters:]{.paramLabel}
            :   `cellName` - name of cell, Optional.empty() for root
                cell.

            [Returns:]{.returnLabel}
            :   Absolute path to the physical location of the cell, or
                `Optional.empty()` if the cell name cannot be resolved.

        []{#getCellPathOrThrow(java.util.Optional)}

        -   #### getCellPathOrThrow

            ``` methodSignature
            Path getCellPathOrThrow​(Optional<String> cellName)
            ```

            [Parameters:]{.paramLabel}
            :   `cellName` - name of cell, Optional.empty() for root
                cell.

            [Returns:]{.returnLabel}
            :   Absolute path to the physical location of the cell

            [Throws:]{.throwsLabel}
            :   `AssertionError` - if cell is not known

        []{#getCellPathOrThrow(com.facebook.buck.core.cell.name.CanonicalCellName)}

        -   #### getCellPathOrThrow

            ``` methodSignature
            Path getCellPathOrThrow​(CanonicalCellName cellName)
            ```

            [Returns:]{.returnLabel}
            :   Absolute path to the physical location of the cell that
                contains the provided target

            [Throws:]{.throwsLabel}
            :   `AssertionError` - if cell is not known

        []{#resolveCellRelativePath(com.facebook.buck.core.model.CellRelativePath)}

        -   #### resolveCellRelativePath

            ``` methodSignature
            Path resolveCellRelativePath​(CellRelativePath cellRelativePath)
            ```

            ::: block
            Resolve a cell-relative path to an absolute path.
            :::

        []{#getCellPathsByRootCellExternalName()}

        -   #### getCellPathsByRootCellExternalName

            ``` methodSignature
            com.google.common.collect.ImmutableMap<String,​AbsPath> getCellPathsByRootCellExternalName()
            ```

            [Returns:]{.returnLabel}
            :   absolute paths to all cells this resolver knows about.
                The key is the name of the cell in the root cell\'s
                config (this is not necessarily the canonical name).

        []{#getCanonicalCellName(java.nio.file.Path)}

        -   #### getCanonicalCellName

            ``` methodSignature
            Optional<String> getCanonicalCellName​(Path cellPath)
            ```

            ::: block
            Returns a cell name that can be used to refer to the cell at
            the given path.
            Returns `Optional.empty()` if the path refers to the root
            cell. Returns the lexicographically smallest name if the
            cell path has multiple names.

            Note: this is not the inverse of
            [`getCellPath(Optional)`](#getCellPath(java.util.Optional)),
            which returns the current, rather than the root, cell path
            if the cell name is empty.
            :::

            [Throws:]{.throwsLabel}
            :   `IllegalArgumentException` - if cell path is not known
                to the CellPathResolver.

        []{#getCanonicalCellName(com.facebook.buck.core.filesystems.AbsPath)}

        -   #### getCanonicalCellName

            ``` methodSignature
            default Optional<String> getCanonicalCellName​(AbsPath cellPath)
            ```

            ::: block
            Abs-path version of
            [`getCanonicalCellName(Path)`](#getCanonicalCellName(java.nio.file.Path)).
            :::

        []{#getKnownRoots()}

        -   #### getKnownRoots

            ``` methodSignature
            com.google.common.collect.ImmutableSortedSet<AbsPath> getKnownRoots()
            ```

            [Returns:]{.returnLabel}
            :   paths to roots of all cells known to this resolver.
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
