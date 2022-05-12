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
[Package]{.packageLabelInType} [com.facebook.buck.io.filesystem](package-summary.html)
:::

## Class EmbeddedCellBuckOutInfo {#class-embeddedcellbuckoutinfo .title title="Class EmbeddedCellBuckOutInfo"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.io.filesystem.EmbeddedCellBuckOutInfo

::: description
-   

    ------------------------------------------------------------------------

        public abstract class EmbeddedCellBuckOutInfo
        extends Object

    ::: block
    Information to create the buck-out of cell when it\'s going to be
    embedded in the root cell buck-out.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                   Description
          ----------------------------- -------------
          `EmbeddedCellBuckOutInfo()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Path`                | `getCellBuckOut()`    | ::: block             |
        |                       |                       | Returns an absolute   |
        |                       |                       | path to the cell\'s   |
        |                       |                       | buck-out embedded     |
        |                       |                       | inside the root\'s    |
        |                       |                       | buck-out              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstra               | `getCellName()`       |                       |
        | ct CanonicalCellName` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract BuckPaths`  | `ge                   |                       |
        |                       | tMainCellBuckPaths()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Path`       | `getMainCellRoot()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Emb           | `of​(Path mainCellRoot |                       |
        | eddedCellBuckOutInfo` | ,   BuckPaths mainCel |                       |
        |                       | lBuckPaths,   Canonic |                       |
        |                       | alCellName cellName)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

        []{#<init>()}

        -   #### EmbeddedCellBuckOutInfo

                public EmbeddedCellBuckOutInfo()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getMainCellRoot()}

        -   #### getMainCellRoot

            ``` methodSignature
            public abstract Path getMainCellRoot()
            ```

        []{#getMainCellBuckPaths()}

        -   #### getMainCellBuckPaths

            ``` methodSignature
            public abstract BuckPaths getMainCellBuckPaths()
            ```

        []{#getCellName()}

        -   #### getCellName

            ``` methodSignature
            public abstract CanonicalCellName getCellName()
            ```

        []{#getCellBuckOut()}

        -   #### getCellBuckOut

            ``` methodSignature
            @Derived
            public Path getCellBuckOut()
            ```

            ::: block
            Returns an absolute path to the cell\'s buck-out embedded
            inside the root\'s buck-out
            :::

        []{#of(java.nio.file.Path,com.facebook.buck.io.filesystem.BuckPaths,com.facebook.buck.core.cell.name.CanonicalCellName)}

        -   #### of

            ``` methodSignature
            public static EmbeddedCellBuckOutInfo of​(Path mainCellRoot,
                                                     BuckPaths mainCellBuckPaths,
                                                     CanonicalCellName cellName)
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
