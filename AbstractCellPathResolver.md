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

## Class AbstractCellPathResolver {#class-abstractcellpathresolver .title title="Class AbstractCellPathResolver"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.cell.AbstractCellPathResolver

::: description
-   

    All Implemented Interfaces:
    :   `CellPathResolver`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `CellPathResolverView`, `DefaultCellPathResolver`

    ------------------------------------------------------------------------

        public abstract class AbstractCellPathResolver
        extends Object
        implements CellPathResolver

    ::: block
    Contains base logic for
    [`CellPathResolver`](CellPathResolver.html "interface in com.facebook.buck.core.cell").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                    Description
          ------------------------------ -------------
          `AbstractCellPathResolver()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Path`                | `getCe                |                       |
        |                       | llPathOrThrow​(Canonic |                       |
        |                       | alCellName cellName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getC                 |                       |
        |                       | ellPathOrThrow​(Option |                       |
        |                       | al<String> cellName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `getKnownRoots()`     |                       |
        | ommon.collect.Immutab |                       |                       |
        | leSortedSet<AbsPath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `resolveCellRelati    | ::: block             |
        |                       | vePath​(CellRelativePa | Resolve a             |
        |                       | th cellRelativePath)` | cell-relative path to |
        |                       |                       | an absolute path.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.cell.CellPathResolver}

            ### Methods inherited from interface com.facebook.buck.core.cell.[CellPathResolver](CellPathResolver.html "interface in com.facebook.buck.core.cell")

            `getCanonicalCellName, getCanonicalCellName, getCellNameResolver, getCellPath, getCellPathsByRootCellExternalName, getCurrentCellName, getNewCellPathResolver`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### AbstractCellPathResolver

                public AbstractCellPathResolver()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getKnownRoots()}

        -   #### getKnownRoots

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<AbsPath> getKnownRoots()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getKnownRoots` in interface `CellPathResolver`

            [Returns:]{.returnLabel}
            :   sorted set of known roots in reverse natural order

        []{#getCellPathOrThrow(java.util.Optional)}

        -   #### getCellPathOrThrow

            ``` methodSignature
            public Path getCellPathOrThrow​(Optional<String> cellName)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCellPathOrThrow` in interface `CellPathResolver`

            [Parameters:]{.paramLabel}
            :   `cellName` - name of cell, Optional.empty() for root
                cell.

            [Returns:]{.returnLabel}
            :   Absolute path to the physical location of the cell

        []{#getCellPathOrThrow(com.facebook.buck.core.cell.name.CanonicalCellName)}

        -   #### getCellPathOrThrow

            ``` methodSignature
            public Path getCellPathOrThrow​(CanonicalCellName cellName)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCellPathOrThrow` in interface `CellPathResolver`

            [Returns:]{.returnLabel}
            :   Absolute path to the physical location of the cell that
                contains the provided target

        []{#resolveCellRelativePath(com.facebook.buck.core.model.CellRelativePath)}

        -   #### resolveCellRelativePath

            ``` methodSignature
            public Path resolveCellRelativePath​(CellRelativePath cellRelativePath)
            ```

            ::: block
            [Description copied from
            interface: `CellPathResolver`]{.descfrmTypeLabel}
            :::

            ::: block
            Resolve a cell-relative path to an absolute path.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolveCellRelativePath` in
                interface `CellPathResolver`
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
