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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.cell.nameresolver](package-summary.html)
:::

## Interface CellNameResolver {#interface-cellnameresolver .title title="Interface CellNameResolver"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `DefaultCellNameResolver`

    ------------------------------------------------------------------------

        public interface CellNameResolver

    ::: block
    CellNameResolver can be used for resolving cell aliases to their
    [`CanonicalCellName`](../name/CanonicalCellName.html "class in com.facebook.buck.core.cell.name").
    For a multi-cell build, each cell may have a different set of names
    that are visible to that cell (defined in that cell\'s .buckconfig),
    but each cell has a single canonical name. In addition, the names
    are not necessarily consistent across cells, two cells can have
    different names for the same cell (e.g. the most well-known such
    inconsistency would be that the empty name maps to the current cell
    in all cells).

    The CellNameResolver is different for each cell and most things
    should convert to a
    [`CanonicalCellName`](../name/CanonicalCellName.html "class in com.facebook.buck.core.cell.name")
    as soon as possible and deal only with those from then on.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `defau                | `                     | ::: block             |
        | lt CanonicalCellName` | getCurrentCellName()` | Cell name resolver    |
        |                       |                       | works in context of   |
        |                       |                       | some cell.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `getKnownCells()`     | ::: block             |
        | ommon.collect.Immutab |                       | Gets the mapping for  |
        | leMap<Optional<String |                       | all the available     |
        | >,​CanonicalCellName>` |                       | local names.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CanonicalCellName`   | `getName​(Optiona      | ::: block             |
        |                       | l<String> localName)` | Resolves the local    |
        |                       |                       | name to the           |
        |                       |                       | [`CanonicalCel        |
        |                       |                       | lName`](../name/Canon |
        |                       |                       | icalCellName.html "cl |
        |                       |                       | ass in com.facebook.b |
        |                       |                       | uck.core.cell.name"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optiona              | `getNam               | ::: block             |
        | l<CanonicalCellName>` | eIfResolvable​(Optiona | Returns the           |
        |                       | l<String> localName)` | [`CanonicalCe         |
        |                       |                       | llName`](../name/Cano |
        |                       |                       | nicalCellName.html "c |
        |                       |                       | lass in com.facebook. |
        |                       |                       | buck.core.cell.name") |
        |                       |                       | for this local name   |
        |                       |                       | if it can be          |
        |                       |                       | resolved.             |
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

        []{#getNameIfResolvable(java.util.Optional)}

        -   #### getNameIfResolvable

            ``` methodSignature
            Optional<CanonicalCellName> getNameIfResolvable​(Optional<String> localName)
            ```

            ::: block
            Returns the
            [`CanonicalCellName`](../name/CanonicalCellName.html "class in com.facebook.buck.core.cell.name")
            for this local name if it can be resolved.
            :::

        []{#getName(java.util.Optional)}

        -   #### getName

            ``` methodSignature
            CanonicalCellName getName​(Optional<String> localName)
            ```

            ::: block
            Resolves the local name to the
            [`CanonicalCellName`](../name/CanonicalCellName.html "class in com.facebook.buck.core.cell.name").
            :::

            [Throws:]{.throwsLabel}
            :   `UnknownCellException` - if the alias is not resolvable.

        []{#getKnownCells()}

        -   #### getKnownCells

            ``` methodSignature
            com.google.common.collect.ImmutableMap<Optional<String>,​CanonicalCellName> getKnownCells()
            ```

            ::: block
            Gets the mapping for all the available local names.
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
