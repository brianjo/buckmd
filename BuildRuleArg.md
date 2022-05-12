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
-   Nested \| 
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.description.arg](package-summary.html)
:::

## Interface BuildRuleArg {#interface-buildrulearg .title title="Interface BuildRuleArg"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `ConstructorArg`, `DataTransferObject`

    ```{=html}
    <!-- -->
    ```

    All Known Subinterfaces:
    :   `AbstractGenruleDescription.CommonArg`, `AndroidKotlinCoreArg`,
        `AndroidLibraryDescription.CoreArg`,
        `AppleNativeTargetDescriptionArg`,
        `CxxBinaryDescription.CommonArg`, `CxxConstructorArg`,
        `CxxLibraryDescription.CommonArg`,
        `GroovyLibraryDescription.CoreArg`,
        `HasSystemFrameworkAndLibraries`, `JavacPluginArgs`,
        `JavaLibraryDescription.CoreArg`, `JavaTestDescription.CoreArg`,
        `JvmLibraryArg`, `KotlinLibraryDescription.CoreArg`,
        `LinkableCxxConstructorArg`, `RustCommonArgs`,
        `ScalaLibraryDescription.CoreArg`, `SwiftCommonArg`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AndroidAarDescriptionArg`,
        `AndroidAppModularityDescriptionArg`,
        `AndroidBinaryDescriptionArg`,
        `AndroidBuildConfigDescriptionArg`,
        `AndroidBundleDescriptionArg`,
        `AndroidInstrumentationApkDescriptionArg`,
        `AndroidInstrumentationTestDescriptionArg`,
        `AndroidLibraryDescriptionArg`, `AndroidManifestDescriptionArg`,
        `AndroidPrebuiltAarDescriptionArg`,
        `AndroidResourceDescriptionArg`, `ApkGenruleDescriptionArg`,
        `AppleAssetCatalogDescriptionArg`, `AppleBinaryDescriptionArg`,
        `AppleBundleDescriptionArg`, `AppleLibraryDescriptionArg`,
        `ApplePackageDescriptionArg`, `AppleResourceDescriptionArg`,
        `AppleTestDescriptionArg`, `AppleToolchainDescriptionArg`,
        `AppleToolchainSetDescriptionArg`, `AppleWrapperResourceArg`,
        `CgoLibraryDescriptionArg`, `CommandAliasDescriptionArg`,
        `CsharpLibraryDescriptionArg`, `CxxBinaryDescriptionArg`,
        `CxxGenruleDescriptionArg`, `CxxLibraryDescriptionArg`,
        `CxxLuaExtensionDescriptionArg`,
        `CxxPrecompiledHeaderDescriptionArg`,
        `CxxPythonExtensionDescriptionArg`, `CxxTestDescriptionArg`,
        `CxxToolchainDescriptionArg`, `DBinaryDescriptionArg`,
        `DLibraryDescriptionArg`, `DTestDescriptionArg`,
        `ExportFileDescriptionArg`, `ExternalTestRunnerDescriptionArg`,
        `FileGroupDescriptionArg`, `GenAidlDescriptionArg`,
        `GenruleDescriptionArg`, `GoBinaryDescriptionArg`,
        `GoLibraryDescriptionArg`, `GoTestDescriptionArg`,
        `GoTestRunnerDescriptionArg`, `GroovyLibraryDescriptionArg`,
        `GroovyTestDescriptionArg`, `GwtBinaryDescriptionArg`,
        `HalideLibraryDescriptionArg`, `HaskellBinaryDescriptionArg`,
        `HaskellGhciDescriptionArg`, `HaskellHaddockDescriptionArg`,
        `HaskellLibraryDescriptionArg`,
        `HaskellPrebuiltLibraryDescriptionArg`,
        `HttpArchiveDescriptionArg`, `HttpFileDescriptionArg`,
        `JarGenruleDescriptionArg`,
        `JavaAnnotationProcessorDescriptionArg`,
        `JavaBinaryDescriptionArg`, `JavaLibraryDescriptionArg`,
        `JavaPluginDescriptionArg`, `JavaTestDescriptionArg`,
        `JavaTestRunnerDescriptionArg`, `JsBundleDescriptionArg`,
        `JsBundleGenruleDescriptionArg`, `JsLibraryDescriptionArg`,
        `KeystoreDescriptionArg`, `KotlinLibraryDescriptionArg`,
        `KotlinTestDescriptionArg`, `LegacyToolchainDescriptionArg`,
        `LuaBinaryDescriptionArg`, `LuaLibraryDescriptionArg`,
        `NdkLibraryDescriptionArg`, `NdkToolchainDescriptionArg`,
        `OcamlBinaryDescriptionArg`, `OcamlLibraryDescriptionArg`,
        `PrebuiltAppleFrameworkDescriptionArg`,
        `PrebuiltCxxLibraryDescriptionArg`,
        `PrebuiltCxxLibraryGroupDescriptionArg`,
        `PrebuiltDotnetLibraryDescriptionArg`,
        `PrebuiltGoLibraryDescriptionArg`, `PrebuiltJarDescriptionArg`,
        `PrebuiltNativeLibraryDescriptionArg`,
        `PrebuiltOcamlLibraryDescriptionArg`,
        `PrebuiltPythonLibraryDescriptionArg`,
        `PrebuiltRustLibraryDescriptionArg`,
        `PythonBinaryDescriptionArg`, `PythonLibraryDescriptionArg`,
        `PythonTestDescriptionArg`, `PythonTestRunnerDescriptionArg`,
        `RemoteFileDescriptionArg`, `RobolectricTestDescriptionArg`,
        `RustBinaryDescriptionArg`, `RustLibraryDescriptionArg`,
        `RustTestDescriptionArg`, `ScalaLibraryDescriptionArg`,
        `ScalaTestDescriptionArg`, `ShBinaryDescriptionArg`,
        `ShTestDescriptionArg`, `SkylarkDescriptionArg`,
        `SwiftLibraryDescriptionArg`, `SwiftToolchainDescriptionArg`,
        `TestSuiteDescriptionArg`, `VersionedAliasDescriptionArg`,
        `WorkerToolDescriptionArg`, `XcodeScriptDescriptionArg`,
        `XcodeWorkspaceConfigDescriptionArg`, `ZipFileDescriptionArg`

    ------------------------------------------------------------------------

        public interface BuildRuleArg
        extends ConstructorArg

    ::: block
    Common arguments for build rules (but not configuration rules)
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                                  Description
          ------------------- -------------------------------------- -------------
          `static String`     `DEFAULT_TARGET_PLATFORM_PARAM_NAME`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `co                   | `getCompatibleWith()` | ::: block             |
        | m.google.common.colle |                       | A list of             |
        | ct.ImmutableList<Unco |                       | `config_setting` a    |
        | nfiguredBuildTarget>` |                       | target is compatible  |
        |                       |                       | with.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Unco        | `getDef               | ::: block             |
        | nfiguredBuildTarget>` | aultTargetPlatform()` | The name of build     |
        |                       |                       | target default        |
        |                       |                       | \"new\" platform: it  |
        |                       |                       | is used when a        |
        |                       |                       | platform is not       |
        |                       |                       | specified either      |
        |                       |                       | globally or in a      |
        |                       |                       | target which used     |
        |                       |                       | this target as a      |
        |                       |                       | dependency.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getLabels()`         |                       |
        | common.collect.Immuta |                       |                       |
        | bleSortedSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getLicenses()`       |                       |
        | e.common.collect.Immu |                       |                       |
        | tableSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `labelsContainsAnyOf  |                       |
        |                       | ​(Set<String> labels)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.ConstructorArg}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[ConstructorArg](ConstructorArg.html "interface in com.facebook.buck.core.description.arg")

            `getName`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#DEFAULT_TARGET_PLATFORM_PARAM_NAME}

        -   #### DEFAULT_TARGET_PLATFORM_PARAM_NAME

                static final String DEFAULT_TARGET_PLATFORM_PARAM_NAME

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.core.description.arg.BuildRuleArg.DEFAULT_TARGET_PLATFORM_PARAM_NAME)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getLicenses()}

        -   #### getLicenses

            ``` methodSignature
            com.google.common.collect.ImmutableSet<SourcePath> getLicenses()
            ```

        []{#getLabels()}

        -   #### getLabels

            ``` methodSignature
            @NaturalOrder
            com.google.common.collect.ImmutableSortedSet<String> getLabels()
            ```

        []{#getDefaultTargetPlatform()}

        -   #### getDefaultTargetPlatform

            ``` methodSignature
            Optional<UnconfiguredBuildTarget> getDefaultTargetPlatform()
            ```

            ::: block
            The name of build target default \"new\" platform: it is
            used when a platform is not specified either globally or in
            a target which used this target as a dependency.
            The value is a build target, but we specify it as string,
            because this function is not actually called, but the attr
            is fetched by name from the raw (unconfigured) target node.
            :::

        []{#getCompatibleWith()}

        -   #### getCompatibleWith

            ``` methodSignature
            com.google.common.collect.ImmutableList<UnconfiguredBuildTarget> getCompatibleWith()
            ```

            ::: block
            A list of `config_setting` a target is compatible with.
            :::

        []{#labelsContainsAnyOf(java.util.Set)}

        -   #### labelsContainsAnyOf

            ``` methodSignature
            @Derived
            default boolean labelsContainsAnyOf​(Set<String> labels)
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
-   Nested \| 
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
