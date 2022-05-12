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
-   [Tree](package-tree.html)
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

<div>

-   Summary: 
-   Nested \| 
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
::: subTitle
[Package]{.packageLabelInType} [com.facebook.buck.core.model](package-summary.html)
:::

## Interface Flavored {#interface-flavored .title title="Interface Flavored"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `AndroidBinaryDescription`, `AndroidBundleDescription`,
        `AndroidLibraryDescription`, `AndroidPrebuiltAarDescription`,
        `AndroidResourceDescription`, `AppleBinaryDescription`,
        `AppleBundleDescription`, `AppleLibraryDescription`,
        `ApplePackageDescription`, `AppleResourceDescription`,
        `AppleTestDescription`, `CgoLibraryDescription`,
        `CoreDataModelDescription`, `CxxBinaryDescription`,
        `CxxBinaryFlavored`, `CxxGenruleDescription`,
        `CxxLibraryDescription`, `CxxLibraryFlavored`,
        `CxxLuaExtensionDescription`, `CxxPythonExtensionDescription`,
        `CxxTestDescription`, `GoBinaryDescription`,
        `GoLibraryDescription`, `GoTestDescription`,
        `HalideLibraryDescription`, `HaskellBinaryDescription`,
        `HaskellLibraryDescription`, `JavaLibraryDescription`,
        `JsBundleDescription`, `JsBundleGenruleDescription`,
        `JsLibraryDescription`, `KotlinLibraryDescription`,
        `OcamlLibraryDescription`, `PrebuiltAppleFrameworkDescription`,
        `PrebuiltPythonLibraryDescription`, `PythonLibraryDescription`,
        `RustBinaryDescription`, `RustLibraryDescription`,
        `RustTestDescription`, `ScalaLibraryDescription`,
        `SceneKitAssetsDescription`, `SwiftLibraryDescription`,
        `XcodePrebuildScriptDescription`

    ------------------------------------------------------------------------

        public interface Flavored

    ::: block
    When applied to a
    [`DescriptionWithTargetGraph`](../rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")
    this indicates that it supports flavours.
    This is only required to be implemented by Descriptions where the
    flavored BuildTarget should be buildable in a top-level
    [`Build`](../../command/Build.html "class in com.facebook.buck.command").
    i.e. this should be implemented by
    [`DescriptionWithTargetGraph`](../rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")s
    where the may have a flavored
    [`BuildTarget`](BuildTarget.html "class in com.facebook.buck.core.model") -
    it is not required where only the
    [`BuildRule`](../rules/BuildRule.html "interface in com.facebook.buck.core.rules")s
    are flavored.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                             Method                                                                                                                             Description
          ----------------------------------------------------------------------------- ---------------------------------------------------------------------------------------------------------------------------------- -------------
          `default Optional<com.google.common.collect.ImmutableSet<FlavorDomain<?>>>`   `flavorDomains​(TargetConfiguration toolchainTargetConfiguration)`                                                                   
          `default boolean`                                                             `hasFlavors​(com.google.common.collect.ImmutableSet<Flavor> flavors,           TargetConfiguration toolchainTargetConfiguration)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Default
          Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#hasFlavors(com.google.common.collect.ImmutableSet,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### hasFlavors

            ``` methodSignature
            default boolean hasFlavors​(com.google.common.collect.ImmutableSet<Flavor> flavors,
                                       TargetConfiguration toolchainTargetConfiguration)
            ```

            [Parameters:]{.paramLabel}
            :   `flavors` - The set of
                [`Flavor`](Flavor.html "interface in com.facebook.buck.core.model")s
                to consider. All must match.
            :   `toolchainTargetConfiguration` -

            [Returns:]{.returnLabel}
            :   Whether a
                [`BuildRule`](../rules/BuildRule.html "interface in com.facebook.buck.core.rules")
                of the given
                [`Flavor`](Flavor.html "interface in com.facebook.buck.core.model")
                can be created.

        []{#flavorDomains(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### flavorDomains

            ``` methodSignature
            default Optional<com.google.common.collect.ImmutableSet<FlavorDomain<?>>> flavorDomains​(TargetConfiguration toolchainTargetConfiguration)
            ```
    :::
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
-   [Tree](package-tree.html)
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

<div>

-   Summary: 
-   Nested \| 
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
