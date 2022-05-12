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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.util](package-summary.html)
:::

## Interface DirectoryCleaner.PathSelector {#interface-directorycleaner.pathselector .title title="Interface DirectoryCleaner.PathSelector"}
:::

::: contentContainer
::: description
-   

    Enclosing class:
    :   [DirectoryCleaner](DirectoryCleaner.html "class in com.facebook.buck.util")

    ------------------------------------------------------------------------

        public static interface DirectoryCleaner.PathSelector
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `int`                 | `comparePa            | ::: block             |
        |                       | ths​(DirectoryCleaner. | Returns the preferred |
        |                       | PathStats path1,      | sorting order to      |
        |                       |         DirectoryClea | delete paths.         |
        |                       | ner.PathStats path2)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<Path>`      | `getCandidatesToD     |                       |
        |                       | elete​(Path rootPath)` |                       |
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

        []{#getCandidatesToDelete(java.nio.file.Path)}

        -   #### getCandidatesToDelete

            ``` methodSignature
            Iterable<Path> getCandidatesToDelete​(Path rootPath)
                                          throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#comparePaths(com.facebook.buck.util.DirectoryCleaner.PathStats,com.facebook.buck.util.DirectoryCleaner.PathStats)}

        -   #### comparePaths

            ``` methodSignature
            int comparePaths​(DirectoryCleaner.PathStats path1,
                             DirectoryCleaner.PathStats path2)
            ```

            ::: block
            Returns the preferred sorting order to delete paths.
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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
