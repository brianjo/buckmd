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

## Class Cells {#class-cells .title title="Class Cells"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.cell.Cells

::: description
-   

    ------------------------------------------------------------------------

        public class Cells
        extends Object

    ::: block
    Access all cells.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor              Description
          ------------------------ -------------
          `Cells​(Cell rootCell)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                 Method                                  Description
          ------------------------------------------------- --------------------------------------- -------------
          `com.google.common.collect.ImmutableList<Cell>`   `getAllCells()`                          
          `Cell`                                            `getCell​(CanonicalCellName cellName)`    
          `CellProvider`                                    `getCellProvider()`                      
          `Cell`                                            `getRootCell()`                          
          `AbsPath`                                         `getSuperRootPath()`                     

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

        []{#<init>(com.facebook.buck.core.cell.Cell)}

        -   #### Cells

                public Cells​(Cell rootCell)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getRootCell()}

        -   #### getRootCell

            ``` methodSignature
            public Cell getRootCell()
            ```

        []{#getCell(com.facebook.buck.core.cell.name.CanonicalCellName)}

        -   #### getCell

            ``` methodSignature
            public Cell getCell​(CanonicalCellName cellName)
            ```

        []{#getAllCells()}

        -   #### getAllCells

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Cell> getAllCells()
            ```

        []{#getCellProvider()}

        -   #### getCellProvider

            ``` methodSignature
            public CellProvider getCellProvider()
            ```

        []{#getSuperRootPath()}

        -   #### getSuperRootPath

            ``` methodSignature
            public AbsPath getSuperRootPath()
            ```

            [Returns:]{.returnLabel}
            :   Path of the topmost cell\'s path that roots all other
                cells
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
