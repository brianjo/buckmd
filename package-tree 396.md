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
# Hierarchy For Package com.facebook.buck.features.js {#hierarchy-for-package-com.facebook.buck.features.js .title}

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
            -   com.facebook.buck.features.js.[[JsBundle]{.typeNameLink}](JsBundle.html "class in com.facebook.buck.features.js")
                (implements
                com.facebook.buck.features.js.[JsBundleOutputs](JsBundleOutputs.html "interface in com.facebook.buck.features.js"))
            -   com.facebook.buck.features.js.[[JsBundleAndroid]{.typeNameLink}](JsBundleAndroid.html "class in com.facebook.buck.features.js")
                (implements
                com.facebook.buck.android.packageable.[AndroidPackageable](../../android/packageable/AndroidPackageable.html "interface in com.facebook.buck.android.packageable"),
                com.facebook.buck.features.js.[JsBundleOutputs](JsBundleOutputs.html "interface in com.facebook.buck.features.js"))
            -   com.facebook.buck.features.js.[[JsDependenciesFile]{.typeNameLink}](JsDependenciesFile.html "class in com.facebook.buck.features.js")
                (implements
                com.facebook.buck.features.js.[JsDependenciesOutputs](JsDependenciesOutputs.html "interface in com.facebook.buck.features.js"))
        -   com.facebook.buck.rules.modern.[[ModernBuildRule]{.typeNameLink}](../../rules/modern/ModernBuildRule.html "class in com.facebook.buck.rules.modern")\<T\>
            (implements
            com.facebook.buck.core.rules.attr.[SupportsInputBasedRuleKey](../../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr"))
            -   com.facebook.buck.shell.[[BaseGenrule]{.typeNameLink}](../../shell/BaseGenrule.html "class in com.facebook.buck.shell")\<T\>
                (implements
                com.facebook.buck.core.rules.attr.[HasMultipleOutputs](../../core/rules/attr/HasMultipleOutputs.html "interface in com.facebook.buck.core.rules.attr"),
                com.facebook.buck.core.model.[HasOutputName](../../core/model/HasOutputName.html "interface in com.facebook.buck.core.model"))
                -   com.facebook.buck.features.js.[[JsBundleGenrule]{.typeNameLink}](JsBundleGenrule.html "class in com.facebook.buck.features.js")
                    (implements
                    com.facebook.buck.android.packageable.[AndroidPackageable](../../android/packageable/AndroidPackageable.html "interface in com.facebook.buck.android.packageable"),
                    com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"),
                    com.facebook.buck.features.js.[JsBundleOutputs](JsBundleOutputs.html "interface in com.facebook.buck.features.js"),
                    com.facebook.buck.features.js.[JsDependenciesOutputs](JsDependenciesOutputs.html "interface in com.facebook.buck.features.js"))
            -   com.facebook.buck.features.js.[[JsFile]{.typeNameLink}](JsFile.html "class in com.facebook.buck.features.js")\<T\>
            -   com.facebook.buck.features.js.[[JsLibrary]{.typeNameLink}](JsLibrary.html "class in com.facebook.buck.features.js")
    -   com.facebook.buck.shell.[[AbstractGenruleDescription]{.typeNameLink}](../../shell/AbstractGenruleDescription.html "class in com.facebook.buck.shell")\<T\>
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>)
        -   com.facebook.buck.features.js.[[JsBundleGenruleDescription]{.typeNameLink}](JsBundleGenruleDescription.html "class in com.facebook.buck.features.js")
            (implements
            com.facebook.buck.core.model.[Flavored](../../core/model/Flavored.html "interface in com.facebook.buck.core.model"),
            com.facebook.buck.apple.[HasAppleBundleResourcesDescription](../../apple/HasAppleBundleResourcesDescription.html "interface in com.facebook.buck.apple")\<T\>,
            com.facebook.buck.features.js.[JsBundleOutputsDescription](JsBundleOutputsDescription.html "interface in com.facebook.buck.features.js")\<T\>)
    -   com.facebook.buck.features.js.[[JsBundleDescription]{.typeNameLink}](JsBundleDescription.html "class in com.facebook.buck.features.js")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.model.[Flavored](../../core/model/Flavored.html "interface in com.facebook.buck.core.model"),
        com.facebook.buck.apple.[HasAppleBundleResourcesDescription](../../apple/HasAppleBundleResourcesDescription.html "interface in com.facebook.buck.apple")\<T\>,
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>,
        com.facebook.buck.features.js.[JsBundleOutputsDescription](JsBundleOutputsDescription.html "interface in com.facebook.buck.features.js")\<T\>)
    -   com.facebook.buck.features.js.[[JsBundleDescriptionArg]{.typeNameLink}](JsBundleDescriptionArg.html "class in com.facebook.buck.features.js")
    -   com.facebook.buck.features.js.[[JsBundleDescriptionArg.Builder]{.typeNameLink}](JsBundleDescriptionArg.Builder.html "class in com.facebook.buck.features.js")
    -   com.facebook.buck.features.js.[[JsBundleGenruleDescriptionArg]{.typeNameLink}](JsBundleGenruleDescriptionArg.html "class in com.facebook.buck.features.js")
    -   com.facebook.buck.features.js.[[JsBundleGenruleDescriptionArg.Builder]{.typeNameLink}](JsBundleGenruleDescriptionArg.Builder.html "class in com.facebook.buck.features.js")
    -   com.facebook.buck.features.js.[[JsDescriptionsProvider]{.typeNameLink}](JsDescriptionsProvider.html "class in com.facebook.buck.features.js")
        (implements
        com.facebook.buck.core.model.targetgraph.[DescriptionProvider](../../core/model/targetgraph/DescriptionProvider.html "interface in com.facebook.buck.core.model.targetgraph"))
    -   com.facebook.buck.features.js.[[JsFlavors]{.typeNameLink}](JsFlavors.html "class in com.facebook.buck.features.js")
    -   com.facebook.buck.features.js.[[JsLibraryDescription]{.typeNameLink}](JsLibraryDescription.html "class in com.facebook.buck.features.js")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.model.[Flavored](../../core/model/Flavored.html "interface in com.facebook.buck.core.model"),
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>)
    -   com.facebook.buck.features.js.[[JsLibraryDescriptionArg]{.typeNameLink}](JsLibraryDescriptionArg.html "class in com.facebook.buck.features.js")
    -   com.facebook.buck.features.js.[[JsLibraryDescriptionArg.Builder]{.typeNameLink}](JsLibraryDescriptionArg.Builder.html "class in com.facebook.buck.features.js")
    -   com.facebook.buck.features.js.[[JsModule]{.typeNameLink}](JsModule.html "class in com.facebook.buck.features.js")
    -   com.facebook.buck.features.js.[[JsUtil]{.typeNameLink}](JsUtil.html "class in com.facebook.buck.features.js")
    -   org.pf4j.Plugin
        -   com.facebook.buck.features.js.[[JsModuleAdapterPlugin]{.typeNameLink}](JsModuleAdapterPlugin.html "class in com.facebook.buck.features.js")
