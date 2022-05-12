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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
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

## Class CellPathResolverView {#class-cellpathresolverview .title title="Class CellPathResolverView"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.cell.AbstractCellPathResolver](AbstractCellPathResolver.html "class in com.facebook.buck.core.cell")

    -   -   com.facebook.buck.core.cell.CellPathResolverView

::: description
-   

    All Implemented Interfaces:
    :   `CellPathResolver`

    ------------------------------------------------------------------------

        public final class CellPathResolverView
        extends AbstractCellPathResolver

    ::: block
    View of a subset of cells of a cell path resolver.
    Views are used for non-root cells, to ensure that only the subset of
    cell names that the cell declares are visible within that cell.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                         Description
          ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `CellPathResolverView​(CellPathResolver delegate,                     CellNameResolver cellNameResolver,                     com.google.common.collect.ImmutableSet<String> declaredCellNames,                     Path cellPath)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `eq                   |                       |
        |                       | uals​(Object another)` |                       |
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
        | `com.google.co        | `getCellPathsByRo     |                       |
        | mmon.collect.Immutabl | otCellExternalName()` |                       |
        | eMap<String,​AbsPath>` |                       |                       |
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
        | `int`                 | `hashCode()`          |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.cell.AbstractCellPathResolver}

            ### Methods inherited from class com.facebook.buck.core.cell.[AbstractCellPathResolver](AbstractCellPathResolver.html "class in com.facebook.buck.core.cell")

            `getCellPathOrThrow, getCellPathOrThrow, getKnownRoots, resolveCellRelativePath`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.cell.CellPathResolver}

            ### Methods inherited from interface com.facebook.buck.core.cell.[CellPathResolver](CellPathResolver.html "interface in com.facebook.buck.core.cell")

            `getCanonicalCellName, getCurrentCellName`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.cell.CellPathResolver,com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.google.common.collect.ImmutableSet,java.nio.file.Path)}

        -   #### CellPathResolverView

                public CellPathResolverView​(CellPathResolver delegate,
                                            CellNameResolver cellNameResolver,
                                            com.google.common.collect.ImmutableSet<String> declaredCellNames,
                                            Path cellPath)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getCellNameResolver()}

        -   #### getCellNameResolver

            ``` methodSignature
            public CellNameResolver getCellNameResolver()
            ```

            ::: block
            [Description copied from
            interface: `CellPathResolver`]{.descfrmTypeLabel}
            :::

            ::: block
            Provides access to the
            [`CellNameResolver`](nameresolver/CellNameResolver.html "interface in com.facebook.buck.core.cell.nameresolver")
            for this cell. This is to assist in migration to the new
            name/path resolvers.
            :::

        []{#getNewCellPathResolver()}

        -   #### getNewCellPathResolver

            ``` methodSignature
            public NewCellPathResolver getNewCellPathResolver()
            ```

            ::: block
            [Description copied from
            interface: `CellPathResolver`]{.descfrmTypeLabel}
            :::

            ::: block
            Provides access to the
            [`NewCellPathResolver`](NewCellPathResolver.html "interface in com.facebook.buck.core.cell").
            This is to assist in migration to the new name/path
            resolvers.
            :::

        []{#getCellPath(java.util.Optional)}

        -   #### getCellPath

            ``` methodSignature
            public Optional<Path> getCellPath​(Optional<String> cellName)
            ```

            [Parameters:]{.paramLabel}
            :   `cellName` - name of cell, Optional.empty() for root
                cell.

            [Returns:]{.returnLabel}
            :   Absolute path to the physical location of the cell, or
                `Optional.empty()` if the cell name cannot be resolved.

        []{#getCellPathsByRootCellExternalName()}

        -   #### getCellPathsByRootCellExternalName

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​AbsPath> getCellPathsByRootCellExternalName()
            ```

            [Returns:]{.returnLabel}
            :   absolute paths to all cells this resolver knows about.
                The key is the name of the cell in the root cell\'s
                config (this is not necessarily the canonical name).

        []{#getCanonicalCellName(java.nio.file.Path)}

        -   #### getCanonicalCellName

            ``` methodSignature
            public Optional<String> getCanonicalCellName​(Path cellPath)
            ```

            ::: block
            [Description copied from
            interface: `CellPathResolver`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns a cell name that can be used to refer to the cell at
            the given path.
            Returns `Optional.empty()` if the path refers to the root
            cell. Returns the lexicographically smallest name if the
            cell path has multiple names.

            Note: this is not the inverse of
            [`CellPathResolver.getCellPath(Optional)`](CellPathResolver.html#getCellPath(java.util.Optional)),
            which returns the current, rather than the root, cell path
            if the cell name is empty.
            :::

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object another)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`
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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
