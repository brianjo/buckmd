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

## Interface BuildCellRelativePathFactory {#interface-buildcellrelativepathfactory .title title="Interface BuildCellRelativePathFactory"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `DefaultBuildCellRelativePathFactory`

    ------------------------------------------------------------------------

        public interface BuildCellRelativePathFactory
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `B                    | `from​(Ou              | ::: block             |
        | uildCellRelativePath` | tputPath outputPath)` | Converts an           |
        |                       |                       | OutputPath to a       |
        |                       |                       | B                     |
        |                       |                       | uildCellRelativePath. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `B                    | `from​(Path bu         | ::: block             |
        | uildCellRelativePath` | ildableRelativePath)` | Converts a Path       |
        |                       |                       | relative to the       |
        |                       |                       | Buildable\'s          |
        |                       |                       | ProjectFilesystem to  |
        |                       |                       | a                     |
        |                       |                       | B                     |
        |                       |                       | uildCellRelativePath. |
        |                       |                       | :::                   |
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

        []{#from(java.nio.file.Path)}

        -   #### from

            ``` methodSignature
            BuildCellRelativePath from​(Path buildableRelativePath)
            ```

            ::: block
            Converts a Path relative to the Buildable\'s
            ProjectFilesystem to a BuildCellRelativePath.
            :::

        []{#from(com.facebook.buck.rules.modern.OutputPath)}

        -   #### from

            ``` methodSignature
            BuildCellRelativePath from​(OutputPath outputPath)
            ```

            ::: block
            Converts an OutputPath to a BuildCellRelativePath.
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
