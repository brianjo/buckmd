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
-   Tree
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Hierarchy For Package com.facebook.buck.android {#hierarchy-for-package-com.facebook.buck.android .title}

[Package Hierarchies:]{.packageHierarchyLabel}

-   [All Packages](../../../../overview-tree.html)
:::

::: contentContainer
::: {.section role="region"}
## Class Hierarchy {#class-hierarchy title="Class Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   com.facebook.buck.android.[[AabBuilderStep]{.typeNameLink}](AabBuilderStep.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.step.[Step](../step/Step.html "interface in com.facebook.buck.step"))
    -   com.facebook.buck.core.rules.impl.[[AbstractBuildRule]{.typeNameLink}](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")
        (implements
        com.facebook.buck.core.rules.[BuildRule](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules"))
        -   com.facebook.buck.android.[[Aapt2Link]{.typeNameLink}](Aapt2Link.html "class in com.facebook.buck.android")
        -   com.facebook.buck.android.[[AaptPackageResources]{.typeNameLink}](AaptPackageResources.html "class in com.facebook.buck.android")
        -   com.facebook.buck.core.rules.impl.[[AbstractBuildRuleWithDeclaredAndExtraDeps]{.typeNameLink}](../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")
            (implements
            com.facebook.buck.core.rules.attr.[HasDeclaredAndExtraDeps](../core/rules/attr/HasDeclaredAndExtraDeps.html "interface in com.facebook.buck.core.rules.attr"))
            -   com.facebook.buck.android.[[AndroidAar]{.typeNameLink}](AndroidAar.html "class in com.facebook.buck.android")
                (implements
                com.facebook.buck.jvm.core.[HasClasspathEntries](../jvm/core/HasClasspathEntries.html "interface in com.facebook.buck.jvm.core"))
            -   com.facebook.buck.android.[[AndroidBuildConfig]{.typeNameLink}](AndroidBuildConfig.html "class in com.facebook.buck.android")
            -   com.facebook.buck.android.[[AndroidInstrumentationTest]{.typeNameLink}](AndroidInstrumentationTest.html "class in com.facebook.buck.android")
                (implements
                com.facebook.buck.core.test.rule.[ExternalTestRunnerRule](../core/test/rule/ExternalTestRunnerRule.html "interface in com.facebook.buck.core.test.rule"),
                com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"),
                com.facebook.buck.core.test.rule.[TestRule](../core/test/rule/TestRule.html "interface in com.facebook.buck.core.test.rule"))
            -   com.facebook.buck.android.[[AndroidResource]{.typeNameLink}](AndroidResource.html "class in com.facebook.buck.android")
                (implements
                com.facebook.buck.android.packageable.[AndroidPackageable](packageable/AndroidPackageable.html "interface in com.facebook.buck.android.packageable"),
                com.facebook.buck.android.[HasAndroidResourceDeps](HasAndroidResourceDeps.html "interface in com.facebook.buck.android"),
                com.facebook.buck.jvm.core.[HasClasspathDeps](../jvm/core/HasClasspathDeps.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.core.rules.attr.[InitializableFromDisk](../core/rules/attr/InitializableFromDisk.html "interface in com.facebook.buck.core.rules.attr")\<T\>,
                com.facebook.buck.core.rules.attr.[SupportsInputBasedRuleKey](../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr"))
            -   com.facebook.buck.android.[[AndroidResourceIndex]{.typeNameLink}](AndroidResourceIndex.html "class in com.facebook.buck.android")
            -   com.facebook.buck.android.[[GenAidl]{.typeNameLink}](GenAidl.html "class in com.facebook.buck.android")
            -   com.facebook.buck.jvm.java.[[JavaTest]{.typeNameLink}](../jvm/java/JavaTest.html "class in com.facebook.buck.jvm.java")
                (implements
                com.facebook.buck.core.rules.attr.[ExportDependencies](../core/rules/attr/ExportDependencies.html "interface in com.facebook.buck.core.rules.attr"),
                com.facebook.buck.core.test.rule.[ExternalTestRunnerRule](../core/test/rule/ExternalTestRunnerRule.html "interface in com.facebook.buck.core.test.rule"),
                com.facebook.buck.jvm.core.[HasClasspathEntries](../jvm/core/HasClasspathEntries.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.core.rules.attr.[HasPostBuildSteps](../core/rules/attr/HasPostBuildSteps.html "interface in com.facebook.buck.core.rules.attr"),
                com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"),
                com.facebook.buck.core.test.rule.[TestRule](../core/test/rule/TestRule.html "interface in com.facebook.buck.core.test.rule"))
                -   com.facebook.buck.android.[[RobolectricTest]{.typeNameLink}](RobolectricTest.html "class in com.facebook.buck.android")
            -   com.facebook.buck.jvm.java.[[JavaTestX]{.typeNameLink}](../jvm/java/JavaTestX.html "class in com.facebook.buck.jvm.java")
                (implements
                com.facebook.buck.core.rules.attr.[ExportDependencies](../core/rules/attr/ExportDependencies.html "interface in com.facebook.buck.core.rules.attr"),
                com.facebook.buck.core.test.rule.[ExternalTestRunnerRule](../core/test/rule/ExternalTestRunnerRule.html "interface in com.facebook.buck.core.test.rule"),
                com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"),
                com.facebook.buck.core.test.rule.[TestXRule](../core/test/rule/TestXRule.html "interface in com.facebook.buck.core.test.rule"))
                -   com.facebook.buck.android.[[RobolectricTestX]{.typeNameLink}](RobolectricTestX.html "class in com.facebook.buck.android")
            -   com.facebook.buck.android.[[NativeLibraryProguardGenerator]{.typeNameLink}](NativeLibraryProguardGenerator.html "class in com.facebook.buck.android")
            -   com.facebook.buck.android.[[NdkLibrary]{.typeNameLink}](NdkLibrary.html "class in com.facebook.buck.android")
                (implements
                com.facebook.buck.android.packageable.[AndroidPackageable](packageable/AndroidPackageable.html "interface in com.facebook.buck.android.packageable"),
                com.facebook.buck.android.[NativeLibraryBuildRule](NativeLibraryBuildRule.html "interface in com.facebook.buck.android"))
            -   com.facebook.buck.android.[[PrebuiltNativeLibrary]{.typeNameLink}](PrebuiltNativeLibrary.html "class in com.facebook.buck.android")
                (implements
                com.facebook.buck.android.packageable.[AndroidPackageable](packageable/AndroidPackageable.html "interface in com.facebook.buck.android.packageable"),
                com.facebook.buck.android.[NativeLibraryBuildRule](NativeLibraryBuildRule.html "interface in com.facebook.buck.android"))
            -   com.facebook.buck.android.[[PreDexMerge]{.typeNameLink}](PreDexMerge.html "class in com.facebook.buck.android")
                (implements
                com.facebook.buck.android.[HasDexFiles](HasDexFiles.html "interface in com.facebook.buck.android"))
                -   com.facebook.buck.android.[[PreDexSingleDexMerge]{.typeNameLink}](PreDexSingleDexMerge.html "class in com.facebook.buck.android")
                -   com.facebook.buck.android.[[PreDexSplitDexMerge]{.typeNameLink}](PreDexSplitDexMerge.html "class in com.facebook.buck.android")
            -   com.facebook.buck.android.[[PreDexSplitDexGroup]{.typeNameLink}](PreDexSplitDexGroup.html "class in com.facebook.buck.android")
                (implements
                com.facebook.buck.core.rules.attr.[InitializableFromDisk](../core/rules/attr/InitializableFromDisk.html "interface in com.facebook.buck.core.rules.attr")\<T\>,
                com.facebook.buck.core.rules.attr.[SupportsInputBasedRuleKey](../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr"))
            -   com.facebook.buck.android.[[UnstrippedNativeLibraries]{.typeNameLink}](UnstrippedNativeLibraries.html "class in com.facebook.buck.android")
                (implements
                com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"),
                com.facebook.buck.core.rules.attr.[SupportsInputBasedRuleKey](../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr"))
            -   com.facebook.buck.android.[[UnzipAar]{.typeNameLink}](UnzipAar.html "class in com.facebook.buck.android")
                (implements
                com.facebook.buck.core.rules.attr.[InitializableFromDisk](../core/rules/attr/InitializableFromDisk.html "interface in com.facebook.buck.core.rules.attr")\<T\>)
        -   com.facebook.buck.android.[[AndroidAppModularity]{.typeNameLink}](AndroidAppModularity.html "class in com.facebook.buck.android")
        -   com.facebook.buck.android.[[AndroidAppModularityVerification]{.typeNameLink}](AndroidAppModularityVerification.html "class in com.facebook.buck.android")
        -   com.facebook.buck.android.[[AndroidBinary]{.typeNameLink}](AndroidBinary.html "class in com.facebook.buck.android")
            (implements
            com.facebook.buck.jvm.core.[HasClasspathDeps](../jvm/core/HasClasspathDeps.html "interface in com.facebook.buck.jvm.core"),
            com.facebook.buck.jvm.core.[HasClasspathEntries](../jvm/core/HasClasspathEntries.html "interface in com.facebook.buck.jvm.core"),
            com.facebook.buck.core.rules.attr.[HasDeclaredAndExtraDeps](../core/rules/attr/HasDeclaredAndExtraDeps.html "interface in com.facebook.buck.core.rules.attr"),
            com.facebook.buck.android.[HasInstallableApk](HasInstallableApk.html "interface in com.facebook.buck.android"),
            com.facebook.buck.core.rules.attr.[HasInstallHelpers](../core/rules/attr/HasInstallHelpers.html "interface in com.facebook.buck.core.rules.attr"),
            com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"),
            com.facebook.buck.core.rules.attr.[SupportsInputBasedRuleKey](../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr"))
            -   com.facebook.buck.android.[[AndroidInstrumentationApk]{.typeNameLink}](AndroidInstrumentationApk.html "class in com.facebook.buck.android")
        -   com.facebook.buck.android.[[AndroidBinaryExopackageSymlinkTree]{.typeNameLink}](AndroidBinaryExopackageSymlinkTree.html "class in com.facebook.buck.android")
        -   com.facebook.buck.android.[[AndroidBinaryNonExoInstaller]{.typeNameLink}](AndroidBinaryNonExoInstaller.html "class in com.facebook.buck.android")
            (implements
            com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"))
        -   com.facebook.buck.android.[[AndroidBundle]{.typeNameLink}](AndroidBundle.html "class in com.facebook.buck.android")
            (implements
            com.facebook.buck.jvm.core.[HasClasspathEntries](../jvm/core/HasClasspathEntries.html "interface in com.facebook.buck.jvm.core"),
            com.facebook.buck.core.rules.attr.[HasDeclaredAndExtraDeps](../core/rules/attr/HasDeclaredAndExtraDeps.html "interface in com.facebook.buck.core.rules.attr"),
            com.facebook.buck.android.[HasInstallableApk](HasInstallableApk.html "interface in com.facebook.buck.android"),
            com.facebook.buck.core.rules.attr.[HasInstallHelpers](../core/rules/attr/HasInstallHelpers.html "interface in com.facebook.buck.core.rules.attr"),
            com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"),
            com.facebook.buck.core.rules.attr.[SupportsInputBasedRuleKey](../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr"))
        -   com.facebook.buck.android.[[AndroidManifest]{.typeNameLink}](AndroidManifest.html "class in com.facebook.buck.android")
        -   com.facebook.buck.android.[[AssembleDirectories]{.typeNameLink}](AssembleDirectories.html "class in com.facebook.buck.android")
        -   com.facebook.buck.android.[[CopyNativeLibraries]{.typeNameLink}](CopyNativeLibraries.html "class in com.facebook.buck.android")
            (implements
            com.facebook.buck.core.rules.attr.[SupportsInputBasedRuleKey](../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr"))
        -   com.facebook.buck.android.[[DummyRDotJava]{.typeNameLink}](DummyRDotJava.html "class in com.facebook.buck.android")
            (implements
            com.facebook.buck.jvm.core.[HasJavaAbi](../jvm/core/HasJavaAbi.html "interface in com.facebook.buck.jvm.core"),
            com.facebook.buck.core.rules.attr.[InitializableFromDisk](../core/rules/attr/InitializableFromDisk.html "interface in com.facebook.buck.core.rules.attr")\<T\>,
            com.facebook.buck.core.rules.attr.[SupportsInputBasedRuleKey](../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr"))
        -   com.facebook.buck.android.[[ExopackageDeviceDirectoryLister]{.typeNameLink}](ExopackageDeviceDirectoryLister.html "class in com.facebook.buck.android")
        -   com.facebook.buck.android.[[ExopackageFilesInstaller]{.typeNameLink}](ExopackageFilesInstaller.html "class in com.facebook.buck.android")
        -   com.facebook.buck.android.[[ExopackageInstallFinisher]{.typeNameLink}](ExopackageInstallFinisher.html "class in com.facebook.buck.android")
        -   com.facebook.buck.android.[[ExopackageResourcesInstaller]{.typeNameLink}](ExopackageResourcesInstaller.html "class in com.facebook.buck.android")
        -   com.facebook.buck.android.[[GenerateRDotJava]{.typeNameLink}](GenerateRDotJava.html "class in com.facebook.buck.android")
        -   com.facebook.buck.android.[[GenerateStringResources]{.typeNameLink}](GenerateStringResources.html "class in com.facebook.buck.android")
        -   com.facebook.buck.android.[[MergeAssets]{.typeNameLink}](MergeAssets.html "class in com.facebook.buck.android")
        -   com.facebook.buck.rules.modern.[[ModernBuildRule]{.typeNameLink}](../rules/modern/ModernBuildRule.html "class in com.facebook.buck.rules.modern")\<T\>
            (implements
            com.facebook.buck.core.rules.attr.[SupportsInputBasedRuleKey](../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr"))
            -   com.facebook.buck.android.[[Aapt2Compile]{.typeNameLink}](Aapt2Compile.html "class in com.facebook.buck.android")
            -   com.facebook.buck.shell.[[BaseGenrule]{.typeNameLink}](../shell/BaseGenrule.html "class in com.facebook.buck.shell")\<T\>
                (implements
                com.facebook.buck.core.rules.attr.[HasMultipleOutputs](../core/rules/attr/HasMultipleOutputs.html "interface in com.facebook.buck.core.rules.attr"),
                com.facebook.buck.core.model.[HasOutputName](../core/model/HasOutputName.html "interface in com.facebook.buck.core.model"))
                -   com.facebook.buck.android.[[ApkGenrule]{.typeNameLink}](ApkGenrule.html "class in com.facebook.buck.android")
                    (implements
                    com.facebook.buck.jvm.core.[HasClasspathEntries](../jvm/core/HasClasspathEntries.html "interface in com.facebook.buck.jvm.core"),
                    com.facebook.buck.android.[HasInstallableApk](HasInstallableApk.html "interface in com.facebook.buck.android"),
                    com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"))
            -   com.facebook.buck.android.[[DexProducedFromJavaLibrary]{.typeNameLink}](DexProducedFromJavaLibrary.html "class in com.facebook.buck.android")
                (implements
                com.facebook.buck.core.rules.attr.[InitializableFromDisk](../core/rules/attr/InitializableFromDisk.html "interface in com.facebook.buck.core.rules.attr")\<T\>)
            -   com.facebook.buck.android.[[MergeThirdPartyJarResources]{.typeNameLink}](MergeThirdPartyJarResources.html "class in com.facebook.buck.android")
                (implements
                com.facebook.buck.rules.modern.[Buildable](../rules/modern/Buildable.html "interface in com.facebook.buck.rules.modern"))
            -   com.facebook.buck.rules.modern.[[PipelinedModernBuildRule]{.typeNameLink}](../rules/modern/PipelinedModernBuildRule.html "class in com.facebook.buck.rules.modern")\<State,​T\>
                (implements
                com.facebook.buck.core.rules.pipeline.[SupportsPipelining](../core/rules/pipeline/SupportsPipelining.html "interface in com.facebook.buck.core.rules.pipeline")\<T\>)
                -   com.facebook.buck.jvm.java.[[DefaultJavaLibrary]{.typeNameLink}](../jvm/java/DefaultJavaLibrary.html "class in com.facebook.buck.jvm.java")
                    (implements
                    com.facebook.buck.android.packageable.[AndroidPackageable](packageable/AndroidPackageable.html "interface in com.facebook.buck.android.packageable"),
                    com.facebook.buck.core.rules.attr.[ExportDependencies](../core/rules/attr/ExportDependencies.html "interface in com.facebook.buck.core.rules.attr"),
                    com.facebook.buck.core.rules.attr.[InitializableFromDisk](../core/rules/attr/InitializableFromDisk.html "interface in com.facebook.buck.core.rules.attr")\<T\>,
                    com.facebook.buck.jvm.core.[JavaLibrary](../jvm/core/JavaLibrary.html "interface in com.facebook.buck.jvm.core"),
                    com.facebook.buck.jvm.java.[JavaLibraryWithTests](../jvm/java/JavaLibraryWithTests.html "interface in com.facebook.buck.jvm.java"),
                    com.facebook.buck.jvm.java.[MaybeRequiredForSourceOnlyAbi](../jvm/java/MaybeRequiredForSourceOnlyAbi.html "interface in com.facebook.buck.jvm.java"),
                    com.facebook.buck.core.rules.attr.[SupportsDependencyFileRuleKey](../core/rules/attr/SupportsDependencyFileRuleKey.html "interface in com.facebook.buck.core.rules.attr"))
                    -   com.facebook.buck.android.[[AndroidLibrary]{.typeNameLink}](AndroidLibrary.html "class in com.facebook.buck.android")
                        (implements
                        com.facebook.buck.android.packageable.[AndroidPackageable](packageable/AndroidPackageable.html "interface in com.facebook.buck.android.packageable"))
                        -   com.facebook.buck.android.[[AndroidPrebuiltAar]{.typeNameLink}](AndroidPrebuiltAar.html "class in com.facebook.buck.android")
                            (implements
                            com.facebook.buck.android.[HasAndroidResourceDeps](HasAndroidResourceDeps.html "interface in com.facebook.buck.android"),
                            com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"))
            -   com.facebook.buck.android.[[SplitUberRDotJavaJar]{.typeNameLink}](SplitUberRDotJavaJar.html "class in com.facebook.buck.android")
                (implements
                com.facebook.buck.rules.modern.[Buildable](../rules/modern/Buildable.html "interface in com.facebook.buck.rules.modern"))
            -   com.facebook.buck.android.[[StripLinkable]{.typeNameLink}](StripLinkable.html "class in com.facebook.buck.android")
            -   com.facebook.buck.android.[[UnitTestOptions]{.typeNameLink}](UnitTestOptions.html "class in com.facebook.buck.android")
            -   com.facebook.buck.android.[[WriteFileHashCode]{.typeNameLink}](WriteFileHashCode.html "class in com.facebook.buck.android")
                (implements
                com.facebook.buck.rules.modern.[Buildable](../rules/modern/Buildable.html "interface in com.facebook.buck.rules.modern"))
        -   com.facebook.buck.core.rules.impl.[[NoopBuildRule]{.typeNameLink}](../core/rules/impl/NoopBuildRule.html "class in com.facebook.buck.core.rules.impl")
            (implements
            com.facebook.buck.core.rules.attr.[SupportsInputBasedRuleKey](../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr"))
            -   com.facebook.buck.android.[[NdkToolchainBuildRule]{.typeNameLink}](NdkToolchainBuildRule.html "class in com.facebook.buck.android")
                (implements
                com.facebook.buck.android.toolchain.ndk.[ProvidesNdkCxxPlatform](toolchain/ndk/ProvidesNdkCxxPlatform.html "interface in com.facebook.buck.android.toolchain.ndk"))
        -   com.facebook.buck.android.[[PackageStringAssets]{.typeNameLink}](PackageStringAssets.html "class in com.facebook.buck.android")
        -   com.facebook.buck.android.[[ResourcesFilter]{.typeNameLink}](ResourcesFilter.html "class in com.facebook.buck.android")
            (implements
            com.facebook.buck.android.[FilteredResourcesProvider](FilteredResourcesProvider.html "interface in com.facebook.buck.android"),
            com.facebook.buck.core.rules.attr.[InitializableFromDisk](../core/rules/attr/InitializableFromDisk.html "interface in com.facebook.buck.core.rules.attr")\<T\>)
        -   com.facebook.buck.android.[[SplitResources]{.typeNameLink}](SplitResources.html "class in com.facebook.buck.android")
    -   com.facebook.buck.step.[[AbstractExecutionStep]{.typeNameLink}](../step/AbstractExecutionStep.html "class in com.facebook.buck.step")
        (implements
        com.facebook.buck.step.[Step](../step/Step.html "interface in com.facebook.buck.step"))
        -   com.facebook.buck.android.[[ExtractFromAndroidManifestStep]{.typeNameLink}](ExtractFromAndroidManifestStep.html "class in com.facebook.buck.android")
        -   com.facebook.buck.android.[[HashInputJarsToDexStep]{.typeNameLink}](HashInputJarsToDexStep.html "class in com.facebook.buck.android")
            (implements
            com.facebook.buck.android.[SmartDexingStep.DexInputHashesProvider](SmartDexingStep.DexInputHashesProvider.html "interface in com.facebook.buck.android"))
    -   com.facebook.buck.shell.[[AbstractGenruleDescription]{.typeNameLink}](../shell/AbstractGenruleDescription.html "class in com.facebook.buck.shell")\<T\>
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>)
        -   com.facebook.buck.android.[[ApkGenruleDescription]{.typeNameLink}](ApkGenruleDescription.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AdbHelper]{.typeNameLink}](AdbHelper.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.android.exopackage.[AndroidDevicesHelper](exopackage/AndroidDevicesHelper.html "interface in com.facebook.buck.android.exopackage"))
    -   com.facebook.buck.android.[[AndroidAarDescription]{.typeNameLink}](AndroidAarDescription.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>)
    -   com.facebook.buck.android.[[AndroidAarDescriptionArg]{.typeNameLink}](AndroidAarDescriptionArg.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AndroidAarDescriptionArg.Builder]{.typeNameLink}](AndroidAarDescriptionArg.Builder.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AndroidApkBuildable]{.typeNameLink}](AndroidApkBuildable.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AndroidAppModularityDescription]{.typeNameLink}](AndroidAppModularityDescription.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>)
    -   com.facebook.buck.android.[[AndroidAppModularityDescriptionArg]{.typeNameLink}](AndroidAppModularityDescriptionArg.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AndroidAppModularityDescriptionArg.Builder]{.typeNameLink}](AndroidAppModularityDescriptionArg.Builder.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AndroidAppModularityGraphEnhancer]{.typeNameLink}](AndroidAppModularityGraphEnhancer.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AndroidBinaryDescription]{.typeNameLink}](AndroidBinaryDescription.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.model.[Flavored](../core/model/Flavored.html "interface in com.facebook.buck.core.model"),
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>)
    -   com.facebook.buck.android.[[AndroidBinaryDescriptionArg]{.typeNameLink}](AndroidBinaryDescriptionArg.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AndroidBinaryDescriptionArg.Builder]{.typeNameLink}](AndroidBinaryDescriptionArg.Builder.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AndroidBinaryFactory]{.typeNameLink}](AndroidBinaryFactory.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AndroidBinaryFilesInfo]{.typeNameLink}](AndroidBinaryFilesInfo.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AndroidBinaryGraphEnhancer]{.typeNameLink}](AndroidBinaryGraphEnhancer.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AndroidBinaryGraphEnhancerFactory]{.typeNameLink}](AndroidBinaryGraphEnhancerFactory.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AndroidBinaryOptimizer]{.typeNameLink}](AndroidBinaryOptimizer.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"))
        -   com.facebook.buck.android.[[AndroidApkOptimizer]{.typeNameLink}](AndroidApkOptimizer.html "class in com.facebook.buck.android")
        -   com.facebook.buck.android.[[AndroidBundleOptimizer]{.typeNameLink}](AndroidBundleOptimizer.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AndroidBinaryPathUtility]{.typeNameLink}](AndroidBinaryPathUtility.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AndroidBuckConfig]{.typeNameLink}](AndroidBuckConfig.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AndroidBuildConfigDescription]{.typeNameLink}](AndroidBuildConfigDescription.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>)
    -   com.facebook.buck.android.[[AndroidBuildConfigDescriptionArg]{.typeNameLink}](AndroidBuildConfigDescriptionArg.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AndroidBuildConfigDescriptionArg.Builder]{.typeNameLink}](AndroidBuildConfigDescriptionArg.Builder.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AndroidBundleBuildable]{.typeNameLink}](AndroidBundleBuildable.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AndroidBundleDescription]{.typeNameLink}](AndroidBundleDescription.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.model.[Flavored](../core/model/Flavored.html "interface in com.facebook.buck.core.model"),
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>)
    -   com.facebook.buck.android.[[AndroidBundleDescriptionArg]{.typeNameLink}](AndroidBundleDescriptionArg.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AndroidBundleDescriptionArg.Builder]{.typeNameLink}](AndroidBundleDescriptionArg.Builder.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AndroidBundleFactory]{.typeNameLink}](AndroidBundleFactory.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AndroidClasspathProvider]{.typeNameLink}](AndroidClasspathProvider.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.jvm.java.[ExtraClasspathProvider](../jvm/java/ExtraClasspathProvider.html "interface in com.facebook.buck.jvm.java"))
    -   com.facebook.buck.android.[[AndroidDescriptionsProvider]{.typeNameLink}](AndroidDescriptionsProvider.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.core.model.targetgraph.[DescriptionProvider](../core/model/targetgraph/DescriptionProvider.html "interface in com.facebook.buck.core.model.targetgraph"))
    -   com.facebook.buck.android.[[AndroidInstallConfig]{.typeNameLink}](AndroidInstallConfig.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AndroidInstrumentationApkDescription]{.typeNameLink}](AndroidInstrumentationApkDescription.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>)
    -   com.facebook.buck.android.[[AndroidInstrumentationApkDescriptionArg]{.typeNameLink}](AndroidInstrumentationApkDescriptionArg.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AndroidInstrumentationApkDescriptionArg.Builder]{.typeNameLink}](AndroidInstrumentationApkDescriptionArg.Builder.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AndroidInstrumentationTestDescription]{.typeNameLink}](AndroidInstrumentationTestDescription.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>)
    -   com.facebook.buck.android.[[AndroidInstrumentationTestDescriptionArg]{.typeNameLink}](AndroidInstrumentationTestDescriptionArg.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AndroidInstrumentationTestDescriptionArg.Builder]{.typeNameLink}](AndroidInstrumentationTestDescriptionArg.Builder.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AndroidLibrary.Builder]{.typeNameLink}](AndroidLibrary.Builder.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AndroidLibraryDescription]{.typeNameLink}](AndroidLibraryDescription.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.model.[Flavored](../core/model/Flavored.html "interface in com.facebook.buck.core.model"),
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>)
    -   com.facebook.buck.android.[[AndroidLibraryDescriptionArg]{.typeNameLink}](AndroidLibraryDescriptionArg.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AndroidLibraryDescriptionArg.Builder]{.typeNameLink}](AndroidLibraryDescriptionArg.Builder.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AndroidLibraryGraphEnhancer]{.typeNameLink}](AndroidLibraryGraphEnhancer.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AndroidManifestDescription]{.typeNameLink}](AndroidManifestDescription.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>)
    -   com.facebook.buck.android.[[AndroidManifestDescriptionArg]{.typeNameLink}](AndroidManifestDescriptionArg.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AndroidManifestDescriptionArg.Builder]{.typeNameLink}](AndroidManifestDescriptionArg.Builder.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AndroidManifestFactory]{.typeNameLink}](AndroidManifestFactory.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AndroidModuleConsistencyStep]{.typeNameLink}](AndroidModuleConsistencyStep.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.step.[Step](../step/Step.html "interface in com.facebook.buck.step"))
    -   com.facebook.buck.android.[[AndroidNativeLibsPackageableGraphEnhancer]{.typeNameLink}](AndroidNativeLibsPackageableGraphEnhancer.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AndroidPrebuiltAarDescription]{.typeNameLink}](AndroidPrebuiltAarDescription.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.model.[Flavored](../core/model/Flavored.html "interface in com.facebook.buck.core.model"),
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>)
    -   com.facebook.buck.android.[[AndroidPrebuiltAarDescriptionArg]{.typeNameLink}](AndroidPrebuiltAarDescriptionArg.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AndroidPrebuiltAarDescriptionArg.Builder]{.typeNameLink}](AndroidPrebuiltAarDescriptionArg.Builder.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AndroidResourceDescription]{.typeNameLink}](AndroidResourceDescription.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.model.[Flavored](../core/model/Flavored.html "interface in com.facebook.buck.core.model"),
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>)
    -   com.facebook.buck.android.[[AndroidResourceDescriptionArg]{.typeNameLink}](AndroidResourceDescriptionArg.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AndroidResourceDescriptionArg.Builder]{.typeNameLink}](AndroidResourceDescriptionArg.Builder.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AndroidResourceHelper]{.typeNameLink}](AndroidResourceHelper.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AndroidTransitiveDependencyGraph]{.typeNameLink}](AndroidTransitiveDependencyGraph.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[ApkBuilderStep]{.typeNameLink}](ApkBuilderStep.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.step.[Step](../step/Step.html "interface in com.facebook.buck.step"))
    -   com.facebook.buck.android.[[ApkGenruleDescriptionArg]{.typeNameLink}](ApkGenruleDescriptionArg.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[ApkGenruleDescriptionArg.Builder]{.typeNameLink}](ApkGenruleDescriptionArg.Builder.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[ApkInstallStep]{.typeNameLink}](ApkInstallStep.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.step.[Step](../step/Step.html "interface in com.facebook.buck.step"))
    -   com.facebook.buck.android.[[AppBuilderBase]{.typeNameLink}](AppBuilderBase.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AppBuilderBase.PrivateKeyAndCertificate]{.typeNameLink}](AppBuilderBase.PrivateKeyAndCertificate.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AppModularityMetadataUtil]{.typeNameLink}](AppModularityMetadataUtil.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[BuckEventAndroidLogger]{.typeNameLink}](BuckEventAndroidLogger.html "class in com.facebook.buck.android")
        (implements com.android.common.utils.ILogger)
    -   com.facebook.buck.android.[[BuildConfigs]{.typeNameLink}](BuildConfigs.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[ClassNameFilter]{.typeNameLink}](ClassNameFilter.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[CompileStringsStep]{.typeNameLink}](CompileStringsStep.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.step.[Step](../step/Step.html "interface in com.facebook.buck.step"))
    -   com.facebook.buck.android.[[ConcatStep]{.typeNameLink}](ConcatStep.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.step.[Step](../step/Step.html "interface in com.facebook.buck.step"))
    -   com.facebook.buck.android.[[ConstraintBasedAndroidNativeTargetConfigurationMatcher]{.typeNameLink}](ConstraintBasedAndroidNativeTargetConfigurationMatcher.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.android.[AndroidNativeTargetConfigurationMatcher](AndroidNativeTargetConfigurationMatcher.html "interface in com.facebook.buck.android"))
    -   com.facebook.buck.android.[[CopyNativeLibraries.StrippedObjectDescription]{.typeNameLink}](CopyNativeLibraries.StrippedObjectDescription.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"))
    -   com.facebook.buck.android.[[DefaultAndroidLibraryCompilerFactory]{.typeNameLink}](DefaultAndroidLibraryCompilerFactory.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.android.[AndroidLibraryCompilerFactory](AndroidLibraryCompilerFactory.html "interface in com.facebook.buck.android"))
    -   com.facebook.buck.android.[[DefaultAndroidManifestReader]{.typeNameLink}](DefaultAndroidManifestReader.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.android.[AndroidManifestReader](AndroidManifestReader.html "interface in com.facebook.buck.android"))
    -   com.facebook.buck.android.[[DxConfig]{.typeNameLink}](DxConfig.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[ExopackageArgsHelper]{.typeNameLink}](ExopackageArgsHelper.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[FilterResourcesSteps]{.typeNameLink}](FilterResourcesSteps.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[FilterResourcesSteps.Builder]{.typeNameLink}](FilterResourcesSteps.Builder.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[FilterResourcesSteps.DefaultDrawableFinder]{.typeNameLink}](FilterResourcesSteps.DefaultDrawableFinder.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.android.[FilterResourcesSteps.DrawableFinder](FilterResourcesSteps.DrawableFinder.html "interface in com.facebook.buck.android"))
    -   com.facebook.buck.android.[[FilterResourcesSteps.ResourceFilter]{.typeNameLink}](FilterResourcesSteps.ResourceFilter.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"))
    -   com.facebook.buck.android.[[GenAidlDescription]{.typeNameLink}](GenAidlDescription.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>)
    -   com.facebook.buck.android.[[GenAidlDescriptionArg]{.typeNameLink}](GenAidlDescriptionArg.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[GenAidlDescriptionArg.Builder]{.typeNameLink}](GenAidlDescriptionArg.Builder.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[GenerateBuildConfigStep]{.typeNameLink}](GenerateBuildConfigStep.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.step.[Step](../step/Step.html "interface in com.facebook.buck.step"))
    -   com.facebook.buck.android.[[GenerateManifestStep]{.typeNameLink}](GenerateManifestStep.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.step.[Step](../step/Step.html "interface in com.facebook.buck.step"))
    -   com.facebook.buck.android.[[GetStringsFilesStep]{.typeNameLink}](GetStringsFilesStep.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.step.[Step](../step/Step.html "interface in com.facebook.buck.step"))
    -   com.facebook.buck.android.[[HasInstallableApk.ApkInfo]{.typeNameLink}](HasInstallableApk.ApkInfo.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[IdentityResourcesProvider]{.typeNameLink}](IdentityResourcesProvider.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.android.[FilteredResourcesProvider](FilteredResourcesProvider.html "interface in com.facebook.buck.android"))
    -   com.facebook.buck.android.[[IntraDexReorderStep]{.typeNameLink}](IntraDexReorderStep.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.step.[Step](../step/Step.html "interface in com.facebook.buck.step"))
    -   com.facebook.buck.android.[[KeystoreProperties]{.typeNameLink}](KeystoreProperties.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[MergeAndroidResourcesStep]{.typeNameLink}](MergeAndroidResourcesStep.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.step.[Step](../step/Step.html "interface in com.facebook.buck.step"))
    -   com.facebook.buck.android.[[ModuleInfo]{.typeNameLink}](ModuleInfo.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[NativeFilesInfo]{.typeNameLink}](NativeFilesInfo.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"))
    -   com.facebook.buck.android.[[NdkLibraryDescription]{.typeNameLink}](NdkLibraryDescription.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>)
    -   com.facebook.buck.android.[[NdkLibraryDescriptionArg]{.typeNameLink}](NdkLibraryDescriptionArg.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[NdkLibraryDescriptionArg.Builder]{.typeNameLink}](NdkLibraryDescriptionArg.Builder.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[NdkToolchainDescription]{.typeNameLink}](NdkToolchainDescription.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>)
    -   com.facebook.buck.android.[[NdkToolchainDescriptionArg]{.typeNameLink}](NdkToolchainDescriptionArg.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[NdkToolchainDescriptionArg.Builder]{.typeNameLink}](NdkToolchainDescriptionArg.Builder.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[NoDxArgsHelper]{.typeNameLink}](NoDxArgsHelper.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[NoopAndroidNativeTargetConfigurationMatcher]{.typeNameLink}](NoopAndroidNativeTargetConfigurationMatcher.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.android.[AndroidNativeTargetConfigurationMatcher](AndroidNativeTargetConfigurationMatcher.html "interface in com.facebook.buck.android"))
    -   com.facebook.buck.android.[[PackagedResource]{.typeNameLink}](PackagedResource.html "class in com.facebook.buck.android")
        (implements java.util.function.Supplier\<T\>)
    -   com.facebook.buck.android.[[PrebuiltNativeLibraryDescription]{.typeNameLink}](PrebuiltNativeLibraryDescription.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>)
    -   com.facebook.buck.android.[[PrebuiltNativeLibraryDescriptionArg]{.typeNameLink}](PrebuiltNativeLibraryDescriptionArg.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[PrebuiltNativeLibraryDescriptionArg.Builder]{.typeNameLink}](PrebuiltNativeLibraryDescriptionArg.Builder.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[PreDexedFilesSorter]{.typeNameLink}](PreDexedFilesSorter.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[PreDexedFilesSorter.DexStoreContents]{.typeNameLink}](PreDexedFilesSorter.DexStoreContents.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[PreDexedFilesSorter.Result]{.typeNameLink}](PreDexedFilesSorter.Result.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[ProGuardConfig]{.typeNameLink}](ProGuardConfig.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[ProguardMapping]{.typeNameLink}](ProguardMapping.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[RedexArgsHelper]{.typeNameLink}](RedexArgsHelper.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[ReplaceManifestPlaceholdersStep]{.typeNameLink}](ReplaceManifestPlaceholdersStep.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.step.[Step](../step/Step.html "interface in com.facebook.buck.step"))
    -   com.facebook.buck.android.[[ResourceFilesInfo]{.typeNameLink}](ResourceFilesInfo.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"))
    -   com.facebook.buck.android.[[ResourceFilters]{.typeNameLink}](ResourceFilters.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[ResourceFilters.Qualifiers]{.typeNameLink}](ResourceFilters.Qualifiers.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[ResourcesFilter.BuildOutput]{.typeNameLink}](ResourcesFilter.BuildOutput.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[RobolectricTestDescription]{.typeNameLink}](RobolectricTestDescription.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>)
    -   com.facebook.buck.android.[[RobolectricTestDescriptionArg]{.typeNameLink}](RobolectricTestDescriptionArg.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[RobolectricTestDescriptionArg.Builder]{.typeNameLink}](RobolectricTestDescriptionArg.Builder.html "class in com.facebook.buck.android")
    -   com.facebook.buck.shell.[[ShellStep]{.typeNameLink}](../shell/ShellStep.html "class in com.facebook.buck.shell")
        (implements
        com.facebook.buck.step.[Step](../step/Step.html "interface in com.facebook.buck.step"))
        -   com.facebook.buck.android.[[AaptStep]{.typeNameLink}](AaptStep.html "class in com.facebook.buck.android")
        -   com.facebook.buck.android.[[AidlStep]{.typeNameLink}](AidlStep.html "class in com.facebook.buck.android")
        -   com.facebook.buck.android.[[DxStep]{.typeNameLink}](DxStep.html "class in com.facebook.buck.android")
        -   com.facebook.buck.android.[[InstrumentationStep]{.typeNameLink}](InstrumentationStep.html "class in com.facebook.buck.android")
        -   com.facebook.buck.android.[[NdkBuildStep]{.typeNameLink}](NdkBuildStep.html "class in com.facebook.buck.android")
        -   com.facebook.buck.android.[[ProGuardObfuscateStep]{.typeNameLink}](ProGuardObfuscateStep.html "class in com.facebook.buck.android")
        -   com.facebook.buck.android.[[StripStep]{.typeNameLink}](StripStep.html "class in com.facebook.buck.android")
        -   com.facebook.buck.android.[[ZipalignStep]{.typeNameLink}](ZipalignStep.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[SmartDexingStep]{.typeNameLink}](SmartDexingStep.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.step.[Step](../step/Step.html "interface in com.facebook.buck.step"))
    -   com.facebook.buck.android.[[SplitZipStep]{.typeNameLink}](SplitZipStep.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.step.[Step](../step/Step.html "interface in com.facebook.buck.step"))
    -   com.facebook.buck.android.[[StringResources]{.typeNameLink}](StringResources.html "class in com.facebook.buck.android")
    -   java.lang.[[Throwable]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Throwable.html?is-external=true "class or interface in java.lang"){.externalLink}
        (implements
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   java.lang.[[Exception]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Exception.html?is-external=true "class or interface in java.lang"){.externalLink}
            -   java.io.[[IOException]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/io/IOException.html?is-external=true "class or interface in java.io"){.externalLink}
                -   com.facebook.buck.android.[[AdbHelper.CommandFailedException]{.typeNameLink}](AdbHelper.CommandFailedException.html "class in com.facebook.buck.android")
            -   com.facebook.buck.android.[[MergeAndroidResourcesStep.DuplicateResourceException]{.typeNameLink}](MergeAndroidResourcesStep.DuplicateResourceException.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[UnsortedAndroidResourceDeps]{.typeNameLink}](UnsortedAndroidResourceDeps.html "class in com.facebook.buck.android")
    -   com.facebook.buck.android.[[WriteAppModuleMetadataStep]{.typeNameLink}](WriteAppModuleMetadataStep.html "class in com.facebook.buck.android")
        (implements
        com.facebook.buck.step.[Step](../step/Step.html "interface in com.facebook.buck.step"))
:::

::: {.section role="region"}
## Interface Hierarchy {#interface-hierarchy title="Interface Hierarchy"}

-   com.facebook.buck.android.[[AndroidLibraryCompilerFactory]{.typeNameLink}](AndroidLibraryCompilerFactory.html "interface in com.facebook.buck.android")
-   com.facebook.buck.android.[[AndroidLinkableMetadata]{.typeNameLink}](AndroidLinkableMetadata.html "interface in com.facebook.buck.android")
-   com.facebook.buck.android.[[AndroidManifestReader]{.typeNameLink}](AndroidManifestReader.html "interface in com.facebook.buck.android")
-   com.facebook.buck.android.[[AndroidNativeTargetConfigurationMatcher]{.typeNameLink}](AndroidNativeTargetConfigurationMatcher.html "interface in com.facebook.buck.android")
-   com.facebook.buck.core.description.arg.[[DataTransferObject]{.typeNameLink}](../core/description/arg/DataTransferObject.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.core.description.arg.[[ConstructorArg]{.typeNameLink}](../core/description/arg/ConstructorArg.html "interface in com.facebook.buck.core.description.arg")
        -   com.facebook.buck.core.description.arg.[[BuildRuleArg]{.typeNameLink}](../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")
            -   com.facebook.buck.jvm.java.[[JvmLibraryArg]{.typeNameLink}](../jvm/java/JvmLibraryArg.html "interface in com.facebook.buck.jvm.java")
                (also extends
                com.facebook.buck.jvm.java.[MaybeRequiredForSourceOnlyAbiArg](../jvm/java/MaybeRequiredForSourceOnlyAbiArg.html "interface in com.facebook.buck.jvm.java"))
                -   com.facebook.buck.jvm.java.[[JavaLibraryDescription.CoreArg]{.typeNameLink}](../jvm/java/JavaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.java")
                    (also extends
                    com.facebook.buck.core.description.arg.[HasDeclaredDeps](../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg"),
                    com.facebook.buck.core.description.arg.[HasProvidedDeps](../core/description/arg/HasProvidedDeps.html "interface in com.facebook.buck.core.description.arg"),
                    com.facebook.buck.core.description.arg.[HasSrcs](../core/description/arg/HasSrcs.html "interface in com.facebook.buck.core.description.arg"),
                    com.facebook.buck.core.description.arg.[HasTests](../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg"))
                    -   com.facebook.buck.android.[[AndroidLibraryDescription.CoreArg]{.typeNameLink}](AndroidLibraryDescription.CoreArg.html "interface in com.facebook.buck.android")
                        (also extends
                        com.facebook.buck.android.[AndroidKotlinCoreArg](AndroidKotlinCoreArg.html "interface in com.facebook.buck.android"),
                        com.facebook.buck.core.description.arg.[HasDepsQuery](../core/description/arg/HasDepsQuery.html "interface in com.facebook.buck.core.description.arg"),
                        com.facebook.buck.core.description.arg.[HasProvidedDepsQuery](../core/description/arg/HasProvidedDepsQuery.html "interface in com.facebook.buck.core.description.arg"))
                    -   com.facebook.buck.jvm.kotlin.[[KotlinLibraryDescription.CoreArg]{.typeNameLink}](../jvm/kotlin/KotlinLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.kotlin")
                        -   com.facebook.buck.android.[[AndroidKotlinCoreArg]{.typeNameLink}](AndroidKotlinCoreArg.html "interface in com.facebook.buck.android")
                            -   com.facebook.buck.android.[[AndroidLibraryDescription.CoreArg]{.typeNameLink}](AndroidLibraryDescription.CoreArg.html "interface in com.facebook.buck.android")
                                (also extends
                                com.facebook.buck.core.description.arg.[HasDepsQuery](../core/description/arg/HasDepsQuery.html "interface in com.facebook.buck.core.description.arg"),
                                com.facebook.buck.core.description.arg.[HasProvidedDepsQuery](../core/description/arg/HasProvidedDepsQuery.html "interface in com.facebook.buck.core.description.arg"),
                                com.facebook.buck.jvm.java.[JavaLibraryDescription.CoreArg](../jvm/java/JavaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.java"))
-   com.facebook.buck.android.[[DexWithClasses]{.typeNameLink}](DexWithClasses.html "interface in com.facebook.buck.android")
-   com.facebook.buck.android.[[FilteredResourcesProvider]{.typeNameLink}](FilteredResourcesProvider.html "interface in com.facebook.buck.android")
-   com.facebook.buck.android.[[FilterResourcesSteps.DrawableFinder]{.typeNameLink}](FilterResourcesSteps.DrawableFinder.html "interface in com.facebook.buck.android")
-   com.facebook.buck.android.[[FilterResourcesSteps.ImageScaler]{.typeNameLink}](FilterResourcesSteps.ImageScaler.html "interface in com.facebook.buck.android")
-   com.facebook.buck.android.[[HasAndroidResourceDeps]{.typeNameLink}](HasAndroidResourceDeps.html "interface in com.facebook.buck.android")
-   com.facebook.buck.core.description.arg.[[HasApplicationModuleBlacklist]{.typeNameLink}](../core/description/arg/HasApplicationModuleBlacklist.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.android.[[AndroidGraphEnhancerArgs]{.typeNameLink}](AndroidGraphEnhancerArgs.html "interface in com.facebook.buck.android")
        (also extends
        com.facebook.buck.android.[HasDuplicateAndroidResourceTypes](HasDuplicateAndroidResourceTypes.html "interface in com.facebook.buck.android"))
-   com.facebook.buck.core.description.arg.[[HasDeclaredDeps]{.typeNameLink}](../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.core.description.arg.[[HasDepsQuery]{.typeNameLink}](../core/description/arg/HasDepsQuery.html "interface in com.facebook.buck.core.description.arg")
        -   com.facebook.buck.android.[[AndroidLibraryDescription.CoreArg]{.typeNameLink}](AndroidLibraryDescription.CoreArg.html "interface in com.facebook.buck.android")
            (also extends
            com.facebook.buck.android.[AndroidKotlinCoreArg](AndroidKotlinCoreArg.html "interface in com.facebook.buck.android"),
            com.facebook.buck.core.description.arg.[HasProvidedDepsQuery](../core/description/arg/HasProvidedDepsQuery.html "interface in com.facebook.buck.core.description.arg"),
            com.facebook.buck.jvm.java.[JavaLibraryDescription.CoreArg](../jvm/java/JavaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.java"))
    -   com.facebook.buck.jvm.java.[[JavaLibraryDescription.CoreArg]{.typeNameLink}](../jvm/java/JavaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.java")
        (also extends
        com.facebook.buck.core.description.arg.[HasProvidedDeps](../core/description/arg/HasProvidedDeps.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasSrcs](../core/description/arg/HasSrcs.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasTests](../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.jvm.java.[JvmLibraryArg](../jvm/java/JvmLibraryArg.html "interface in com.facebook.buck.jvm.java"))
        -   com.facebook.buck.android.[[AndroidLibraryDescription.CoreArg]{.typeNameLink}](AndroidLibraryDescription.CoreArg.html "interface in com.facebook.buck.android")
            (also extends
            com.facebook.buck.android.[AndroidKotlinCoreArg](AndroidKotlinCoreArg.html "interface in com.facebook.buck.android"),
            com.facebook.buck.core.description.arg.[HasDepsQuery](../core/description/arg/HasDepsQuery.html "interface in com.facebook.buck.core.description.arg"),
            com.facebook.buck.core.description.arg.[HasProvidedDepsQuery](../core/description/arg/HasProvidedDepsQuery.html "interface in com.facebook.buck.core.description.arg"))
        -   com.facebook.buck.jvm.kotlin.[[KotlinLibraryDescription.CoreArg]{.typeNameLink}](../jvm/kotlin/KotlinLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.kotlin")
            -   com.facebook.buck.android.[[AndroidKotlinCoreArg]{.typeNameLink}](AndroidKotlinCoreArg.html "interface in com.facebook.buck.android")
                -   com.facebook.buck.android.[[AndroidLibraryDescription.CoreArg]{.typeNameLink}](AndroidLibraryDescription.CoreArg.html "interface in com.facebook.buck.android")
                    (also extends
                    com.facebook.buck.core.description.arg.[HasDepsQuery](../core/description/arg/HasDepsQuery.html "interface in com.facebook.buck.core.description.arg"),
                    com.facebook.buck.core.description.arg.[HasProvidedDepsQuery](../core/description/arg/HasProvidedDepsQuery.html "interface in com.facebook.buck.core.description.arg"),
                    com.facebook.buck.jvm.java.[JavaLibraryDescription.CoreArg](../jvm/java/JavaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.java"))
-   com.facebook.buck.android.[[HasDexFiles]{.typeNameLink}](HasDexFiles.html "interface in com.facebook.buck.android")
-   com.facebook.buck.android.[[HasDuplicateAndroidResourceTypes]{.typeNameLink}](HasDuplicateAndroidResourceTypes.html "interface in com.facebook.buck.android")
    -   com.facebook.buck.android.[[AndroidGraphEnhancerArgs]{.typeNameLink}](AndroidGraphEnhancerArgs.html "interface in com.facebook.buck.android")
        (also extends
        com.facebook.buck.core.description.arg.[HasApplicationModuleBlacklist](../core/description/arg/HasApplicationModuleBlacklist.html "interface in com.facebook.buck.core.description.arg"))
-   com.facebook.buck.android.[[HasExopackageArgs]{.typeNameLink}](HasExopackageArgs.html "interface in com.facebook.buck.android")
-   com.facebook.buck.android.[[HasInstallableApk]{.typeNameLink}](HasInstallableApk.html "interface in com.facebook.buck.android")
-   com.facebook.buck.core.description.arg.[[HasProvidedDeps]{.typeNameLink}](../core/description/arg/HasProvidedDeps.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.core.description.arg.[[HasProvidedDepsQuery]{.typeNameLink}](../core/description/arg/HasProvidedDepsQuery.html "interface in com.facebook.buck.core.description.arg")
        -   com.facebook.buck.android.[[AndroidLibraryDescription.CoreArg]{.typeNameLink}](AndroidLibraryDescription.CoreArg.html "interface in com.facebook.buck.android")
            (also extends
            com.facebook.buck.android.[AndroidKotlinCoreArg](AndroidKotlinCoreArg.html "interface in com.facebook.buck.android"),
            com.facebook.buck.core.description.arg.[HasDepsQuery](../core/description/arg/HasDepsQuery.html "interface in com.facebook.buck.core.description.arg"),
            com.facebook.buck.jvm.java.[JavaLibraryDescription.CoreArg](../jvm/java/JavaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.java"))
    -   com.facebook.buck.jvm.java.[[JavaLibraryDescription.CoreArg]{.typeNameLink}](../jvm/java/JavaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.java")
        (also extends
        com.facebook.buck.core.description.arg.[HasDeclaredDeps](../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasSrcs](../core/description/arg/HasSrcs.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasTests](../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.jvm.java.[JvmLibraryArg](../jvm/java/JvmLibraryArg.html "interface in com.facebook.buck.jvm.java"))
        -   com.facebook.buck.android.[[AndroidLibraryDescription.CoreArg]{.typeNameLink}](AndroidLibraryDescription.CoreArg.html "interface in com.facebook.buck.android")
            (also extends
            com.facebook.buck.android.[AndroidKotlinCoreArg](AndroidKotlinCoreArg.html "interface in com.facebook.buck.android"),
            com.facebook.buck.core.description.arg.[HasDepsQuery](../core/description/arg/HasDepsQuery.html "interface in com.facebook.buck.core.description.arg"),
            com.facebook.buck.core.description.arg.[HasProvidedDepsQuery](../core/description/arg/HasProvidedDepsQuery.html "interface in com.facebook.buck.core.description.arg"))
        -   com.facebook.buck.jvm.kotlin.[[KotlinLibraryDescription.CoreArg]{.typeNameLink}](../jvm/kotlin/KotlinLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.kotlin")
            -   com.facebook.buck.android.[[AndroidKotlinCoreArg]{.typeNameLink}](AndroidKotlinCoreArg.html "interface in com.facebook.buck.android")
                -   com.facebook.buck.android.[[AndroidLibraryDescription.CoreArg]{.typeNameLink}](AndroidLibraryDescription.CoreArg.html "interface in com.facebook.buck.android")
                    (also extends
                    com.facebook.buck.core.description.arg.[HasDepsQuery](../core/description/arg/HasDepsQuery.html "interface in com.facebook.buck.core.description.arg"),
                    com.facebook.buck.core.description.arg.[HasProvidedDepsQuery](../core/description/arg/HasProvidedDepsQuery.html "interface in com.facebook.buck.core.description.arg"),
                    com.facebook.buck.jvm.java.[JavaLibraryDescription.CoreArg](../jvm/java/JavaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.java"))
-   com.facebook.buck.core.description.arg.[[HasSrcs]{.typeNameLink}](../core/description/arg/HasSrcs.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.jvm.java.[[JavaLibraryDescription.CoreArg]{.typeNameLink}](../jvm/java/JavaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.java")
        (also extends
        com.facebook.buck.core.description.arg.[HasDeclaredDeps](../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasProvidedDeps](../core/description/arg/HasProvidedDeps.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasTests](../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.jvm.java.[JvmLibraryArg](../jvm/java/JvmLibraryArg.html "interface in com.facebook.buck.jvm.java"))
        -   com.facebook.buck.android.[[AndroidLibraryDescription.CoreArg]{.typeNameLink}](AndroidLibraryDescription.CoreArg.html "interface in com.facebook.buck.android")
            (also extends
            com.facebook.buck.android.[AndroidKotlinCoreArg](AndroidKotlinCoreArg.html "interface in com.facebook.buck.android"),
            com.facebook.buck.core.description.arg.[HasDepsQuery](../core/description/arg/HasDepsQuery.html "interface in com.facebook.buck.core.description.arg"),
            com.facebook.buck.core.description.arg.[HasProvidedDepsQuery](../core/description/arg/HasProvidedDepsQuery.html "interface in com.facebook.buck.core.description.arg"))
        -   com.facebook.buck.jvm.kotlin.[[KotlinLibraryDescription.CoreArg]{.typeNameLink}](../jvm/kotlin/KotlinLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.kotlin")
            -   com.facebook.buck.android.[[AndroidKotlinCoreArg]{.typeNameLink}](AndroidKotlinCoreArg.html "interface in com.facebook.buck.android")
                -   com.facebook.buck.android.[[AndroidLibraryDescription.CoreArg]{.typeNameLink}](AndroidLibraryDescription.CoreArg.html "interface in com.facebook.buck.android")
                    (also extends
                    com.facebook.buck.core.description.arg.[HasDepsQuery](../core/description/arg/HasDepsQuery.html "interface in com.facebook.buck.core.description.arg"),
                    com.facebook.buck.core.description.arg.[HasProvidedDepsQuery](../core/description/arg/HasProvidedDepsQuery.html "interface in com.facebook.buck.core.description.arg"),
                    com.facebook.buck.jvm.java.[JavaLibraryDescription.CoreArg](../jvm/java/JavaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.java"))
-   com.facebook.buck.core.description.arg.[[HasTests]{.typeNameLink}](../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.jvm.java.[[JavaLibraryDescription.CoreArg]{.typeNameLink}](../jvm/java/JavaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.java")
        (also extends
        com.facebook.buck.core.description.arg.[HasDeclaredDeps](../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasProvidedDeps](../core/description/arg/HasProvidedDeps.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasSrcs](../core/description/arg/HasSrcs.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.jvm.java.[JvmLibraryArg](../jvm/java/JvmLibraryArg.html "interface in com.facebook.buck.jvm.java"))
        -   com.facebook.buck.android.[[AndroidLibraryDescription.CoreArg]{.typeNameLink}](AndroidLibraryDescription.CoreArg.html "interface in com.facebook.buck.android")
            (also extends
            com.facebook.buck.android.[AndroidKotlinCoreArg](AndroidKotlinCoreArg.html "interface in com.facebook.buck.android"),
            com.facebook.buck.core.description.arg.[HasDepsQuery](../core/description/arg/HasDepsQuery.html "interface in com.facebook.buck.core.description.arg"),
            com.facebook.buck.core.description.arg.[HasProvidedDepsQuery](../core/description/arg/HasProvidedDepsQuery.html "interface in com.facebook.buck.core.description.arg"))
        -   com.facebook.buck.jvm.kotlin.[[KotlinLibraryDescription.CoreArg]{.typeNameLink}](../jvm/kotlin/KotlinLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.kotlin")
            -   com.facebook.buck.android.[[AndroidKotlinCoreArg]{.typeNameLink}](AndroidKotlinCoreArg.html "interface in com.facebook.buck.android")
                -   com.facebook.buck.android.[[AndroidLibraryDescription.CoreArg]{.typeNameLink}](AndroidLibraryDescription.CoreArg.html "interface in com.facebook.buck.android")
                    (also extends
                    com.facebook.buck.core.description.arg.[HasDepsQuery](../core/description/arg/HasDepsQuery.html "interface in com.facebook.buck.core.description.arg"),
                    com.facebook.buck.core.description.arg.[HasProvidedDepsQuery](../core/description/arg/HasProvidedDepsQuery.html "interface in com.facebook.buck.core.description.arg"),
                    com.facebook.buck.jvm.java.[JavaLibraryDescription.CoreArg](../jvm/java/JavaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.java"))
-   com.facebook.buck.jvm.java.[[MaybeRequiredForSourceOnlyAbiArg]{.typeNameLink}](../jvm/java/MaybeRequiredForSourceOnlyAbiArg.html "interface in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[JvmLibraryArg]{.typeNameLink}](../jvm/java/JvmLibraryArg.html "interface in com.facebook.buck.jvm.java")
        (also extends
        com.facebook.buck.core.description.arg.[BuildRuleArg](../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg"))
        -   com.facebook.buck.jvm.java.[[JavaLibraryDescription.CoreArg]{.typeNameLink}](../jvm/java/JavaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.java")
            (also extends
            com.facebook.buck.core.description.arg.[HasDeclaredDeps](../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg"),
            com.facebook.buck.core.description.arg.[HasProvidedDeps](../core/description/arg/HasProvidedDeps.html "interface in com.facebook.buck.core.description.arg"),
            com.facebook.buck.core.description.arg.[HasSrcs](../core/description/arg/HasSrcs.html "interface in com.facebook.buck.core.description.arg"),
            com.facebook.buck.core.description.arg.[HasTests](../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg"))
            -   com.facebook.buck.android.[[AndroidLibraryDescription.CoreArg]{.typeNameLink}](AndroidLibraryDescription.CoreArg.html "interface in com.facebook.buck.android")
                (also extends
                com.facebook.buck.android.[AndroidKotlinCoreArg](AndroidKotlinCoreArg.html "interface in com.facebook.buck.android"),
                com.facebook.buck.core.description.arg.[HasDepsQuery](../core/description/arg/HasDepsQuery.html "interface in com.facebook.buck.core.description.arg"),
                com.facebook.buck.core.description.arg.[HasProvidedDepsQuery](../core/description/arg/HasProvidedDepsQuery.html "interface in com.facebook.buck.core.description.arg"))
            -   com.facebook.buck.jvm.kotlin.[[KotlinLibraryDescription.CoreArg]{.typeNameLink}](../jvm/kotlin/KotlinLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.kotlin")
                -   com.facebook.buck.android.[[AndroidKotlinCoreArg]{.typeNameLink}](AndroidKotlinCoreArg.html "interface in com.facebook.buck.android")
                    -   com.facebook.buck.android.[[AndroidLibraryDescription.CoreArg]{.typeNameLink}](AndroidLibraryDescription.CoreArg.html "interface in com.facebook.buck.android")
                        (also extends
                        com.facebook.buck.core.description.arg.[HasDepsQuery](../core/description/arg/HasDepsQuery.html "interface in com.facebook.buck.core.description.arg"),
                        com.facebook.buck.core.description.arg.[HasProvidedDepsQuery](../core/description/arg/HasProvidedDepsQuery.html "interface in com.facebook.buck.core.description.arg"),
                        com.facebook.buck.jvm.java.[JavaLibraryDescription.CoreArg](../jvm/java/JavaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.java"))
-   com.facebook.buck.android.[[NativeLibraryBuildRule]{.typeNameLink}](NativeLibraryBuildRule.html "interface in com.facebook.buck.android")
-   com.facebook.buck.android.[[SmartDexingStep.DexInputHashesProvider]{.typeNameLink}](SmartDexingStep.DexInputHashesProvider.html "interface in com.facebook.buck.android")
-   com.facebook.buck.android.[[UnsortedAndroidResourceDeps.Callback]{.typeNameLink}](UnsortedAndroidResourceDeps.Callback.html "interface in com.facebook.buck.android")
:::

::: {.section role="region"}
## Enum Hierarchy {#enum-hierarchy title="Enum Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   java.lang.[[Enum]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<E\>
        (implements
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   com.facebook.buck.android.[[AndroidBuckConfig.NdkSearchOrderEntry]{.typeNameLink}](AndroidBuckConfig.NdkSearchOrderEntry.html "enum in com.facebook.buck.android")
        -   com.facebook.buck.android.[[AndroidInstallConfig.ConcurrentInstall]{.typeNameLink}](AndroidInstallConfig.ConcurrentInstall.html "enum in com.facebook.buck.android")
            (implements
            com.facebook.buck.util.randomizedtrial.[WithProbability](../util/randomizedtrial/WithProbability.html "interface in com.facebook.buck.util.randomizedtrial"))
        -   com.facebook.buck.android.[[AndroidLibraryDescription.JvmLanguage]{.typeNameLink}](AndroidLibraryDescription.JvmLanguage.html "enum in com.facebook.buck.android")
        -   com.facebook.buck.android.[[BinaryType]{.typeNameLink}](BinaryType.html "enum in com.facebook.buck.android")
        -   com.facebook.buck.android.[[CompressionAlgorithm]{.typeNameLink}](CompressionAlgorithm.html "enum in com.facebook.buck.android")
        -   com.facebook.buck.android.[[DxStep.Option]{.typeNameLink}](DxStep.Option.html "enum in com.facebook.buck.android")
        -   com.facebook.buck.android.[[HasDuplicateAndroidResourceTypes.DuplicateResourceBehaviour]{.typeNameLink}](HasDuplicateAndroidResourceTypes.DuplicateResourceBehaviour.html "enum in com.facebook.buck.android")
        -   com.facebook.buck.android.[[ResourceFilters.Density]{.typeNameLink}](ResourceFilters.Density.html "enum in com.facebook.buck.android")
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
-   Tree
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

[]{#skip.navbar.bottom}
:::