:::

::: {.section role="region"}
## Interface Hierarchy {#interface-hierarchy title="Interface Hierarchy"}

-   com.facebook.buck.core.rulekey.[[AllowsNonAnnotatedFields]{.typeNameLink}](../../core/rulekey/AllowsNonAnnotatedFields.html "interface in com.facebook.buck.core.rulekey")
    -   com.facebook.buck.core.rules.[[BuildRule]{.typeNameLink}](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
        (also extends
        com.facebook.buck.core.build.action.[BuildEngineAction](../../core/build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action"),
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        com.facebook.buck.core.rules.[HasNameAndType](../../core/rules/HasNameAndType.html "interface in com.facebook.buck.core.rules"))
        -   com.facebook.buck.features.js.[[JsBundleOutputs]{.typeNameLink}](JsBundleOutputs.html "interface in com.facebook.buck.features.js")
        -   com.facebook.buck.features.js.[[JsDependenciesOutputs]{.typeNameLink}](JsDependenciesOutputs.html "interface in com.facebook.buck.features.js")
-   com.facebook.buck.core.description.[[BaseDescription]{.typeNameLink}](../../core/description/BaseDescription.html "interface in com.facebook.buck.core.description")\<T\>
    -   com.facebook.buck.core.description.[[Description]{.typeNameLink}](../../core/description/Description.html "interface in com.facebook.buck.core.description")\<T\>
        -   com.facebook.buck.core.rules.[[DescriptionWithTargetGraph]{.typeNameLink}](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>
            -   com.facebook.buck.features.js.[[JsBundleOutputsDescription]{.typeNameLink}](JsBundleOutputsDescription.html "interface in com.facebook.buck.features.js")\<T\>
-   com.facebook.buck.core.build.action.[[BuildEngineAction]{.typeNameLink}](../../core/build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")
    -   com.facebook.buck.core.rules.[[BuildRule]{.typeNameLink}](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
        (also extends
        com.facebook.buck.core.rulekey.[AllowsNonAnnotatedFields](../../core/rulekey/AllowsNonAnnotatedFields.html "interface in com.facebook.buck.core.rulekey"),
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        com.facebook.buck.core.rules.[HasNameAndType](../../core/rules/HasNameAndType.html "interface in com.facebook.buck.core.rules"))
        -   com.facebook.buck.features.js.[[JsBundleOutputs]{.typeNameLink}](JsBundleOutputs.html "interface in com.facebook.buck.features.js")
        -   com.facebook.buck.features.js.[[JsDependenciesOutputs]{.typeNameLink}](JsDependenciesOutputs.html "interface in com.facebook.buck.features.js")
-   java.lang.[[Comparable]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>
    -   com.facebook.buck.core.rules.[[BuildRule]{.typeNameLink}](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
        (also extends
        com.facebook.buck.core.rulekey.[AllowsNonAnnotatedFields](../../core/rulekey/AllowsNonAnnotatedFields.html "interface in com.facebook.buck.core.rulekey"),
        com.facebook.buck.core.build.action.[BuildEngineAction](../../core/build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action"),
        com.facebook.buck.core.rules.[HasNameAndType](../../core/rules/HasNameAndType.html "interface in com.facebook.buck.core.rules"))
        -   com.facebook.buck.features.js.[[JsBundleOutputs]{.typeNameLink}](JsBundleOutputs.html "interface in com.facebook.buck.features.js")
        -   com.facebook.buck.features.js.[[JsDependenciesOutputs]{.typeNameLink}](JsDependenciesOutputs.html "interface in com.facebook.buck.features.js")
-   com.facebook.buck.features.js.[[HasBundleName]{.typeNameLink}](HasBundleName.html "interface in com.facebook.buck.features.js")
-   com.facebook.buck.features.js.[[HasExtraJson]{.typeNameLink}](HasExtraJson.html "interface in com.facebook.buck.features.js")
-   com.facebook.buck.core.rules.[[HasNameAndType]{.typeNameLink}](../../core/rules/HasNameAndType.html "interface in com.facebook.buck.core.rules")
    -   com.facebook.buck.core.rules.[[BuildRule]{.typeNameLink}](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
        (also extends
        com.facebook.buck.core.rulekey.[AllowsNonAnnotatedFields](../../core/rulekey/AllowsNonAnnotatedFields.html "interface in com.facebook.buck.core.rulekey"),
        com.facebook.buck.core.build.action.[BuildEngineAction](../../core/build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action"),
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>)
        -   com.facebook.buck.features.js.[[JsBundleOutputs]{.typeNameLink}](JsBundleOutputs.html "interface in com.facebook.buck.features.js")
        -   com.facebook.buck.features.js.[[JsDependenciesOutputs]{.typeNameLink}](JsDependenciesOutputs.html "interface in com.facebook.buck.features.js")
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
