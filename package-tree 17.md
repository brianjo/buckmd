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
-   Tree
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Hierarchy For Package com.facebook.buck.cxx.toolchain {#hierarchy-for-package-com.facebook.buck.cxx.toolchain .title}

[Package Hierarchies:]{.packageHierarchyLabel}

-   [All Packages](../../../../../overview-tree.html)
:::

::: contentContainer
::: {.section role="region"}
## Class Hierarchy {#class-hierarchy title="Class Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   com.facebook.buck.core.rules.impl.[[AbstractBuildRule]{.typeNameLink}](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")
        (implements
        com.facebook.buck.core.rules.[BuildRule](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules"))
        -   com.facebook.buck.core.rules.impl.[[SymlinkTree]{.typeNameLink}](../../core/rules/impl/SymlinkTree.html "class in com.facebook.buck.core.rules.impl")
            (implements
            com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"),
            com.facebook.buck.core.rules.attr.[SupportsInputBasedRuleKey](../../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr"))
            -   com.facebook.buck.core.rules.impl.[[MappedSymlinkTree]{.typeNameLink}](../../core/rules/impl/MappedSymlinkTree.html "class in com.facebook.buck.core.rules.impl")
                -   com.facebook.buck.cxx.toolchain.[[HeaderSymlinkTree]{.typeNameLink}](HeaderSymlinkTree.html "class in com.facebook.buck.cxx.toolchain")
                    -   com.facebook.buck.cxx.toolchain.[[HeaderSymlinkTreeWithModuleMap]{.typeNameLink}](HeaderSymlinkTreeWithModuleMap.html "class in com.facebook.buck.cxx.toolchain")
    -   com.facebook.buck.cxx.toolchain.[[BuildRuleResolverCacheByTargetConfiguration]{.typeNameLink}](BuildRuleResolverCacheByTargetConfiguration.html "class in com.facebook.buck.cxx.toolchain")\<T\>
    -   com.facebook.buck.cxx.toolchain.[[CxxFlavorSanitizer]{.typeNameLink}](CxxFlavorSanitizer.html "class in com.facebook.buck.cxx.toolchain")
    -   com.facebook.buck.cxx.toolchain.[[CxxPlatformsProvider]{.typeNameLink}](CxxPlatformsProvider.html "class in com.facebook.buck.cxx.toolchain")
        (implements
        com.facebook.buck.core.toolchain.[Toolchain](../../core/toolchain/Toolchain.html "interface in com.facebook.buck.core.toolchain"))
    -   com.facebook.buck.cxx.toolchain.[[CxxToolProvider]{.typeNameLink}](CxxToolProvider.html "class in com.facebook.buck.cxx.toolchain")\<T\>
        -   com.facebook.buck.cxx.toolchain.[[CompilerProvider]{.typeNameLink}](CompilerProvider.html "class in com.facebook.buck.cxx.toolchain")
        -   com.facebook.buck.cxx.toolchain.[[PreprocessorProvider]{.typeNameLink}](PreprocessorProvider.html "class in com.facebook.buck.cxx.toolchain")
    -   com.facebook.buck.cxx.toolchain.[[CxxToolTypeInferer]{.typeNameLink}](CxxToolTypeInferer.html "class in com.facebook.buck.cxx.toolchain")
    -   com.facebook.buck.cxx.toolchain.[[DebugPathSanitizer]{.typeNameLink}](DebugPathSanitizer.html "class in com.facebook.buck.cxx.toolchain")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"))
        -   com.facebook.buck.cxx.toolchain.[[PrefixMapDebugPathSanitizer]{.typeNameLink}](PrefixMapDebugPathSanitizer.html "class in com.facebook.buck.cxx.toolchain")
    -   com.facebook.buck.core.toolchain.tool.[[DelegatingTool]{.typeNameLink}](../../core/toolchain/tool/DelegatingTool.html "class in com.facebook.buck.core.toolchain.tool")
        (implements
        com.facebook.buck.core.toolchain.tool.[Tool](../../core/toolchain/tool/Tool.html "interface in com.facebook.buck.core.toolchain.tool"))
        -   com.facebook.buck.cxx.toolchain.[[BsdArchiver]{.typeNameLink}](BsdArchiver.html "class in com.facebook.buck.cxx.toolchain")
            (implements
            com.facebook.buck.cxx.toolchain.[Archiver](Archiver.html "interface in com.facebook.buck.cxx.toolchain"))
        -   com.facebook.buck.cxx.toolchain.[[ClangPreprocessor]{.typeNameLink}](ClangPreprocessor.html "class in com.facebook.buck.cxx.toolchain")
            (implements
            com.facebook.buck.cxx.toolchain.[Preprocessor](Preprocessor.html "interface in com.facebook.buck.cxx.toolchain"))
            -   com.facebook.buck.cxx.toolchain.[[ClangWindowsPreprocessor]{.typeNameLink}](ClangWindowsPreprocessor.html "class in com.facebook.buck.cxx.toolchain")
                (implements
                com.facebook.buck.cxx.toolchain.[Preprocessor](Preprocessor.html "interface in com.facebook.buck.cxx.toolchain"))
        -   com.facebook.buck.cxx.toolchain.[[ClangWindowsArchiver]{.typeNameLink}](ClangWindowsArchiver.html "class in com.facebook.buck.cxx.toolchain")
            (implements
            com.facebook.buck.cxx.toolchain.[Archiver](Archiver.html "interface in com.facebook.buck.cxx.toolchain"))
        -   com.facebook.buck.cxx.toolchain.[[DefaultCompiler]{.typeNameLink}](DefaultCompiler.html "class in com.facebook.buck.cxx.toolchain")
            (implements
            com.facebook.buck.cxx.toolchain.[Compiler](Compiler.html "interface in com.facebook.buck.cxx.toolchain"))
            -   com.facebook.buck.cxx.toolchain.[[ClangCompiler]{.typeNameLink}](ClangCompiler.html "class in com.facebook.buck.cxx.toolchain")
                -   com.facebook.buck.cxx.toolchain.[[ClangWindowsCompiler]{.typeNameLink}](ClangWindowsCompiler.html "class in com.facebook.buck.cxx.toolchain")
            -   com.facebook.buck.cxx.toolchain.[[GccCompiler]{.typeNameLink}](GccCompiler.html "class in com.facebook.buck.cxx.toolchain")
            -   com.facebook.buck.cxx.toolchain.[[WindowsCompiler]{.typeNameLink}](WindowsCompiler.html "class in com.facebook.buck.cxx.toolchain")
                -   com.facebook.buck.cxx.toolchain.[[ClangClCompiler]{.typeNameLink}](ClangClCompiler.html "class in com.facebook.buck.cxx.toolchain")
            -   com.facebook.buck.cxx.toolchain.[[WindowsMl64Compiler]{.typeNameLink}](WindowsMl64Compiler.html "class in com.facebook.buck.cxx.toolchain")
        -   com.facebook.buck.cxx.toolchain.[[GccPreprocessor]{.typeNameLink}](GccPreprocessor.html "class in com.facebook.buck.cxx.toolchain")
            (implements
            com.facebook.buck.cxx.toolchain.[Preprocessor](Preprocessor.html "interface in com.facebook.buck.cxx.toolchain"))
        -   com.facebook.buck.cxx.toolchain.[[GnuArchiver]{.typeNameLink}](GnuArchiver.html "class in com.facebook.buck.cxx.toolchain")
            (implements
            com.facebook.buck.cxx.toolchain.[Archiver](Archiver.html "interface in com.facebook.buck.cxx.toolchain"))
        -   com.facebook.buck.cxx.toolchain.[[WindowsArchiver]{.typeNameLink}](WindowsArchiver.html "class in com.facebook.buck.cxx.toolchain")
            (implements
            com.facebook.buck.cxx.toolchain.[Archiver](Archiver.html "interface in com.facebook.buck.cxx.toolchain"))
        -   com.facebook.buck.cxx.toolchain.[[WindowsPreprocessor]{.typeNameLink}](WindowsPreprocessor.html "class in com.facebook.buck.cxx.toolchain")
            (implements
            com.facebook.buck.cxx.toolchain.[Preprocessor](Preprocessor.html "interface in com.facebook.buck.cxx.toolchain"))
            -   com.facebook.buck.cxx.toolchain.[[ClangClPreprocessor]{.typeNameLink}](ClangClPreprocessor.html "class in com.facebook.buck.cxx.toolchain")
                (implements
                com.facebook.buck.cxx.toolchain.[Preprocessor](Preprocessor.html "interface in com.facebook.buck.cxx.toolchain"))
    -   com.facebook.buck.cxx.toolchain.[[ElfSharedLibraryInterfaceParams]{.typeNameLink}](ElfSharedLibraryInterfaceParams.html "class in com.facebook.buck.cxx.toolchain")
        (implements
        com.facebook.buck.cxx.toolchain.[SharedLibraryInterfaceParams](SharedLibraryInterfaceParams.html "interface in com.facebook.buck.cxx.toolchain"))
    -   com.facebook.buck.cxx.toolchain.[[FasterPattern]{.typeNameLink}](FasterPattern.html "class in com.facebook.buck.cxx.toolchain")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"))
    -   com.facebook.buck.cxx.toolchain.[[HeaderVerification]{.typeNameLink}](HeaderVerification.html "class in com.facebook.buck.cxx.toolchain")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"))
    -   com.facebook.buck.cxx.toolchain.ImmutableCxxPlatform.Builder
        -   com.facebook.buck.cxx.toolchain.[[CxxPlatform.Builder]{.typeNameLink}](CxxPlatform.Builder.html "class in com.facebook.buck.cxx.toolchain")
    -   com.facebook.buck.cxx.toolchain.[[InferBuckConfig]{.typeNameLink}](InferBuckConfig.html "class in com.facebook.buck.cxx.toolchain")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"))
    -   com.facebook.buck.cxx.toolchain.[[MachoDylibStubParams]{.typeNameLink}](MachoDylibStubParams.html "class in com.facebook.buck.cxx.toolchain")
        (implements
        com.facebook.buck.cxx.toolchain.[SharedLibraryInterfaceParams](SharedLibraryInterfaceParams.html "interface in com.facebook.buck.cxx.toolchain"))
    -   com.facebook.buck.cxx.toolchain.[[PosixNmSymbolNameTool]{.typeNameLink}](PosixNmSymbolNameTool.html "class in com.facebook.buck.cxx.toolchain")
        (implements
        com.facebook.buck.cxx.toolchain.[SymbolNameTool](SymbolNameTool.html "interface in com.facebook.buck.cxx.toolchain"))
    -   com.facebook.buck.cxx.toolchain.[[ProviderBasedUnresolvedCxxPlatform]{.typeNameLink}](ProviderBasedUnresolvedCxxPlatform.html "class in com.facebook.buck.cxx.toolchain")
        (implements
        com.facebook.buck.cxx.toolchain.[ProviderBackedCxxPlatform](ProviderBackedCxxPlatform.html "interface in com.facebook.buck.cxx.toolchain"),
        com.facebook.buck.cxx.toolchain.[UnresolvedCxxPlatform](UnresolvedCxxPlatform.html "interface in com.facebook.buck.cxx.toolchain"))
:::

::: {.section role="region"}
## Interface Hierarchy {#interface-hierarchy title="Interface Hierarchy"}

-   com.facebook.buck.core.rulekey.[[AddsToRuleKey]{.typeNameLink}](../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey")
    -   com.facebook.buck.core.toolchain.tool.[[Tool]{.typeNameLink}](../../core/toolchain/tool/Tool.html "interface in com.facebook.buck.core.toolchain.tool")
        -   com.facebook.buck.cxx.toolchain.[[Archiver]{.typeNameLink}](Archiver.html "interface in com.facebook.buck.cxx.toolchain")
        -   com.facebook.buck.cxx.toolchain.[[Compiler]{.typeNameLink}](Compiler.html "interface in com.facebook.buck.cxx.toolchain")
        -   com.facebook.buck.cxx.toolchain.[[Preprocessor]{.typeNameLink}](Preprocessor.html "interface in com.facebook.buck.cxx.toolchain")
-   com.facebook.buck.cxx.toolchain.[[ArchiverProvider]{.typeNameLink}](ArchiverProvider.html "interface in com.facebook.buck.cxx.toolchain")
-   com.facebook.buck.core.description.arg.[[DataTransferObject]{.typeNameLink}](../../core/description/arg/DataTransferObject.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.core.description.arg.[[ConstructorArg]{.typeNameLink}](../../core/description/arg/ConstructorArg.html "interface in com.facebook.buck.core.description.arg")
        -   com.facebook.buck.core.description.arg.[[BuildRuleArg]{.typeNameLink}](../../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")
            -   com.facebook.buck.cxx.toolchain.[[HasSystemFrameworkAndLibraries]{.typeNameLink}](HasSystemFrameworkAndLibraries.html "interface in com.facebook.buck.cxx.toolchain")
-   com.facebook.buck.core.model.[[FlavorConvertible]{.typeNameLink}](../../core/model/FlavorConvertible.html "interface in com.facebook.buck.core.model")
    -   com.facebook.buck.cxx.toolchain.[[CxxPlatform]{.typeNameLink}](CxxPlatform.html "interface in com.facebook.buck.cxx.toolchain")
    -   com.facebook.buck.cxx.toolchain.[[UnresolvedCxxPlatform]{.typeNameLink}](UnresolvedCxxPlatform.html "interface in com.facebook.buck.cxx.toolchain")
-   com.facebook.buck.cxx.toolchain.[[PathShortener]{.typeNameLink}](PathShortener.html "interface in com.facebook.buck.cxx.toolchain")
-   com.facebook.buck.cxx.toolchain.[[ProviderBackedCxxPlatform]{.typeNameLink}](ProviderBackedCxxPlatform.html "interface in com.facebook.buck.cxx.toolchain")
-   com.facebook.buck.cxx.toolchain.[[ProvidesCxxPlatform]{.typeNameLink}](ProvidesCxxPlatform.html "interface in com.facebook.buck.cxx.toolchain")
-   com.facebook.buck.cxx.toolchain.[[SharedLibraryInterfaceFactory]{.typeNameLink}](SharedLibraryInterfaceFactory.html "interface in com.facebook.buck.cxx.toolchain")
-   com.facebook.buck.cxx.toolchain.[[SharedLibraryInterfaceParams]{.typeNameLink}](SharedLibraryInterfaceParams.html "interface in com.facebook.buck.cxx.toolchain")
-   com.facebook.buck.cxx.toolchain.[[SymbolNameTool]{.typeNameLink}](SymbolNameTool.html "interface in com.facebook.buck.cxx.toolchain")
-   com.facebook.buck.core.toolchain.[[Toolchain]{.typeNameLink}](../../core/toolchain/Toolchain.html "interface in com.facebook.buck.core.toolchain")
    -   com.facebook.buck.core.toolchain.[[ToolchainWithCapability]{.typeNameLink}](../../core/toolchain/ToolchainWithCapability.html "interface in com.facebook.buck.core.toolchain")
        -   com.facebook.buck.cxx.toolchain.[[CxxPlatformsSupplier]{.typeNameLink}](CxxPlatformsSupplier.html "interface in com.facebook.buck.cxx.toolchain")
:::

::: {.section role="region"}
## Enum Hierarchy {#enum-hierarchy title="Enum Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   java.lang.[[Enum]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<E\>
        (implements
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   com.facebook.buck.cxx.toolchain.[[ArchiveContents]{.typeNameLink}](ArchiveContents.html "enum in com.facebook.buck.cxx.toolchain")
        -   com.facebook.buck.cxx.toolchain.[[ArchiverProvider.LegacyArchiverType]{.typeNameLink}](ArchiverProvider.LegacyArchiverType.html "enum in com.facebook.buck.cxx.toolchain")
        -   com.facebook.buck.cxx.toolchain.[[ArchiverProvider.Type]{.typeNameLink}](ArchiverProvider.Type.html "enum in com.facebook.buck.cxx.toolchain")
        -   com.facebook.buck.cxx.toolchain.[[CxxToolProvider.Type]{.typeNameLink}](CxxToolProvider.Type.html "enum in com.facebook.buck.cxx.toolchain")
        -   com.facebook.buck.cxx.toolchain.[[DependencyTrackingMode]{.typeNameLink}](DependencyTrackingMode.html "enum in com.facebook.buck.cxx.toolchain")
        -   com.facebook.buck.cxx.toolchain.[[HeaderMode]{.typeNameLink}](HeaderMode.html "enum in com.facebook.buck.cxx.toolchain")
            (implements
            com.facebook.buck.core.model.[FlavorConvertible](../../core/model/FlavorConvertible.html "interface in com.facebook.buck.core.model"))
        -   com.facebook.buck.cxx.toolchain.[[HeaderVerification.Mode]{.typeNameLink}](HeaderVerification.Mode.html "enum in com.facebook.buck.cxx.toolchain")
        -   com.facebook.buck.cxx.toolchain.[[HeaderVisibility]{.typeNameLink}](HeaderVisibility.html "enum in com.facebook.buck.cxx.toolchain")
            (implements
            com.facebook.buck.core.model.[FlavorConvertible](../../core/model/FlavorConvertible.html "interface in com.facebook.buck.core.model"))
        -   com.facebook.buck.cxx.toolchain.[[LinkerMapMode]{.typeNameLink}](LinkerMapMode.html "enum in com.facebook.buck.cxx.toolchain")
            (implements
            com.facebook.buck.core.model.[FlavorConvertible](../../core/model/FlavorConvertible.html "interface in com.facebook.buck.core.model"))
        -   com.facebook.buck.cxx.toolchain.[[PicType]{.typeNameLink}](PicType.html "enum in com.facebook.buck.cxx.toolchain")
        -   com.facebook.buck.cxx.toolchain.[[SharedLibraryInterfaceParams.Kind]{.typeNameLink}](SharedLibraryInterfaceParams.Kind.html "enum in com.facebook.buck.cxx.toolchain")
        -   com.facebook.buck.cxx.toolchain.[[SharedLibraryInterfaceParams.Type]{.typeNameLink}](SharedLibraryInterfaceParams.Type.html "enum in com.facebook.buck.cxx.toolchain")
        -   com.facebook.buck.cxx.toolchain.[[StripStyle]{.typeNameLink}](StripStyle.html "enum in com.facebook.buck.cxx.toolchain")
            (implements
            com.facebook.buck.core.model.[FlavorConvertible](../../core/model/FlavorConvertible.html "interface in com.facebook.buck.core.model"))
        -   com.facebook.buck.cxx.toolchain.[[ToolType]{.typeNameLink}](ToolType.html "enum in com.facebook.buck.cxx.toolchain")
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
-   Tree
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

[]{#skip.navbar.bottom}
:::
