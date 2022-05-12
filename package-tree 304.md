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
# Hierarchy For Package com.facebook.buck.swift {#hierarchy-for-package-com.facebook.buck.swift .title}

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
        -   com.facebook.buck.core.rules.impl.[[NoopBuildRule]{.typeNameLink}](../core/rules/impl/NoopBuildRule.html "class in com.facebook.buck.core.rules.impl")
            (implements
            com.facebook.buck.core.rules.attr.[SupportsInputBasedRuleKey](../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr"))
            -   com.facebook.buck.swift.[[SwiftToolchainBuildRule]{.typeNameLink}](SwiftToolchainBuildRule.html "class in com.facebook.buck.swift")
        -   com.facebook.buck.swift.[[SwiftCompile]{.typeNameLink}](SwiftCompile.html "class in com.facebook.buck.swift")
            (implements
            com.facebook.buck.core.rules.attr.[SupportsInputBasedRuleKey](../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr"))
    -   com.facebook.buck.swift.[[SwiftBuckConfig]{.typeNameLink}](SwiftBuckConfig.html "class in com.facebook.buck.swift")
        (implements
        com.facebook.buck.core.config.[ConfigView](../core/config/ConfigView.html "interface in com.facebook.buck.core.config")\<T\>)
    -   com.facebook.buck.swift.[[SwiftDescriptions]{.typeNameLink}](SwiftDescriptions.html "class in com.facebook.buck.swift")
    -   com.facebook.buck.swift.[[SwiftDescriptionsProvider]{.typeNameLink}](SwiftDescriptionsProvider.html "class in com.facebook.buck.swift")
        (implements
        com.facebook.buck.core.model.targetgraph.[DescriptionProvider](../core/model/targetgraph/DescriptionProvider.html "interface in com.facebook.buck.core.model.targetgraph"))
    -   com.facebook.buck.swift.[[SwiftLibraryDescription]{.typeNameLink}](SwiftLibraryDescription.html "class in com.facebook.buck.swift")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.model.[Flavored](../core/model/Flavored.html "interface in com.facebook.buck.core.model"),
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>)
    -   com.facebook.buck.swift.[[SwiftLibraryDescriptionArg]{.typeNameLink}](SwiftLibraryDescriptionArg.html "class in com.facebook.buck.swift")
    -   com.facebook.buck.swift.[[SwiftLibraryDescriptionArg.Builder]{.typeNameLink}](SwiftLibraryDescriptionArg.Builder.html "class in com.facebook.buck.swift")
    -   com.facebook.buck.swift.[[SwiftRuntimeNativeLinkableGroup]{.typeNameLink}](SwiftRuntimeNativeLinkableGroup.html "class in com.facebook.buck.swift")
        (implements
        com.facebook.buck.cxx.toolchain.nativelink.[NativeLinkableGroup](../cxx/toolchain/nativelink/NativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink"))
    -   com.facebook.buck.swift.[[SwiftToolchainDescription]{.typeNameLink}](SwiftToolchainDescription.html "class in com.facebook.buck.swift")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>)
    -   com.facebook.buck.swift.[[SwiftToolchainDescriptionArg]{.typeNameLink}](SwiftToolchainDescriptionArg.html "class in com.facebook.buck.swift")
    -   com.facebook.buck.swift.[[SwiftToolchainDescriptionArg.Builder]{.typeNameLink}](SwiftToolchainDescriptionArg.Builder.html "class in com.facebook.buck.swift")
:::

::: {.section role="region"}
## Interface Hierarchy {#interface-hierarchy title="Interface Hierarchy"}

-   com.facebook.buck.core.description.arg.[[DataTransferObject]{.typeNameLink}](../core/description/arg/DataTransferObject.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.core.description.arg.[[ConstructorArg]{.typeNameLink}](../core/description/arg/ConstructorArg.html "interface in com.facebook.buck.core.description.arg")
        -   com.facebook.buck.core.description.arg.[[BuildRuleArg]{.typeNameLink}](../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")
            -   com.facebook.buck.swift.[[SwiftCommonArg]{.typeNameLink}](SwiftCommonArg.html "interface in com.facebook.buck.swift")
:::

::: {.section role="region"}
## Enum Hierarchy {#enum-hierarchy title="Enum Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   java.lang.[[Enum]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<E\>
        (implements
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   com.facebook.buck.swift.[[SwiftLibraryDescription.Type]{.typeNameLink}](SwiftLibraryDescription.Type.html "enum in com.facebook.buck.swift")
            (implements
            com.facebook.buck.core.model.[FlavorConvertible](../core/model/FlavorConvertible.html "interface in com.facebook.buck.core.model"))
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
