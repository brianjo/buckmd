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
# Hierarchy For Package com.facebook.buck.features.rust {#hierarchy-for-package-com.facebook.buck.features.rust .title}

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
            -   com.facebook.buck.core.rules.impl.[[NoopBuildRuleWithDeclaredAndExtraDeps]{.typeNameLink}](../../core/rules/impl/NoopBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")
                -   com.facebook.buck.features.rust.[[RustLibrary]{.typeNameLink}](RustLibrary.html "class in com.facebook.buck.features.rust")
                    (implements
                    com.facebook.buck.cxx.toolchain.nativelink.[LegacyNativeLinkableGroup](../../cxx/toolchain/nativelink/LegacyNativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink"))
            -   com.facebook.buck.features.rust.[[RustTest]{.typeNameLink}](RustTest.html "class in com.facebook.buck.features.rust")
                (implements
                com.facebook.buck.core.rules.tool.[BinaryBuildRule](../../core/rules/tool/BinaryBuildRule.html "interface in com.facebook.buck.core.rules.tool"),
                com.facebook.buck.core.test.rule.[ExternalTestRunnerRule](../../core/test/rule/ExternalTestRunnerRule.html "interface in com.facebook.buck.core.test.rule"),
                com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"),
                com.facebook.buck.core.test.rule.[TestRule](../../core/test/rule/TestRule.html "interface in com.facebook.buck.core.test.rule"))
        -   com.facebook.buck.rules.modern.[[ModernBuildRule]{.typeNameLink}](../../rules/modern/ModernBuildRule.html "class in com.facebook.buck.rules.modern")\<T\>
            (implements
            com.facebook.buck.core.rules.attr.[SupportsInputBasedRuleKey](../../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr"))
            -   com.facebook.buck.features.rust.[[RustCompileRule]{.typeNameLink}](RustCompileRule.html "class in com.facebook.buck.features.rust")
    -   com.facebook.buck.features.rust.[[ConfigBasedUnresolvedRustPlatform]{.typeNameLink}](ConfigBasedUnresolvedRustPlatform.html "class in com.facebook.buck.features.rust")
        (implements
        com.facebook.buck.features.rust.[UnresolvedRustPlatform](UnresolvedRustPlatform.html "interface in com.facebook.buck.features.rust"))
    -   org.pf4j.Plugin
        -   com.facebook.buck.features.rust.[[RustModuleAdapterPlugin]{.typeNameLink}](RustModuleAdapterPlugin.html "class in com.facebook.buck.features.rust")
    -   com.facebook.buck.features.rust.[[PrebuiltRustLibraryDescription]{.typeNameLink}](PrebuiltRustLibraryDescription.html "class in com.facebook.buck.features.rust")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.versions.[VersionPropagator](../../versions/VersionPropagator.html "interface in com.facebook.buck.versions")\<A\>)
    -   com.facebook.buck.features.rust.[[PrebuiltRustLibraryDescriptionArg]{.typeNameLink}](PrebuiltRustLibraryDescriptionArg.html "class in com.facebook.buck.features.rust")
    -   com.facebook.buck.features.rust.[[PrebuiltRustLibraryDescriptionArg.Builder]{.typeNameLink}](PrebuiltRustLibraryDescriptionArg.Builder.html "class in com.facebook.buck.features.rust")
    -   com.facebook.buck.features.rust.[[RustBinaryDescription]{.typeNameLink}](RustBinaryDescription.html "class in com.facebook.buck.features.rust")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.model.[Flavored](../../core/model/Flavored.html "interface in com.facebook.buck.core.model"),
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>,
        com.facebook.buck.versions.[VersionRoot](../../versions/VersionRoot.html "interface in com.facebook.buck.versions")\<A\>)
    -   com.facebook.buck.features.rust.[[RustBinaryDescriptionArg]{.typeNameLink}](RustBinaryDescriptionArg.html "class in com.facebook.buck.features.rust")
    -   com.facebook.buck.features.rust.[[RustBinaryDescriptionArg.Builder]{.typeNameLink}](RustBinaryDescriptionArg.Builder.html "class in com.facebook.buck.features.rust")
    -   com.facebook.buck.features.rust.[[RustBuckConfig]{.typeNameLink}](RustBuckConfig.html "class in com.facebook.buck.features.rust")
    -   com.facebook.buck.features.rust.[[RustCompileUtils]{.typeNameLink}](RustCompileUtils.html "class in com.facebook.buck.features.rust")
    -   com.facebook.buck.features.rust.[[RustDescriptionEnhancer]{.typeNameLink}](RustDescriptionEnhancer.html "class in com.facebook.buck.features.rust")
    -   com.facebook.buck.features.rust.[[RustDescriptionsProvider]{.typeNameLink}](RustDescriptionsProvider.html "class in com.facebook.buck.features.rust")
        (implements
        com.facebook.buck.core.model.targetgraph.[DescriptionProvider](../../core/model/targetgraph/DescriptionProvider.html "interface in com.facebook.buck.core.model.targetgraph"))
    -   com.facebook.buck.features.rust.[[RustLibraryArg]{.typeNameLink}](RustLibraryArg.html "class in com.facebook.buck.features.rust")
        (implements
        com.facebook.buck.rules.args.[Arg](../../rules/args/Arg.html "interface in com.facebook.buck.rules.args"),
        com.facebook.buck.rules.args.[HasSourcePath](../../rules/args/HasSourcePath.html "interface in com.facebook.buck.rules.args"))
    -   com.facebook.buck.features.rust.[[RustLibraryDescription]{.typeNameLink}](RustLibraryDescription.html "class in com.facebook.buck.features.rust")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.model.[Flavored](../../core/model/Flavored.html "interface in com.facebook.buck.core.model"),
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>,
        com.facebook.buck.versions.[VersionPropagator](../../versions/VersionPropagator.html "interface in com.facebook.buck.versions")\<A\>)
    -   com.facebook.buck.features.rust.[[RustLibraryDescriptionArg]{.typeNameLink}](RustLibraryDescriptionArg.html "class in com.facebook.buck.features.rust")
    -   com.facebook.buck.features.rust.[[RustLibraryDescriptionArg.Builder]{.typeNameLink}](RustLibraryDescriptionArg.Builder.html "class in com.facebook.buck.features.rust")
    -   com.facebook.buck.features.rust.[[RustModule]{.typeNameLink}](RustModule.html "class in com.facebook.buck.features.rust")
    -   com.facebook.buck.features.rust.[[RustPlatformFactory]{.typeNameLink}](RustPlatformFactory.html "class in com.facebook.buck.features.rust")
    -   com.facebook.buck.features.rust.[[RustTestDescription]{.typeNameLink}](RustTestDescription.html "class in com.facebook.buck.features.rust")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.model.[Flavored](../../core/model/Flavored.html "interface in com.facebook.buck.core.model"),
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>,
        com.facebook.buck.versions.[VersionRoot](../../versions/VersionRoot.html "interface in com.facebook.buck.versions")\<A\>)
    -   com.facebook.buck.features.rust.[[RustTestDescriptionArg]{.typeNameLink}](RustTestDescriptionArg.html "class in com.facebook.buck.features.rust")
    -   com.facebook.buck.features.rust.[[RustTestDescriptionArg.Builder]{.typeNameLink}](RustTestDescriptionArg.Builder.html "class in com.facebook.buck.features.rust")
    -   com.facebook.buck.features.rust.[[RustToolchainFactory]{.typeNameLink}](RustToolchainFactory.html "class in com.facebook.buck.features.rust")
        (implements
        com.facebook.buck.core.toolchain.[ToolchainFactory](../../core/toolchain/ToolchainFactory.html "interface in com.facebook.buck.core.toolchain")\<T\>)
    -   com.facebook.buck.features.rust.[[RustToolchainSupplier]{.typeNameLink}](RustToolchainSupplier.html "class in com.facebook.buck.features.rust")
        (implements
        com.facebook.buck.core.toolchain.[ToolchainSupplier](../../core/toolchain/ToolchainSupplier.html "interface in com.facebook.buck.core.toolchain"))
:::

::: {.section role="region"}
## Interface Hierarchy {#interface-hierarchy title="Interface Hierarchy"}

-   com.facebook.buck.core.description.arg.[[DataTransferObject]{.typeNameLink}](../../core/description/arg/DataTransferObject.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.core.description.arg.[[ConstructorArg]{.typeNameLink}](../../core/description/arg/ConstructorArg.html "interface in com.facebook.buck.core.description.arg")
        -   com.facebook.buck.core.description.arg.[[BuildRuleArg]{.typeNameLink}](../../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")
            -   com.facebook.buck.features.rust.[[RustCommonArgs]{.typeNameLink}](RustCommonArgs.html "interface in com.facebook.buck.features.rust")
                (also extends
                com.facebook.buck.core.description.arg.[HasDefaultPlatform](../../core/description/arg/HasDefaultPlatform.html "interface in com.facebook.buck.core.description.arg"),
                com.facebook.buck.features.rust.[HasNamedDeclaredDeps](HasNamedDeclaredDeps.html "interface in com.facebook.buck.features.rust"),
                com.facebook.buck.core.description.arg.[HasSrcs](../../core/description/arg/HasSrcs.html "interface in com.facebook.buck.core.description.arg"))
-   com.facebook.buck.core.model.[[FlavorConvertible]{.typeNameLink}](../../core/model/FlavorConvertible.html "interface in com.facebook.buck.core.model")
    -   com.facebook.buck.features.rust.[[UnresolvedRustPlatform]{.typeNameLink}](UnresolvedRustPlatform.html "interface in com.facebook.buck.features.rust")
-   com.facebook.buck.core.description.arg.[[HasDeclaredDeps]{.typeNameLink}](../../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.features.rust.[[HasNamedDeclaredDeps]{.typeNameLink}](HasNamedDeclaredDeps.html "interface in com.facebook.buck.features.rust")
        -   com.facebook.buck.features.rust.[[RustCommonArgs]{.typeNameLink}](RustCommonArgs.html "interface in com.facebook.buck.features.rust")
            (also extends
            com.facebook.buck.core.description.arg.[BuildRuleArg](../../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg"),
            com.facebook.buck.core.description.arg.[HasDefaultPlatform](../../core/description/arg/HasDefaultPlatform.html "interface in com.facebook.buck.core.description.arg"),
            com.facebook.buck.core.description.arg.[HasSrcs](../../core/description/arg/HasSrcs.html "interface in com.facebook.buck.core.description.arg"))
-   com.facebook.buck.core.description.arg.[[HasDefaultPlatform]{.typeNameLink}](../../core/description/arg/HasDefaultPlatform.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.features.rust.[[RustCommonArgs]{.typeNameLink}](RustCommonArgs.html "interface in com.facebook.buck.features.rust")
        (also extends
        com.facebook.buck.core.description.arg.[BuildRuleArg](../../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.features.rust.[HasNamedDeclaredDeps](HasNamedDeclaredDeps.html "interface in com.facebook.buck.features.rust"),
        com.facebook.buck.core.description.arg.[HasSrcs](../../core/description/arg/HasSrcs.html "interface in com.facebook.buck.core.description.arg"))
-   com.facebook.buck.core.description.arg.[[HasSrcs]{.typeNameLink}](../../core/description/arg/HasSrcs.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.features.rust.[[RustCommonArgs]{.typeNameLink}](RustCommonArgs.html "interface in com.facebook.buck.features.rust")
        (also extends
        com.facebook.buck.core.description.arg.[BuildRuleArg](../../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasDefaultPlatform](../../core/description/arg/HasDefaultPlatform.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.features.rust.[HasNamedDeclaredDeps](HasNamedDeclaredDeps.html "interface in com.facebook.buck.features.rust"))
-   com.facebook.buck.core.toolchain.[[Toolchain]{.typeNameLink}](../../core/toolchain/Toolchain.html "interface in com.facebook.buck.core.toolchain")
    -   com.facebook.buck.features.rust.[[RustToolchain]{.typeNameLink}](RustToolchain.html "interface in com.facebook.buck.features.rust")
:::

::: {.section role="region"}
## Enum Hierarchy {#enum-hierarchy title="Enum Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   java.lang.[[Enum]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<E\>
        (implements
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   com.facebook.buck.features.rust.[[CrateType]{.typeNameLink}](CrateType.html "enum in com.facebook.buck.features.rust")
        -   com.facebook.buck.features.rust.[[RustBinaryDescription.Type]{.typeNameLink}](RustBinaryDescription.Type.html "enum in com.facebook.buck.features.rust")
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
