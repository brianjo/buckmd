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
[Package]{.packageLabelInType} [com.facebook.buck.core.description.arg](package-summary.html)
:::

## Interface ConstructorArg {#interface-constructorarg .title title="Interface ConstructorArg"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `DataTransferObject`

    ```{=html}
    <!-- -->
    ```

    All Known Subinterfaces:
    :   `AbstractGenruleDescription.CommonArg`, `AndroidKotlinCoreArg`,
        `AndroidLibraryDescription.CoreArg`,
        `AppleNativeTargetDescriptionArg`, `BuildRuleArg`,
        `ConfigurationRuleArg`, `CxxBinaryDescription.CommonArg`,
        `CxxConstructorArg`, `CxxLibraryDescription.CommonArg`,
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
        `AndroidPlatformArg`, `AndroidPrebuiltAarDescriptionArg`,
        `AndroidResourceDescriptionArg`, `ApkGenruleDescriptionArg`,
        `AppleAssetCatalogDescriptionArg`, `AppleBinaryDescriptionArg`,
        `AppleBundleDescriptionArg`, `AppleLibraryDescriptionArg`,
        `ApplePackageDescriptionArg`, `AppleResourceDescriptionArg`,
        `AppleTestDescriptionArg`, `AppleToolchainDescriptionArg`,
        `AppleToolchainSetDescriptionArg`, `AppleWrapperResourceArg`,
        `CgoLibraryDescriptionArg`, `CommandAliasDescriptionArg`,
        `ConfigSettingArg`, `ConstraintSettingArg`,
        `ConstraintValueArg`, `CsharpLibraryDescriptionArg`,
        `CxxBinaryDescriptionArg`, `CxxGenruleDescriptionArg`,
        `CxxLibraryDescriptionArg`, `CxxLuaExtensionDescriptionArg`,
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
        `PlatformArg`, `PrebuiltAppleFrameworkDescriptionArg`,
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

        public interface ConstructorArg
        extends DataTransferObject

    ::: block
    Marker interface for all rule args including configuration rules.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `String`              | `getName()`           | ::: block             |
        |                       |                       | Each rule has a name  |
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

        []{#getName()}

        -   #### getName

            ``` methodSignature
            String getName()
            ```

            ::: block
            Each rule has a name
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
