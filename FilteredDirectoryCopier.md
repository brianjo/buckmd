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

## Interface FilteredDirectoryCopier {#interface-filtereddirectorycopier .title title="Interface FilteredDirectoryCopier"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `DefaultFilteredDirectoryCopier`

    ------------------------------------------------------------------------

        public interface FilteredDirectoryCopier
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `c                    | ::: block             |
        |                       | opyDir​(ProjectFilesys | Creates a filtered    |
        |                       | tem filesystem,       | copy of a directory.  |
        |                       |   Path srcDir,        | :::                   |
        |                       |  Path destDir,        |                       |
        |                       |  java.util.function.P |                       |
        |                       | redicate<Path> pred)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `copyDirs             | ::: block             |
        |                       | ​(ProjectFilesystem fi | Copies multiple       |
        |                       | lesystem,         Map | directories while     |
        |                       | <Path,​Path> sourcesTo | filtering out         |
        |                       | Destinations,         | individual files      |
        |                       |  java.util.function.P | which fail a          |
        |                       | redicate<Path> pred)` | predicate.            |
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

        []{#copyDirs(com.facebook.buck.io.filesystem.ProjectFilesystem,java.util.Map,java.util.function.Predicate)}

        -   #### copyDirs

            ``` methodSignature
            void copyDirs​(ProjectFilesystem filesystem,
                          Map<Path,​Path> sourcesToDestinations,
                          java.util.function.Predicate<Path> pred)
                   throws IOException
            ```

            ::: block
            Copies multiple directories while filtering out individual
            files which fail a predicate.
            :::

            [Parameters:]{.paramLabel}
            :   `sourcesToDestinations` - mapping from source to
                destination directories
            :   `pred` - predicate to test against

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#copyDir(com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path,java.nio.file.Path,java.util.function.Predicate)}

        -   #### copyDir

            ``` methodSignature
            void copyDir​(ProjectFilesystem filesystem,
                         Path srcDir,
                         Path destDir,
                         java.util.function.Predicate<Path> pred)
                  throws IOException
            ```

            ::: block
            Creates a filtered copy of a directory.
            :::

            [Parameters:]{.paramLabel}
            :   `srcDir` - source directory
            :   `destDir` - destination directory
            :   `pred` - a predicate to determine which files should be
                copied.

            [Throws:]{.throwsLabel}
            :   `IOException`
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
