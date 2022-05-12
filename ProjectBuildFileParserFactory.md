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

## Interface ProjectBuildFileParserFactory {#interface-projectbuildfileparserfactory .title title="Interface ProjectBuildFileParserFactory"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `FileParserFactory<BuildFileManifest>`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `DefaultProjectBuildFileParserFactory`

    ------------------------------------------------------------------------

        public interface ProjectBuildFileParserFactory
        extends FileParserFactory<BuildFileManifest>

    ::: block
    Factory for creating instances of {link ProjectBuildFileParser}.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Pr                   | `createFilePa         | ::: block             |
        | ojectBuildFileParser` | rser​(BuckEventBus eve | Creates an instance   |
        |                       | ntBus,                | of                    |
        |                       |   Cell cell,          | [`ProjectBuildFileP   |
        |                       |         Watchman watc | arser`](api/ProjectBu |
        |                       | hman,                 | ildFileParser.html "i |
        |                       |  boolean threadSafe)` | nterface in com.faceb |
        |                       |                       | ook.buck.parser.api") |
        |                       |                       | based on passed in    |
        |                       |                       | options.              |
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
            ProjectBuildFileParser createFileParser​(BuckEventBus eventBus,
                                                    Cell cell,
                                                    Watchman watchman,
                                                    boolean threadSafe)
            ```

            ::: block
            Creates an instance of
            [`ProjectBuildFileParser`](api/ProjectBuildFileParser.html "interface in com.facebook.buck.parser.api")
            based on passed in options.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `createFileParser` in
                interface `FileParserFactory<BuildFileManifest>`
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
