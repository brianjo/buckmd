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
# Hierarchy For Package com.facebook.buck.features.lua {#hierarchy-for-package-com.facebook.buck.features.lua .title}

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
            -   com.facebook.buck.features.lua.[[LuaBinary]{.typeNameLink}](LuaBinary.html "class in com.facebook.buck.features.lua")
                (implements
                com.facebook.buck.core.rules.tool.[BinaryBuildRule](../../core/rules/tool/BinaryBuildRule.html "interface in com.facebook.buck.core.rules.tool"),
                com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"))
            -   com.facebook.buck.features.lua.[[LuaStandaloneBinary]{.typeNameLink}](LuaStandaloneBinary.html "class in com.facebook.buck.features.lua")
            -   com.facebook.buck.core.rules.impl.[[NoopBuildRuleWithDeclaredAndExtraDeps]{.typeNameLink}](../../core/rules/impl/NoopBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")
                -   com.facebook.buck.features.lua.[[CxxLuaExtension]{.typeNameLink}](CxxLuaExtension.html "class in com.facebook.buck.features.lua")
                    (implements
                    com.facebook.buck.cxx.toolchain.nativelink.[NativeLinkTargetGroup](../../cxx/toolchain/nativelink/NativeLinkTargetGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink"))
                -   com.facebook.buck.features.lua.[[LuaLibrary]{.typeNameLink}](LuaLibrary.html "class in com.facebook.buck.features.lua")
                    (implements
                    com.facebook.buck.features.lua.[LuaPackageable](LuaPackageable.html "interface in com.facebook.buck.features.lua"))
    -   com.facebook.buck.features.lua.[[CxxLuaExtensionDescription]{.typeNameLink}](CxxLuaExtensionDescription.html "class in com.facebook.buck.features.lua")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.model.[Flavored](../../core/model/Flavored.html "interface in com.facebook.buck.core.model"),
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>,
        com.facebook.buck.versions.[VersionPropagator](../../versions/VersionPropagator.html "interface in com.facebook.buck.versions")\<A\>)
    -   com.facebook.buck.features.lua.[[CxxLuaExtensionDescriptionArg]{.typeNameLink}](CxxLuaExtensionDescriptionArg.html "class in com.facebook.buck.features.lua")
    -   com.facebook.buck.features.lua.[[CxxLuaExtensionDescriptionArg.Builder]{.typeNameLink}](CxxLuaExtensionDescriptionArg.Builder.html "class in com.facebook.buck.features.lua")
    -   com.facebook.buck.features.lua.[[LuaBinaryDescription]{.typeNameLink}](LuaBinaryDescription.html "class in com.facebook.buck.features.lua")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>,
        com.facebook.buck.versions.[VersionRoot](../../versions/VersionRoot.html "interface in com.facebook.buck.versions")\<A\>)
    -   com.facebook.buck.features.lua.[[LuaBinaryDescriptionArg]{.typeNameLink}](LuaBinaryDescriptionArg.html "class in com.facebook.buck.features.lua")
    -   com.facebook.buck.features.lua.[[LuaBinaryDescriptionArg.Builder]{.typeNameLink}](LuaBinaryDescriptionArg.Builder.html "class in com.facebook.buck.features.lua")
    -   com.facebook.buck.features.lua.[[LuaBuckConfig]{.typeNameLink}](LuaBuckConfig.html "class in com.facebook.buck.features.lua")
    -   com.facebook.buck.features.lua.[[LuaDescriptionsProvider]{.typeNameLink}](LuaDescriptionsProvider.html "class in com.facebook.buck.features.lua")
        (implements
        com.facebook.buck.core.model.targetgraph.[DescriptionProvider](../../core/model/targetgraph/DescriptionProvider.html "interface in com.facebook.buck.core.model.targetgraph"))
    -   com.facebook.buck.features.lua.[[LuaLibraryDescription]{.typeNameLink}](LuaLibraryDescription.html "class in com.facebook.buck.features.lua")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.versions.[VersionPropagator](../../versions/VersionPropagator.html "interface in com.facebook.buck.versions")\<A\>)
    -   com.facebook.buck.features.lua.[[LuaLibraryDescriptionArg]{.typeNameLink}](LuaLibraryDescriptionArg.html "class in com.facebook.buck.features.lua")
    -   com.facebook.buck.features.lua.[[LuaLibraryDescriptionArg.Builder]{.typeNameLink}](LuaLibraryDescriptionArg.Builder.html "class in com.facebook.buck.features.lua")
    -   com.facebook.buck.features.lua.[[LuaModule]{.typeNameLink}](LuaModule.html "class in com.facebook.buck.features.lua")
    -   com.facebook.buck.features.lua.[[LuaPlatform]{.typeNameLink}](LuaPlatform.html "class in com.facebook.buck.features.lua")
        (implements
        com.facebook.buck.core.model.[FlavorConvertible](../../core/model/FlavorConvertible.html "interface in com.facebook.buck.core.model"))
    -   com.facebook.buck.features.lua.[[LuaPlatformsProviderFactory]{.typeNameLink}](LuaPlatformsProviderFactory.html "class in com.facebook.buck.features.lua")
        (implements
        com.facebook.buck.core.toolchain.[ToolchainFactory](../../core/toolchain/ToolchainFactory.html "interface in com.facebook.buck.core.toolchain")\<T\>)
    -   com.facebook.buck.features.lua.[[LuaToolchainsSupplier]{.typeNameLink}](LuaToolchainsSupplier.html "class in com.facebook.buck.features.lua")
        (implements
        com.facebook.buck.core.toolchain.[ToolchainSupplier](../../core/toolchain/ToolchainSupplier.html "interface in com.facebook.buck.core.toolchain"))
    -   com.facebook.buck.features.lua.[[LuaUtil]{.typeNameLink}](LuaUtil.html "class in com.facebook.buck.features.lua")
    -   org.pf4j.Plugin
        -   com.facebook.buck.features.lua.[[LuaModuleAdapterPlugin]{.typeNameLink}](LuaModuleAdapterPlugin.html "class in com.facebook.buck.features.lua")
    -   com.facebook.buck.features.lua.[[SystemLuaCxxLibrary]{.typeNameLink}](SystemLuaCxxLibrary.html "class in com.facebook.buck.features.lua")
        (implements
        com.facebook.buck.cxx.[AbstractCxxLibraryGroup](../../cxx/AbstractCxxLibraryGroup.html "interface in com.facebook.buck.cxx"),
        com.facebook.buck.cxx.toolchain.nativelink.[NativeLinkableGroup](../../cxx/toolchain/nativelink/NativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink"))
:::

::: {.section role="region"}
## Interface Hierarchy {#interface-hierarchy title="Interface Hierarchy"}

-   com.facebook.buck.features.lua.[[LuaPackageable]{.typeNameLink}](LuaPackageable.html "interface in com.facebook.buck.features.lua")
-   com.facebook.buck.features.lua.[[Starter]{.typeNameLink}](Starter.html "interface in com.facebook.buck.features.lua")
-   com.facebook.buck.core.toolchain.[[Toolchain]{.typeNameLink}](../../core/toolchain/Toolchain.html "interface in com.facebook.buck.core.toolchain")
    -   com.facebook.buck.features.lua.[[LuaPlatformsProvider]{.typeNameLink}](LuaPlatformsProvider.html "interface in com.facebook.buck.features.lua")
:::

::: {.section role="region"}
## Enum Hierarchy {#enum-hierarchy title="Enum Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   java.lang.[[Enum]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<E\>
        (implements
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   com.facebook.buck.features.lua.[[LuaBinaryDescription.StarterType]{.typeNameLink}](LuaBinaryDescription.StarterType.html "enum in com.facebook.buck.features.lua")
        -   com.facebook.buck.features.lua.[[LuaPlatform.PackageStyle]{.typeNameLink}](LuaPlatform.PackageStyle.html "enum in com.facebook.buck.features.lua")
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
