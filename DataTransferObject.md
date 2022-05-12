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
-   Method

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   Method

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

## Interface DataTransferObject {#interface-datatransferobject .title title="Interface DataTransferObject"}
:::

::: contentContainer
::: description
-   

    All Known Subinterfaces:
    :   `AbstractGenruleDescription.CommonArg`, `AndroidKotlinCoreArg`,
        `AndroidLibraryDescription.CoreArg`,
        `AppleNativeTargetDescriptionArg`, `BuildRuleArg`,
        `ConfigurationRuleArg`, `ConstructorArg`,
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
        `AndroidPlatformArg`, `AndroidPrebuiltAarDescriptionArg`,
        `AndroidResourceDescriptionArg`, `ApkGenruleDescriptionArg`,
        `AppleAssetCatalogDescriptionArg`,
        `AppleAssetCatalogsCompilationOptions`,
        `AppleBinaryDescriptionArg`, `AppleBundleDescriptionArg`,
        `AppleLibraryDescriptionArg`, `ApplePackageDescriptionArg`,
        `AppleResourceDescriptionArg`, `AppleTestDescriptionArg`,
        `AppleToolchainDescriptionArg`,
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

        public interface DataTransferObject

    ::: block
    Immutable object is marked with this marker, and this object has a
    builder companion, e. g. for `MyData` there\'s `MyData.Builder`,
    that builder is created with static `  builder()` method, and the
    builder has `build()` method to build `MyData`.
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
-   Method

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   Method

</div>

[]{#skip.navbar.bottom}
:::
