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
[Package]{.packageLabelInType} [com.facebook.buck.core.build.action](package-summary.html)
:::

## Interface BuildEngineAction {#interface-buildengineaction .title title="Interface BuildEngineAction"}
:::

::: contentContainer
::: description
-   

    All Known Subinterfaces:
    :   `Action`, `BinaryBuildRule`, `BuildRule`, `BuildRuleWithBinary`,
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
        `AbstractAction`, `AbstractBuildRule`,
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
        `CompareAbis`, `CopyAction`, `CopyNativeLibraries`,
        `CoreDataModel`, `CsharpLibrary`, `CxxBinary`,
        `CxxCompilationDatabase`, `CxxGenrule`, `CxxLibraryGroup`,
        `CxxLink`, `CxxLuaExtension`, `CxxPrecompiledHeaderTemplate`,
        `CxxPrefixHeader`, `CxxPreprocessAndCompile`,
        `CxxPythonExtension`, `CxxStrip`, `CxxTest`, `CxxThinLTOIndex`,
        `CxxThinLTOOpt`, `DBinary`, `DCompileBuildRule`,
        `DefaultJavaLibrary`, `DefaultWorkerToolRule`,
        `DependencyAggregation`, `DexProducedFromJavaLibrary`,
        `DLibrary`, `DTest`, `DummyRDotJava`,
        `ExopackageDeviceDirectoryLister`, `ExopackageFilesInstaller`,
        `ExopackageInstallFinisher`, `ExopackageResourcesInstaller`,
        `ExportFile`, `ExternallyBuiltApplePackage`,
        `ExternalTestRunner`, `Filegroup`, `GenAidl`,
        `GenerateRDotJava`, `GenerateStringResources`, `Genrule`,
        `GenruleBinary`, `GoBinary`, `GoCompile`, `GoLibrary`, `GoTest`,
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
        `RuleAnalysisLegacyTestBuildRuleView`, `RunAction`,
        `RustCompileRule`, `RustLibrary`, `RustTest`, `SceneKitAssets`,
        `ShBinary`, `ShTest`, `SplitResources`, `SplitUberRDotJavaJar`,
        `StandardJavacPlugin`, `StripLinkable`, `SwiftCompile`,
        `SwiftToolchainBuildRule`, `SymlinkTree`, `TestSuite`,
        `UnitTestOptions`, `UnstrippedNativeLibraries`, `UnzipAar`,
        `WriteAction`, `WriteFile`, `WriteFileHashCode`,
        `WriteStringTemplateRule`, `Zip`

    ------------------------------------------------------------------------

        public interface BuildEngineAction

    ::: block
    Interface for marking objects that the
    [`BuildEngine`](../engine/BuildEngine.html "interface in com.facebook.buck.core.build.engine")
    can build. Eventually, this will become the
    [`Action`](../../rules/actions/Action.html "interface in com.facebook.buck.core.rules.actions")
    interface itself. However, we keep this one around for compatibility
    between existing
    [`BuildRule`](../../rules/BuildRule.html "interface in com.facebook.buck.core.rules")s
    and the new
    [`Action`](../../rules/actions/Action.html "interface in com.facebook.buck.core.rules.actions")s.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `BuildTarget`         | `getBuildTarget()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getDependencies()`   |                       |
        | .common.collect.Immut |                       |                       |
        | ableSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `ge                   |                       |
        | e.common.collect.Immu | tSourcePathOutputs()` |                       |
        | tableSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isCacheable()`       | ::: block             |
        |                       |                       | Whether this          |
        |                       |                       | [`BuildEngin          |
        |                       |                       | eAction`](BuildEngine |
        |                       |                       | Action.html "interfac |
        |                       |                       | e in com.facebook.buc |
        |                       |                       | k.core.build.action") |
        |                       |                       | can be cached.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `should               |                       |
        |                       | RespectInputSizeLimit |                       |
        |                       | ForRemoteExecution()` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildTarget()}

        -   #### getBuildTarget

            ``` methodSignature
            BuildTarget getBuildTarget()
            ```

            [Returns:]{.returnLabel}
            :   the
                [`BuildTarget`](../../model/BuildTarget.html "class in com.facebook.buck.core.model")
                of the rule corresponding to this action

        []{#getDependencies()}

        -   #### getDependencies

            ``` methodSignature
            com.google.common.collect.ImmutableSet<BuildTarget> getDependencies()
            ```

            [Returns:]{.returnLabel}
            :   a set of dependencies required for this
                [`BuildEngineAction`](BuildEngineAction.html "interface in com.facebook.buck.core.build.action")
                to build, as identified by the
                [`BuildTarget`](../../model/BuildTarget.html "class in com.facebook.buck.core.model").

        []{#getSourcePathOutputs()}

        -   #### getSourcePathOutputs

            ``` methodSignature
            com.google.common.collect.ImmutableSet<SourcePath> getSourcePathOutputs()
            ```

            [Returns:]{.returnLabel}
            :   the set of outputs this
                [`BuildEngineAction`](BuildEngineAction.html "interface in com.facebook.buck.core.build.action")
                builds. This is here for legacy as BuildRules deal with
                [`SourcePath`](../../sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")

        []{#isCacheable()}

        -   #### isCacheable

            ``` methodSignature
            boolean isCacheable()
            ```

            ::: block
            Whether this
            [`BuildEngineAction`](BuildEngineAction.html "interface in com.facebook.buck.core.build.action")
            can be cached.
            Uncached build rules are never written out to cache, never
            read from cache, and does not count in cache statistics.
            This rule is useful for artifacts which cannot be easily
            normalized.
            :::

        []{#shouldRespectInputSizeLimitForRemoteExecution()}

        -   #### shouldRespectInputSizeLimitForRemoteExecution

            ``` methodSignature
            default boolean shouldRespectInputSizeLimitForRemoteExecution()
            ```

            [Returns:]{.returnLabel}
            :   true if this rule should only be allowed to be executed
                via Remote Execution if it satisfies input size limits.
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
