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

## Interface CxxBinaryDescription.CommonArg {#interface-cxxbinarydescription.commonarg .title title="Interface CxxBinaryDescription.CommonArg"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `BuildRuleArg`, `ConstructorArg`, `CxxConstructorArg`,
        `DataTransferObject`, `HasDeclaredDeps`, `HasDefaultFlavors`,
        `HasDefaultPlatform`, `HasDepsQuery`,
        `HasSystemFrameworkAndLibraries`, `HasTests`,
        `HasVersionUniverse`, `LinkableCxxConstructorArg`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `CgoLibraryDescriptionArg`, `CxxBinaryDescriptionArg`,
        `CxxTestDescriptionArg`, `HalideLibraryDescriptionArg`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [CxxBinaryDescription](CxxBinaryDescription.html "class in com.facebook.buck.cxx")

    ------------------------------------------------------------------------

        public static interface CxxBinaryDescription.CommonArg
        extends LinkableCxxConstructorArg, HasVersionUniverse, HasDepsQuery
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

          Modifier and Type   Method                      Description
          ------------------- --------------------------- -------------
          `default boolean`   `getLinkDepsQueryWhole()`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
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
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.HasDepsQuery}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[HasDepsQuery](../core/description/arg/HasDepsQuery.html "interface in com.facebook.buck.core.description.arg")

            `getDepsQuery, withDepsQuery`

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

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.versions.HasVersionUniverse}

            ### Methods inherited from interface com.facebook.buck.versions.[HasVersionUniverse](../versions/HasVersionUniverse.html "interface in com.facebook.buck.versions")

            `getVersionUniverse`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.LinkableCxxConstructorArg}

            ### Methods inherited from interface com.facebook.buck.cxx.[LinkableCxxConstructorArg](LinkableCxxConstructorArg.html "interface in com.facebook.buck.cxx")

            `getFatLto, getLinkGroup, getLinkGroupMap, getLinkStyle, getThinLto`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getLinkDepsQueryWhole()}

        -   #### getLinkDepsQueryWhole

            ``` methodSignature
            @Default
            default boolean getLinkDepsQueryWhole()
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
