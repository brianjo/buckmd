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
[Package]{.packageLabelInType} [com.facebook.buck.core.cell.impl](package-summary.html)
:::

## Class CellMappingsFactory {#class-cellmappingsfactory .title title="Class CellMappingsFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.cell.impl.CellMappingsFactory

::: description
-   

    ------------------------------------------------------------------------

        public class CellMappingsFactory
        extends Object

    ::: block
    Utilities for creating
    [`NewCellPathResolver`](../NewCellPathResolver.html "interface in com.facebook.buck.core.cell")
    and
    [`CellNameResolver`](../nameresolver/CellNameResolver.html "interface in com.facebook.buck.core.cell.nameresolver").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static               | `create​(A             | ::: block             |
        |  NewCellPathResolver` | bsPath rootPath,      | Creates a             |
        |                       |   Config rootConfig)` | [`NewCellPa           |
        |                       |                       | thResolver`](../NewCe |
        |                       |                       | llPathResolver.html " |
        |                       |                       | interface in com.face |
        |                       |                       | book.buck.core.cell") |
        |                       |                       | from the root cell\'s |
        |                       |                       | path and config.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `createCellNa         | ::: block             |
        | tic CellNameResolver` | meResolver​(AbsPath ce | Creates a             |
        |                       | llPath,               | [`CellName            |
        |                       |          Config confi | Resolver`](../nameres |
        |                       | g,                    | olver/CellNameResolve |
        |                       |     NewCellPathResolv | r.html "interface in  |
        |                       | er cellPathResolver)` | com.facebook.buck.cor |
        |                       |                       | e.cell.nameresolver") |
        |                       |                       | for a cell.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#create(com.facebook.buck.core.filesystems.AbsPath,com.facebook.buck.util.config.Config)}

        -   #### create

            ``` methodSignature
            public static NewCellPathResolver create​(AbsPath rootPath,
                                                     Config rootConfig)
            ```

            ::: block
            Creates a
            [`NewCellPathResolver`](../NewCellPathResolver.html "interface in com.facebook.buck.core.cell")
            from the root cell\'s path and config. We currently require
            that all cells appear in the root cell\'s config.
            :::

        []{#createCellNameResolver(com.facebook.buck.core.filesystems.AbsPath,com.facebook.buck.util.config.Config,com.facebook.buck.core.cell.NewCellPathResolver)}

        -   #### createCellNameResolver

            ``` methodSignature
            public static CellNameResolver createCellNameResolver​(AbsPath cellPath,
                                                                  Config config,
                                                                  NewCellPathResolver cellPathResolver)
            ```

            ::: block
            Creates a
            [`CellNameResolver`](../nameresolver/CellNameResolver.html "interface in com.facebook.buck.core.cell.nameresolver")
            for a cell.
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
