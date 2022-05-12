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
[Package]{.packageLabelInType} [com.facebook.buck.parser.api](package-summary.html)
:::

## Interface FileParser\<T extends [FileManifest](FileManifest.html "interface in com.facebook.buck.parser.api")\> {#interface-fileparsert-extends-filemanifest .title title="Interface FileParser"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AutoCloseable`

    ```{=html}
    <!-- -->
    ```

    All Known Subinterfaces:
    :   `PackageFileParser`, `ProjectBuildFileParser`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `ConcurrentProjectBuildFileParser`,
        `EventReportingProjectBuildFileParser`,
        `ForwardingProjectBuildFileParserDecorator`,
        `HybridProjectBuildFileParser`,
        `PythonDslProjectBuildFileParser`, `SkylarkPackageFileParser`,
        `SkylarkProjectBuildFileParser`,
        `TargetCountVerificationParserDecorator`

    ------------------------------------------------------------------------

        public interface FileParser<T extends FileManifest>
        extends AutoCloseable

    ::: block
    Generic file parser, meant to be extended for more specific parsers.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `close()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getIncludedF         | ::: block             |
        | common.collect.Immuta | iles​(Path parseFile)` | Collects the loaded   |
        | bleSortedSet<String>` |                       | files and extensions  |
        |                       |                       | when parsing the      |
        |                       |                       | `parseFile` build     |
        |                       |                       | spec.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `T`                   | `getMani              | ::: block             |
        |                       | fest​(Path parseFile)` | Collect all           |
        |                       |                       | information from a    |
        |                       |                       | particular, along     |
        |                       |                       | with metadata about   |
        |                       |                       | the information, for  |
        |                       |                       | example which other   |
        |                       |                       | files were also       |
        |                       |                       | parsed.               |
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

        []{#getManifest(java.nio.file.Path)}

        -   #### getManifest

            ``` methodSignature
            T getManifest​(Path parseFile)
                   throws BuildFileParseException,
                          InterruptedException,
                          IOException
            ```

            ::: block
            Collect all information from a particular, along with
            metadata about the information, for example which other
            files were also parsed.
            :::

            [Parameters:]{.paramLabel}
            :   `parseFile` - should be an absolute path to a file. Must
                have rootPath as its prefix.

            [Throws:]{.throwsLabel}
            :   `BuildFileParseException`
            :   `InterruptedException`
            :   `IOException`

        []{#getIncludedFiles(java.nio.file.Path)}

        -   #### getIncludedFiles

            ``` methodSignature
            com.google.common.collect.ImmutableSortedSet<String> getIncludedFiles​(Path parseFile)
                                                                           throws BuildFileParseException,
                                                                                  InterruptedException,
                                                                                  IOException
            ```

            ::: block
            Collects the loaded files and extensions when parsing the
            `parseFile` build spec.
            :::

            [Parameters:]{.paramLabel}
            :   `parseFile` - should be an absolute path to a file. Must
                have rootPath as its prefix.

            [Throws:]{.throwsLabel}
            :   `BuildFileParseException`
            :   `InterruptedException`
            :   `IOException`

        []{#close()}

        -   #### close

            ``` methodSignature
            void close()
                throws BuildFileParseException,
                       InterruptedException,
                       IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

            [Throws:]{.throwsLabel}
            :   `BuildFileParseException`
            :   `InterruptedException`
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
