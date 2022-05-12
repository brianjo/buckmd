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

## Interface ProjectBuildFileParser {#interface-projectbuildfileparser .title title="Interface ProjectBuildFileParser"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AutoCloseable`, `FileParser<BuildFileManifest>`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `ConcurrentProjectBuildFileParser`,
        `EventReportingProjectBuildFileParser`,
        `ForwardingProjectBuildFileParserDecorator`,
        `HybridProjectBuildFileParser`,
        `PythonDslProjectBuildFileParser`,
        `SkylarkProjectBuildFileParser`,
        `TargetCountVerificationParserDecorator`

    ------------------------------------------------------------------------

        public interface ProjectBuildFileParser
        extends FileParser<BuildFileManifest>

    ::: block
    Parses buck build files (usually BUCK files) and retrieve rule
    information from them.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `globResultsM         | ::: block             |
        |                       | atchCurrentState​(Path | Checks if existing    |
        |                       |  buildFile,           | `GlobSpec`s with      |
        |                       |                    co | results are the same  |
        |                       | m.google.common.colle | as current state in   |
        |                       | ct.ImmutableList<Glob | the file system.      |
        |                       | SpecWithResult> exist | :::                   |
        |                       | ingGlobsWithResults)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `reportProfile()`     | ::: block             |
        |                       |                       | Reports profile       |
        |                       |                       | information captured  |
        |                       |                       | while parsing build   |
        |                       |                       | files.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.parser.api.FileParser}

            ### Methods inherited from interface com.facebook.buck.parser.api.[FileParser](FileParser.html "interface in com.facebook.buck.parser.api")

            `close, getIncludedFiles, getManifest`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#reportProfile()}

        -   #### reportProfile

            ``` methodSignature
            void reportProfile()
                        throws IOException
            ```

            ::: block
            Reports profile information captured while parsing build
            files.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#globResultsMatchCurrentState(java.nio.file.Path,com.google.common.collect.ImmutableList)}

        -   #### globResultsMatchCurrentState

            ``` methodSignature
            boolean globResultsMatchCurrentState​(Path buildFile,
                                                 com.google.common.collect.ImmutableList<GlobSpecWithResult> existingGlobsWithResults)
                                          throws IOException,
                                                 InterruptedException
            ```

            ::: block
            Checks if existing `GlobSpec`s with results are the same as
            current state in the file system.
            :::

            [Parameters:]{.paramLabel}
            :   `existingGlobsWithResults` - the existing (deserialized)
                `GlobSpecWithResult` to check the file system state
                against.
            :   `buildFile` - the buildFile location to be used by the
                Globber.

            [Returns:]{.returnLabel}
            :   `true` if glob expansion produces results matching
                previously recorded ones, `false` otherwise.

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `InterruptedException`
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
