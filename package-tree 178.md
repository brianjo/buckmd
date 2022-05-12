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
# Hierarchy For Package com.facebook.buck.cxx {#hierarchy-for-package-com.facebook.buck.cxx .title}

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
            -   com.facebook.buck.cxx.[[CxxBinary]{.typeNameLink}](CxxBinary.html "class in com.facebook.buck.cxx")
                (implements
                com.facebook.buck.core.rules.tool.[BinaryBuildRule](../core/rules/tool/BinaryBuildRule.html "interface in com.facebook.buck.core.rules.tool"),
                com.facebook.buck.cxx.[HasAppleDebugSymbolDeps](HasAppleDebugSymbolDeps.html "interface in com.facebook.buck.cxx"),
                com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"),
                com.facebook.buck.core.rules.attr.[HasSupplementaryOutputs](../core/rules/attr/HasSupplementaryOutputs.html "interface in com.facebook.buck.core.rules.attr"),
                com.facebook.buck.cxx.[NativeTestable](NativeTestable.html "interface in com.facebook.buck.cxx"),
                com.facebook.buck.core.rules.attr.[SupportsInputBasedRuleKey](../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr"))
            -   com.facebook.buck.cxx.[[CxxTest]{.typeNameLink}](CxxTest.html "class in com.facebook.buck.cxx")
                (implements
                com.facebook.buck.core.rules.tool.[BinaryBuildRule](../core/rules/tool/BinaryBuildRule.html "interface in com.facebook.buck.core.rules.tool"),
                com.facebook.buck.core.test.rule.[ExternalTestRunnerRule](../core/test/rule/ExternalTestRunnerRule.html "interface in com.facebook.buck.core.test.rule"),
                com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"),
                com.facebook.buck.core.test.rule.[TestRule](../core/test/rule/TestRule.html "interface in com.facebook.buck.core.test.rule"))
            -   com.facebook.buck.core.rules.impl.[[NoopBuildRuleWithDeclaredAndExtraDeps]{.typeNameLink}](../core/rules/impl/NoopBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")
                -   com.facebook.buck.cxx.[[CxxGenrule]{.typeNameLink}](CxxGenrule.html "class in com.facebook.buck.cxx")
                    (implements
                    com.facebook.buck.core.model.[HasOutputName](../core/model/HasOutputName.html "interface in com.facebook.buck.core.model"))
                -   com.facebook.buck.cxx.[[CxxLibraryGroup]{.typeNameLink}](CxxLibraryGroup.html "class in com.facebook.buck.cxx")
                    (implements
                    com.facebook.buck.cxx.[AbstractCxxLibraryGroup](AbstractCxxLibraryGroup.html "interface in com.facebook.buck.cxx"),
                    com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"),
                    com.facebook.buck.cxx.toolchain.nativelink.[LegacyNativeLinkableGroup](toolchain/nativelink/LegacyNativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink"),
                    com.facebook.buck.cxx.toolchain.nativelink.[LegacyNativeLinkTargetGroup](toolchain/nativelink/LegacyNativeLinkTargetGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink"),
                    com.facebook.buck.cxx.[NativeTestable](NativeTestable.html "interface in com.facebook.buck.cxx"))
                -   com.facebook.buck.cxx.[[PrebuiltCxxLibrary]{.typeNameLink}](PrebuiltCxxLibrary.html "class in com.facebook.buck.cxx")
                    (implements
                    com.facebook.buck.cxx.[AbstractCxxLibraryGroup](AbstractCxxLibraryGroup.html "interface in com.facebook.buck.cxx"))
                -   com.facebook.buck.cxx.[[PrebuiltCxxLibraryGroupDescription.CustomPrebuiltCxxLibrary]{.typeNameLink}](PrebuiltCxxLibraryGroupDescription.CustomPrebuiltCxxLibrary.html "class in com.facebook.buck.cxx")
                    (implements
                    com.facebook.buck.cxx.[AbstractCxxLibraryGroup](AbstractCxxLibraryGroup.html "interface in com.facebook.buck.cxx"),
                    com.facebook.buck.cxx.toolchain.nativelink.[LegacyNativeLinkableGroup](toolchain/nativelink/LegacyNativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink"))
                -   com.facebook.buck.cxx.[[PreInclude]{.typeNameLink}](PreInclude.html "class in com.facebook.buck.cxx")
                    (implements
                    com.facebook.buck.cxx.[CxxPreprocessorDep](CxxPreprocessorDep.html "interface in com.facebook.buck.cxx"),
                    com.facebook.buck.cxx.toolchain.nativelink.[NativeLinkableGroup](toolchain/nativelink/NativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink"))
                    -   com.facebook.buck.cxx.[[CxxPrecompiledHeaderTemplate]{.typeNameLink}](CxxPrecompiledHeaderTemplate.html "class in com.facebook.buck.cxx")
                        (implements
                        com.facebook.buck.android.packageable.[AndroidPackageable](../android/packageable/AndroidPackageable.html "interface in com.facebook.buck.android.packageable"))
                    -   com.facebook.buck.cxx.[[CxxPrefixHeader]{.typeNameLink}](CxxPrefixHeader.html "class in com.facebook.buck.cxx")
        -   com.facebook.buck.cxx.[[CxxCompilationDatabase]{.typeNameLink}](CxxCompilationDatabase.html "class in com.facebook.buck.cxx")
            (implements
            com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"))
        -   com.facebook.buck.cxx.[[CxxStrip]{.typeNameLink}](CxxStrip.html "class in com.facebook.buck.cxx")
            (implements
            com.facebook.buck.core.rules.attr.[SupportsInputBasedRuleKey](../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr"))
        -   com.facebook.buck.rules.modern.[[ModernBuildRule]{.typeNameLink}](../rules/modern/ModernBuildRule.html "class in com.facebook.buck.rules.modern")\<T\>
            (implements
            com.facebook.buck.core.rules.attr.[SupportsInputBasedRuleKey](../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr"))
            -   com.facebook.buck.cxx.[[Archive]{.typeNameLink}](Archive.html "class in com.facebook.buck.cxx")
            -   com.facebook.buck.cxx.[[CxxLink]{.typeNameLink}](CxxLink.html "class in com.facebook.buck.cxx")
                (implements
                com.facebook.buck.cxx.[HasAppleDebugSymbolDeps](HasAppleDebugSymbolDeps.html "interface in com.facebook.buck.cxx"),
                com.facebook.buck.core.rules.attr.[HasSupplementaryOutputs](../core/rules/attr/HasSupplementaryOutputs.html "interface in com.facebook.buck.core.rules.attr"),
                com.facebook.buck.core.rules.schedule.[OverrideScheduleRule](../core/rules/schedule/OverrideScheduleRule.html "interface in com.facebook.buck.core.rules.schedule"))
            -   com.facebook.buck.cxx.[[CxxPreprocessAndCompile]{.typeNameLink}](CxxPreprocessAndCompile.html "class in com.facebook.buck.cxx")
                (implements
                com.facebook.buck.cxx.[CxxIntermediateBuildProduct](CxxIntermediateBuildProduct.html "interface in com.facebook.buck.cxx"),
                com.facebook.buck.core.rules.attr.[SupportsDependencyFileRuleKey](../core/rules/attr/SupportsDependencyFileRuleKey.html "interface in com.facebook.buck.core.rules.attr"))
            -   com.facebook.buck.cxx.[[CxxThinLTOIndex]{.typeNameLink}](CxxThinLTOIndex.html "class in com.facebook.buck.cxx")
                (implements
                com.facebook.buck.cxx.[HasAppleDebugSymbolDeps](HasAppleDebugSymbolDeps.html "interface in com.facebook.buck.cxx"),
                com.facebook.buck.core.rules.schedule.[OverrideScheduleRule](../core/rules/schedule/OverrideScheduleRule.html "interface in com.facebook.buck.core.rules.schedule"),
                com.facebook.buck.core.rules.attr.[SupportsInputBasedRuleKey](../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr"))
            -   com.facebook.buck.cxx.[[CxxThinLTOOpt]{.typeNameLink}](CxxThinLTOOpt.html "class in com.facebook.buck.cxx")
                (implements
                com.facebook.buck.cxx.[CxxIntermediateBuildProduct](CxxIntermediateBuildProduct.html "interface in com.facebook.buck.cxx"))
            -   com.facebook.buck.cxx.[[MachoDylibStubRule]{.typeNameLink}](MachoDylibStubRule.html "class in com.facebook.buck.cxx")
        -   com.facebook.buck.core.rules.impl.[[SymlinkTree]{.typeNameLink}](../core/rules/impl/SymlinkTree.html "class in com.facebook.buck.core.rules.impl")
            (implements
            com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"),
            com.facebook.buck.core.rules.attr.[SupportsInputBasedRuleKey](../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr"))
            -   com.facebook.buck.core.rules.impl.[[MappedSymlinkTree]{.typeNameLink}](../core/rules/impl/MappedSymlinkTree.html "class in com.facebook.buck.core.rules.impl")
                -   com.facebook.buck.cxx.toolchain.[[HeaderSymlinkTree]{.typeNameLink}](toolchain/HeaderSymlinkTree.html "class in com.facebook.buck.cxx.toolchain")
                    -   com.facebook.buck.cxx.[[HeaderSymlinkTreeWithHeaderMap]{.typeNameLink}](HeaderSymlinkTreeWithHeaderMap.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.shell.[[AbstractGenruleDescription]{.typeNameLink}](../shell/AbstractGenruleDescription.html "class in com.facebook.buck.shell")\<T\>
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>)
        -   com.facebook.buck.cxx.[[CxxGenruleDescription]{.typeNameLink}](CxxGenruleDescription.html "class in com.facebook.buck.cxx")
            (implements
            com.facebook.buck.core.model.[Flavored](../core/model/Flavored.html "interface in com.facebook.buck.core.model"),
            com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>,
            com.facebook.buck.versions.[VersionPropagator](../versions/VersionPropagator.html "interface in com.facebook.buck.versions")\<A\>)
    -   com.facebook.buck.rules.macros.[[AbstractMacroExpanderWithoutPrecomputedWork]{.typeNameLink}](../rules/macros/AbstractMacroExpanderWithoutPrecomputedWork.html "class in com.facebook.buck.rules.macros")\<T\>
        (implements
        com.facebook.buck.rules.macros.[MacroExpander](../rules/macros/MacroExpander.html "interface in com.facebook.buck.rules.macros")\<T,​P\>)
        -   com.facebook.buck.rules.macros.[[BuildTargetMacroExpander]{.typeNameLink}](../rules/macros/BuildTargetMacroExpander.html "class in com.facebook.buck.rules.macros")\<M\>
            -   com.facebook.buck.rules.macros.[[AbstractLocationMacroExpander]{.typeNameLink}](../rules/macros/AbstractLocationMacroExpander.html "class in com.facebook.buck.rules.macros")\<T\>
                -   com.facebook.buck.rules.macros.[[LocationMacroExpander]{.typeNameLink}](../rules/macros/LocationMacroExpander.html "class in com.facebook.buck.rules.macros")
                    -   com.facebook.buck.cxx.[[CxxLocationMacroExpander]{.typeNameLink}](CxxLocationMacroExpander.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[CxxBinaryDescription]{.typeNameLink}](CxxBinaryDescription.html "class in com.facebook.buck.cxx")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.model.[Flavored](../core/model/Flavored.html "interface in com.facebook.buck.core.model"),
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>,
        com.facebook.buck.core.description.attr.[ImplicitFlavorsInferringDescription](../core/description/attr/ImplicitFlavorsInferringDescription.html "interface in com.facebook.buck.core.description.attr"),
        com.facebook.buck.core.description.metadata.[MetadataProvidingDescription](../core/description/metadata/MetadataProvidingDescription.html "interface in com.facebook.buck.core.description.metadata")\<T\>,
        com.facebook.buck.versions.[VersionRoot](../versions/VersionRoot.html "interface in com.facebook.buck.versions")\<A\>)
    -   com.facebook.buck.cxx.[[CxxBinaryDescriptionArg]{.typeNameLink}](CxxBinaryDescriptionArg.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[CxxBinaryDescriptionArg.Builder]{.typeNameLink}](CxxBinaryDescriptionArg.Builder.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[CxxBinaryFactory]{.typeNameLink}](CxxBinaryFactory.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[CxxBinaryFlavored]{.typeNameLink}](CxxBinaryFlavored.html "class in com.facebook.buck.cxx")
        (implements
        com.facebook.buck.core.model.[Flavored](../core/model/Flavored.html "interface in com.facebook.buck.core.model"))
    -   com.facebook.buck.cxx.[[CxxBinaryImplicitFlavors]{.typeNameLink}](CxxBinaryImplicitFlavors.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[CxxBinaryMetadataFactory]{.typeNameLink}](CxxBinaryMetadataFactory.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[CxxCompilationDatabaseEntry]{.typeNameLink}](CxxCompilationDatabaseEntry.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[CxxDeps]{.typeNameLink}](CxxDeps.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[CxxDeps.Builder]{.typeNameLink}](CxxDeps.Builder.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[CxxDescriptionEnhancer]{.typeNameLink}](CxxDescriptionEnhancer.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[CxxDescriptionsProvider]{.typeNameLink}](CxxDescriptionsProvider.html "class in com.facebook.buck.cxx")
        (implements
        com.facebook.buck.core.model.targetgraph.[DescriptionProvider](../core/model/targetgraph/DescriptionProvider.html "interface in com.facebook.buck.core.model.targetgraph"))
    -   com.facebook.buck.cxx.[[CxxFlags]{.typeNameLink}](CxxFlags.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[CxxFlags.TranslateMacrosArgsFunction]{.typeNameLink}](CxxFlags.TranslateMacrosArgsFunction.html "class in com.facebook.buck.cxx")
        (implements
        com.facebook.buck.rules.args.[AddsToRuleKeyFunction](../rules/args/AddsToRuleKeyFunction.html "interface in com.facebook.buck.rules.args")\<T,​F\>)
    -   com.facebook.buck.cxx.[[CxxFlags.TranslateMacrosFunction]{.typeNameLink}](CxxFlags.TranslateMacrosFunction.html "class in com.facebook.buck.cxx")
        (implements
        com.facebook.buck.rules.args.[AddsToRuleKeyFunction](../rules/args/AddsToRuleKeyFunction.html "interface in com.facebook.buck.rules.args")\<T,​F\>)
    -   com.facebook.buck.cxx.[[CxxGenruleDescriptionArg]{.typeNameLink}](CxxGenruleDescriptionArg.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[CxxGenruleDescriptionArg.Builder]{.typeNameLink}](CxxGenruleDescriptionArg.Builder.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[CxxHeaders]{.typeNameLink}](CxxHeaders.html "class in com.facebook.buck.cxx")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"),
        com.facebook.buck.core.rules.attr.[HasCustomDepsLogic](../core/rules/attr/HasCustomDepsLogic.html "interface in com.facebook.buck.core.rules.attr"))
        -   com.facebook.buck.cxx.[[CxxHeadersDir]{.typeNameLink}](CxxHeadersDir.html "class in com.facebook.buck.cxx")
        -   com.facebook.buck.cxx.[[CxxRawHeaders]{.typeNameLink}](CxxRawHeaders.html "class in com.facebook.buck.cxx")
        -   com.facebook.buck.cxx.[[CxxSymlinkTreeHeaders]{.typeNameLink}](CxxSymlinkTreeHeaders.html "class in com.facebook.buck.cxx")
            (implements
            com.facebook.buck.rules.keys.[RuleKeyAppendable](../rules/keys/RuleKeyAppendable.html "interface in com.facebook.buck.rules.keys"))
    -   com.facebook.buck.cxx.[[CxxInferEnhancer]{.typeNameLink}](CxxInferEnhancer.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[CxxLibraryDescription]{.typeNameLink}](CxxLibraryDescription.html "class in com.facebook.buck.cxx")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.model.[Flavored](../core/model/Flavored.html "interface in com.facebook.buck.core.model"),
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>,
        com.facebook.buck.core.description.attr.[ImplicitFlavorsInferringDescription](../core/description/attr/ImplicitFlavorsInferringDescription.html "interface in com.facebook.buck.core.description.attr"),
        com.facebook.buck.core.description.metadata.[MetadataProvidingDescription](../core/description/metadata/MetadataProvidingDescription.html "interface in com.facebook.buck.core.description.metadata")\<T\>,
        com.facebook.buck.versions.[VersionPropagator](../versions/VersionPropagator.html "interface in com.facebook.buck.versions")\<A\>)
    -   com.facebook.buck.cxx.[[CxxLibraryDescriptionArg]{.typeNameLink}](CxxLibraryDescriptionArg.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[CxxLibraryDescriptionArg.Builder]{.typeNameLink}](CxxLibraryDescriptionArg.Builder.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[CxxLibraryFactory]{.typeNameLink}](CxxLibraryFactory.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[CxxLibraryFlavored]{.typeNameLink}](CxxLibraryFlavored.html "class in com.facebook.buck.cxx")
        (implements
        com.facebook.buck.core.model.[Flavored](../core/model/Flavored.html "interface in com.facebook.buck.core.model"))
    -   com.facebook.buck.cxx.[[CxxLibraryImplicitFlavors]{.typeNameLink}](CxxLibraryImplicitFlavors.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[CxxLibraryMetadataFactory]{.typeNameLink}](CxxLibraryMetadataFactory.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[CxxLink.Impl]{.typeNameLink}](CxxLink.Impl.html "class in com.facebook.buck.cxx")
        (implements
        com.facebook.buck.rules.modern.[Buildable](../rules/modern/Buildable.html "interface in com.facebook.buck.rules.modern"))
    -   com.facebook.buck.cxx.[[CxxLinkableEnhancer]{.typeNameLink}](CxxLinkableEnhancer.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[CxxLinkAndCompileRules]{.typeNameLink}](CxxLinkAndCompileRules.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[CxxLinkOptions]{.typeNameLink}](CxxLinkOptions.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[CxxPrecompiledHeaderDescription]{.typeNameLink}](CxxPrecompiledHeaderDescription.html "class in com.facebook.buck.cxx")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.versions.[VersionPropagator](../versions/VersionPropagator.html "interface in com.facebook.buck.versions")\<A\>)
    -   com.facebook.buck.cxx.[[CxxPrecompiledHeaderDescriptionArg]{.typeNameLink}](CxxPrecompiledHeaderDescriptionArg.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[CxxPrecompiledHeaderDescriptionArg.Builder]{.typeNameLink}](CxxPrecompiledHeaderDescriptionArg.Builder.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[CxxPrepareForLinkStep]{.typeNameLink}](CxxPrepareForLinkStep.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[CxxPreprocessables]{.typeNameLink}](CxxPreprocessables.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[CxxPreprocessorInput]{.typeNameLink}](CxxPreprocessorInput.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[CxxSource]{.typeNameLink}](CxxSource.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[CxxSourceRuleFactory]{.typeNameLink}](CxxSourceRuleFactory.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[CxxSourceTypes]{.typeNameLink}](CxxSourceTypes.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[CxxTestDescription]{.typeNameLink}](CxxTestDescription.html "class in com.facebook.buck.cxx")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.model.[Flavored](../core/model/Flavored.html "interface in com.facebook.buck.core.model"),
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>,
        com.facebook.buck.core.description.metadata.[MetadataProvidingDescription](../core/description/metadata/MetadataProvidingDescription.html "interface in com.facebook.buck.core.description.metadata")\<T\>,
        com.facebook.buck.versions.[VersionRoot](../versions/VersionRoot.html "interface in com.facebook.buck.versions")\<A\>)
    -   com.facebook.buck.cxx.[[CxxTestDescriptionArg]{.typeNameLink}](CxxTestDescriptionArg.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[CxxTestDescriptionArg.Builder]{.typeNameLink}](CxxTestDescriptionArg.Builder.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[CxxThinLTOIndex.Impl]{.typeNameLink}](CxxThinLTOIndex.Impl.html "class in com.facebook.buck.cxx")
        (implements
        com.facebook.buck.rules.modern.[Buildable](../rules/modern/Buildable.html "interface in com.facebook.buck.rules.modern"))
    -   com.facebook.buck.cxx.[[CxxThinLTOIndexArg]{.typeNameLink}](CxxThinLTOIndexArg.html "class in com.facebook.buck.cxx")
        (implements
        com.facebook.buck.rules.args.[Arg](../rules/args/Arg.html "interface in com.facebook.buck.rules.args"))
    -   com.facebook.buck.cxx.[[CxxThinLTOOpt.Impl]{.typeNameLink}](CxxThinLTOOpt.Impl.html "class in com.facebook.buck.cxx")
        (implements
        com.facebook.buck.rules.modern.[Buildable](../rules/modern/Buildable.html "interface in com.facebook.buck.rules.modern"))
    -   com.facebook.buck.cxx.[[CxxToolchainDescription]{.typeNameLink}](CxxToolchainDescription.html "class in com.facebook.buck.cxx")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>)
    -   com.facebook.buck.cxx.[[CxxToolchainDescriptionArg]{.typeNameLink}](CxxToolchainDescriptionArg.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[CxxToolchainDescriptionArg.Builder]{.typeNameLink}](CxxToolchainDescriptionArg.Builder.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[CxxToolFlags]{.typeNameLink}](CxxToolFlags.html "class in com.facebook.buck.cxx")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"))
        -   com.facebook.buck.cxx.[[ExplicitCxxToolFlags]{.typeNameLink}](ExplicitCxxToolFlags.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.toolchain.[[DebugPathSanitizer]{.typeNameLink}](toolchain/DebugPathSanitizer.html "class in com.facebook.buck.cxx.toolchain")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"))
        -   com.facebook.buck.cxx.[[NoopDebugPathSanitizer]{.typeNameLink}](NoopDebugPathSanitizer.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[DepsBuilder]{.typeNameLink}](DepsBuilder.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[FrameworkDependencies]{.typeNameLink}](FrameworkDependencies.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.ImmutableCxxPreprocessorInput.Builder
        -   com.facebook.buck.cxx.[[CxxPreprocessorInput.Builder]{.typeNameLink}](CxxPreprocessorInput.Builder.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.ImmutableExplicitCxxToolFlags.Builder
        -   com.facebook.buck.cxx.[[ExplicitCxxToolFlags.Builder]{.typeNameLink}](ExplicitCxxToolFlags.Builder.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.ImmutablePreprocessorFlags.Builder
        -   com.facebook.buck.cxx.[[PreprocessorFlags.Builder]{.typeNameLink}](PreprocessorFlags.Builder.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[LinkableListFilterFactory]{.typeNameLink}](LinkableListFilterFactory.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[MachoDylibStubRuleFactory]{.typeNameLink}](MachoDylibStubRuleFactory.html "class in com.facebook.buck.cxx")
        (implements
        com.facebook.buck.cxx.toolchain.[SharedLibraryInterfaceFactory](toolchain/SharedLibraryInterfaceFactory.html "interface in com.facebook.buck.cxx.toolchain"))
    -   com.facebook.buck.cxx.[[MachoDylibStubScrubContentsStep]{.typeNameLink}](MachoDylibStubScrubContentsStep.html "class in com.facebook.buck.cxx")
        (implements
        com.facebook.buck.step.[Step](../step/Step.html "interface in com.facebook.buck.step"))
    -   com.facebook.buck.cxx.[[Omnibus]{.typeNameLink}](Omnibus.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[Omnibus.OmnibusLibraries]{.typeNameLink}](Omnibus.OmnibusLibraries.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[OmnibusRoots]{.typeNameLink}](OmnibusRoots.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[OmnibusRoots.Builder]{.typeNameLink}](OmnibusRoots.Builder.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[PrebuiltCxxLibraryDescription]{.typeNameLink}](PrebuiltCxxLibraryDescription.html "class in com.facebook.buck.cxx")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>,
        com.facebook.buck.versions.[VersionPropagator](../versions/VersionPropagator.html "interface in com.facebook.buck.versions")\<A\>)
    -   com.facebook.buck.cxx.[[PrebuiltCxxLibraryDescriptionArg]{.typeNameLink}](PrebuiltCxxLibraryDescriptionArg.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[PrebuiltCxxLibraryDescriptionArg.Builder]{.typeNameLink}](PrebuiltCxxLibraryDescriptionArg.Builder.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[PrebuiltCxxLibraryGroupDescription]{.typeNameLink}](PrebuiltCxxLibraryGroupDescription.html "class in com.facebook.buck.cxx")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.versions.[VersionPropagator](../versions/VersionPropagator.html "interface in com.facebook.buck.versions")\<A\>)
    -   com.facebook.buck.cxx.[[PrebuiltCxxLibraryGroupDescriptionArg]{.typeNameLink}](PrebuiltCxxLibraryGroupDescriptionArg.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[PrebuiltCxxLibraryGroupDescriptionArg.Builder]{.typeNameLink}](PrebuiltCxxLibraryGroupDescriptionArg.Builder.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[PreprocessorFlags]{.typeNameLink}](PreprocessorFlags.html "class in com.facebook.buck.cxx")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"))
    -   com.facebook.buck.cxx.[[RelativeLinkArg]{.typeNameLink}](RelativeLinkArg.html "class in com.facebook.buck.cxx")
        (implements
        com.facebook.buck.rules.args.[Arg](../rules/args/Arg.html "interface in com.facebook.buck.rules.args"))
    -   com.facebook.buck.shell.[[ShellStep]{.typeNameLink}](../shell/ShellStep.html "class in com.facebook.buck.shell")
        (implements
        com.facebook.buck.step.[Step](../step/Step.html "interface in com.facebook.buck.step"))
        -   com.facebook.buck.cxx.[[MachoScrubContentSectionsStep]{.typeNameLink}](MachoScrubContentSectionsStep.html "class in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[TransitiveCxxPreprocessorInputCache]{.typeNameLink}](TransitiveCxxPreprocessorInputCache.html "class in com.facebook.buck.cxx")
:::

::: {.section role="region"}
## Interface Hierarchy {#interface-hierarchy title="Interface Hierarchy"}

-   com.facebook.buck.core.rulekey.[[AddsToRuleKey]{.typeNameLink}](../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey")
    -   com.facebook.buck.cxx.[[LinkOutputPostprocessor]{.typeNameLink}](LinkOutputPostprocessor.html "interface in com.facebook.buck.cxx")
-   com.facebook.buck.core.rulekey.[[AllowsNonAnnotatedFields]{.typeNameLink}](../core/rulekey/AllowsNonAnnotatedFields.html "interface in com.facebook.buck.core.rulekey")
    -   com.facebook.buck.core.rules.[[BuildRule]{.typeNameLink}](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
        (also extends
        com.facebook.buck.core.build.action.[BuildEngineAction](../core/build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action"),
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        com.facebook.buck.core.rules.[HasNameAndType](../core/rules/HasNameAndType.html "interface in com.facebook.buck.core.rules"))
        -   com.facebook.buck.cxx.[[CxxIntermediateBuildProduct]{.typeNameLink}](CxxIntermediateBuildProduct.html "interface in com.facebook.buck.cxx")
        -   com.facebook.buck.cxx.[[HasAppleDebugSymbolDeps]{.typeNameLink}](HasAppleDebugSymbolDeps.html "interface in com.facebook.buck.cxx")
-   com.facebook.buck.android.packageable.[[AndroidPackageable]{.typeNameLink}](../android/packageable/AndroidPackageable.html "interface in com.facebook.buck.android.packageable")
    -   com.facebook.buck.cxx.[[AbstractCxxLibraryGroup]{.typeNameLink}](AbstractCxxLibraryGroup.html "interface in com.facebook.buck.cxx")
        (also extends
        com.facebook.buck.cxx.[CxxPreprocessorDep](CxxPreprocessorDep.html "interface in com.facebook.buck.cxx"),
        com.facebook.buck.cxx.toolchain.nativelink.[NativeLinkableGroup](toolchain/nativelink/NativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink"))
-   com.facebook.buck.core.build.action.[[BuildEngineAction]{.typeNameLink}](../core/build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")
    -   com.facebook.buck.core.rules.[[BuildRule]{.typeNameLink}](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
        (also extends
        com.facebook.buck.core.rulekey.[AllowsNonAnnotatedFields](../core/rulekey/AllowsNonAnnotatedFields.html "interface in com.facebook.buck.core.rulekey"),
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        com.facebook.buck.core.rules.[HasNameAndType](../core/rules/HasNameAndType.html "interface in com.facebook.buck.core.rules"))
        -   com.facebook.buck.cxx.[[CxxIntermediateBuildProduct]{.typeNameLink}](CxxIntermediateBuildProduct.html "interface in com.facebook.buck.cxx")
        -   com.facebook.buck.cxx.[[HasAppleDebugSymbolDeps]{.typeNameLink}](HasAppleDebugSymbolDeps.html "interface in com.facebook.buck.cxx")
-   java.lang.[[Comparable]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>
    -   com.facebook.buck.core.rules.[[BuildRule]{.typeNameLink}](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
        (also extends
        com.facebook.buck.core.rulekey.[AllowsNonAnnotatedFields](../core/rulekey/AllowsNonAnnotatedFields.html "interface in com.facebook.buck.core.rulekey"),
        com.facebook.buck.core.build.action.[BuildEngineAction](../core/build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action"),
        com.facebook.buck.core.rules.[HasNameAndType](../core/rules/HasNameAndType.html "interface in com.facebook.buck.core.rules"))
        -   com.facebook.buck.cxx.[[CxxIntermediateBuildProduct]{.typeNameLink}](CxxIntermediateBuildProduct.html "interface in com.facebook.buck.cxx")
        -   com.facebook.buck.cxx.[[HasAppleDebugSymbolDeps]{.typeNameLink}](HasAppleDebugSymbolDeps.html "interface in com.facebook.buck.cxx")
-   com.facebook.buck.cxx.[[CxxLibraryDescription.TransitiveCxxPreprocessorInputFunction]{.typeNameLink}](CxxLibraryDescription.TransitiveCxxPreprocessorInputFunction.html "interface in com.facebook.buck.cxx")
-   com.facebook.buck.cxx.[[CxxLibraryDescriptionDelegate]{.typeNameLink}](CxxLibraryDescriptionDelegate.html "interface in com.facebook.buck.cxx")
-   com.facebook.buck.cxx.[[CxxLibraryDescriptionDelegate.ConfiguredDelegate]{.typeNameLink}](CxxLibraryDescriptionDelegate.ConfiguredDelegate.html "interface in com.facebook.buck.cxx")
-   com.facebook.buck.cxx.[[CxxPreprocessorDep]{.typeNameLink}](CxxPreprocessorDep.html "interface in com.facebook.buck.cxx")
    -   com.facebook.buck.cxx.[[AbstractCxxLibraryGroup]{.typeNameLink}](AbstractCxxLibraryGroup.html "interface in com.facebook.buck.cxx")
        (also extends
        com.facebook.buck.android.packageable.[AndroidPackageable](../android/packageable/AndroidPackageable.html "interface in com.facebook.buck.android.packageable"),
        com.facebook.buck.cxx.toolchain.nativelink.[NativeLinkableGroup](toolchain/nativelink/NativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink"))
-   com.facebook.buck.core.description.arg.[[DataTransferObject]{.typeNameLink}](../core/description/arg/DataTransferObject.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.core.description.arg.[[ConstructorArg]{.typeNameLink}](../core/description/arg/ConstructorArg.html "interface in com.facebook.buck.core.description.arg")
        -   com.facebook.buck.core.description.arg.[[BuildRuleArg]{.typeNameLink}](../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")
            -   com.facebook.buck.cxx.[[CxxConstructorArg]{.typeNameLink}](CxxConstructorArg.html "interface in com.facebook.buck.cxx")
                (also extends
                com.facebook.buck.core.description.arg.[HasDeclaredDeps](../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg"),
                com.facebook.buck.core.model.[HasDefaultFlavors](../core/model/HasDefaultFlavors.html "interface in com.facebook.buck.core.model"),
                com.facebook.buck.core.description.arg.[HasDefaultPlatform](../core/description/arg/HasDefaultPlatform.html "interface in com.facebook.buck.core.description.arg"),
                com.facebook.buck.cxx.toolchain.[HasSystemFrameworkAndLibraries](toolchain/HasSystemFrameworkAndLibraries.html "interface in com.facebook.buck.cxx.toolchain"),
                com.facebook.buck.core.description.arg.[HasTests](../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg"))
                -   com.facebook.buck.cxx.[[LinkableCxxConstructorArg]{.typeNameLink}](LinkableCxxConstructorArg.html "interface in com.facebook.buck.cxx")
                    -   com.facebook.buck.cxx.[[CxxBinaryDescription.CommonArg]{.typeNameLink}](CxxBinaryDescription.CommonArg.html "interface in com.facebook.buck.cxx")
                        (also extends
                        com.facebook.buck.core.description.arg.[HasDepsQuery](../core/description/arg/HasDepsQuery.html "interface in com.facebook.buck.core.description.arg"),
                        com.facebook.buck.versions.[HasVersionUniverse](../versions/HasVersionUniverse.html "interface in com.facebook.buck.versions"))
                    -   com.facebook.buck.cxx.[[CxxLibraryDescription.CommonArg]{.typeNameLink}](CxxLibraryDescription.CommonArg.html "interface in com.facebook.buck.cxx")
            -   com.facebook.buck.cxx.toolchain.[[HasSystemFrameworkAndLibraries]{.typeNameLink}](toolchain/HasSystemFrameworkAndLibraries.html "interface in com.facebook.buck.cxx.toolchain")
                -   com.facebook.buck.cxx.[[CxxConstructorArg]{.typeNameLink}](CxxConstructorArg.html "interface in com.facebook.buck.cxx")
                    (also extends
                    com.facebook.buck.core.description.arg.[BuildRuleArg](../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg"),
                    com.facebook.buck.core.description.arg.[HasDeclaredDeps](../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg"),
                    com.facebook.buck.core.model.[HasDefaultFlavors](../core/model/HasDefaultFlavors.html "interface in com.facebook.buck.core.model"),
                    com.facebook.buck.core.description.arg.[HasDefaultPlatform](../core/description/arg/HasDefaultPlatform.html "interface in com.facebook.buck.core.description.arg"),
                    com.facebook.buck.core.description.arg.[HasTests](../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg"))
                    -   com.facebook.buck.cxx.[[LinkableCxxConstructorArg]{.typeNameLink}](LinkableCxxConstructorArg.html "interface in com.facebook.buck.cxx")
                        -   com.facebook.buck.cxx.[[CxxBinaryDescription.CommonArg]{.typeNameLink}](CxxBinaryDescription.CommonArg.html "interface in com.facebook.buck.cxx")
                            (also extends
                            com.facebook.buck.core.description.arg.[HasDepsQuery](../core/description/arg/HasDepsQuery.html "interface in com.facebook.buck.core.description.arg"),
                            com.facebook.buck.versions.[HasVersionUniverse](../versions/HasVersionUniverse.html "interface in com.facebook.buck.versions"))
                        -   com.facebook.buck.cxx.[[CxxLibraryDescription.CommonArg]{.typeNameLink}](CxxLibraryDescription.CommonArg.html "interface in com.facebook.buck.cxx")
-   com.facebook.buck.core.description.arg.[[HasDeclaredDeps]{.typeNameLink}](../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.cxx.[[CxxConstructorArg]{.typeNameLink}](CxxConstructorArg.html "interface in com.facebook.buck.cxx")
        (also extends
        com.facebook.buck.core.description.arg.[BuildRuleArg](../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.model.[HasDefaultFlavors](../core/model/HasDefaultFlavors.html "interface in com.facebook.buck.core.model"),
        com.facebook.buck.core.description.arg.[HasDefaultPlatform](../core/description/arg/HasDefaultPlatform.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.cxx.toolchain.[HasSystemFrameworkAndLibraries](toolchain/HasSystemFrameworkAndLibraries.html "interface in com.facebook.buck.cxx.toolchain"),
        com.facebook.buck.core.description.arg.[HasTests](../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg"))
        -   com.facebook.buck.cxx.[[LinkableCxxConstructorArg]{.typeNameLink}](LinkableCxxConstructorArg.html "interface in com.facebook.buck.cxx")
            -   com.facebook.buck.cxx.[[CxxBinaryDescription.CommonArg]{.typeNameLink}](CxxBinaryDescription.CommonArg.html "interface in com.facebook.buck.cxx")
                (also extends
                com.facebook.buck.core.description.arg.[HasDepsQuery](../core/description/arg/HasDepsQuery.html "interface in com.facebook.buck.core.description.arg"),
                com.facebook.buck.versions.[HasVersionUniverse](../versions/HasVersionUniverse.html "interface in com.facebook.buck.versions"))
            -   com.facebook.buck.cxx.[[CxxLibraryDescription.CommonArg]{.typeNameLink}](CxxLibraryDescription.CommonArg.html "interface in com.facebook.buck.cxx")
    -   com.facebook.buck.core.description.arg.[[HasDepsQuery]{.typeNameLink}](../core/description/arg/HasDepsQuery.html "interface in com.facebook.buck.core.description.arg")
        -   com.facebook.buck.cxx.[[CxxBinaryDescription.CommonArg]{.typeNameLink}](CxxBinaryDescription.CommonArg.html "interface in com.facebook.buck.cxx")
            (also extends
            com.facebook.buck.versions.[HasVersionUniverse](../versions/HasVersionUniverse.html "interface in com.facebook.buck.versions"),
            com.facebook.buck.cxx.[LinkableCxxConstructorArg](LinkableCxxConstructorArg.html "interface in com.facebook.buck.cxx"))
-   com.facebook.buck.core.model.[[HasDefaultFlavors]{.typeNameLink}](../core/model/HasDefaultFlavors.html "interface in com.facebook.buck.core.model")
    -   com.facebook.buck.cxx.[[CxxConstructorArg]{.typeNameLink}](CxxConstructorArg.html "interface in com.facebook.buck.cxx")
        (also extends
        com.facebook.buck.core.description.arg.[BuildRuleArg](../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasDeclaredDeps](../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasDefaultPlatform](../core/description/arg/HasDefaultPlatform.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.cxx.toolchain.[HasSystemFrameworkAndLibraries](toolchain/HasSystemFrameworkAndLibraries.html "interface in com.facebook.buck.cxx.toolchain"),
        com.facebook.buck.core.description.arg.[HasTests](../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg"))
        -   com.facebook.buck.cxx.[[LinkableCxxConstructorArg]{.typeNameLink}](LinkableCxxConstructorArg.html "interface in com.facebook.buck.cxx")
            -   com.facebook.buck.cxx.[[CxxBinaryDescription.CommonArg]{.typeNameLink}](CxxBinaryDescription.CommonArg.html "interface in com.facebook.buck.cxx")
                (also extends
                com.facebook.buck.core.description.arg.[HasDepsQuery](../core/description/arg/HasDepsQuery.html "interface in com.facebook.buck.core.description.arg"),
                com.facebook.buck.versions.[HasVersionUniverse](../versions/HasVersionUniverse.html "interface in com.facebook.buck.versions"))
            -   com.facebook.buck.cxx.[[CxxLibraryDescription.CommonArg]{.typeNameLink}](CxxLibraryDescription.CommonArg.html "interface in com.facebook.buck.cxx")
-   com.facebook.buck.core.description.arg.[[HasDefaultPlatform]{.typeNameLink}](../core/description/arg/HasDefaultPlatform.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.cxx.[[CxxConstructorArg]{.typeNameLink}](CxxConstructorArg.html "interface in com.facebook.buck.cxx")
        (also extends
        com.facebook.buck.core.description.arg.[BuildRuleArg](../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasDeclaredDeps](../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.model.[HasDefaultFlavors](../core/model/HasDefaultFlavors.html "interface in com.facebook.buck.core.model"),
        com.facebook.buck.cxx.toolchain.[HasSystemFrameworkAndLibraries](toolchain/HasSystemFrameworkAndLibraries.html "interface in com.facebook.buck.cxx.toolchain"),
        com.facebook.buck.core.description.arg.[HasTests](../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg"))
        -   com.facebook.buck.cxx.[[LinkableCxxConstructorArg]{.typeNameLink}](LinkableCxxConstructorArg.html "interface in com.facebook.buck.cxx")
            -   com.facebook.buck.cxx.[[CxxBinaryDescription.CommonArg]{.typeNameLink}](CxxBinaryDescription.CommonArg.html "interface in com.facebook.buck.cxx")
                (also extends
                com.facebook.buck.core.description.arg.[HasDepsQuery](../core/description/arg/HasDepsQuery.html "interface in com.facebook.buck.core.description.arg"),
                com.facebook.buck.versions.[HasVersionUniverse](../versions/HasVersionUniverse.html "interface in com.facebook.buck.versions"))
            -   com.facebook.buck.cxx.[[CxxLibraryDescription.CommonArg]{.typeNameLink}](CxxLibraryDescription.CommonArg.html "interface in com.facebook.buck.cxx")
-   com.facebook.buck.core.rules.[[HasNameAndType]{.typeNameLink}](../core/rules/HasNameAndType.html "interface in com.facebook.buck.core.rules")
    -   com.facebook.buck.core.rules.[[BuildRule]{.typeNameLink}](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
        (also extends
        com.facebook.buck.core.rulekey.[AllowsNonAnnotatedFields](../core/rulekey/AllowsNonAnnotatedFields.html "interface in com.facebook.buck.core.rulekey"),
        com.facebook.buck.core.build.action.[BuildEngineAction](../core/build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action"),
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>)
        -   com.facebook.buck.cxx.[[CxxIntermediateBuildProduct]{.typeNameLink}](CxxIntermediateBuildProduct.html "interface in com.facebook.buck.cxx")
        -   com.facebook.buck.cxx.[[HasAppleDebugSymbolDeps]{.typeNameLink}](HasAppleDebugSymbolDeps.html "interface in com.facebook.buck.cxx")
-   com.facebook.buck.core.description.arg.[[HasTests]{.typeNameLink}](../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.cxx.[[CxxConstructorArg]{.typeNameLink}](CxxConstructorArg.html "interface in com.facebook.buck.cxx")
        (also extends
        com.facebook.buck.core.description.arg.[BuildRuleArg](../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasDeclaredDeps](../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.model.[HasDefaultFlavors](../core/model/HasDefaultFlavors.html "interface in com.facebook.buck.core.model"),
        com.facebook.buck.core.description.arg.[HasDefaultPlatform](../core/description/arg/HasDefaultPlatform.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.cxx.toolchain.[HasSystemFrameworkAndLibraries](toolchain/HasSystemFrameworkAndLibraries.html "interface in com.facebook.buck.cxx.toolchain"))
        -   com.facebook.buck.cxx.[[LinkableCxxConstructorArg]{.typeNameLink}](LinkableCxxConstructorArg.html "interface in com.facebook.buck.cxx")
            -   com.facebook.buck.cxx.[[CxxBinaryDescription.CommonArg]{.typeNameLink}](CxxBinaryDescription.CommonArg.html "interface in com.facebook.buck.cxx")
                (also extends
                com.facebook.buck.core.description.arg.[HasDepsQuery](../core/description/arg/HasDepsQuery.html "interface in com.facebook.buck.core.description.arg"),
                com.facebook.buck.versions.[HasVersionUniverse](../versions/HasVersionUniverse.html "interface in com.facebook.buck.versions"))
            -   com.facebook.buck.cxx.[[CxxLibraryDescription.CommonArg]{.typeNameLink}](CxxLibraryDescription.CommonArg.html "interface in com.facebook.buck.cxx")
-   com.facebook.buck.versions.[[HasVersionUniverse]{.typeNameLink}](../versions/HasVersionUniverse.html "interface in com.facebook.buck.versions")
    -   com.facebook.buck.cxx.[[CxxBinaryDescription.CommonArg]{.typeNameLink}](CxxBinaryDescription.CommonArg.html "interface in com.facebook.buck.cxx")
        (also extends
        com.facebook.buck.core.description.arg.[HasDepsQuery](../core/description/arg/HasDepsQuery.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.cxx.[LinkableCxxConstructorArg](LinkableCxxConstructorArg.html "interface in com.facebook.buck.cxx"))
-   com.facebook.buck.cxx.toolchain.nativelink.[[NativeLinkableGroup]{.typeNameLink}](toolchain/nativelink/NativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink")
    -   com.facebook.buck.cxx.[[AbstractCxxLibraryGroup]{.typeNameLink}](AbstractCxxLibraryGroup.html "interface in com.facebook.buck.cxx")
        (also extends
        com.facebook.buck.android.packageable.[AndroidPackageable](../android/packageable/AndroidPackageable.html "interface in com.facebook.buck.android.packageable"),
        com.facebook.buck.cxx.[CxxPreprocessorDep](CxxPreprocessorDep.html "interface in com.facebook.buck.cxx"))
-   com.facebook.buck.cxx.[[NativeTestable]{.typeNameLink}](NativeTestable.html "interface in com.facebook.buck.cxx")
-   com.facebook.buck.cxx.[[Omnibus.OmnibusLibrary]{.typeNameLink}](Omnibus.OmnibusLibrary.html "interface in com.facebook.buck.cxx")
-   com.facebook.buck.cxx.[[Omnibus.OmnibusRoot]{.typeNameLink}](Omnibus.OmnibusRoot.html "interface in com.facebook.buck.cxx")
-   com.facebook.buck.cxx.[[UntrackedHeaderReporter]{.typeNameLink}](UntrackedHeaderReporter.html "interface in com.facebook.buck.cxx")
:::

::: {.section role="region"}
## Enum Hierarchy {#enum-hierarchy title="Enum Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   java.lang.[[Enum]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<E\>
        (implements
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   com.facebook.buck.cxx.[[CxxInferEnhancer.InferFlavors]{.typeNameLink}](CxxInferEnhancer.InferFlavors.html "enum in com.facebook.buck.cxx")
            (implements
            com.facebook.buck.core.model.[FlavorConvertible](../core/model/FlavorConvertible.html "interface in com.facebook.buck.core.model"))
        -   com.facebook.buck.cxx.[[CxxLibraryDescription.MetadataType]{.typeNameLink}](CxxLibraryDescription.MetadataType.html "enum in com.facebook.buck.cxx")
            (implements
            com.facebook.buck.core.model.[FlavorConvertible](../core/model/FlavorConvertible.html "interface in com.facebook.buck.core.model"))
        -   com.facebook.buck.cxx.[[CxxLibraryDescription.Type]{.typeNameLink}](CxxLibraryDescription.Type.html "enum in com.facebook.buck.cxx")
            (implements
            com.facebook.buck.core.model.[FlavorConvertible](../core/model/FlavorConvertible.html "interface in com.facebook.buck.core.model"))
        -   com.facebook.buck.cxx.[[CxxPreprocessables.IncludeType]{.typeNameLink}](CxxPreprocessables.IncludeType.html "enum in com.facebook.buck.cxx")
        -   com.facebook.buck.cxx.[[CxxSource.Type]{.typeNameLink}](CxxSource.Type.html "enum in com.facebook.buck.cxx")
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
