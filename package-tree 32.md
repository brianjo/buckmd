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
# Hierarchy For Package com.facebook.buck.features.haskell {#hierarchy-for-package-com.facebook.buck.features.haskell .title}

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
        -   com.facebook.buck.core.rules.impl.[[AbstractBuildRuleWithDeclaredAndExtraDeps]{.typeNameLink}](../../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")
            (implements
            com.facebook.buck.core.rules.attr.[HasDeclaredAndExtraDeps](../../core/rules/attr/HasDeclaredAndExtraDeps.html "interface in com.facebook.buck.core.rules.attr"))
            -   com.facebook.buck.core.rules.tool.[[BinaryWrapperRule]{.typeNameLink}](../../core/rules/tool/BinaryWrapperRule.html "class in com.facebook.buck.core.rules.tool")
                (implements
                com.facebook.buck.core.rules.tool.[BinaryBuildRule](../../core/rules/tool/BinaryBuildRule.html "interface in com.facebook.buck.core.rules.tool"),
                com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"))
                -   com.facebook.buck.features.haskell.[[HaskellBinary]{.typeNameLink}](HaskellBinary.html "class in com.facebook.buck.features.haskell")
            -   com.facebook.buck.features.haskell.[[HaskellCompileRule]{.typeNameLink}](HaskellCompileRule.html "class in com.facebook.buck.features.haskell")
            -   com.facebook.buck.features.haskell.[[HaskellGhciRule]{.typeNameLink}](HaskellGhciRule.html "class in com.facebook.buck.features.haskell")
                (implements
                com.facebook.buck.core.rules.tool.[BinaryBuildRule](../../core/rules/tool/BinaryBuildRule.html "interface in com.facebook.buck.core.rules.tool"))
            -   com.facebook.buck.features.haskell.[[HaskellHaddockLibRule]{.typeNameLink}](HaskellHaddockLibRule.html "class in com.facebook.buck.features.haskell")
            -   com.facebook.buck.features.haskell.[[HaskellHaddockRule]{.typeNameLink}](HaskellHaddockRule.html "class in com.facebook.buck.features.haskell")
            -   com.facebook.buck.features.haskell.[[HaskellLinkRule]{.typeNameLink}](HaskellLinkRule.html "class in com.facebook.buck.features.haskell")
            -   com.facebook.buck.features.haskell.[[HaskellPackageRule]{.typeNameLink}](HaskellPackageRule.html "class in com.facebook.buck.features.haskell")
            -   com.facebook.buck.core.rules.impl.[[NoopBuildRuleWithDeclaredAndExtraDeps]{.typeNameLink}](../../core/rules/impl/NoopBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")
                -   com.facebook.buck.features.haskell.[[HaskellLibrary]{.typeNameLink}](HaskellLibrary.html "class in com.facebook.buck.features.haskell")
                    (implements
                    com.facebook.buck.cxx.[CxxPreprocessorDep](../../cxx/CxxPreprocessorDep.html "interface in com.facebook.buck.cxx"),
                    com.facebook.buck.features.haskell.[HaskellCompileDep](HaskellCompileDep.html "interface in com.facebook.buck.features.haskell"),
                    com.facebook.buck.features.haskell.[HaskellOmnibusLinkable](HaskellOmnibusLinkable.html "interface in com.facebook.buck.features.haskell"),
                    com.facebook.buck.cxx.toolchain.nativelink.[LegacyNativeLinkableGroup](../../cxx/toolchain/nativelink/LegacyNativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink"))
                -   com.facebook.buck.features.haskell.[[PrebuiltHaskellLibrary]{.typeNameLink}](PrebuiltHaskellLibrary.html "class in com.facebook.buck.features.haskell")
                    (implements
                    com.facebook.buck.cxx.[CxxPreprocessorDep](../../cxx/CxxPreprocessorDep.html "interface in com.facebook.buck.cxx"),
                    com.facebook.buck.features.haskell.[HaskellCompileDep](HaskellCompileDep.html "interface in com.facebook.buck.features.haskell"),
                    com.facebook.buck.features.haskell.[HaskellOmnibusLinkable](HaskellOmnibusLinkable.html "interface in com.facebook.buck.features.haskell"),
                    com.facebook.buck.cxx.toolchain.nativelink.[NativeLinkableGroup](../../cxx/toolchain/nativelink/NativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink"))
    -   com.facebook.buck.features.haskell.[[HaskellBinaryDescription]{.typeNameLink}](HaskellBinaryDescription.html "class in com.facebook.buck.features.haskell")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.model.[Flavored](../../core/model/Flavored.html "interface in com.facebook.buck.core.model"),
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>,
        com.facebook.buck.versions.[VersionRoot](../../versions/VersionRoot.html "interface in com.facebook.buck.versions")\<A\>)
    -   com.facebook.buck.features.haskell.[[HaskellBinaryDescriptionArg]{.typeNameLink}](HaskellBinaryDescriptionArg.html "class in com.facebook.buck.features.haskell")
    -   com.facebook.buck.features.haskell.[[HaskellBinaryDescriptionArg.Builder]{.typeNameLink}](HaskellBinaryDescriptionArg.Builder.html "class in com.facebook.buck.features.haskell")
    -   com.facebook.buck.features.haskell.[[HaskellBuckConfig]{.typeNameLink}](HaskellBuckConfig.html "class in com.facebook.buck.features.haskell")
    -   com.facebook.buck.features.haskell.[[HaskellDescriptionsProvider]{.typeNameLink}](HaskellDescriptionsProvider.html "class in com.facebook.buck.features.haskell")
        (implements
        com.facebook.buck.core.model.targetgraph.[DescriptionProvider](../../core/model/targetgraph/DescriptionProvider.html "interface in com.facebook.buck.core.model.targetgraph"))
    -   com.facebook.buck.features.haskell.[[HaskellDescriptionUtils]{.typeNameLink}](HaskellDescriptionUtils.html "class in com.facebook.buck.features.haskell")
    -   com.facebook.buck.features.haskell.[[HaskellGhciDescription]{.typeNameLink}](HaskellGhciDescription.html "class in com.facebook.buck.features.haskell")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>,
        com.facebook.buck.versions.[VersionRoot](../../versions/VersionRoot.html "interface in com.facebook.buck.versions")\<A\>)
    -   com.facebook.buck.features.haskell.[[HaskellGhciDescriptionArg]{.typeNameLink}](HaskellGhciDescriptionArg.html "class in com.facebook.buck.features.haskell")
    -   com.facebook.buck.features.haskell.[[HaskellGhciDescriptionArg.Builder]{.typeNameLink}](HaskellGhciDescriptionArg.Builder.html "class in com.facebook.buck.features.haskell")
    -   com.facebook.buck.features.haskell.[[HaskellHaddockDescription]{.typeNameLink}](HaskellHaddockDescription.html "class in com.facebook.buck.features.haskell")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>,
        com.facebook.buck.versions.[VersionPropagator](../../versions/VersionPropagator.html "interface in com.facebook.buck.versions")\<A\>)
    -   com.facebook.buck.features.haskell.[[HaskellHaddockDescriptionArg]{.typeNameLink}](HaskellHaddockDescriptionArg.html "class in com.facebook.buck.features.haskell")
    -   com.facebook.buck.features.haskell.[[HaskellHaddockDescriptionArg.Builder]{.typeNameLink}](HaskellHaddockDescriptionArg.Builder.html "class in com.facebook.buck.features.haskell")
    -   com.facebook.buck.features.haskell.[[HaskellLibraryDescription]{.typeNameLink}](HaskellLibraryDescription.html "class in com.facebook.buck.features.haskell")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.model.[Flavored](../../core/model/Flavored.html "interface in com.facebook.buck.core.model"),
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>,
        com.facebook.buck.versions.[VersionPropagator](../../versions/VersionPropagator.html "interface in com.facebook.buck.versions")\<A\>)
    -   com.facebook.buck.features.haskell.[[HaskellLibraryDescriptionArg]{.typeNameLink}](HaskellLibraryDescriptionArg.html "class in com.facebook.buck.features.haskell")
    -   com.facebook.buck.features.haskell.[[HaskellLibraryDescriptionArg.Builder]{.typeNameLink}](HaskellLibraryDescriptionArg.Builder.html "class in com.facebook.buck.features.haskell")
    -   com.facebook.buck.features.haskell.[[HaskellModule]{.typeNameLink}](HaskellModule.html "class in com.facebook.buck.features.haskell")
    -   com.facebook.buck.features.haskell.[[HaskellPlatformsFactory]{.typeNameLink}](HaskellPlatformsFactory.html "class in com.facebook.buck.features.haskell")
    -   com.facebook.buck.features.haskell.[[HaskellPlatformsProviderFactory]{.typeNameLink}](HaskellPlatformsProviderFactory.html "class in com.facebook.buck.features.haskell")
        (implements
        com.facebook.buck.core.toolchain.[ToolchainFactory](../../core/toolchain/ToolchainFactory.html "interface in com.facebook.buck.core.toolchain")\<T\>)
    -   com.facebook.buck.features.haskell.[[HaskellPrebuiltLibraryDescription]{.typeNameLink}](HaskellPrebuiltLibraryDescription.html "class in com.facebook.buck.features.haskell")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.versions.[VersionPropagator](../../versions/VersionPropagator.html "interface in com.facebook.buck.versions")\<A\>)
    -   com.facebook.buck.features.haskell.[[HaskellPrebuiltLibraryDescriptionArg]{.typeNameLink}](HaskellPrebuiltLibraryDescriptionArg.html "class in com.facebook.buck.features.haskell")
    -   com.facebook.buck.features.haskell.[[HaskellPrebuiltLibraryDescriptionArg.Builder]{.typeNameLink}](HaskellPrebuiltLibraryDescriptionArg.Builder.html "class in com.facebook.buck.features.haskell")
    -   com.facebook.buck.features.haskell.[[HaskellToolchainSupplier]{.typeNameLink}](HaskellToolchainSupplier.html "class in com.facebook.buck.features.haskell")
        (implements
        com.facebook.buck.core.toolchain.[ToolchainSupplier](../../core/toolchain/ToolchainSupplier.html "interface in com.facebook.buck.core.toolchain"))
    -   org.pf4j.Plugin
        -   com.facebook.buck.features.haskell.[[HaskellModuleAdapterPlugin]{.typeNameLink}](HaskellModuleAdapterPlugin.html "class in com.facebook.buck.features.haskell")
:::

::: {.section role="region"}
## Interface Hierarchy {#interface-hierarchy title="Interface Hierarchy"}

-   com.facebook.buck.features.haskell.[[HaskellCompileDep]{.typeNameLink}](HaskellCompileDep.html "interface in com.facebook.buck.features.haskell")
-   com.facebook.buck.cxx.toolchain.nativelink.[[NativeLinkableGroup]{.typeNameLink}](../../cxx/toolchain/nativelink/NativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink")
    -   com.facebook.buck.features.haskell.[[HaskellOmnibusLinkable]{.typeNameLink}](HaskellOmnibusLinkable.html "interface in com.facebook.buck.features.haskell")
-   com.facebook.buck.core.toolchain.[[Toolchain]{.typeNameLink}](../../core/toolchain/Toolchain.html "interface in com.facebook.buck.core.toolchain")
    -   com.facebook.buck.features.haskell.[[HaskellPlatformsProvider]{.typeNameLink}](HaskellPlatformsProvider.html "interface in com.facebook.buck.features.haskell")
:::

::: {.section role="region"}
## Enum Hierarchy {#enum-hierarchy title="Enum Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   java.lang.[[Enum]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<E\>
        (implements
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   com.facebook.buck.features.haskell.[[HaskellBinaryDescription.Type]{.typeNameLink}](HaskellBinaryDescription.Type.html "enum in com.facebook.buck.features.haskell")
            (implements
            com.facebook.buck.core.model.[FlavorConvertible](../../core/model/FlavorConvertible.html "interface in com.facebook.buck.core.model"))
        -   com.facebook.buck.features.haskell.[[HaskellLibraryDescription.Type]{.typeNameLink}](HaskellLibraryDescription.Type.html "enum in com.facebook.buck.features.haskell")
            (implements
            com.facebook.buck.core.model.[FlavorConvertible](../../core/model/FlavorConvertible.html "interface in com.facebook.buck.core.model"))
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
