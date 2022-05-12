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
# Hierarchy For Package com.facebook.buck.apple.toolchain {#hierarchy-for-package-com.facebook.buck.apple.toolchain .title}

[Package Hierarchies:]{.packageHierarchyLabel}

-   [All Packages](../../../../../overview-tree.html)
:::

::: contentContainer
::: {.section role="region"}
## Class Hierarchy {#class-hierarchy title="Class Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   com.facebook.buck.apple.toolchain.[[AppleCxxPlatform]{.typeNameLink}](AppleCxxPlatform.html "class in com.facebook.buck.apple.toolchain")
        (implements
        com.facebook.buck.core.model.[FlavorConvertible](../../core/model/FlavorConvertible.html "interface in com.facebook.buck.core.model"))
    -   com.facebook.buck.apple.toolchain.[[AppleCxxPlatformsProvider]{.typeNameLink}](AppleCxxPlatformsProvider.html "class in com.facebook.buck.apple.toolchain")
        (implements
        com.facebook.buck.cxx.toolchain.[CxxPlatformsSupplier](../../cxx/toolchain/CxxPlatformsSupplier.html "interface in com.facebook.buck.cxx.toolchain"))
    -   com.facebook.buck.apple.toolchain.[[ApplePlatform]{.typeNameLink}](ApplePlatform.html "class in com.facebook.buck.apple.toolchain")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"),
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>)
    -   com.facebook.buck.apple.toolchain.[[AppleSdk]{.typeNameLink}](AppleSdk.html "class in com.facebook.buck.apple.toolchain")
    -   com.facebook.buck.apple.toolchain.[[AppleSdkPaths]{.typeNameLink}](AppleSdkPaths.html "class in com.facebook.buck.apple.toolchain")
    -   com.facebook.buck.apple.toolchain.[[CodeSignIdentity]{.typeNameLink}](CodeSignIdentity.html "class in com.facebook.buck.apple.toolchain")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"))
    -   com.facebook.buck.apple.toolchain.ImmutableAppleCxxPlatform.Builder
        -   com.facebook.buck.apple.toolchain.[[AppleCxxPlatform.Builder]{.typeNameLink}](AppleCxxPlatform.Builder.html "class in com.facebook.buck.apple.toolchain")
    -   com.facebook.buck.apple.toolchain.ImmutableApplePlatform.Builder
        -   com.facebook.buck.apple.toolchain.[[ApplePlatform.Builder]{.typeNameLink}](ApplePlatform.Builder.html "class in com.facebook.buck.apple.toolchain")
    -   com.facebook.buck.apple.toolchain.ImmutableAppleSdk.Builder
        -   com.facebook.buck.apple.toolchain.[[AppleSdk.Builder]{.typeNameLink}](AppleSdk.Builder.html "class in com.facebook.buck.apple.toolchain")
    -   com.facebook.buck.apple.toolchain.ImmutableAppleSdkPaths.Builder
        -   com.facebook.buck.apple.toolchain.[[AppleSdkPaths.Builder]{.typeNameLink}](AppleSdkPaths.Builder.html "class in com.facebook.buck.apple.toolchain")
    -   com.facebook.buck.apple.toolchain.ImmutableAppleToolchain.Builder
        -   com.facebook.buck.apple.toolchain.[[AppleToolchain.Builder]{.typeNameLink}](AppleToolchain.Builder.html "class in com.facebook.buck.apple.toolchain")
    -   com.facebook.buck.apple.toolchain.ImmutableProvisioningProfileMetadata.Builder
        -   com.facebook.buck.apple.toolchain.[[ProvisioningProfileMetadata.Builder]{.typeNameLink}](ProvisioningProfileMetadata.Builder.html "class in com.facebook.buck.apple.toolchain")
    -   com.facebook.buck.apple.toolchain.[[ProvisioningProfileMetadata]{.typeNameLink}](ProvisioningProfileMetadata.html "class in com.facebook.buck.apple.toolchain")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"))
    -   com.facebook.buck.apple.toolchain.[[ProvisioningProfileStore]{.typeNameLink}](ProvisioningProfileStore.html "class in com.facebook.buck.apple.toolchain")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"),
        com.facebook.buck.core.toolchain.[Toolchain](../../core/toolchain/Toolchain.html "interface in com.facebook.buck.core.toolchain"))
:::

::: {.section role="region"}
## Interface Hierarchy {#interface-hierarchy title="Interface Hierarchy"}

-   com.facebook.buck.apple.toolchain.[[AppleToolchain]{.typeNameLink}](AppleToolchain.html "interface in com.facebook.buck.apple.toolchain")
-   com.facebook.buck.core.model.[[FlavorConvertible]{.typeNameLink}](../../core/model/FlavorConvertible.html "interface in com.facebook.buck.core.model")
    -   com.facebook.buck.apple.toolchain.[[UnresolvedAppleCxxPlatform]{.typeNameLink}](UnresolvedAppleCxxPlatform.html "interface in com.facebook.buck.apple.toolchain")
-   com.facebook.buck.core.toolchain.[[Toolchain]{.typeNameLink}](../../core/toolchain/Toolchain.html "interface in com.facebook.buck.core.toolchain")
    -   com.facebook.buck.apple.toolchain.[[AppleDeveloperDirectoryForTestsProvider]{.typeNameLink}](AppleDeveloperDirectoryForTestsProvider.html "interface in com.facebook.buck.apple.toolchain")
    -   com.facebook.buck.apple.toolchain.[[AppleDeveloperDirectoryProvider]{.typeNameLink}](AppleDeveloperDirectoryProvider.html "interface in com.facebook.buck.apple.toolchain")
    -   com.facebook.buck.apple.toolchain.[[CodeSignIdentityStore]{.typeNameLink}](CodeSignIdentityStore.html "interface in com.facebook.buck.apple.toolchain")
    -   com.facebook.buck.core.toolchain.[[ToolchainWithCapability]{.typeNameLink}](../../core/toolchain/ToolchainWithCapability.html "interface in com.facebook.buck.core.toolchain")
        -   com.facebook.buck.core.toolchain.[[ComparableToolchain]{.typeNameLink}](../../core/toolchain/ComparableToolchain.html "interface in com.facebook.buck.core.toolchain")
            -   com.facebook.buck.apple.toolchain.[[AppleSdkLocation]{.typeNameLink}](AppleSdkLocation.html "interface in com.facebook.buck.apple.toolchain")
            -   com.facebook.buck.apple.toolchain.[[AppleToolchainProvider]{.typeNameLink}](AppleToolchainProvider.html "interface in com.facebook.buck.apple.toolchain")
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
