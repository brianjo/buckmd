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

## Interface BuildRule {#interface-buildrule .title title="Interface BuildRule"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AllowsNonAnnotatedFields`, `BuildEngineAction`,
        `Comparable<BuildRule>`, `HasNameAndType`

    ```{=html}
    <!-- -->
    ```

    All Known Subinterfaces:
    :   `BinaryBuildRule`, `BuildRuleWithBinary`,
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

        public interface BuildRule
        extends Comparable<BuildRule>, AllowsNonAnnotatedFields, BuildEngineAction, HasNameAndType
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `default int`         | `compa                |                       |
        |                       | reTo​(BuildRule that)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getBuildDeps()`      |                       |
        | SortedSet<BuildRule>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.com       | `                     |                       |
        | mon.collect.Immutable | getBuildSteps​(BuildCo |                       |
        | List<? extends Step>` | ntext context,        |                       |
        |                       |        BuildableConte |                       |
        |                       | xt buildableContext)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildTarget`         | `getBuildTarget()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default String`      | `get                  |                       |
        |                       | FullyQualifiedName()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ProjectFilesystem`   | `ge                   |                       |
        |                       | tProjectFilesystem()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `get                  |                       |
        |                       | SourcePathToOutput()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `hasBuildSteps()`     | ::: block             |
        |                       |                       | Whether this          |
        |                       |                       | [`BuildRul            |
        |                       |                       | e`](BuildRule.html "i |
        |                       |                       | nterface in com.faceb |
        |                       |                       | ook.buck.core.rules") |
        |                       |                       | may have any steps to |
        |                       |                       | build.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isCacheable()`       | ::: block             |
        |                       |                       | Whether this          |
        |                       |                       | [`BuildRul            |
        |                       |                       | e`](BuildRule.html "i |
        |                       |                       | nterface in com.faceb |
        |                       |                       | ook.buck.core.rules") |
        |                       |                       | can be cached.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `out                  |                       |
        |                       | putFileCanBeCopied()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `should               |                       |
        |                       | RespectInputSizeLimit |                       |
        |                       | ForRemoteExecution()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `updateBuildRul       | ::: block             |
        |                       | eResolver​(BuildRuleRe | Updates the           |
        |                       | solver ruleResolver)` | BuildRuleResolver and |
        |                       |                       | associated objects    |
        |                       |                       | for this build rule.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.build.action.BuildEngineAction}

            ### Methods inherited from interface com.facebook.buck.core.build.action.[BuildEngineAction](../build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")

            `getDependencies, getSourcePathOutputs`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.HasNameAndType}

            ### Methods inherited from interface com.facebook.buck.core.rules.[HasNameAndType](HasNameAndType.html "interface in com.facebook.buck.core.rules")

            `getType`
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

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildTarget` in interface `BuildEngineAction`

            [Returns:]{.returnLabel}
            :   the
                [`BuildTarget`](../model/BuildTarget.html "class in com.facebook.buck.core.model")
                of the rule corresponding to this action

        []{#getFullyQualifiedName()}

        -   #### getFullyQualifiedName

            ``` methodSignature
            default String getFullyQualifiedName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFullyQualifiedName` in interface `HasNameAndType`

        []{#getBuildDeps()}

        -   #### getBuildDeps

            ``` methodSignature
            SortedSet<BuildRule> getBuildDeps()
            ```

            [Returns:]{.returnLabel}

            :   the set of rules that must be built before this rule.
                Normally, this matches the value of the `deps` argument
                for this build rule in the build file in which it was
                defined.

                However, there are special cases where other arguments
                pull in implicit dependencies (e.g., the `keystore`
                argument in `android_binary`). In these cases, the
                implicit dependencies are also included in the set
                returned by this method. The value of the original
                `deps` argument, as defined in the build file, must be
                accessed via a custom getter provided by the build rule.

        []{#toString()}

        -   #### toString

            ``` methodSignature
            String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

            [Returns:]{.returnLabel}
            :   the same value as
                [`getFullyQualifiedName()`](#getFullyQualifiedName())

        []{#getBuildSteps(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.build.buildable.context.BuildableContext)}

        -   #### getBuildSteps

            ``` methodSignature
            com.google.common.collect.ImmutableList<? extends Step> getBuildSteps​(BuildContext context,
                                                                                  BuildableContext buildableContext)
            ```

        []{#getSourcePathToOutput()}

        -   #### getSourcePathToOutput

            ``` methodSignature
            @Nullable
            SourcePath getSourcePathToOutput()
            ```

        []{#outputFileCanBeCopied()}

        -   #### outputFileCanBeCopied

            ``` methodSignature
            default boolean outputFileCanBeCopied()
            ```

            [Returns:]{.returnLabel}
            :   true if the output of this build rule is compatible with
                `buck build --out`. To be compatible, that means (1)
                [`getSourcePathToOutput()`](#getSourcePathToOutput())
                cannot return `null`, and (2) the output file works as
                intended when copied to an arbitrary path (i.e., does
                not have any dependencies on relative symlinks).

        []{#getProjectFilesystem()}

        -   #### getProjectFilesystem

            ``` methodSignature
            ProjectFilesystem getProjectFilesystem()
            ```

        []{#isCacheable()}

        -   #### isCacheable

            ``` methodSignature
            boolean isCacheable()
            ```

            ::: block
            Whether this
            [`BuildRule`](BuildRule.html "interface in com.facebook.buck.core.rules")
            can be cached.
            Uncached build rules are never written out to cache, never
            read from cache, and does not count in cache statistics.
            This rule is useful for artifacts which cannot be easily
            normalized.

            Uncached rules are not always rebuilt, however, as long as
            the existing on-disk representation is up to date. This
            means that these rules can take advantage of
            [`SupportsInputBasedRuleKey`](attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr")
            to prevent rebuilding.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `isCacheable` in interface `BuildEngineAction`

        []{#hasBuildSteps()}

        -   #### hasBuildSteps

            ``` methodSignature
            boolean hasBuildSteps()
            ```

            ::: block
            Whether this
            [`BuildRule`](BuildRule.html "interface in com.facebook.buck.core.rules")
            may have any steps to build.
            :::

        []{#compareTo(com.facebook.buck.core.rules.BuildRule)}

        -   #### compareTo

            ``` methodSignature
            default int compareTo​(BuildRule that)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `compareTo` in interface `Comparable<BuildRule>`

        []{#updateBuildRuleResolver(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### updateBuildRuleResolver

            ``` methodSignature
            void updateBuildRuleResolver​(BuildRuleResolver ruleResolver)
            ```

            ::: block
            Updates the BuildRuleResolver and associated objects for
            this build rule.
            Build rules sometimes hold field references to build rule
            resolvers. If this build rule is to be cached, it must
            update its BuildRuleResolver when a new action graph is
            constructed to avoid leaking the entire action graph it was
            originally associated with.
            :::

        []{#shouldRespectInputSizeLimitForRemoteExecution()}

        -   #### shouldRespectInputSizeLimitForRemoteExecution

            ``` methodSignature
            default boolean shouldRespectInputSizeLimitForRemoteExecution()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `shouldRespectInputSizeLimitForRemoteExecution` in
                interface `BuildEngineAction`

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
