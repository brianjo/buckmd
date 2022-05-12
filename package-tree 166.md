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
# Hierarchy For Package com.facebook.buck.apple {#hierarchy-for-package-com.facebook.buck.apple .title}

[Package Hierarchies:]{.packageHierarchyLabel}

-   [All Packages](../../../../overview-tree.html)
:::

::: contentContainer
::: {.section role="region"}
## Class Hierarchy {#class-hierarchy title="Class Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   com.facebook.buck.core.rules.impl.[[AbstractBuildRule]{.typeNameLink}](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")
        (implements
        com.facebook.buck.core.rules.[BuildRule](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules"))
        -   com.facebook.buck.core.rules.impl.[[AbstractBuildRuleWithDeclaredAndExtraDeps]{.typeNameLink}](../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")
            (implements
            com.facebook.buck.core.rules.attr.[HasDeclaredAndExtraDeps](../core/rules/attr/HasDeclaredAndExtraDeps.html "interface in com.facebook.buck.core.rules.attr"))
            -   com.facebook.buck.apple.[[AppleTest]{.typeNameLink}](AppleTest.html "class in com.facebook.buck.apple")
                (implements
                com.facebook.buck.core.test.rule.[ExternalTestRunnerRule](../core/test/rule/ExternalTestRunnerRule.html "interface in com.facebook.buck.core.test.rule"),
                com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"),
                com.facebook.buck.core.test.rule.[TestRule](../core/test/rule/TestRule.html "interface in com.facebook.buck.core.test.rule"))
            -   com.facebook.buck.apple.[[AppleTestAggregatedDependencies]{.typeNameLink}](AppleTestAggregatedDependencies.html "class in com.facebook.buck.apple")
            -   com.facebook.buck.apple.[[AppleTestX]{.typeNameLink}](AppleTestX.html "class in com.facebook.buck.apple")
                (implements
                com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"),
                com.facebook.buck.core.test.rule.[TestXRule](../core/test/rule/TestXRule.html "interface in com.facebook.buck.core.test.rule"))
            -   com.facebook.buck.apple.[[BuiltinApplePackage]{.typeNameLink}](BuiltinApplePackage.html "class in com.facebook.buck.apple")
            -   com.facebook.buck.apple.[[CoreDataModel]{.typeNameLink}](CoreDataModel.html "class in com.facebook.buck.apple")
            -   com.facebook.buck.apple.[[MultiarchFile]{.typeNameLink}](MultiarchFile.html "class in com.facebook.buck.apple")
                (implements
                com.facebook.buck.cxx.[HasAppleDebugSymbolDeps](../cxx/HasAppleDebugSymbolDeps.html "interface in com.facebook.buck.cxx"))
            -   com.facebook.buck.apple.[[PrebuiltAppleFramework]{.typeNameLink}](PrebuiltAppleFramework.html "class in com.facebook.buck.apple")
                (implements
                com.facebook.buck.cxx.[CxxPreprocessorDep](../cxx/CxxPreprocessorDep.html "interface in com.facebook.buck.cxx"),
                com.facebook.buck.core.model.[HasOutputName](../core/model/HasOutputName.html "interface in com.facebook.buck.core.model"),
                com.facebook.buck.cxx.toolchain.nativelink.[LegacyNativeLinkableGroup](../cxx/toolchain/nativelink/LegacyNativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink"))
            -   com.facebook.buck.apple.[[SceneKitAssets]{.typeNameLink}](SceneKitAssets.html "class in com.facebook.buck.apple")
        -   com.facebook.buck.apple.[[AppleAssetCatalog]{.typeNameLink}](AppleAssetCatalog.html "class in com.facebook.buck.apple")
        -   com.facebook.buck.apple.[[AppleBundle]{.typeNameLink}](AppleBundle.html "class in com.facebook.buck.apple")
            (implements
            com.facebook.buck.core.rules.tool.[BinaryBuildRule](../core/rules/tool/BinaryBuildRule.html "interface in com.facebook.buck.core.rules.tool"),
            com.facebook.buck.apple.[BuildRuleWithBinary](BuildRuleWithBinary.html "interface in com.facebook.buck.apple"),
            com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"),
            com.facebook.buck.cxx.[NativeTestable](../cxx/NativeTestable.html "interface in com.facebook.buck.cxx"))
        -   com.facebook.buck.apple.[[AppleDebuggableBinary]{.typeNameLink}](AppleDebuggableBinary.html "class in com.facebook.buck.apple")
            (implements
            com.facebook.buck.apple.[BuildRuleWithBinary](BuildRuleWithBinary.html "interface in com.facebook.buck.apple"),
            com.facebook.buck.core.rules.attr.[HasDeclaredAndExtraDeps](../core/rules/attr/HasDeclaredAndExtraDeps.html "interface in com.facebook.buck.core.rules.attr"),
            com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"))
        -   com.facebook.buck.apple.[[AppleDsym]{.typeNameLink}](AppleDsym.html "class in com.facebook.buck.apple")
            (implements
            com.facebook.buck.core.rules.attr.[HasPostBuildSteps](../core/rules/attr/HasPostBuildSteps.html "interface in com.facebook.buck.core.rules.attr"),
            com.facebook.buck.core.rules.attr.[SupportsInputBasedRuleKey](../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr"))
        -   com.facebook.buck.rules.modern.[[ModernBuildRule]{.typeNameLink}](../rules/modern/ModernBuildRule.html "class in com.facebook.buck.rules.modern")\<T\>
            (implements
            com.facebook.buck.core.rules.attr.[SupportsInputBasedRuleKey](../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr"))
            -   com.facebook.buck.shell.[[BaseGenrule]{.typeNameLink}](../shell/BaseGenrule.html "class in com.facebook.buck.shell")\<T\>
                (implements
                com.facebook.buck.core.rules.attr.[HasMultipleOutputs](../core/rules/attr/HasMultipleOutputs.html "interface in com.facebook.buck.core.rules.attr"),
                com.facebook.buck.core.model.[HasOutputName](../core/model/HasOutputName.html "interface in com.facebook.buck.core.model"))
                -   com.facebook.buck.apple.[[ExternallyBuiltApplePackage]{.typeNameLink}](ExternallyBuiltApplePackage.html "class in com.facebook.buck.apple")
        -   com.facebook.buck.core.rules.impl.[[NoopBuildRule]{.typeNameLink}](../core/rules/impl/NoopBuildRule.html "class in com.facebook.buck.core.rules.impl")
            (implements
            com.facebook.buck.core.rules.attr.[SupportsInputBasedRuleKey](../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr"))
            -   com.facebook.buck.apple.[[AppleToolchainBuildRule]{.typeNameLink}](AppleToolchainBuildRule.html "class in com.facebook.buck.apple")
            -   com.facebook.buck.apple.[[AppleToolchainSetBuildRule]{.typeNameLink}](AppleToolchainSetBuildRule.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[AppleAssetCatalogDescription]{.typeNameLink}](AppleAssetCatalogDescription.html "class in com.facebook.buck.apple")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>)
    -   com.facebook.buck.apple.[[AppleAssetCatalogDescriptionArg]{.typeNameLink}](AppleAssetCatalogDescriptionArg.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[AppleAssetCatalogDescriptionArg.Builder]{.typeNameLink}](AppleAssetCatalogDescriptionArg.Builder.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[AppleAssetCatalogsCompilationOptions]{.typeNameLink}](AppleAssetCatalogsCompilationOptions.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[AppleAssetCatalogsCompilationOptions.Builder]{.typeNameLink}](AppleAssetCatalogsCompilationOptions.Builder.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[AppleBinaryDescription]{.typeNameLink}](AppleBinaryDescription.html "class in com.facebook.buck.apple")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.model.[Flavored](../core/model/Flavored.html "interface in com.facebook.buck.core.model"),
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>,
        com.facebook.buck.core.description.attr.[ImplicitFlavorsInferringDescription](../core/description/attr/ImplicitFlavorsInferringDescription.html "interface in com.facebook.buck.core.description.attr"),
        com.facebook.buck.core.description.metadata.[MetadataProvidingDescription](../core/description/metadata/MetadataProvidingDescription.html "interface in com.facebook.buck.core.description.metadata")\<T\>)
    -   com.facebook.buck.apple.[[AppleBinaryDescriptionArg]{.typeNameLink}](AppleBinaryDescriptionArg.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[AppleBinaryDescriptionArg.Builder]{.typeNameLink}](AppleBinaryDescriptionArg.Builder.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[AppleBuildRules]{.typeNameLink}](AppleBuildRules.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[AppleBundleDescription]{.typeNameLink}](AppleBundleDescription.html "class in com.facebook.buck.apple")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.model.[Flavored](../core/model/Flavored.html "interface in com.facebook.buck.core.model"),
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>,
        com.facebook.buck.core.description.metadata.[MetadataProvidingDescription](../core/description/metadata/MetadataProvidingDescription.html "interface in com.facebook.buck.core.description.metadata")\<T\>)
    -   com.facebook.buck.apple.[[AppleBundleDescriptionArg]{.typeNameLink}](AppleBundleDescriptionArg.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[AppleBundleDescriptionArg.Builder]{.typeNameLink}](AppleBundleDescriptionArg.Builder.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[AppleBundleResources]{.typeNameLink}](AppleBundleResources.html "class in com.facebook.buck.apple")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"))
    -   com.facebook.buck.apple.[[AppleConfig]{.typeNameLink}](AppleConfig.html "class in com.facebook.buck.apple")
        (implements
        com.facebook.buck.core.config.[ConfigView](../core/config/ConfigView.html "interface in com.facebook.buck.core.config")\<T\>)
    -   com.facebook.buck.apple.[[AppleDependenciesCache]{.typeNameLink}](AppleDependenciesCache.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[AppleDescriptionProvider]{.typeNameLink}](AppleDescriptionProvider.html "class in com.facebook.buck.apple")
        (implements
        com.facebook.buck.core.model.targetgraph.[DescriptionProvider](../core/model/targetgraph/DescriptionProvider.html "interface in com.facebook.buck.core.model.targetgraph"))
    -   com.facebook.buck.apple.[[AppleDescriptions]{.typeNameLink}](AppleDescriptions.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[AppleHeaderVisibilities]{.typeNameLink}](AppleHeaderVisibilities.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[AppleInfoPlistParsing]{.typeNameLink}](AppleInfoPlistParsing.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[AppleLibraryDescription]{.typeNameLink}](AppleLibraryDescription.html "class in com.facebook.buck.apple")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.model.[Flavored](../core/model/Flavored.html "interface in com.facebook.buck.core.model"),
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>,
        com.facebook.buck.core.description.attr.[ImplicitFlavorsInferringDescription](../core/description/attr/ImplicitFlavorsInferringDescription.html "interface in com.facebook.buck.core.description.attr"),
        com.facebook.buck.core.description.metadata.[MetadataProvidingDescription](../core/description/metadata/MetadataProvidingDescription.html "interface in com.facebook.buck.core.description.metadata")\<T\>,
        com.facebook.buck.versions.[VersionPropagator](../versions/VersionPropagator.html "interface in com.facebook.buck.versions")\<A\>)
    -   com.facebook.buck.apple.[[AppleLibraryDescriptionArg]{.typeNameLink}](AppleLibraryDescriptionArg.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[AppleLibraryDescriptionArg.Builder]{.typeNameLink}](AppleLibraryDescriptionArg.Builder.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[AppleLibraryDescriptionSwiftEnhancer]{.typeNameLink}](AppleLibraryDescriptionSwiftEnhancer.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[AppleLibrarySwiftMetadata]{.typeNameLink}](AppleLibrarySwiftMetadata.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[ApplePackageDescription]{.typeNameLink}](ApplePackageDescription.html "class in com.facebook.buck.apple")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.model.[Flavored](../core/model/Flavored.html "interface in com.facebook.buck.core.model"),
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>)
    -   com.facebook.buck.apple.[[ApplePackageDescriptionArg]{.typeNameLink}](ApplePackageDescriptionArg.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[ApplePackageDescriptionArg.Builder]{.typeNameLink}](ApplePackageDescriptionArg.Builder.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[ApplePlatforms]{.typeNameLink}](ApplePlatforms.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[AppleResourceDescription]{.typeNameLink}](AppleResourceDescription.html "class in com.facebook.buck.apple")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.model.[Flavored](../core/model/Flavored.html "interface in com.facebook.buck.core.model"),
        com.facebook.buck.apple.[HasAppleBundleResourcesDescription](HasAppleBundleResourcesDescription.html "interface in com.facebook.buck.apple")\<T\>)
    -   com.facebook.buck.apple.[[AppleResourceDescriptionArg]{.typeNameLink}](AppleResourceDescriptionArg.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[AppleResourceDescriptionArg.Builder]{.typeNameLink}](AppleResourceDescriptionArg.Builder.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[AppleResourceProcessing]{.typeNameLink}](AppleResourceProcessing.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[AppleResources]{.typeNameLink}](AppleResources.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[AppleTestDescription]{.typeNameLink}](AppleTestDescription.html "class in com.facebook.buck.apple")
        (implements
        com.facebook.buck.apple.[AppleLibrarySwiftDelegate](AppleLibrarySwiftDelegate.html "interface in com.facebook.buck.apple"),
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.model.[Flavored](../core/model/Flavored.html "interface in com.facebook.buck.core.model"),
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>,
        com.facebook.buck.core.description.metadata.[MetadataProvidingDescription](../core/description/metadata/MetadataProvidingDescription.html "interface in com.facebook.buck.core.description.metadata")\<T\>)
    -   com.facebook.buck.apple.[[AppleTestDescriptionArg]{.typeNameLink}](AppleTestDescriptionArg.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[AppleTestDescriptionArg.Builder]{.typeNameLink}](AppleTestDescriptionArg.Builder.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[AppleToolchainDescription]{.typeNameLink}](AppleToolchainDescription.html "class in com.facebook.buck.apple")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>)
    -   com.facebook.buck.apple.[[AppleToolchainDescriptionArg]{.typeNameLink}](AppleToolchainDescriptionArg.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[AppleToolchainDescriptionArg.Builder]{.typeNameLink}](AppleToolchainDescriptionArg.Builder.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[AppleToolchainSetDescription]{.typeNameLink}](AppleToolchainSetDescription.html "class in com.facebook.buck.apple")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>)
    -   com.facebook.buck.apple.[[AppleToolchainSetDescriptionArg]{.typeNameLink}](AppleToolchainSetDescriptionArg.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[AppleToolchainSetDescriptionArg.Builder]{.typeNameLink}](AppleToolchainSetDescriptionArg.Builder.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[AppleWrapperResourceArg]{.typeNameLink}](AppleWrapperResourceArg.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[AppleWrapperResourceArg.Builder]{.typeNameLink}](AppleWrapperResourceArg.Builder.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[AppleXCodeDescriptionClassSupplier]{.typeNameLink}](AppleXCodeDescriptionClassSupplier.html "class in com.facebook.buck.apple")
        (implements
        com.facebook.buck.apple.[XCodeDescriptionClassSupplier](XCodeDescriptionClassSupplier.html "interface in com.facebook.buck.apple"))
    -   com.facebook.buck.apple.[[CoreDataModelDescription]{.typeNameLink}](CoreDataModelDescription.html "class in com.facebook.buck.apple")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.model.[Flavored](../core/model/Flavored.html "interface in com.facebook.buck.core.model"))
    -   com.facebook.buck.apple.[[Flavors]{.typeNameLink}](Flavors.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[GroupedSource]{.typeNameLink}](GroupedSource.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[IdbOutputParsing]{.typeNameLink}](IdbOutputParsing.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[IdbRunTestsStep]{.typeNameLink}](IdbRunTestsStep.html "class in com.facebook.buck.apple")
        (implements
        com.facebook.buck.step.[Step](../step/Step.html "interface in com.facebook.buck.step"))
    -   com.facebook.buck.apple.ImmutableAppleBundleResources.Builder
        -   com.facebook.buck.apple.[[AppleBundleResources.Builder]{.typeNameLink}](AppleBundleResources.Builder.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[InfoPlistSubstitution]{.typeNameLink}](InfoPlistSubstitution.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[MultiarchFileInfos]{.typeNameLink}](MultiarchFileInfos.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[PrebuiltAppleFrameworkDescription]{.typeNameLink}](PrebuiltAppleFrameworkDescription.html "class in com.facebook.buck.apple")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.model.[Flavored](../core/model/Flavored.html "interface in com.facebook.buck.core.model"),
        com.facebook.buck.core.description.metadata.[MetadataProvidingDescription](../core/description/metadata/MetadataProvidingDescription.html "interface in com.facebook.buck.core.description.metadata")\<T\>)
    -   com.facebook.buck.apple.[[PrebuiltAppleFrameworkDescriptionArg]{.typeNameLink}](PrebuiltAppleFrameworkDescriptionArg.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[PrebuiltAppleFrameworkDescriptionArg.Builder]{.typeNameLink}](PrebuiltAppleFrameworkDescriptionArg.Builder.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[RuleUtils]{.typeNameLink}](RuleUtils.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[SceneKitAssetsDescription]{.typeNameLink}](SceneKitAssetsDescription.html "class in com.facebook.buck.apple")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.model.[Flavored](../core/model/Flavored.html "interface in com.facebook.buck.core.model"))
    -   com.facebook.buck.shell.[[ShellStep]{.typeNameLink}](../shell/ShellStep.html "class in com.facebook.buck.shell")
        (implements
        com.facebook.buck.step.[Step](../step/Step.html "interface in com.facebook.buck.step"))
        -   com.facebook.buck.apple.[[LibtoolStep]{.typeNameLink}](LibtoolStep.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[SourcePathWithAppleBundleDestination]{.typeNameLink}](SourcePathWithAppleBundleDestination.html "class in com.facebook.buck.apple")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"),
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>)
    -   com.facebook.buck.apple.[[TestCaseSummariesBuildingIdb]{.typeNameLink}](TestCaseSummariesBuildingIdb.html "class in com.facebook.buck.apple")
        (implements
        com.facebook.buck.apple.[IdbOutputParsing.IdbResultCallback](IdbOutputParsing.IdbResultCallback.html "interface in com.facebook.buck.apple"))
    -   com.facebook.buck.apple.[[XCodeDescriptions]{.typeNameLink}](XCodeDescriptions.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[XCodeDescriptionsFactory]{.typeNameLink}](XCodeDescriptionsFactory.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[XcodePostbuildScriptDescription]{.typeNameLink}](XcodePostbuildScriptDescription.html "class in com.facebook.buck.apple")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>)
    -   com.facebook.buck.apple.[[XcodePrebuildScriptDescription]{.typeNameLink}](XcodePrebuildScriptDescription.html "class in com.facebook.buck.apple")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.model.[Flavored](../core/model/Flavored.html "interface in com.facebook.buck.core.model"))
    -   com.facebook.buck.apple.[[XcodeScriptDescriptionArg]{.typeNameLink}](XcodeScriptDescriptionArg.html "class in com.facebook.buck.apple")
    -   com.facebook.buck.apple.[[XcodeScriptDescriptionArg.Builder]{.typeNameLink}](XcodeScriptDescriptionArg.Builder.html "class in com.facebook.buck.apple")
