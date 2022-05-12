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
-   Package
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Package com.facebook.buck.core.cell {#package-com.facebook.buck.core.cell .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [Cell](Cell.html "interface       | ::: block                         |
    |  in com.facebook.buck.core.cell") | Represents a single checkout of a |
    |                                   | code base.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CellPathResolver]                |                                   |
    | (CellPathResolver.html "interface |                                   |
    |  in com.facebook.buck.core.cell") |                                   |
    +-----------------------------------+-----------------------------------+
    | [NewCellPathResolver](Ne          | ::: block                         |
    | wCellPathResolver.html "interface | The                               |
    |  in com.facebook.buck.core.cell") | [`NewCellPathResolver`](Ne        |
    |                                   | wCellPathResolver.html "interface |
    |                                   |  in com.facebook.buck.core.cell") |
    |                                   | maps between                      |
    |                                   | [`CanonicalCellName`](name/Ca     |
    |                                   | nonicalCellName.html "class in co |
    |                                   | m.facebook.buck.core.cell.name")s |
    |                                   | and the absolute                  |
    |                                   | [`Path`](htt                      |
    |                                   | p://docs.oracle.com/javase/7/docs |
    |                                   | /api/java/nio/file/Path.html?is-e |
    |                                   | xternal=true "class or interface  |
    |                                   | in java.nio.file"){.externalLink} |
    |                                   | that they are rooted at.          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [AbstractCellPathResolver](Abs    | ::: block                         |
    | tractCellPathResolver.html "class | Contains base logic for           |
    |  in com.facebook.buck.core.cell") | [`CellPathResolver`](             |
    |                                   | CellPathResolver.html "interface  |
    |                                   | in com.facebook.buck.core.cell"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [C                                | ::: block                         |
    | ellConfig](CellConfig.html "class | Hierarcical configuration of      |
    |  in com.facebook.buck.core.cell") | cell/section/key/value            |
    |                                   | quadruples.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CellConfig.Builde                | ::: block                         |
    | r](CellConfig.Builder.html "class | A builder for                     |
    |  in com.facebook.buck.core.cell") | [`Cell                            |
    |                                   | Config`](CellConfig.html "class i |
    |                                   | n com.facebook.buck.core.cell")s. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CellName](CellName.html "class   | ::: block                         |
    |  in com.facebook.buck.core.cell") | Describes a cell name relative to |
    |                                   | another cell.                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CellPathResolverView]            | ::: block                         |
    | (CellPathResolverView.html "class | View of a subset of cells of a    |
    |  in com.facebook.buck.core.cell") | cell path resolver.               |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CellP                            |                                   |
    | rovider](CellProvider.html "class |                                   |
    |  in com.facebook.buck.core.cell") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Cells](Cells.html "class         | ::: block                         |
    |  in com.facebook.buck.core.cell") | Access all cells.                 |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DefaultCel                       | ::: block                         |
    | lNameResolverProvider](DefaultCel | Cell name resolver provider from  |
    | lNameResolverProvider.html "class | the root cell.                    |
    |  in com.facebook.buck.core.cell") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | DefaultNewCellPathResolver](Defau | Implementation of                 |
    | ltNewCellPathResolver.html "class | [`NewCellPathResolver`](Ne        |
    |  in com.facebook.buck.core.cell") | wCellPathResolver.html "interface |
    |                                   |  in com.facebook.buck.core.cell") |
    |                                   | based on the path to name map     |
    |                                   | (this is assumed to be 1-1).      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Exception                         | Description                       |
    +===================================+===================================+
    | [Inva                             | ::: block                         |
    | lidCellOverrideException](Invalid | An exception thrown when trying   |
    | CellOverrideException.html "class | to perform invalid cell override. |
    |  in com.facebook.buck.core.cell") | :::                               |
    +-----------------------------------+-----------------------------------+

    : Exception Summary[ ]{.tabEnd}
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../../index.html)
-   Package
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

[]{#skip.navbar.bottom}
:::
