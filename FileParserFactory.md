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
[Package]{.packageLabelInType} [com.facebook.buck.parser](package-summary.html)
:::

## Interface FileParserFactory\<T extends [FileManifest](api/FileManifest.html "interface in com.facebook.buck.parser.api")\> {#interface-fileparserfactoryt-extends-filemanifest .title title="Interface FileParserFactory"}
:::

::: contentContainer
::: description
-   

    All Known Subinterfaces:
    :   `ProjectBuildFileParserFactory`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `DefaultProjectBuildFileParserFactory`,
        `PackageFileParserFactory`

    ------------------------------------------------------------------------

        public interface FileParserFactory<T extends FileManifest>

    ::: block
    Factory for creating instances of
    [`FileParser`](api/FileParser.html "interface in com.facebook.buck.parser.api").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `FileParser<T>`       | `createFilePa         | ::: block             |
        |                       | rser​(BuckEventBus eve | Creates an instance   |
        |                       | ntBus,                | of {link              |
        |                       |   Cell cell,          | Pr                    |
        |                       |         Watchman watc | ojectBuildFileParser} |
        |                       | hman,                 | based on passed in    |
        |                       |  boolean threadSafe)` | options.              |
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

        []{#createFileParser(com.facebook.buck.event.BuckEventBus,com.facebook.buck.core.cell.Cell,com.facebook.buck.io.watchman.Watchman,boolean)}

        -   #### createFileParser

            ``` methodSignature
            FileParser<T> createFileParser​(BuckEventBus eventBus,
                                           Cell cell,
                                           Watchman watchman,
                                           boolean threadSafe)
            ```

            ::: block
            Creates an instance of {link ProjectBuildFileParser} based
            on passed in options.
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
