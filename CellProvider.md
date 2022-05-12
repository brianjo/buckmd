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

## Class CellProvider {#class-cellprovider .title title="Class CellProvider"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.cell.CellProvider

::: description
-   

    ------------------------------------------------------------------------

        public final class CellProvider
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `CellProvider​(NewCel              | ::: block                         |
        | lPathResolver newCellPathResolver | Create a cell provider with a     |
        | ,             java.util.function. | specific cell loader, and         |
        | Function<CellProvider,​com.google. | optionally a special factory      |
        | common.cache.CacheLoader<AbsPath, | function for the root cell.       |
        | ​Cell>> cellCacheLoader,           | :::                               |
        |    java.util.function.Function<Ce |                                   |
        | llProvider,​Cell> rootCellLoader)` |                                   |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Cell`                | `g                    | ::: block             |
        |                       | etCellByCanonicalCell | Get cell object by    |
        |                       | Name​(CanonicalCellNam | canonicall cell name  |
        |                       | e canonicalCellName)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Cell`                | `getCell              |                       |
        |                       | ByPath​(AbsPath path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Cell`                | `getC                 |                       |
        |                       | ellByPath​(Path path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getLoadedCells()`    |                       |
        | common.collect.Immuta |                       |                       |
        | bleMap<AbsPath,​Cell>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Cells`               | `getRootCell()`       |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.cell.NewCellPathResolver,java.util.function.Function,java.util.function.Function)}

        -   #### CellProvider

                public CellProvider​(NewCellPathResolver newCellPathResolver,
                                    java.util.function.Function<CellProvider,​com.google.common.cache.CacheLoader<AbsPath,​Cell>> cellCacheLoader,
                                    @Nullable
                                    java.util.function.Function<CellProvider,​Cell> rootCellLoader)

            ::: block
            Create a cell provider with a specific cell loader, and
            optionally a special factory function for the root cell.
            The indirection for passing in CellProvider allows cells to
            reference the current CellProvider object.
            :::
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getCellByPath(java.nio.file.Path)}

        -   #### getCellByPath

            ``` methodSignature
            public Cell getCellByPath​(Path path)
            ```

        []{#getCellByPath(com.facebook.buck.core.filesystems.AbsPath)}

        -   #### getCellByPath

            ``` methodSignature
            public Cell getCellByPath​(AbsPath path)
            ```

        []{#getCellByCanonicalCellName(com.facebook.buck.core.cell.name.CanonicalCellName)}

        -   #### getCellByCanonicalCellName

            ``` methodSignature
            public Cell getCellByCanonicalCellName​(CanonicalCellName canonicalCellName)
            ```

            ::: block
            Get cell object by canonicall cell name
            :::

        []{#getRootCell()}

        -   #### getRootCell

            ``` methodSignature
            public Cells getRootCell()
            ```

        []{#getLoadedCells()}

        -   #### getLoadedCells

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<AbsPath,​Cell> getLoadedCells()
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
