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
[Package]{.packageLabelInType} [com.facebook.buck.core.rulekey](package-summary.html)
:::

## Interface AddsToRuleKey {#interface-addstorulekey .title title="Interface AddsToRuleKey"}
:::

::: contentContainer
::: description
-   

    All Known Subinterfaces:
    :   `AddsToRuleKeyFunction<T,​F>`, `ArchiveDependencySupplier`,
        `Archiver`, `Arg`, `Artifact`, `BoundArtifact`, `Buildable`,
        `BuildArtifact`, `CommandLineArgs`,
        `CommandLineArgs.ArgAndFormatString`, `Compiler`,
        `ExopackagePathAndHash`, `ExtraClasspathProvider`, `Javac`,
        `JavaClassHashesProvider`, `Kotlinc`, `Linker`,
        `LinkOutputPostprocessor`, `NdkCxxPlatformCompiler`,
        `PipelinedBuildable<State>`, `Preprocessor`, `PythonComponents`,
        `RuleKeyAppendable`, `SourceArtifact`, `Symlinks`, `Tool`,
        `ToolArg`, `WorkerTool`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AndroidApkBuildable`, `AndroidApkOptimizer`,
        `AndroidBinaryOptimizer`, `AndroidBundleBuildable`,
        `AndroidBundleOptimizer`, `AndroidClasspathProvider`,
        `AndroidPlatformTarget`, `APKModule`, `APKModuleGraph`,
        `AppleAssetCatalogsCompilationOptions`, `AppleBundleResources`,
        `ApplePlatform`, `BsdArchiver`, `BuildableAndTarget`,
        `CalculateSourceAbi.SourceAbiBuildable`, `ClangClCompiler`,
        `ClangClPreprocessor`, `ClangCompiler`, `ClangPreprocessor`,
        `ClangWindowsArchiver`, `ClangWindowsCompiler`,
        `ClangWindowsPreprocessor`, `CodeSignIdentity`, `CommandTool`,
        `CompileToJarStepFactory`, `CompositeArg`,
        `ConstantJavacProvider`,
        `CopyNativeLibraries.StrippedObjectDescription`,
        `CxxFlags.TranslateMacrosArgsFunction`,
        `CxxFlags.TranslateMacrosFunction`, `CxxHeaders`,
        `CxxHeadersDir`, `CxxLink.Impl`, `CxxRawHeaders`,
        `CxxSymlinkTreeHeaders`, `CxxThinLTOIndex.Impl`,
        `CxxThinLTOIndexArg`, `CxxThinLTOOpt.Impl`, `CxxToolFlags`,
        `DarwinLinker`, `DebugPathSanitizer`, `DefaultCompiler`,
        `DefaultJavaClassHashesProvider`, `DelegatingTool`,
        `ExplicitCxxToolFlags`, `ExternalJavac`, `ExternalKotlinc`,
        `ExtraClasspathProvider.EmptyExtraClasspathProvider`,
        `FasterPattern`, `Filegroup`, `FileListableLinkerInputArg`,
        `FilterResourcesSteps.ResourceFilter`, `FormatArg`,
        `FrameworkPath`, `GccCompiler`, `GccPreprocessor`,
        `GenruleAndroidTools`, `GenruleBuildable`, `GnuArchiver`,
        `GnuLinker`, `Groovyc`, `HashedFileTool`, `HeaderVerification`,
        `ImmutableRunInfo`, `InferBuckConfig`, `InferDistTool`,
        `InferPlatform`, `InstallTrigger`, `JarBackedJavac`,
        `JarBackedJavacProvider`, `JarBackedReflectedKotlinc`,
        `JarBuildStepsFactory`,
        `JarBuildStepsFactory.JavaDependencyInfo`,
        `JavacLanguageLevelOptions`, `JavacOptions`,
        `JavacPluginParams`, `JavacToJarStepFactory`,
        `JdkProvidedInMemoryJavac`, `Jsr199Javac`,
        `KotlincToJarStepFactory`, `ManifestEntries`,
        `MergeThirdPartyJarResources`, `NativeFilesInfo`,
        `NoopDebugPathSanitizer`, `OcamlCCompileStep.Args`,
        `OcamlDebugLauncherStep.Args`, `OcamlMLCompileStep.Args`,
        `OutputArtifact`, `OutputLabel`, `OutputPath`,
        `PrefixMapDebugPathSanitizer`, `PreprocessorFlags`,
        `ProvisioningProfileMetadata`, `ProvisioningProfileStore`,
        `ProxyArg`, `PublicOutputPath`, `PythonEnvironment`,
        `PythonMappedComponents`, `PythonPackageComponents`,
        `PythonVersion`, `RedexOptions`, `RelativeLinkArg`,
        `RemoveClassesPatternsMatcher`, `ResolvedJavacPluginProperties`,
        `ResourceFilesInfo`, `ResourcesParameters`, `RunInfo`,
        `RunInfoLegacyTool`, `RustLibraryArg`, `SanitizedArg`,
        `ScalacToJarStepFactory`, `SourceArtifactImpl`, `SourcePathArg`,
        `SourcePathWithAppleBundleDestination`, `SourceSet`,
        `SourceTreePath`, `SourceWithFlags`, `SplitUberRDotJavaJar`,
        `StringArg`, `SwiftTargetTriple`, `SymlinkDir`, `SymlinkMap`,
        `SymlinkPack`, `UnusedDependenciesFinderFactory`,
        `VersionedTool`, `WindowsArchiver`, `WindowsCompiler`,
        `WindowsLinker`, `WindowsMl64Compiler`, `WindowsPreprocessor`,
        `WorkerMacroArg`, `WriteFileHashCode`, `WriteToFileArg`, `Zip`,
        `ZipArchiveDependencySupplier`

    ------------------------------------------------------------------------

        public interface AddsToRuleKey

    ::: block
    Identifies a class that uses
    [`AddToRuleKey`](AddToRuleKey.html "annotation in com.facebook.buck.core.rulekey")
    annotations to indicate fields that should be added to rule keys.
    Value.Immutable annotated classes can use
    [`AddToRuleKey`](AddToRuleKey.html "annotation in com.facebook.buck.core.rulekey")
    on methods to indicate that the method\'s return value should be
    added to rule keys.
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