:::

::: {.section role="region"}
## Interface Hierarchy {#interface-hierarchy title="Interface Hierarchy"}

-   com.facebook.buck.apple.[[AbstractIdbFailureInfo]{.typeNameLink}](AbstractIdbFailureInfo.html "interface in com.facebook.buck.apple")
-   com.facebook.buck.apple.[[AbstractIdbTestResult]{.typeNameLink}](AbstractIdbTestResult.html "interface in com.facebook.buck.apple")
-   com.facebook.buck.core.rulekey.[[AllowsNonAnnotatedFields]{.typeNameLink}](../core/rulekey/AllowsNonAnnotatedFields.html "interface in com.facebook.buck.core.rulekey")
    -   com.facebook.buck.core.rules.[[BuildRule]{.typeNameLink}](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
        (also extends
        com.facebook.buck.core.build.action.[BuildEngineAction](../core/build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action"),
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        com.facebook.buck.core.rules.[HasNameAndType](../core/rules/HasNameAndType.html "interface in com.facebook.buck.core.rules"))
        -   com.facebook.buck.apple.[[BuildRuleWithBinary]{.typeNameLink}](BuildRuleWithBinary.html "interface in com.facebook.buck.apple")
-   com.facebook.buck.apple.[[AppleCustomLinkingDepsDescription]{.typeNameLink}](AppleCustomLinkingDepsDescription.html "interface in com.facebook.buck.apple")
-   com.facebook.buck.apple.[[AppleLibrarySwiftDelegate]{.typeNameLink}](AppleLibrarySwiftDelegate.html "interface in com.facebook.buck.apple")
-   com.facebook.buck.core.build.action.[[BuildEngineAction]{.typeNameLink}](../core/build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")
    -   com.facebook.buck.core.rules.[[BuildRule]{.typeNameLink}](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
        (also extends
        com.facebook.buck.core.rulekey.[AllowsNonAnnotatedFields](../core/rulekey/AllowsNonAnnotatedFields.html "interface in com.facebook.buck.core.rulekey"),
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        com.facebook.buck.core.rules.[HasNameAndType](../core/rules/HasNameAndType.html "interface in com.facebook.buck.core.rules"))
        -   com.facebook.buck.apple.[[BuildRuleWithBinary]{.typeNameLink}](BuildRuleWithBinary.html "interface in com.facebook.buck.apple")
-   java.lang.[[Comparable]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>
    -   com.facebook.buck.core.rules.[[BuildRule]{.typeNameLink}](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
        (also extends
        com.facebook.buck.core.rulekey.[AllowsNonAnnotatedFields](../core/rulekey/AllowsNonAnnotatedFields.html "interface in com.facebook.buck.core.rulekey"),
        com.facebook.buck.core.build.action.[BuildEngineAction](../core/build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action"),
        com.facebook.buck.core.rules.[HasNameAndType](../core/rules/HasNameAndType.html "interface in com.facebook.buck.core.rules"))
        -   com.facebook.buck.apple.[[BuildRuleWithBinary]{.typeNameLink}](BuildRuleWithBinary.html "interface in com.facebook.buck.apple")
-   com.facebook.buck.core.description.arg.[[DataTransferObject]{.typeNameLink}](../core/description/arg/DataTransferObject.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.core.description.arg.[[ConstructorArg]{.typeNameLink}](../core/description/arg/ConstructorArg.html "interface in com.facebook.buck.core.description.arg")
        -   com.facebook.buck.core.description.arg.[[BuildRuleArg]{.typeNameLink}](../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")
            -   com.facebook.buck.cxx.[[CxxConstructorArg]{.typeNameLink}](../cxx/CxxConstructorArg.html "interface in com.facebook.buck.cxx")
                (also extends
                com.facebook.buck.core.description.arg.[HasDeclaredDeps](../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg"),
                com.facebook.buck.core.model.[HasDefaultFlavors](../core/model/HasDefaultFlavors.html "interface in com.facebook.buck.core.model"),
                com.facebook.buck.core.description.arg.[HasDefaultPlatform](../core/description/arg/HasDefaultPlatform.html "interface in com.facebook.buck.core.description.arg"),
                com.facebook.buck.cxx.toolchain.[HasSystemFrameworkAndLibraries](../cxx/toolchain/HasSystemFrameworkAndLibraries.html "interface in com.facebook.buck.cxx.toolchain"),
                com.facebook.buck.core.description.arg.[HasTests](../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg"))
                -   com.facebook.buck.cxx.[[LinkableCxxConstructorArg]{.typeNameLink}](../cxx/LinkableCxxConstructorArg.html "interface in com.facebook.buck.cxx")
                    -   com.facebook.buck.cxx.[[CxxLibraryDescription.CommonArg]{.typeNameLink}](../cxx/CxxLibraryDescription.CommonArg.html "interface in com.facebook.buck.cxx")
                        -   com.facebook.buck.apple.[[AppleNativeTargetDescriptionArg]{.typeNameLink}](AppleNativeTargetDescriptionArg.html "interface in com.facebook.buck.apple")
                            (also extends
                            com.facebook.buck.swift.[SwiftCommonArg](../swift/SwiftCommonArg.html "interface in com.facebook.buck.swift"))
            -   com.facebook.buck.cxx.toolchain.[[HasSystemFrameworkAndLibraries]{.typeNameLink}](../cxx/toolchain/HasSystemFrameworkAndLibraries.html "interface in com.facebook.buck.cxx.toolchain")
                -   com.facebook.buck.cxx.[[CxxConstructorArg]{.typeNameLink}](../cxx/CxxConstructorArg.html "interface in com.facebook.buck.cxx")
                    (also extends
                    com.facebook.buck.core.description.arg.[BuildRuleArg](../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg"),
                    com.facebook.buck.core.description.arg.[HasDeclaredDeps](../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg"),
                    com.facebook.buck.core.model.[HasDefaultFlavors](../core/model/HasDefaultFlavors.html "interface in com.facebook.buck.core.model"),
                    com.facebook.buck.core.description.arg.[HasDefaultPlatform](../core/description/arg/HasDefaultPlatform.html "interface in com.facebook.buck.core.description.arg"),
                    com.facebook.buck.core.description.arg.[HasTests](../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg"))
                    -   com.facebook.buck.cxx.[[LinkableCxxConstructorArg]{.typeNameLink}](../cxx/LinkableCxxConstructorArg.html "interface in com.facebook.buck.cxx")
                        -   com.facebook.buck.cxx.[[CxxLibraryDescription.CommonArg]{.typeNameLink}](../cxx/CxxLibraryDescription.CommonArg.html "interface in com.facebook.buck.cxx")
                            -   com.facebook.buck.apple.[[AppleNativeTargetDescriptionArg]{.typeNameLink}](AppleNativeTargetDescriptionArg.html "interface in com.facebook.buck.apple")
                                (also extends
                                com.facebook.buck.swift.[SwiftCommonArg](../swift/SwiftCommonArg.html "interface in com.facebook.buck.swift"))
            -   com.facebook.buck.swift.[[SwiftCommonArg]{.typeNameLink}](../swift/SwiftCommonArg.html "interface in com.facebook.buck.swift")
                -   com.facebook.buck.apple.[[AppleNativeTargetDescriptionArg]{.typeNameLink}](AppleNativeTargetDescriptionArg.html "interface in com.facebook.buck.apple")
                    (also extends
                    com.facebook.buck.cxx.[CxxLibraryDescription.CommonArg](../cxx/CxxLibraryDescription.CommonArg.html "interface in com.facebook.buck.cxx"))
-   org.pf4j.ExtensionPoint
    -   com.facebook.buck.apple.[[XCodeDescriptionClassSupplier]{.typeNameLink}](XCodeDescriptionClassSupplier.html "interface in com.facebook.buck.apple")
-   com.facebook.buck.apple.[[GroupedSource.Visitor]{.typeNameLink}](GroupedSource.Visitor.html "interface in com.facebook.buck.apple")
-   com.facebook.buck.apple.[[HasAppleBundleFields]{.typeNameLink}](HasAppleBundleFields.html "interface in com.facebook.buck.apple")
-   com.facebook.buck.apple.[[HasAppleBundleResourcesDescription]{.typeNameLink}](HasAppleBundleResourcesDescription.html "interface in com.facebook.buck.apple")\<T\>
-   com.facebook.buck.apple.[[HasAppleCodesignFields]{.typeNameLink}](HasAppleCodesignFields.html "interface in com.facebook.buck.apple")
-   com.facebook.buck.core.description.arg.[[HasDeclaredDeps]{.typeNameLink}](../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.cxx.[[CxxConstructorArg]{.typeNameLink}](../cxx/CxxConstructorArg.html "interface in com.facebook.buck.cxx")
        (also extends
        com.facebook.buck.core.description.arg.[BuildRuleArg](../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.model.[HasDefaultFlavors](../core/model/HasDefaultFlavors.html "interface in com.facebook.buck.core.model"),
        com.facebook.buck.core.description.arg.[HasDefaultPlatform](../core/description/arg/HasDefaultPlatform.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.cxx.toolchain.[HasSystemFrameworkAndLibraries](../cxx/toolchain/HasSystemFrameworkAndLibraries.html "interface in com.facebook.buck.cxx.toolchain"),
        com.facebook.buck.core.description.arg.[HasTests](../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg"))
        -   com.facebook.buck.cxx.[[LinkableCxxConstructorArg]{.typeNameLink}](../cxx/LinkableCxxConstructorArg.html "interface in com.facebook.buck.cxx")
            -   com.facebook.buck.cxx.[[CxxLibraryDescription.CommonArg]{.typeNameLink}](../cxx/CxxLibraryDescription.CommonArg.html "interface in com.facebook.buck.cxx")
                -   com.facebook.buck.apple.[[AppleNativeTargetDescriptionArg]{.typeNameLink}](AppleNativeTargetDescriptionArg.html "interface in com.facebook.buck.apple")
                    (also extends
                    com.facebook.buck.swift.[SwiftCommonArg](../swift/SwiftCommonArg.html "interface in com.facebook.buck.swift"))
-   com.facebook.buck.core.model.[[HasDefaultFlavors]{.typeNameLink}](../core/model/HasDefaultFlavors.html "interface in com.facebook.buck.core.model")
    -   com.facebook.buck.cxx.[[CxxConstructorArg]{.typeNameLink}](../cxx/CxxConstructorArg.html "interface in com.facebook.buck.cxx")
        (also extends
        com.facebook.buck.core.description.arg.[BuildRuleArg](../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasDeclaredDeps](../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasDefaultPlatform](../core/description/arg/HasDefaultPlatform.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.cxx.toolchain.[HasSystemFrameworkAndLibraries](../cxx/toolchain/HasSystemFrameworkAndLibraries.html "interface in com.facebook.buck.cxx.toolchain"),
        com.facebook.buck.core.description.arg.[HasTests](../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg"))
        -   com.facebook.buck.cxx.[[LinkableCxxConstructorArg]{.typeNameLink}](../cxx/LinkableCxxConstructorArg.html "interface in com.facebook.buck.cxx")
            -   com.facebook.buck.cxx.[[CxxLibraryDescription.CommonArg]{.typeNameLink}](../cxx/CxxLibraryDescription.CommonArg.html "interface in com.facebook.buck.cxx")
                -   com.facebook.buck.apple.[[AppleNativeTargetDescriptionArg]{.typeNameLink}](AppleNativeTargetDescriptionArg.html "interface in com.facebook.buck.apple")
                    (also extends
                    com.facebook.buck.swift.[SwiftCommonArg](../swift/SwiftCommonArg.html "interface in com.facebook.buck.swift"))
-   com.facebook.buck.core.description.arg.[[HasDefaultPlatform]{.typeNameLink}](../core/description/arg/HasDefaultPlatform.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.cxx.[[CxxConstructorArg]{.typeNameLink}](../cxx/CxxConstructorArg.html "interface in com.facebook.buck.cxx")
        (also extends
        com.facebook.buck.core.description.arg.[BuildRuleArg](../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasDeclaredDeps](../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.model.[HasDefaultFlavors](../core/model/HasDefaultFlavors.html "interface in com.facebook.buck.core.model"),
        com.facebook.buck.cxx.toolchain.[HasSystemFrameworkAndLibraries](../cxx/toolchain/HasSystemFrameworkAndLibraries.html "interface in com.facebook.buck.cxx.toolchain"),
        com.facebook.buck.core.description.arg.[HasTests](../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg"))
        -   com.facebook.buck.cxx.[[LinkableCxxConstructorArg]{.typeNameLink}](../cxx/LinkableCxxConstructorArg.html "interface in com.facebook.buck.cxx")
            -   com.facebook.buck.cxx.[[CxxLibraryDescription.CommonArg]{.typeNameLink}](../cxx/CxxLibraryDescription.CommonArg.html "interface in com.facebook.buck.cxx")
                -   com.facebook.buck.apple.[[AppleNativeTargetDescriptionArg]{.typeNameLink}](AppleNativeTargetDescriptionArg.html "interface in com.facebook.buck.apple")
                    (also extends
                    com.facebook.buck.swift.[SwiftCommonArg](../swift/SwiftCommonArg.html "interface in com.facebook.buck.swift"))
-   com.facebook.buck.apple.[[HasEntitlementsFile]{.typeNameLink}](HasEntitlementsFile.html "interface in com.facebook.buck.apple")
-   com.facebook.buck.core.rules.[[HasNameAndType]{.typeNameLink}](../core/rules/HasNameAndType.html "interface in com.facebook.buck.core.rules")
    -   com.facebook.buck.core.rules.[[BuildRule]{.typeNameLink}](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
        (also extends
        com.facebook.buck.core.rulekey.[AllowsNonAnnotatedFields](../core/rulekey/AllowsNonAnnotatedFields.html "interface in com.facebook.buck.core.rulekey"),
        com.facebook.buck.core.build.action.[BuildEngineAction](../core/build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action"),
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>)
        -   com.facebook.buck.apple.[[BuildRuleWithBinary]{.typeNameLink}](BuildRuleWithBinary.html "interface in com.facebook.buck.apple")
-   com.facebook.buck.core.description.arg.[[HasTests]{.typeNameLink}](../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.cxx.[[CxxConstructorArg]{.typeNameLink}](../cxx/CxxConstructorArg.html "interface in com.facebook.buck.cxx")
        (also extends
        com.facebook.buck.core.description.arg.[BuildRuleArg](../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasDeclaredDeps](../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.model.[HasDefaultFlavors](../core/model/HasDefaultFlavors.html "interface in com.facebook.buck.core.model"),
        com.facebook.buck.core.description.arg.[HasDefaultPlatform](../core/description/arg/HasDefaultPlatform.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.cxx.toolchain.[HasSystemFrameworkAndLibraries](../cxx/toolchain/HasSystemFrameworkAndLibraries.html "interface in com.facebook.buck.cxx.toolchain"))
        -   com.facebook.buck.cxx.[[LinkableCxxConstructorArg]{.typeNameLink}](../cxx/LinkableCxxConstructorArg.html "interface in com.facebook.buck.cxx")
            -   com.facebook.buck.cxx.[[CxxLibraryDescription.CommonArg]{.typeNameLink}](../cxx/CxxLibraryDescription.CommonArg.html "interface in com.facebook.buck.cxx")
                -   com.facebook.buck.apple.[[AppleNativeTargetDescriptionArg]{.typeNameLink}](AppleNativeTargetDescriptionArg.html "interface in com.facebook.buck.apple")
                    (also extends
                    com.facebook.buck.swift.[SwiftCommonArg](../swift/SwiftCommonArg.html "interface in com.facebook.buck.swift"))
-   com.facebook.buck.apple.[[IdbOutputParsing.IdbResultCallback]{.typeNameLink}](IdbOutputParsing.IdbResultCallback.html "interface in com.facebook.buck.apple")
-   com.facebook.buck.apple.[[IdbRunTestsStep.StdoutReadingCallback]{.typeNameLink}](IdbRunTestsStep.StdoutReadingCallback.html "interface in com.facebook.buck.apple")
:::

::: {.section role="region"}
## Enum Hierarchy {#enum-hierarchy title="Enum Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   java.lang.[[Enum]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<E\>
        (implements
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   com.facebook.buck.apple.[[AppleAssetCatalog.ValidationType]{.typeNameLink}](AppleAssetCatalog.ValidationType.html "enum in com.facebook.buck.apple")
        -   com.facebook.buck.apple.[[AppleBuildRules.RecursiveDependenciesMode]{.typeNameLink}](AppleBuildRules.RecursiveDependenciesMode.html "enum in com.facebook.buck.apple")
        -   com.facebook.buck.apple.[[AppleBundleDestination]{.typeNameLink}](AppleBundleDestination.html "enum in com.facebook.buck.apple")
        -   com.facebook.buck.apple.[[AppleBundleExtension]{.typeNameLink}](AppleBundleExtension.html "enum in com.facebook.buck.apple")
        -   com.facebook.buck.apple.[[AppleDebugFormat]{.typeNameLink}](AppleDebugFormat.html "enum in com.facebook.buck.apple")
            (implements
            com.facebook.buck.core.model.[FlavorConvertible](../core/model/FlavorConvertible.html "interface in com.facebook.buck.core.model"))
        -   com.facebook.buck.apple.[[AppleLibraryDescription.Type]{.typeNameLink}](AppleLibraryDescription.Type.html "enum in com.facebook.buck.apple")
            (implements
            com.facebook.buck.core.model.[FlavorConvertible](../core/model/FlavorConvertible.html "interface in com.facebook.buck.core.model"))
        -   com.facebook.buck.apple.[[GroupedSource.Type]{.typeNameLink}](GroupedSource.Type.html "enum in com.facebook.buck.apple")
        -   com.facebook.buck.apple.[[LibtoolStep.Style]{.typeNameLink}](LibtoolStep.Style.html "enum in com.facebook.buck.apple")
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
