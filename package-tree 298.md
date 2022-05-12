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
# Hierarchy For Package com.facebook.buck.rules.modern {#hierarchy-for-package-com.facebook.buck.rules.modern .title}

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
        -   com.facebook.buck.rules.modern.[[ModernBuildRule]{.typeNameLink}](ModernBuildRule.html "class in com.facebook.buck.rules.modern")\<T\>
            (implements
            com.facebook.buck.core.rules.attr.[SupportsInputBasedRuleKey](../../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr"))
            -   com.facebook.buck.rules.modern.[[PipelinedModernBuildRule]{.typeNameLink}](PipelinedModernBuildRule.html "class in com.facebook.buck.rules.modern")\<State,​T\>
                (implements
                com.facebook.buck.core.rules.pipeline.[SupportsPipelining](../../core/rules/pipeline/SupportsPipelining.html "interface in com.facebook.buck.core.rules.pipeline")\<T\>)
    -   com.facebook.buck.rules.modern.[[CustomBehaviorUtils]{.typeNameLink}](CustomBehaviorUtils.html "class in com.facebook.buck.rules.modern")
    -   com.facebook.buck.rules.modern.[[DefaultBuildCellRelativePathFactory]{.typeNameLink}](DefaultBuildCellRelativePathFactory.html "class in com.facebook.buck.rules.modern")
        (implements
        com.facebook.buck.rules.modern.[BuildCellRelativePathFactory](BuildCellRelativePathFactory.html "interface in com.facebook.buck.rules.modern"))
    -   com.facebook.buck.rules.modern.[[DefaultOutputPathResolver]{.typeNameLink}](DefaultOutputPathResolver.html "class in com.facebook.buck.rules.modern")
        (implements
        com.facebook.buck.rules.modern.[OutputPathResolver](OutputPathResolver.html "interface in com.facebook.buck.rules.modern"))
    -   com.facebook.buck.rules.modern.[[Deserializer]{.typeNameLink}](Deserializer.html "class in com.facebook.buck.rules.modern")
    -   com.facebook.buck.rules.modern.[[EmptyMemoizerDeserialization]{.typeNameLink}](EmptyMemoizerDeserialization.html "class in com.facebook.buck.rules.modern")\<T\>
        (implements
        com.facebook.buck.rules.modern.[CustomFieldSerialization](CustomFieldSerialization.html "interface in com.facebook.buck.rules.modern")\<T\>)
    -   com.facebook.buck.rules.modern.[[FieldInfo]{.typeNameLink}](FieldInfo.html "class in com.facebook.buck.rules.modern")\<T\>
    -   com.facebook.buck.rules.modern.[[OutputPath]{.typeNameLink}](OutputPath.html "class in com.facebook.buck.rules.modern")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"))
        -   com.facebook.buck.rules.modern.[[PublicOutputPath]{.typeNameLink}](PublicOutputPath.html "class in com.facebook.buck.rules.modern")
    -   com.facebook.buck.rules.modern.[[OutputPath.Internals]{.typeNameLink}](OutputPath.Internals.html "class in com.facebook.buck.rules.modern")
    -   com.facebook.buck.rules.modern.[[PathSerialization]{.typeNameLink}](PathSerialization.html "class in com.facebook.buck.rules.modern")
        (implements
        com.facebook.buck.rules.modern.[CustomFieldSerialization](CustomFieldSerialization.html "interface in com.facebook.buck.rules.modern")\<T\>)
    -   com.facebook.buck.rules.modern.[[PlatformSerialization]{.typeNameLink}](PlatformSerialization.html "class in com.facebook.buck.rules.modern")
        (implements
        com.facebook.buck.rules.modern.[CustomFieldSerialization](CustomFieldSerialization.html "interface in com.facebook.buck.rules.modern")\<T\>)
    -   com.facebook.buck.rules.modern.[[RemoteExecutionEnabled]{.typeNameLink}](RemoteExecutionEnabled.html "class in com.facebook.buck.rules.modern")
        (implements
        com.facebook.buck.rules.modern.[CustomFieldSerialization](CustomFieldSerialization.html "interface in com.facebook.buck.rules.modern")\<T\>)
    -   com.facebook.buck.rules.modern.[[Serializer]{.typeNameLink}](Serializer.html "class in com.facebook.buck.rules.modern")
    -   com.facebook.buck.rules.modern.[[SourcePathResolverSerialization]{.typeNameLink}](SourcePathResolverSerialization.html "class in com.facebook.buck.rules.modern")
        (implements
        com.facebook.buck.rules.modern.[CustomFieldSerialization](CustomFieldSerialization.html "interface in com.facebook.buck.rules.modern")\<T\>)
:::

::: {.section role="region"}
## Interface Hierarchy {#interface-hierarchy title="Interface Hierarchy"}

-   com.facebook.buck.core.rulekey.[[AddsToRuleKey]{.typeNameLink}](../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey")
    -   com.facebook.buck.rules.modern.[[Buildable]{.typeNameLink}](Buildable.html "interface in com.facebook.buck.rules.modern")
        -   com.facebook.buck.rules.modern.[[PipelinedBuildable]{.typeNameLink}](PipelinedBuildable.html "interface in com.facebook.buck.rules.modern")\<State\>
-   com.facebook.buck.rules.modern.[[BuildCellRelativePathFactory]{.typeNameLink}](BuildCellRelativePathFactory.html "interface in com.facebook.buck.rules.modern")
-   com.facebook.buck.rules.modern.[[ClassInfo]{.typeNameLink}](ClassInfo.html "interface in com.facebook.buck.rules.modern")\<T\>
-   com.facebook.buck.core.rules.modern.annotations.[[CustomClassBehaviorTag]{.typeNameLink}](../../core/rules/modern/annotations/CustomClassBehaviorTag.html "interface in com.facebook.buck.core.rules.modern.annotations")
    -   com.facebook.buck.rules.modern.[[CustomClassSerialization]{.typeNameLink}](CustomClassSerialization.html "interface in com.facebook.buck.rules.modern")\<T\>
-   com.facebook.buck.core.rulekey.[[CustomFieldBehaviorTag]{.typeNameLink}](../../core/rulekey/CustomFieldBehaviorTag.html "interface in com.facebook.buck.core.rulekey")
    -   com.facebook.buck.core.rulekey.[[CustomFieldDepsTag]{.typeNameLink}](../../core/rulekey/CustomFieldDepsTag.html "interface in com.facebook.buck.core.rulekey")
        -   com.facebook.buck.rules.modern.[[CustomFieldDeps]{.typeNameLink}](CustomFieldDeps.html "interface in com.facebook.buck.rules.modern")\<T\>
    -   com.facebook.buck.core.rulekey.[[CustomFieldInputsTag]{.typeNameLink}](../../core/rulekey/CustomFieldInputsTag.html "interface in com.facebook.buck.core.rulekey")
        -   com.facebook.buck.rules.modern.[[CustomFieldInputs]{.typeNameLink}](CustomFieldInputs.html "interface in com.facebook.buck.rules.modern")\<T\>
    -   com.facebook.buck.core.rulekey.[[CustomFieldSerializationTag]{.typeNameLink}](../../core/rulekey/CustomFieldSerializationTag.html "interface in com.facebook.buck.core.rulekey")
        -   com.facebook.buck.rules.modern.[[CustomFieldSerialization]{.typeNameLink}](CustomFieldSerialization.html "interface in com.facebook.buck.rules.modern")\<T\>
-   com.facebook.buck.rules.modern.[[Deserializer.ClassFinder]{.typeNameLink}](Deserializer.ClassFinder.html "interface in com.facebook.buck.rules.modern")
-   com.facebook.buck.rules.modern.[[Deserializer.DataProvider]{.typeNameLink}](Deserializer.DataProvider.html "interface in com.facebook.buck.rules.modern")
-   com.facebook.buck.rules.modern.[[HasBrokenInputBasedRuleKey]{.typeNameLink}](HasBrokenInputBasedRuleKey.html "interface in com.facebook.buck.rules.modern")
-   com.facebook.buck.rules.modern.[[InputRuleResolver]{.typeNameLink}](InputRuleResolver.html "interface in com.facebook.buck.rules.modern")
-   com.facebook.buck.rules.modern.[[InputRuleResolver.UnsafeInternals]{.typeNameLink}](InputRuleResolver.UnsafeInternals.html "interface in com.facebook.buck.rules.modern")
-   com.facebook.buck.rules.modern.[[OutputPathResolver]{.typeNameLink}](OutputPathResolver.html "interface in com.facebook.buck.rules.modern")
-   com.facebook.buck.rules.modern.[[Serializer.Delegate]{.typeNameLink}](Serializer.Delegate.html "interface in com.facebook.buck.rules.modern")
-   com.facebook.buck.rules.modern.[[ValueCreator]{.typeNameLink}](ValueCreator.html "interface in com.facebook.buck.rules.modern")\<E\>
-   com.facebook.buck.rules.modern.[[ValueTypeInfo]{.typeNameLink}](ValueTypeInfo.html "interface in com.facebook.buck.rules.modern")\<T\>
-   com.facebook.buck.rules.modern.[[ValueVisitor]{.typeNameLink}](ValueVisitor.html "interface in com.facebook.buck.rules.modern")\<E\>
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
