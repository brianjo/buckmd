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
[Package]{.packageLabelInType} [com.facebook.buck.rules.modern](package-summary.html)
:::

## Interface OutputPathResolver {#interface-outputpathresolver .title title="Interface OutputPathResolver"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `DefaultOutputPathResolver`

    ------------------------------------------------------------------------

        public interface OutputPathResolver

    ::: block
    Provides Buildable\'s a way to construct Paths to outputs.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Path`                | `getRootPath()`       | ::: block             |
        |                       |                       | Returns a relative    |
        |                       |                       | path to the root      |
        |                       |                       | directory for build   |
        |                       |                       | outputs.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getTempPath()`       | ::: block             |
        |                       |                       | Returns a relative    |
        |                       |                       | path to the root      |
        |                       |                       | directory for         |
        |                       |                       | intermediate build    |
        |                       |                       | outputs.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default Path`        | `getT                 |                       |
        |                       | empPath​(String file)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `resolvePath​(Ou       | ::: block             |
        |                       | tputPath outputPath)` | Returns a relative    |
        |                       |                       | path to the output.   |
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

        []{#getTempPath()}

        -   #### getTempPath

            ``` methodSignature
            Path getTempPath()
            ```

            ::: block
            Returns a relative path to the root directory for
            intermediate build outputs.
            :::

        []{#getTempPath(java.lang.String)}

        -   #### getTempPath

            ``` methodSignature
            default Path getTempPath​(String file)
            ```

        []{#resolvePath(com.facebook.buck.rules.modern.OutputPath)}

        -   #### resolvePath

            ``` methodSignature
            Path resolvePath​(OutputPath outputPath)
            ```

            ::: block
            Returns a relative path to the output.
            :::

        []{#getRootPath()}

        -   #### getRootPath

            ``` methodSignature
            Path getRootPath()
            ```

            ::: block
            Returns a relative path to the root directory for build
            outputs.
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
