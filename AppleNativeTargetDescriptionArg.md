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
[Package]{.packageLabelInType} [com.facebook.buck.apple](package-summary.html)
:::

## Interface AppleNativeTargetDescriptionArg {#interface-applenativetargetdescriptionarg .title title="Interface AppleNativeTargetDescriptionArg"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `BuildRuleArg`, `ConstructorArg`, `CxxConstructorArg`,
        `CxxLibraryDescription.CommonArg`, `DataTransferObject`,
        `HasDeclaredDeps`, `HasDefaultFlavors`, `HasDefaultPlatform`,
        `HasSystemFrameworkAndLibraries`, `HasTests`,
        `LinkableCxxConstructorArg`, `SwiftCommonArg`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AppleBinaryDescriptionArg`, `AppleLibraryDescriptionArg`,
        `AppleTestDescriptionArg`

    ------------------------------------------------------------------------

        public interface AppleNativeTargetDescriptionArg
        extends CxxLibraryDescription.CommonArg, SwiftCommonArg

    ::: block
    Arguments common to Apple targets.
    :::
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
        | `default void`        | `checkModularUsage()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `co                   | `getConfigs()`        |                       |
        | m.google.common.colle |                       |                       |
        | ct.ImmutableSortedMap |                       |                       |
        | <String,​com.google.co |                       |                       |
        | mmon.collect.Immutabl |                       |                       |
        | eMap<String,​String>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `g                    |                       |
        |                       | etHeaderPathPrefix()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Opt                  | `getModulemapMode()`  | ::: block             |
        | ional<ModuleMapMode>` |                       | A modulemap mode, to  |
        |                       |                       | override the one      |
        |                       |                       | specified in          |
        |                       |                       | .buckconfig.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `g                    | ::: block             |
        |                       | etTargetSdkVersion()` | The minimum OS        |
        |                       |                       | version for which     |
        |                       |                       | this target should be |
        |                       |                       | built.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `isModular()`         |                       |
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

            ### Methods inherited from interface com.facebook.buck.cxx.[CxxConstructorArg](../cxx/CxxConstructorArg.html "interface in com.facebook.buck.cxx")

            `checkDuplicateSources, getCompilerFlags, getCxxRuntimeType, getDefaultFlavors, getDefaults, getExecutableName, getHeaderNamespace, getHeaders, getIncludeDirectories, getLangCompilerFlags, getLangPlatformCompilerFlags, getLangPlatformPreprocessorFlags, getLangPreprocessorFlags, getLinkerExtraOutputs, getLinkerFlags, getPlatformCompilerFlags, getPlatformDeps, getPlatformHeaders, getPlatformLinkerFlags, getPlatformPreprocessorFlags, getPlatformSrcs, getPostLinkerFlags, getPostPlatformLinkerFlags, getPrecompiledHeader, getPrefixHeader, getPreprocessorFlags, getPrivateCxxDeps, getRawHeaders, getSrcs`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.CxxLibraryDescription.CommonArg}

            ### Methods inherited from interface com.facebook.buck.cxx.[CxxLibraryDescription.CommonArg](../cxx/CxxLibraryDescription.CommonArg.html "interface in com.facebook.buck.cxx")

            `checkHeadersUsage, getBridgingHeader, getCanBeAsset, getCxxDeps, getExportedCxxDeps, getExportedDeps, getExportedHeaders, getExportedHeaderStyle, getExportedLangPlatformPreprocessorFlags, getExportedLangPreprocessorFlags, getExportedLinkerFlags, getExportedPlatformDeps, getExportedPlatformHeaders, getExportedPlatformLinkerFlags, getExportedPlatformPreprocessorFlags, getExportedPostLinkerFlags, getExportedPostPlatformLinkerFlags, getExportedPreprocessorFlags, getExtraXcodeFiles, getExtraXcodeSources, getForceStatic, getLinkWhole, getModuleName, getPreferredLinkage, getPublicIncludeDirectories, getPublicSystemIncludeDirectories, getSoname, getStaticLibraryBasename, getSupportedPlatformsRegex, getSupportsMergedLinking, getXcodePrivateHeadersSymlinks, getXcodePublicHeadersSymlinks, isReexportAllHeaderDependencies`

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

            ### Methods inherited from interface com.facebook.buck.cxx.toolchain.[HasSystemFrameworkAndLibraries](../cxx/toolchain/HasSystemFrameworkAndLibraries.html "interface in com.facebook.buck.cxx.toolchain")

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
        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.LinkableCxxConstructorArg}

            ### Methods inherited from interface com.facebook.buck.cxx.[LinkableCxxConstructorArg](../cxx/LinkableCxxConstructorArg.html "interface in com.facebook.buck.cxx")

            `getFatLto, getLinkGroup, getLinkGroupMap, getLinkStyle, getThinLto`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.swift.SwiftCommonArg}

            ### Methods inherited from interface com.facebook.buck.swift.[SwiftCommonArg](../swift/SwiftCommonArg.html "interface in com.facebook.buck.swift")

            `getSwiftCompilerFlags, getSwiftVersion`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getConfigs()}

        -   #### getConfigs

            ``` methodSignature
            @NaturalOrder
            com.google.common.collect.ImmutableSortedMap<String,​com.google.common.collect.ImmutableMap<String,​String>> getConfigs()
            ```

        []{#getHeaderPathPrefix()}

        -   #### getHeaderPathPrefix

            ``` methodSignature
            Optional<String> getHeaderPathPrefix()
            ```

        []{#isModular()}

        -   #### isModular

            ``` methodSignature
            @Default
            default boolean isModular()
            ```

        []{#getModulemapMode()}

        -   #### getModulemapMode

            ``` methodSignature
            Optional<ModuleMapMode> getModulemapMode()
            ```

            ::: block
            A modulemap mode, to override the one specified in
            .buckconfig.
            :::

        []{#checkModularUsage()}

        -   #### checkModularUsage

            ``` methodSignature
            @Check
            default void checkModularUsage()
            ```

        []{#getTargetSdkVersion()}

        -   #### getTargetSdkVersion

            ``` methodSignature
            Optional<String> getTargetSdkVersion()
            ```

            ::: block
            The minimum OS version for which this target should be
            built. If set, this will override the config-level option.
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
