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
# Hierarchy For Package com.facebook.buck.rules.coercer {#hierarchy-for-package-com.facebook.buck.rules.coercer .title}

[Package Hierarchies:]{.packageHierarchyLabel}

-   [All Packages](../../../../../overview-tree.html)
:::

::: contentContainer
::: {.section role="region"}
## Class Hierarchy {#class-hierarchy title="Class Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   com.facebook.buck.rules.coercer.[[AbsoluteOutputMacroTypeCoercer]{.typeNameLink}](AbsoluteOutputMacroTypeCoercer.html "class in com.facebook.buck.rules.coercer")
    -   com.facebook.buck.rules.coercer.[[AbstractParamInfo]{.typeNameLink}](AbstractParamInfo.html "class in com.facebook.buck.rules.coercer")\<T\>
        (implements
        com.facebook.buck.rules.coercer.[ParamInfo](ParamInfo.html "interface in com.facebook.buck.rules.coercer")\<T\>)
        -   com.facebook.buck.rules.coercer.[[ReflectionParamInfo]{.typeNameLink}](ReflectionParamInfo.html "class in com.facebook.buck.rules.coercer")\<T\>
    -   com.facebook.buck.rules.coercer.[[BuildConfigFields]{.typeNameLink}](BuildConfigFields.html "class in com.facebook.buck.rules.coercer")
        (implements
        java.lang.[Iterable](http://docs.oracle.com/javase/7/docs/api/java/lang/Iterable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>)
    -   com.facebook.buck.rules.coercer.[[BuildConfigFields.Field]{.typeNameLink}](BuildConfigFields.Field.html "class in com.facebook.buck.rules.coercer")
    -   com.facebook.buck.rules.coercer.[[BuildTargetMacroTypeCoercer]{.typeNameLink}](BuildTargetMacroTypeCoercer.html "class in com.facebook.buck.rules.coercer")\<M\>
    -   com.facebook.buck.rules.coercer.[[CollectionTypeCoercer]{.typeNameLink}](CollectionTypeCoercer.html "class in com.facebook.buck.rules.coercer")\<D,​C,​U,​T\>
        (implements
        com.facebook.buck.rules.coercer.[TypeCoercer](TypeCoercer.html "interface in com.facebook.buck.rules.coercer")\<U,​T\>)
        -   com.facebook.buck.rules.coercer.[[ListTypeCoercer]{.typeNameLink}](ListTypeCoercer.html "class in com.facebook.buck.rules.coercer")\<U,​T\>
            (implements
            com.facebook.buck.rules.coercer.concat.[Concatable](concat/Concatable.html "interface in com.facebook.buck.rules.coercer.concat")\<T\>)
        -   com.facebook.buck.rules.coercer.[[SetTypeCoercer]{.typeNameLink}](SetTypeCoercer.html "class in com.facebook.buck.rules.coercer")\<U,​T\>
        -   com.facebook.buck.rules.coercer.[[SortedSetTypeCoercer]{.typeNameLink}](SortedSetTypeCoercer.html "class in com.facebook.buck.rules.coercer")\<U,​T\>
    -   com.facebook.buck.rules.coercer.[[CxxGenruleFilterAndTargetsMacroTypeCoercer]{.typeNameLink}](CxxGenruleFilterAndTargetsMacroTypeCoercer.html "class in com.facebook.buck.rules.coercer")\<M\>
    -   com.facebook.buck.rules.coercer.[[CxxLinkGroupMappingCoercer]{.typeNameLink}](CxxLinkGroupMappingCoercer.html "class in com.facebook.buck.rules.coercer")
        (implements
        com.facebook.buck.rules.coercer.[TypeCoercer](TypeCoercer.html "interface in com.facebook.buck.rules.coercer")\<U,​T\>)
    -   com.facebook.buck.rules.coercer.[[CxxLinkGroupMappingTargetCoercer]{.typeNameLink}](CxxLinkGroupMappingTargetCoercer.html "class in com.facebook.buck.rules.coercer")
        (implements
        com.facebook.buck.rules.coercer.[TypeCoercer](TypeCoercer.html "interface in com.facebook.buck.rules.coercer")\<U,​T\>)
    -   com.facebook.buck.rules.coercer.[[DataTransferObjectDescriptor]{.typeNameLink}](DataTransferObjectDescriptor.html "class in com.facebook.buck.rules.coercer")\<T\>
    -   com.facebook.buck.rules.coercer.[[DefaultConstructorArgMarshaller]{.typeNameLink}](DefaultConstructorArgMarshaller.html "class in com.facebook.buck.rules.coercer")
        (implements
        com.facebook.buck.rules.coercer.[ConstructorArgMarshaller](ConstructorArgMarshaller.html "interface in com.facebook.buck.rules.coercer"))
    -   com.facebook.buck.rules.coercer.[[DefaultTypeCoercerFactory]{.typeNameLink}](DefaultTypeCoercerFactory.html "class in com.facebook.buck.rules.coercer")
        (implements
        com.facebook.buck.rules.coercer.[TypeCoercerFactory](TypeCoercerFactory.html "interface in com.facebook.buck.rules.coercer"))
    -   com.facebook.buck.rules.coercer.[[EitherTypeCoercer]{.typeNameLink}](EitherTypeCoercer.html "class in com.facebook.buck.rules.coercer")\<LU,​RU,​Left,​Right\>
        (implements
        com.facebook.buck.rules.coercer.[TypeCoercer](TypeCoercer.html "interface in com.facebook.buck.rules.coercer")\<U,​T\>)
    -   com.facebook.buck.rules.coercer.[[EnvMacroTypeCoercer]{.typeNameLink}](EnvMacroTypeCoercer.html "class in com.facebook.buck.rules.coercer")
    -   com.facebook.buck.rules.coercer.[[FrameworkPath]{.typeNameLink}](FrameworkPath.html "class in com.facebook.buck.rules.coercer")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"),
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>)
    -   com.facebook.buck.rules.coercer.[[FrameworkPathTypeCoercer]{.typeNameLink}](FrameworkPathTypeCoercer.html "class in com.facebook.buck.rules.coercer")
        (implements
        com.facebook.buck.rules.coercer.[TypeCoercer](TypeCoercer.html "interface in com.facebook.buck.rules.coercer")\<U,​T\>)
    -   com.facebook.buck.rules.coercer.ImmutableManifestEntries.Builder
        -   com.facebook.buck.rules.coercer.[[ManifestEntries.Builder]{.typeNameLink}](ManifestEntries.Builder.html "class in com.facebook.buck.rules.coercer")
    -   com.facebook.buck.rules.coercer.[[ImmutableTypeCoercer]{.typeNameLink}](ImmutableTypeCoercer.html "class in com.facebook.buck.rules.coercer")\<T\>
        (implements
        com.facebook.buck.rules.coercer.[TypeCoercer](TypeCoercer.html "interface in com.facebook.buck.rules.coercer")\<U,​T\>)
    -   com.facebook.buck.rules.coercer.[[LeafTypeCoercer]{.typeNameLink}](LeafTypeCoercer.html "class in com.facebook.buck.rules.coercer")\<T\>
        (implements
        com.facebook.buck.rules.coercer.[TypeCoercer](TypeCoercer.html "interface in com.facebook.buck.rules.coercer")\<U,​T\>)
        -   com.facebook.buck.rules.coercer.[[BuildConfigFieldsTypeCoercer]{.typeNameLink}](BuildConfigFieldsTypeCoercer.html "class in com.facebook.buck.rules.coercer")
        -   com.facebook.buck.rules.coercer.[[CxxLinkGroupMappingTargetTraversalCoercer]{.typeNameLink}](CxxLinkGroupMappingTargetTraversalCoercer.html "class in com.facebook.buck.rules.coercer")
        -   com.facebook.buck.rules.coercer.[[ManifestEntriesTypeCoercer]{.typeNameLink}](ManifestEntriesTypeCoercer.html "class in com.facebook.buck.rules.coercer")
    -   com.facebook.buck.rules.coercer.[[LeafTypeNewCoercer]{.typeNameLink}](LeafTypeNewCoercer.html "class in com.facebook.buck.rules.coercer")\<U,​T\>
        (implements
        com.facebook.buck.rules.coercer.[TypeCoercer](TypeCoercer.html "interface in com.facebook.buck.rules.coercer")\<U,​T\>)
        -   com.facebook.buck.rules.coercer.[[BuildTargetTypeCoercer]{.typeNameLink}](BuildTargetTypeCoercer.html "class in com.facebook.buck.rules.coercer")
        -   com.facebook.buck.rules.coercer.[[BuildTargetWithOutputsTypeCoercer]{.typeNameLink}](BuildTargetWithOutputsTypeCoercer.html "class in com.facebook.buck.rules.coercer")
        -   com.facebook.buck.rules.coercer.[[LeafUnconfiguredOnlyCoercer]{.typeNameLink}](LeafUnconfiguredOnlyCoercer.html "class in com.facebook.buck.rules.coercer")\<T\>
            -   com.facebook.buck.rules.coercer.[[ConstraintTypeCoercer]{.typeNameLink}](ConstraintTypeCoercer.html "class in com.facebook.buck.rules.coercer")
            -   com.facebook.buck.rules.coercer.[[EnumTypeCoercer]{.typeNameLink}](EnumTypeCoercer.html "class in com.facebook.buck.rules.coercer")\<E\>
            -   com.facebook.buck.rules.coercer.[[FlavorTypeCoercer]{.typeNameLink}](FlavorTypeCoercer.html "class in com.facebook.buck.rules.coercer")
            -   com.facebook.buck.rules.coercer.[[IdentityTypeCoercer]{.typeNameLink}](IdentityTypeCoercer.html "class in com.facebook.buck.rules.coercer")\<T\>
                -   com.facebook.buck.rules.coercer.[[StringTypeCoercer]{.typeNameLink}](StringTypeCoercer.html "class in com.facebook.buck.rules.coercer")
            -   com.facebook.buck.rules.coercer.[[LogLevelTypeCoercer]{.typeNameLink}](LogLevelTypeCoercer.html "class in com.facebook.buck.rules.coercer")
            -   com.facebook.buck.rules.coercer.[[NumberTypeCoercer]{.typeNameLink}](NumberTypeCoercer.html "class in com.facebook.buck.rules.coercer")\<T\>
            -   com.facebook.buck.rules.coercer.[[PathTypeCoercer]{.typeNameLink}](PathTypeCoercer.html "class in com.facebook.buck.rules.coercer")
            -   com.facebook.buck.rules.coercer.[[PatternTypeCoercer]{.typeNameLink}](PatternTypeCoercer.html "class in com.facebook.buck.rules.coercer")
            -   com.facebook.buck.rules.coercer.[[UnconfiguredBuildTargetTypeCoercer]{.typeNameLink}](UnconfiguredBuildTargetTypeCoercer.html "class in com.facebook.buck.rules.coercer")
            -   com.facebook.buck.rules.coercer.[[UnconfiguredBuildTargetWithOutputsTypeCoercer]{.typeNameLink}](UnconfiguredBuildTargetWithOutputsTypeCoercer.html "class in com.facebook.buck.rules.coercer")
        -   com.facebook.buck.rules.coercer.[[SourcePathTypeCoercer]{.typeNameLink}](SourcePathTypeCoercer.html "class in com.facebook.buck.rules.coercer")
    -   com.facebook.buck.rules.coercer.[[ManifestEntries]{.typeNameLink}](ManifestEntries.html "class in com.facebook.buck.rules.coercer")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"))
    -   com.facebook.buck.rules.coercer.[[MapTypeCoercer]{.typeNameLink}](MapTypeCoercer.html "class in com.facebook.buck.rules.coercer")\<KU,​VU,​K,​V\>
        (implements
        com.facebook.buck.rules.coercer.[TypeCoercer](TypeCoercer.html "interface in com.facebook.buck.rules.coercer")\<U,​T\>)
    -   com.facebook.buck.rules.coercer.[[NeededCoverageSpec]{.typeNameLink}](NeededCoverageSpec.html "class in com.facebook.buck.rules.coercer")
        (implements
        com.facebook.buck.versions.[TargetTranslatable](../../versions/TargetTranslatable.html "interface in com.facebook.buck.versions")\<T\>)
    -   com.facebook.buck.rules.coercer.[[NeededCoverageSpecTypeCoercer]{.typeNameLink}](NeededCoverageSpecTypeCoercer.html "class in com.facebook.buck.rules.coercer")
        (implements
        com.facebook.buck.rules.coercer.[TypeCoercer](TypeCoercer.html "interface in com.facebook.buck.rules.coercer")\<U,​T\>)
    -   com.facebook.buck.rules.coercer.[[OptionalTypeCoercer]{.typeNameLink}](OptionalTypeCoercer.html "class in com.facebook.buck.rules.coercer")\<U,​T\>
        (implements
        com.facebook.buck.rules.coercer.[TypeCoercer](TypeCoercer.html "interface in com.facebook.buck.rules.coercer")\<U,​T\>)
    -   com.facebook.buck.rules.coercer.[[OutputMacroTypeCoercer]{.typeNameLink}](OutputMacroTypeCoercer.html "class in com.facebook.buck.rules.coercer")
    -   com.facebook.buck.rules.coercer.[[PairTypeCoercer]{.typeNameLink}](PairTypeCoercer.html "class in com.facebook.buck.rules.coercer")\<FU,​SU,​FIRST,​SECOND\>
        (implements
        com.facebook.buck.rules.coercer.[TypeCoercer](TypeCoercer.html "interface in com.facebook.buck.rules.coercer")\<U,​T\>)
    -   com.facebook.buck.rules.coercer.[[PatternMatchedCollection]{.typeNameLink}](PatternMatchedCollection.html "class in com.facebook.buck.rules.coercer")\<T\>
        (implements
        com.facebook.buck.versions.[TargetTranslatable](../../versions/TargetTranslatable.html "interface in com.facebook.buck.versions")\<T\>)
    -   com.facebook.buck.rules.coercer.[[PatternMatchedCollection.Builder]{.typeNameLink}](PatternMatchedCollection.Builder.html "class in com.facebook.buck.rules.coercer")\<T\>
    -   com.facebook.buck.rules.coercer.[[PatternMatchedCollectionTypeCoercer]{.typeNameLink}](PatternMatchedCollectionTypeCoercer.html "class in com.facebook.buck.rules.coercer")\<T\>
        (implements
        com.facebook.buck.rules.coercer.[TypeCoercer](TypeCoercer.html "interface in com.facebook.buck.rules.coercer")\<U,​T\>)
    -   com.facebook.buck.rules.coercer.[[QueryCoercer]{.typeNameLink}](QueryCoercer.html "class in com.facebook.buck.rules.coercer")
        (implements
        com.facebook.buck.rules.coercer.[TypeCoercer](TypeCoercer.html "interface in com.facebook.buck.rules.coercer")\<U,​T\>)
    -   com.facebook.buck.rules.coercer.[[SortedMapTypeCoercer]{.typeNameLink}](SortedMapTypeCoercer.html "class in com.facebook.buck.rules.coercer")\<KU,​VU,​K,​V\>
        (implements
        com.facebook.buck.rules.coercer.[TypeCoercer](TypeCoercer.html "interface in com.facebook.buck.rules.coercer")\<U,​T\>)
    -   com.facebook.buck.rules.coercer.[[SortedSetConcatable]{.typeNameLink}](SortedSetConcatable.html "class in com.facebook.buck.rules.coercer")\<T\>
        (implements
        com.facebook.buck.rules.coercer.concat.[Concatable](concat/Concatable.html "interface in com.facebook.buck.rules.coercer.concat")\<T\>)
    -   com.facebook.buck.rules.coercer.[[SourceSet]{.typeNameLink}](SourceSet.html "class in com.facebook.buck.rules.coercer")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"),
        com.facebook.buck.versions.[TargetTranslatable](../../versions/TargetTranslatable.html "interface in com.facebook.buck.versions")\<T\>)
    -   com.facebook.buck.rules.coercer.[[SourceSetConcatable]{.typeNameLink}](SourceSetConcatable.html "class in com.facebook.buck.rules.coercer")
        (implements
        com.facebook.buck.rules.coercer.concat.[Concatable](concat/Concatable.html "interface in com.facebook.buck.rules.coercer.concat")\<T\>)
        -   com.facebook.buck.rules.coercer.[[SourceSetTypeCoercer]{.typeNameLink}](SourceSetTypeCoercer.html "class in com.facebook.buck.rules.coercer")
            (implements
            com.facebook.buck.rules.coercer.[TypeCoercer](TypeCoercer.html "interface in com.facebook.buck.rules.coercer")\<U,​T\>)
    -   com.facebook.buck.rules.coercer.[[SourceSortedSet]{.typeNameLink}](SourceSortedSet.html "class in com.facebook.buck.rules.coercer")
        (implements
        com.facebook.buck.versions.[TargetTranslatable](../../versions/TargetTranslatable.html "interface in com.facebook.buck.versions")\<T\>)
    -   com.facebook.buck.rules.coercer.[[SourceSortedSetConcatable]{.typeNameLink}](SourceSortedSetConcatable.html "class in com.facebook.buck.rules.coercer")
        (implements
        com.facebook.buck.rules.coercer.concat.[Concatable](concat/Concatable.html "interface in com.facebook.buck.rules.coercer.concat")\<T\>)
        -   com.facebook.buck.rules.coercer.[[SourceSortedSetTypeCoercer]{.typeNameLink}](SourceSortedSetTypeCoercer.html "class in com.facebook.buck.rules.coercer")
            (implements
            com.facebook.buck.rules.coercer.[TypeCoercer](TypeCoercer.html "interface in com.facebook.buck.rules.coercer")\<U,​T\>)
    -   com.facebook.buck.rules.coercer.[[SourceWithFlagsList]{.typeNameLink}](SourceWithFlagsList.html "class in com.facebook.buck.rules.coercer")
    -   com.facebook.buck.rules.coercer.[[SourceWithFlagsListTypeCoercer]{.typeNameLink}](SourceWithFlagsListTypeCoercer.html "class in com.facebook.buck.rules.coercer")
        (implements
        com.facebook.buck.rules.coercer.[TypeCoercer](TypeCoercer.html "interface in com.facebook.buck.rules.coercer")\<U,​T\>)
    -   com.facebook.buck.rules.coercer.[[SourceWithFlagsTypeCoercer]{.typeNameLink}](SourceWithFlagsTypeCoercer.html "class in com.facebook.buck.rules.coercer")
        (implements
        com.facebook.buck.rules.coercer.[TypeCoercer](TypeCoercer.html "interface in com.facebook.buck.rules.coercer")\<U,​T\>)
    -   com.facebook.buck.rules.coercer.[[StringWithMacrosTypeCoercer]{.typeNameLink}](StringWithMacrosTypeCoercer.html "class in com.facebook.buck.rules.coercer")
        (implements
        com.facebook.buck.rules.coercer.[TypeCoercer](TypeCoercer.html "interface in com.facebook.buck.rules.coercer")\<U,​T\>)
    -   com.facebook.buck.rules.coercer.[[TestRunnerSpecCoercer]{.typeNameLink}](TestRunnerSpecCoercer.html "class in com.facebook.buck.rules.coercer")
        (implements
        com.facebook.buck.rules.coercer.[TypeCoercer](TypeCoercer.html "interface in com.facebook.buck.rules.coercer")\<U,​T\>)
    -   java.lang.[[Throwable]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Throwable.html?is-external=true "class or interface in java.lang"){.externalLink}
        (implements
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   java.lang.[[Exception]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Exception.html?is-external=true "class or interface in java.lang"){.externalLink}
            -   com.facebook.buck.rules.coercer.[[CoerceFailedException]{.typeNameLink}](CoerceFailedException.html "class in com.facebook.buck.rules.coercer")
            -   com.facebook.buck.rules.coercer.[[DataTransferObjectDescriptor.BuilderBuildFailedException]{.typeNameLink}](DataTransferObjectDescriptor.BuilderBuildFailedException.html "class in com.facebook.buck.rules.coercer")
            -   com.facebook.buck.rules.coercer.[[ParamInfoException]{.typeNameLink}](ParamInfoException.html "class in com.facebook.buck.rules.coercer")
    -   com.facebook.buck.rules.coercer.[[VersionMatchedCollection]{.typeNameLink}](VersionMatchedCollection.html "class in com.facebook.buck.rules.coercer")\<T\>
        (implements
        com.facebook.buck.versions.[TargetTranslatable](../../versions/TargetTranslatable.html "interface in com.facebook.buck.versions")\<T\>)
    -   com.facebook.buck.rules.coercer.[[VersionMatchedCollection.Builder]{.typeNameLink}](VersionMatchedCollection.Builder.html "class in com.facebook.buck.rules.coercer")\<T\>
    -   com.facebook.buck.rules.coercer.[[VersionMatchedCollectionTypeCoercer]{.typeNameLink}](VersionMatchedCollectionTypeCoercer.html "class in com.facebook.buck.rules.coercer")\<T\>
        (implements
        com.facebook.buck.rules.coercer.[TypeCoercer](TypeCoercer.html "interface in com.facebook.buck.rules.coercer")\<U,​T\>)
    -   com.facebook.buck.rules.coercer.[[ZeroArgMacroTypeCoercer]{.typeNameLink}](ZeroArgMacroTypeCoercer.html "class in com.facebook.buck.rules.coercer")\<M\>
:::

::: {.section role="region"}
## Interface Hierarchy {#interface-hierarchy title="Interface Hierarchy"}

-   com.facebook.buck.rules.coercer.concat.[[Concatable]{.typeNameLink}](concat/Concatable.html "interface in com.facebook.buck.rules.coercer.concat")\<T\>
    -   com.facebook.buck.rules.coercer.[[TypeCoercer]{.typeNameLink}](TypeCoercer.html "interface in com.facebook.buck.rules.coercer")\<U,​T\>
-   com.facebook.buck.rules.coercer.[[ConstructorArgMarshaller]{.typeNameLink}](ConstructorArgMarshaller.html "interface in com.facebook.buck.rules.coercer")
-   com.facebook.buck.rules.coercer.[[DataTransferObjectDescriptor.BuilderBuildFunction]{.typeNameLink}](DataTransferObjectDescriptor.BuilderBuildFunction.html "interface in com.facebook.buck.rules.coercer")\<T\>
-   com.facebook.buck.rules.coercer.[[ParamInfo]{.typeNameLink}](ParamInfo.html "interface in com.facebook.buck.rules.coercer")\<T\>
-   com.facebook.buck.rules.coercer.[[TypeCoercer.Traversal]{.typeNameLink}](TypeCoercer.Traversal.html "interface in com.facebook.buck.rules.coercer")
    -   com.facebook.buck.rules.coercer.[[ParamInfo.Traversal]{.typeNameLink}](ParamInfo.Traversal.html "interface in com.facebook.buck.rules.coercer")
-   com.facebook.buck.rules.coercer.[[TypeCoercerFactory]{.typeNameLink}](TypeCoercerFactory.html "interface in com.facebook.buck.rules.coercer")
:::

::: {.section role="region"}
## Enum Hierarchy {#enum-hierarchy title="Enum Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   java.lang.[[Enum]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<E\>
        (implements
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   com.facebook.buck.rules.coercer.[[BuildTargetMacroTypeCoercer.TargetOrHost]{.typeNameLink}](BuildTargetMacroTypeCoercer.TargetOrHost.html "enum in com.facebook.buck.rules.coercer")
        -   com.facebook.buck.rules.coercer.[[FrameworkPath.Type]{.typeNameLink}](FrameworkPath.Type.html "enum in com.facebook.buck.rules.coercer")
        -   com.facebook.buck.rules.coercer.[[PathTypeCoercer.PathExistenceVerificationMode]{.typeNameLink}](PathTypeCoercer.PathExistenceVerificationMode.html "enum in com.facebook.buck.rules.coercer")
        -   com.facebook.buck.rules.coercer.[[SourceSet.Type]{.typeNameLink}](SourceSet.Type.html "enum in com.facebook.buck.rules.coercer")
        -   com.facebook.buck.rules.coercer.[[SourceSortedSet.Type]{.typeNameLink}](SourceSortedSet.Type.html "enum in com.facebook.buck.rules.coercer")
        -   com.facebook.buck.rules.coercer.[[SourceWithFlagsList.Type]{.typeNameLink}](SourceWithFlagsList.Type.html "enum in com.facebook.buck.rules.coercer")
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
