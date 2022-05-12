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
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.features.apple.projectV2](package-summary.html)
:::

## Interface ProjectGeneratorOptions {#interface-projectgeneratoroptions .title title="Interface ProjectGeneratorOptions"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface ProjectGeneratorOptions

    ::: block
    Options for how
    [`ProjectGenerator`](ProjectGenerator.html "class in com.facebook.buck.features.apple.projectV2")
    generates Xcode projects.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Interface                           Description
          ------------------- ----------------------------------- -------------
          `static class `     `ProjectGeneratorOptions.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static ProjectGene   | `builder()`           |                       |
        | ratorOptions.Builder` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `shouldAddLink        | ::: block             |
        |                       | edLibrariesAsFlags()` | Add linker flags to   |
        |                       |                       | OTHER_LDFLAGS for     |
        |                       |                       | libraries rather than |
        |                       |                       | to the library build  |
        |                       |                       | phase                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `shouldForceLoad      | ::: block             |
        |                       | LinkWholeLibraries()` | Add linker flags to   |
        |                       |                       | OTHER_LDFLAGS to      |
        |                       |                       | force load of         |
        |                       |                       | libraries with        |
        |                       |                       | link_whole = true     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `shouldGenerateMis    | ::: block             |
        |                       | singUmbrellaHeader()` | Generate an umbrella  |
        |                       |                       | header for modular    |
        |                       |                       | targets without one   |
        |                       |                       | for use in a          |
        |                       |                       | modulemap             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `shouldGene           | ::: block             |
        |                       | rateProjectSchemes()` | Create schemes for    |
        |                       |                       | each project\'s       |
        |                       |                       | contained build and   |
        |                       |                       | test targets.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `shouldGen            | ::: block             |
        |                       | erateReadOnlyFiles()` | Generate read-only    |
        |                       |                       | project files         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `shouldInclud         | ::: block             |
        |                       | eDependenciesTests()` | Include dependencies  |
        |                       |                       | tests in the scheme   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `                     | ::: block             |
        |                       | shouldIncludeTests()` | Include tests that    |
        |                       |                       | test root targets in  |
        |                       |                       | the scheme            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `sho                  | ::: block             |
        |                       | uldLinkSystemSwift()` | Add system swift      |
        |                       |                       | library linker flags  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `shouldUseSh          | ::: block             |
        |                       | ortNamesForTargets()` | Use short BuildTarget |
        |                       |                       | name instead of full  |
        |                       |                       | name for targets      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#shouldUseShortNamesForTargets()}

        -   #### shouldUseShortNamesForTargets

            ``` methodSignature
            @Default
            default boolean shouldUseShortNamesForTargets()
            ```

            ::: block
            Use short BuildTarget name instead of full name for targets
            :::

        []{#shouldGenerateProjectSchemes()}

        -   #### shouldGenerateProjectSchemes

            ``` methodSignature
            @Default
            default boolean shouldGenerateProjectSchemes()
            ```

            ::: block
            Create schemes for each project\'s contained build and test
            targets.
            :::

        []{#shouldGenerateReadOnlyFiles()}

        -   #### shouldGenerateReadOnlyFiles

            ``` methodSignature
            @Default
            default boolean shouldGenerateReadOnlyFiles()
            ```

            ::: block
            Generate read-only project files
            :::

        []{#shouldIncludeTests()}

        -   #### shouldIncludeTests

            ``` methodSignature
            @Default
            default boolean shouldIncludeTests()
            ```

            ::: block
            Include tests that test root targets in the scheme
            :::

        []{#shouldIncludeDependenciesTests()}

        -   #### shouldIncludeDependenciesTests

            ``` methodSignature
            @Default
            default boolean shouldIncludeDependenciesTests()
            ```

            ::: block
            Include dependencies tests in the scheme
            :::

        []{#shouldGenerateMissingUmbrellaHeader()}

        -   #### shouldGenerateMissingUmbrellaHeader

            ``` methodSignature
            @Default
            default boolean shouldGenerateMissingUmbrellaHeader()
            ```

            ::: block
            Generate an umbrella header for modular targets without one
            for use in a modulemap
            :::

        []{#shouldForceLoadLinkWholeLibraries()}

        -   #### shouldForceLoadLinkWholeLibraries

            ``` methodSignature
            @Default
            default boolean shouldForceLoadLinkWholeLibraries()
            ```

            ::: block
            Add linker flags to OTHER_LDFLAGS to force load of libraries
            with link_whole = true
            :::

        []{#shouldAddLinkedLibrariesAsFlags()}

        -   #### shouldAddLinkedLibrariesAsFlags

            ``` methodSignature
            @Default
            default boolean shouldAddLinkedLibrariesAsFlags()
            ```

            ::: block
            Add linker flags to OTHER_LDFLAGS for libraries rather than
            to the library build phase
            :::

        []{#shouldLinkSystemSwift()}

        -   #### shouldLinkSystemSwift

            ``` methodSignature
            @Default
            default boolean shouldLinkSystemSwift()
            ```

            ::: block
            Add system swift library linker flags
            :::

        []{#builder()}

        -   #### builder

            ``` methodSignature
            static ProjectGeneratorOptions.Builder builder()
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
-   [Nested](#nested.class.summary) \| 
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
