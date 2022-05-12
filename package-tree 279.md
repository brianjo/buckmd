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
# Hierarchy For Package com.facebook.buck.features.dotnet {#hierarchy-for-package-com.facebook.buck.features.dotnet .title}

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
            -   com.facebook.buck.features.dotnet.[[CsharpLibrary]{.typeNameLink}](CsharpLibrary.html "class in com.facebook.buck.features.dotnet")
            -   com.facebook.buck.features.dotnet.[[PrebuiltDotnetLibrary]{.typeNameLink}](PrebuiltDotnetLibrary.html "class in com.facebook.buck.features.dotnet")
    -   com.facebook.buck.core.starlark.compatible.[[BuckStarlarkStructObject]{.typeNameLink}](../../core/starlark/compatible/BuckStarlarkStructObject.html "class in com.facebook.buck.core.starlark.compatible")
        (implements com.google.devtools.build.lib.syntax.ClassObject,
        com.google.devtools.build.lib.skylarkinterface.SkylarkValue)
        -   com.facebook.buck.core.rules.providers.impl.[[BuiltInProviderInfo]{.typeNameLink}](../../core/rules/providers/impl/BuiltInProviderInfo.html "class in com.facebook.buck.core.rules.providers.impl")\<T\>
            (implements
            com.facebook.buck.core.rules.providers.[ProviderInfo](../../core/rules/providers/ProviderInfo.html "interface in com.facebook.buck.core.rules.providers")\<U\>)
            -   com.facebook.buck.features.dotnet.[[DotnetLegacyToolchainInfo]{.typeNameLink}](DotnetLegacyToolchainInfo.html "class in com.facebook.buck.features.dotnet")
                -   com.facebook.buck.features.dotnet.[[ImmutableDotnetLegacyToolchainInfo]{.typeNameLink}](ImmutableDotnetLegacyToolchainInfo.html "class in com.facebook.buck.features.dotnet")
            -   com.facebook.buck.features.dotnet.[[DotnetLibraryProviderInfo]{.typeNameLink}](DotnetLibraryProviderInfo.html "class in com.facebook.buck.features.dotnet")
                -   com.facebook.buck.features.dotnet.[[ImmutableDotnetLibraryProviderInfo]{.typeNameLink}](ImmutableDotnetLibraryProviderInfo.html "class in com.facebook.buck.features.dotnet")
    -   com.facebook.buck.features.dotnet.[[CsharpLibraryDescription]{.typeNameLink}](CsharpLibraryDescription.html "class in com.facebook.buck.features.dotnet")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.rules.[LegacyProviderCompatibleDescription](../../core/rules/LegacyProviderCompatibleDescription.html "interface in com.facebook.buck.core.rules")\<T\>)
    -   com.facebook.buck.features.dotnet.[[CsharpLibraryDescriptionArg]{.typeNameLink}](CsharpLibraryDescriptionArg.html "class in com.facebook.buck.features.dotnet")
    -   com.facebook.buck.features.dotnet.[[CsharpLibraryDescriptionArg.Builder]{.typeNameLink}](CsharpLibraryDescriptionArg.Builder.html "class in com.facebook.buck.features.dotnet")
    -   com.facebook.buck.features.dotnet.[[DotnetBuckConfig]{.typeNameLink}](DotnetBuckConfig.html "class in com.facebook.buck.features.dotnet")
        (implements
        com.facebook.buck.core.config.[ConfigView](../../core/config/ConfigView.html "interface in com.facebook.buck.core.config")\<T\>)
    -   com.facebook.buck.features.dotnet.[[DotnetFramework]{.typeNameLink}](DotnetFramework.html "class in com.facebook.buck.features.dotnet")
    -   com.facebook.buck.features.dotnet.[[DotnetModule]{.typeNameLink}](DotnetModule.html "class in com.facebook.buck.features.dotnet")
    -   com.facebook.buck.features.dotnet.[[DotNetRuleProvider]{.typeNameLink}](DotNetRuleProvider.html "class in com.facebook.buck.features.dotnet")
        (implements
        com.facebook.buck.core.model.targetgraph.[BuiltInProviderProvider](../../core/model/targetgraph/BuiltInProviderProvider.html "interface in com.facebook.buck.core.model.targetgraph"),
        com.facebook.buck.core.model.targetgraph.[DescriptionProvider](../../core/model/targetgraph/DescriptionProvider.html "interface in com.facebook.buck.core.model.targetgraph"))
    -   com.facebook.buck.features.dotnet.[[DotnetToolchainSupplier]{.typeNameLink}](DotnetToolchainSupplier.html "class in com.facebook.buck.features.dotnet")
        (implements
        com.facebook.buck.core.toolchain.[ToolchainSupplier](../../core/toolchain/ToolchainSupplier.html "interface in com.facebook.buck.core.toolchain"))
    -   com.facebook.buck.features.dotnet.[[DotnetToolchainSupplier.DotnetToolchainFactory]{.typeNameLink}](DotnetToolchainSupplier.DotnetToolchainFactory.html "class in com.facebook.buck.features.dotnet")
        (implements
        com.facebook.buck.core.toolchain.[ToolchainFactory](../../core/toolchain/ToolchainFactory.html "interface in com.facebook.buck.core.toolchain")\<T\>)
    -   org.pf4j.Plugin
        -   com.facebook.buck.features.dotnet.[[DotnetModuleAdapterPlugin]{.typeNameLink}](DotnetModuleAdapterPlugin.html "class in com.facebook.buck.features.dotnet")
    -   com.facebook.buck.features.dotnet.[[PrebuiltDotnetLibraryDescription]{.typeNameLink}](PrebuiltDotnetLibraryDescription.html "class in com.facebook.buck.features.dotnet")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>)
    -   com.facebook.buck.features.dotnet.[[PrebuiltDotnetLibraryDescriptionArg]{.typeNameLink}](PrebuiltDotnetLibraryDescriptionArg.html "class in com.facebook.buck.features.dotnet")
    -   com.facebook.buck.features.dotnet.[[PrebuiltDotnetLibraryDescriptionArg.Builder]{.typeNameLink}](PrebuiltDotnetLibraryDescriptionArg.Builder.html "class in com.facebook.buck.features.dotnet")
    -   com.facebook.buck.features.dotnet.[[PrebuiltDotnetLibraryRuleDescription]{.typeNameLink}](PrebuiltDotnetLibraryRuleDescription.html "class in com.facebook.buck.features.dotnet")
        (implements
        com.facebook.buck.core.description.[RuleDescription](../../core/description/RuleDescription.html "interface in com.facebook.buck.core.description")\<T\>)
    -   com.facebook.buck.shell.[[ShellStep]{.typeNameLink}](../../shell/ShellStep.html "class in com.facebook.buck.shell")
        (implements
        com.facebook.buck.step.[Step](../../step/Step.html "interface in com.facebook.buck.step"))
        -   com.facebook.buck.features.dotnet.[[CsharpLibraryCompile]{.typeNameLink}](CsharpLibraryCompile.html "class in com.facebook.buck.features.dotnet")
:::

::: {.section role="region"}
## Enum Hierarchy {#enum-hierarchy title="Enum Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   java.lang.[[Enum]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<E\>
        (implements
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   com.facebook.buck.features.dotnet.[[FrameworkVersion]{.typeNameLink}](FrameworkVersion.html "enum in com.facebook.buck.features.dotnet")
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
