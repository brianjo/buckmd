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
-   [Field](#field.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.cxx](package-summary.html)
:::

## Interface LinkableCxxConstructorArg {#interface-linkablecxxconstructorarg .title title="Interface LinkableCxxConstructorArg"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `BuildRuleArg`, `ConstructorArg`, `CxxConstructorArg`,
        `DataTransferObject`, `HasDeclaredDeps`, `HasDefaultFlavors`,
        `HasDefaultPlatform`, `HasSystemFrameworkAndLibraries`,
        `HasTests`

    ```{=html}
    <!-- -->
    ```

    All Known Subinterfaces:
    :   `AppleNativeTargetDescriptionArg`,
        `CxxBinaryDescription.CommonArg`,
        `CxxLibraryDescription.CommonArg`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AppleBinaryDescriptionArg`, `AppleLibraryDescriptionArg`,
        `AppleTestDescriptionArg`, `CgoLibraryDescriptionArg`,
        `CxxBinaryDescriptionArg`, `CxxLibraryDescriptionArg`,
        `CxxTestDescriptionArg`, `HalideLibraryDescriptionArg`

    ------------------------------------------------------------------------

        public interface LinkableCxxConstructorArg
        extends CxxConstructorArg
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.core.description.arg.BuildRuleArg}

            ### Fields inherited from interface com.facebook.buck.core.description.arg.[BuildRuleArg](../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")

            `DEFAULT_TARGET_PLATFORM_PARAM_NAME`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `default boolean`     | `getFatLto()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getLinkGroup()`      | ::: block             |
        |                       |                       | Defines the link      |
        |                       |                       | group.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional             | `getLinkGroupMap()`   | ::: block             |
        | <com.google.common.co |                       | Defines the list of   |
        | llect.ImmutableList<C |                       | link group mappings.  |
        | xxLinkGroupMapping>>` |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Lin         | `getLinkStyle()`      |                       |
        | ker.LinkableDepType>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `getThinLto()`        |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.BuildRuleArg}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[BuildRuleArg](../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")

            `getCompatibleWith, getDefaultTargetPlatform, getLabels, getLicenses, labelsContainsAnyOf`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.ConstructorArg}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[ConstructorArg](../core/description/arg/ConstructorArg.html "interface in com.facebook.buck.core.description.arg")

            `getName`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.CxxConstructorArg}

            ### Methods inherited from interface com.facebook.buck.cxx.[CxxConstructorArg](CxxConstructorArg.html "interface in com.facebook.buck.cxx")

            `checkDuplicateSources, checkHeadersUsage, getCompilerFlags, getCxxDeps, getCxxRuntimeType, getDefaultFlavors, getDefaults, getExecutableName, getHeaderNamespace, getHeaders, getIncludeDirectories, getLangCompilerFlags, getLangPlatformCompilerFlags, getLangPlatformPreprocessorFlags, getLangPreprocessorFlags, getLinkerExtraOutputs, getLinkerFlags, getPlatformCompilerFlags, getPlatformDeps, getPlatformHeaders, getPlatformLinkerFlags, getPlatformPreprocessorFlags, getPlatformSrcs, getPostLinkerFlags, getPostPlatformLinkerFlags, getPrecompiledHeader, getPrefixHeader, getPreprocessorFlags, getPrivateCxxDeps, getRawHeaders, getSrcs`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.HasDeclaredDeps}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[HasDeclaredDeps](../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg")

            `getDeps`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.HasDefaultPlatform}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[HasDefaultPlatform](../core/description/arg/HasDefaultPlatform.html "interface in com.facebook.buck.core.description.arg")

            `getDefaultPlatform`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.toolchain.HasSystemFrameworkAndLibraries}

            ### Methods inherited from interface com.facebook.buck.cxx.toolchain.[HasSystemFrameworkAndLibraries](toolchain/HasSystemFrameworkAndLibraries.html "interface in com.facebook.buck.cxx.toolchain")

            `getFrameworks, getLibraries`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.HasTests}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[HasTests](../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg")

            `getTests`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getLinkStyle()}

        -   #### getLinkStyle

            ``` methodSignature
            Optional<Linker.LinkableDepType> getLinkStyle()
            ```

        []{#getLinkGroupMap()}

        -   #### getLinkGroupMap

            ``` methodSignature
            Optional<com.google.common.collect.ImmutableList<CxxLinkGroupMapping>> getLinkGroupMap()
            ```

            ::: block
            Defines the list of link group mappings. Targets\'
            membership in a group is defined by the order of the list,
            so if more than one mapping matches a single target, the
            group would be the one defined by the first match.
            :::

        []{#getLinkGroup()}

        -   #### getLinkGroup

            ``` methodSignature
            Optional<String> getLinkGroup()
            ```

            ::: block
            Defines the link group. When linking executable code, only
            static libraries which belong to the same group would be
            linked into the executable.
            :::

        []{#getThinLto()}

        -   #### getThinLto

            ``` methodSignature
            @Default
            default boolean getThinLto()
            ```

        []{#getFatLto()}

        -   #### getFatLto

            ``` methodSignature
            @Default
            default boolean getFatLto()
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
-   [Field](#field.summary) \| 
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
