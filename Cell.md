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

## Interface Cell {#interface-cell .title title="Interface Cell"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface Cell

    ::: block
    Represents a single checkout of a code base. Two cells model the
    same code base if their underlying
    [`ProjectFilesystem`](../../io/filesystem/ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem")s
    are equal.
    Should only be constructed by
    [`CellProvider`](CellProvider.html "class in com.facebook.buck.core.cell").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.                 | `getAllCells()`       | ::: block             |
        | google.common.collect |                       | Returns a list of all |
        | .ImmutableList<Cell>` |                       | cells, including this |
        |                       |                       | cell.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `BuckConfig`          | `getBuckConfig()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `<T extends Conf      | `getBuckConf          | ::: block             |
        | igView<BuckConfig>>T` | igView​(Class<T> cls)` | See                   |
        |                       |                       | [`BuckConfig.getVi    |
        |                       |                       | ew(Class)`](../config |
        |                       |                       | /BuckConfig.html#getV |
        |                       |                       | iew(java.lang.Class)) |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CanonicalCellName`   | `getCanonicalName()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Cell`                | `getCell​(Canonic      |                       |
        |                       | alCellName cellName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Cell`                | `ge                   |                       |
        |                       | tCell​(Path cellPath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Cell`                | `getC                 |                       |
        |                       | ellIgnoringVisibility |                       |
        |                       | Check​(Path cellPath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `CellNameResolver`    | `g                    | ::: block             |
        |                       | etCellNameResolver()` | Return the            |
        |                       |                       | [`CellN               |
        |                       |                       | ameResolver`](nameres |
        |                       |                       | olver/CellNameResolve |
        |                       |                       | r.html "interface in  |
        |                       |                       | com.facebook.buck.cor |
        |                       |                       | e.cell.nameresolver") |
        |                       |                       | for this cell.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CellPathResolver`    | `g                    |                       |
        |                       | etCellPathResolver()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `CellProvider`        | `getCellProvider()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ProjectFilesystem`   | `getFilesystem()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `getFilesystem        |                       |
        | rojectFilesystemView` | ViewForSourceFiles()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `getKn                |                       |
        | ommon.collect.Immutab | ownRootsOfAllCells()` |                       |
        | leSortedSet<AbsPath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getLoadedCells()`    |                       |
        | common.collect.Immuta |                       |                       |
        | bleMap<AbsPath,​Cell>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `NewCellPathResolver` | `getN                 | ::: block             |
        |                       | ewCellPathResolver()` | Return the            |
        |                       |                       | [`NewCell             |
        |                       |                       | PathResolver`](NewCel |
        |                       |                       | lPathResolver.html "i |
        |                       |                       | nterface in com.faceb |
        |                       |                       | ook.buck.core.cell"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AbsPath`             | `getRoot()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ToolchainProvider`   | `ge                   |                       |
        |                       | tToolchainProvider()` |                       |
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

        []{#getKnownRootsOfAllCells()}

        -   #### getKnownRootsOfAllCells

            ``` methodSignature
            com.google.common.collect.ImmutableSortedSet<AbsPath> getKnownRootsOfAllCells()
            ```

        []{#getCanonicalName()}

        -   #### getCanonicalName

            ``` methodSignature
            CanonicalCellName getCanonicalName()
            ```

        []{#getFilesystem()}

        -   #### getFilesystem

            ``` methodSignature
            ProjectFilesystem getFilesystem()
            ```

        []{#getFilesystemViewForSourceFiles()}

        -   #### getFilesystemViewForSourceFiles

            ``` methodSignature
            ProjectFilesystemView getFilesystemViewForSourceFiles()
            ```

            [Returns:]{.returnLabel}
            :   [`ProjectFilesystemView`](../../io/filesystem/ProjectFilesystemView.html "interface in com.facebook.buck.io.filesystem")
                that filters out ignores specified for this cell, like
                blacklisted paths and buck-out, to iterate over files
                which are potential direct sources, build files, etc.

        []{#getBuckConfig()}

        -   #### getBuckConfig

            ``` methodSignature
            BuckConfig getBuckConfig()
            ```

        []{#getBuckConfigView(java.lang.Class)}

        -   #### getBuckConfigView

            ``` methodSignature
            <T extends ConfigView<BuckConfig>> T getBuckConfigView​(Class<T> cls)
            ```

            ::: block
            See
            [`BuckConfig.getView(Class)`](../config/BuckConfig.html#getView(java.lang.Class))
            :::

        []{#getCellProvider()}

        -   #### getCellProvider

            ``` methodSignature
            CellProvider getCellProvider()
            ```

        []{#getToolchainProvider()}

        -   #### getToolchainProvider

            ``` methodSignature
            ToolchainProvider getToolchainProvider()
            ```

        []{#getRoot()}

        -   #### getRoot

            ``` methodSignature
            AbsPath getRoot()
            ```

        []{#getCellIgnoringVisibilityCheck(java.nio.file.Path)}

        -   #### getCellIgnoringVisibilityCheck

            ``` methodSignature
            Cell getCellIgnoringVisibilityCheck​(Path cellPath)
            ```

        []{#getCell(java.nio.file.Path)}

        -   #### getCell

            ``` methodSignature
            Cell getCell​(Path cellPath)
            ```

        []{#getCell(com.facebook.buck.core.cell.name.CanonicalCellName)}

        -   #### getCell

            ``` methodSignature
            Cell getCell​(CanonicalCellName cellName)
            ```

        []{#getAllCells()}

        -   #### getAllCells

            ``` methodSignature
            com.google.common.collect.ImmutableList<Cell> getAllCells()
            ```

            ::: block
            Returns a list of all cells, including this cell. If this
            cell is the root, getAllCells will necessarily return all
            possible cells that this build may interact with, since the
            root cell is required to declare a mapping for all cell
            names.
            :::

        []{#getLoadedCells()}

        -   #### getLoadedCells

            ``` methodSignature
            com.google.common.collect.ImmutableMap<AbsPath,​Cell> getLoadedCells()
            ```

            [Returns:]{.returnLabel}
            :   all loaded
                [`Cell`](Cell.html "interface in com.facebook.buck.core.cell")s
                that are children of this
                [`Cell`](Cell.html "interface in com.facebook.buck.core.cell").

        []{#getCellPathResolver()}

        -   #### getCellPathResolver

            ``` methodSignature
            CellPathResolver getCellPathResolver()
            ```

        []{#getNewCellPathResolver()}

        -   #### getNewCellPathResolver

            ``` methodSignature
            NewCellPathResolver getNewCellPathResolver()
            ```

            ::: block
            Return the
            [`NewCellPathResolver`](NewCellPathResolver.html "interface in com.facebook.buck.core.cell").
            This can be used to map between canonical names and cell
            root paths.
            :::

        []{#getCellNameResolver()}

        -   #### getCellNameResolver

            ``` methodSignature
            CellNameResolver getCellNameResolver()
            ```

            ::: block
            Return the
            [`CellNameResolver`](nameresolver/CellNameResolver.html "interface in com.facebook.buck.core.cell.nameresolver")
            for this cell. This can be used to resolve user-provided
            cell aliases to their canonical names.
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
