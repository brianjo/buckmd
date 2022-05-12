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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules](package-summary.html)
:::

## Interface HasNameAndType {#interface-hasnameandtype .title title="Interface HasNameAndType"}
:::

::: contentContainer
::: description
-   

    All Known Subinterfaces:
    :   `BinaryBuildRule`, `BuildRule`, `BuildRuleWithBinary`,
        `CxxIntermediateBuildProduct`, `ExportDependencies`,
        `ExternalTestRunnerRule`, `HasAppleDebugSymbolDeps`,
        `HasJavaClassHashes`, `HasMavenCoordinates`,
        `HasMultipleOutputs`, `HasPostBuildSteps`, `HasRuntimeDeps`,
        `HasSupplementaryOutputs`, `JavaLibrary`, `JsBundleOutputs`,
        `JsDependenciesOutputs`, `MavenPublishable`,
        `MaybeRequiredForSourceOnlyAbi`, `OverrideScheduleRule`,
        `SupportsDependencyFileRuleKey`, `SupportsInputBasedRuleKey`,
        `SupportsPipelining<T>`, `TestRule`, `TestXRule`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `Aapt2Compile`, `Aapt2Link`, `AaptPackageResources`,
        `AbstractBuildRule`,
        `AbstractBuildRuleWithDeclaredAndExtraDeps`, `AndroidAar`,
        `AndroidAppModularity`, `AndroidAppModularityVerification`,
        `AndroidBinary`, `AndroidBinaryExopackageSymlinkTree`,
        `AndroidBinaryNonExoInstaller`, `AndroidBuildConfig`,
        `AndroidBundle`, `AndroidInstrumentationApk`,
        `AndroidInstrumentationTest`, `AndroidLibrary`,
        `AndroidManifest`, `AndroidPrebuiltAar`, `AndroidResource`,
        `AndroidResourceIndex`, `ApkGenrule`, `AppleAssetCatalog`,
        `AppleBundle`, `AppleDebuggableBinary`, `AppleDsym`,
        `AppleTest`, `AppleTestAggregatedDependencies`, `AppleTestX`,
        `AppleToolchainBuildRule`, `AppleToolchainSetBuildRule`,
        `Archive`, `AssembleDirectories`, `BaseGenrule`,
        `BinaryWrapperRule`, `BuiltinApplePackage`, `CalculateClassAbi`,
        `CalculateSourceAbi`, `CalculateSourceAbiFromLibraryTarget`,
        `CGoGenImport`, `CGoGenSource`, `CGoLibrary`, `CommandAlias`,
        `CompareAbis`, `CopyNativeLibraries`, `CoreDataModel`,
        `CsharpLibrary`, `CxxBinary`, `CxxCompilationDatabase`,
        `CxxGenrule`, `CxxLibraryGroup`, `CxxLink`, `CxxLuaExtension`,
        `CxxPrecompiledHeaderTemplate`, `CxxPrefixHeader`,
        `CxxPreprocessAndCompile`, `CxxPythonExtension`, `CxxStrip`,
        `CxxTest`, `CxxThinLTOIndex`, `CxxThinLTOOpt`, `DBinary`,
        `DCompileBuildRule`, `DefaultJavaLibrary`,
        `DefaultWorkerToolRule`, `DependencyAggregation`,
        `DexProducedFromJavaLibrary`, `DLibrary`, `DTest`,
        `DummyRDotJava`, `ExopackageDeviceDirectoryLister`,
        `ExopackageFilesInstaller`, `ExopackageInstallFinisher`,
        `ExopackageResourcesInstaller`, `ExportFile`,
        `ExternallyBuiltApplePackage`, `ExternalTestRunner`,
        `Filegroup`, `GenAidl`, `GenerateRDotJava`,
        `GenerateStringResources`, `Genrule`, `GenruleBinary`,
        `GoBinary`, `GoCompile`, `GoLibrary`, `GoTest`,
        `GoTestCoverSource`, `GoTestMain`, `GoTestRunner`, `GoTestX`,
        `GwtBinary`, `GwtModule`, `HalideCompile`, `HalideLibrary`,
        `HaskellBinary`, `HaskellCompileRule`, `HaskellGhciRule`,
        `HaskellHaddockLibRule`, `HaskellHaddockRule`, `HaskellLibrary`,
        `HaskellLinkRule`, `HaskellPackageRule`, `HeaderSymlinkTree`,
        `HeaderSymlinkTreeWithHeaderMap`,
        `HeaderSymlinkTreeWithModuleMap`, `HttpArchive`, `HttpFile`,
        `HttpFileBinary`, `InferNullsafe`, `JarFattener`, `JarGenrule`,
        `JavaAnnotationProcessor`, `JavaBinary`, `Javadoc`,
        `JavaSourceJar`, `JavaTest`, `JavaTestRunner`, `JavaTestX`,
        `JsBundle`, `JsBundleAndroid`, `JsBundleGenrule`,
        `JsDependenciesFile`, `JsFile`, `JsLibrary`, `JsonConcatenate`,
        `Keystore`, `LuaBinary`, `LuaLibrary`, `LuaStandaloneBinary`,
        `MachoDylibStubRule`, `MappedSymlinkTree`, `MavenUberJar`,
        `MavenUberJar.SourceJar`, `MergeAndroidResourceSources`,
        `MergeAssets`, `MergeThirdPartyJarResources`, `ModernBuildRule`,
        `MultiarchFile`, `NativeLibraryProguardGenerator`, `NdkLibrary`,
        `NdkToolchainBuildRule`, `NoopBuildRule`,
        `NoopBuildRuleWithDeclaredAndExtraDeps`, `OcamlBinary`,
        `OcamlBuild`, `OcamlCCompile`, `OcamlClean`,
        `OcamlDebugLauncher`, `OcamlLibrary`, `OcamlLink`,
        `OcamlMLCompile`, `PackageStringAssets`,
        `PipelinedModernBuildRule`, `PrebuiltAppleFramework`,
        `PrebuiltCxxLibrary`,
        `PrebuiltCxxLibraryGroupDescription.CustomPrebuiltCxxLibrary`,
        `PrebuiltDotnetLibrary`, `PrebuiltHaskellLibrary`,
        `PrebuiltJar`, `PrebuiltNativeLibrary`, `PrebuiltPythonLibrary`,
        `PreDexMerge`, `PreDexSingleDexMerge`, `PreDexSplitDexGroup`,
        `PreDexSplitDexMerge`, `PreInclude`, `PythonBinary`,
        `PythonCompileRule`, `PythonInPlaceBinary`, `PythonLibrary`,
        `PythonPackagedBinary`, `PythonSymlinkTree`, `PythonTest`,
        `PythonTestRunner`, `PythonTestX`, `RemoteFile`,
        `RemoteFileBinary`, `ResourcesFilter`, `RobolectricTest`,
        `RobolectricTestX`, `RuleAnalysisLegacyBinaryBuildRuleView`,
        `RuleAnalysisLegacyBuildRuleView`,
        `RuleAnalysisLegacyTestBuildRuleView`, `RustCompileRule`,
        `RustLibrary`, `RustTest`, `SceneKitAssets`, `ShBinary`,
        `ShTest`, `SplitResources`, `SplitUberRDotJavaJar`,
        `StandardJavacPlugin`, `StripLinkable`, `SwiftCompile`,
        `SwiftToolchainBuildRule`, `SymlinkTree`, `TestSuite`,
        `UnitTestOptions`, `UnstrippedNativeLibraries`, `UnzipAar`,
        `WriteFile`, `WriteFileHashCode`, `WriteStringTemplateRule`,
        `Zip`

    ------------------------------------------------------------------------

        public interface HasNameAndType

    ::: block
    The type of rule descriptions that have both a name and a type, for
    use in eventing and logging.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                      Description
          ------------------- --------------------------- -------------
          `String`            `getFullyQualifiedName()`    
          `String`            `getType()`                  

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

        []{#getFullyQualifiedName()}

        -   #### getFullyQualifiedName

            ``` methodSignature
            String getFullyQualifiedName()
            ```

        []{#getType()}

        -   #### getType

            ``` methodSignature
            String getType()
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
