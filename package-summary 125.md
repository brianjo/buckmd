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

-   [Overview](../../../../../../index.html)
-   Package
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
# Package com.facebook.buck.rules.modern.impl {#package-com.facebook.buck.rules.modern.impl .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [AbstractValueVisitor](AbstractVa | ::: block                         |
    | lueVisitor.html "class in com.fac | An abstract implementation of     |
    | ebook.buck.rules.modern.impl")\<E | ValueVisitor used for             |
    | extends                           | implementations that only care    |
    | [Exception](ht                    | about some underlying             |
    | tp://docs.oracle.com/javase/7/doc | non-composed types.               |
    | s/api/java/lang/Exception.html?is | :::                               |
    | -external=true "class or interfac |                                   |
    | e in java.lang"){.externalLink}\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [BuildTargetTypeInfo](BuildT      | ::: block                         |
    | argetTypeInfo.html "class in com. | TypeInfo for BuildTarget values.  |
    | facebook.buck.rules.modern.impl") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DefaultClassInfo](Defaul         | ::: block                         |
    | tClassInfo.html "class in com.fac | Default implementation of         |
    | ebook.buck.rules.modern.impl")\<T | ClassInfo.                        |
    | extends                           | :::                               |
    | [AddsT                            |                                   |
    | oRuleKey](../../../core/rulekey/A |                                   |
    | ddsToRuleKey.html "interface in c |                                   |
    | om.facebook.buck.core.rulekey")\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [De                               | ::: block                         |
    | faultClassInfoFactory](DefaultCla | Creates and caches the default    |
    | ssInfoFactory.html "class in com. | ClassInfo implementations.        |
    | facebook.buck.rules.modern.impl") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Defa                             |                                   |
    | ultInputRuleResolver](DefaultInpu |                                   |
    | tRuleResolver.html "class in com. |                                   |
    | facebook.buck.rules.modern.impl") |                                   |
    +-----------------------------------+-----------------------------------+
    | [DepsComputingVisitor](DepsCom    | ::: block                         |
    | putingVisitor.html "class in com. | Computes all the deps by visiting |
    | facebook.buck.rules.modern.impl") | all referenced SourcePaths.       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DynamicTypeInfo](Dy              | ::: block                         |
    | namicTypeInfo.html "class in com. | This type info delegates to a     |
    | facebook.buck.rules.modern.impl") | ClassInfo looked up at runtime.   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [E                                | ::: block                         |
    | itherValueTypeInfo](EitherValueTy | ValueTypeInfo for Eithers.        |
    | peInfo.html "class in com.faceboo | :::                               |
    | k.buck.rules.modern.impl")\<L,​R\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [EnumValueTypeInfo](EnumVal       | ::: block                         |
    | ueTypeInfo.html "class in com.fac | ValueTypeInfo for enums.          |
    | ebook.buck.rules.modern.impl")\<T | :::                               |
    | extends                           |                                   |
    | [Enum](ht                         |                                   |
    | tp://docs.oracle.com/javase/7/doc |                                   |
    | s/api/java/lang/Enum.html?is-exte |                                   |
    | rnal=true "class or interface in  |                                   |
    | java.lang"){.externalLink}\<T\>\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [HashCodeValueTypeInfo](HashCode  | ::: block                         |
    | ValueTypeInfo.html "class in com. | ValueTypeInfo for HashCode.       |
    | facebook.buck.rules.modern.impl") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ImmutableMapV                    | ::: block                         |
    | alueTypeInfo](ImmutableMapValueTy | ValueTypeInfo for                 |
    | peInfo.html "class in com.faceboo | ImmutableSortedMaps.              |
    | k.buck.rules.modern.impl")\<K,​V\> | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ImmutableSe                      | ::: block                         |
    | tValueTypeInfo](ImmutableSetValue | ValueTypeInfo for                 |
    | TypeInfo.html "class in com.faceb | ImmutableSortedSets.              |
    | ook.buck.rules.modern.impl")\<T\> | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ImmutableSortedMapValueTy        | ::: block                         |
    | peInfo](ImmutableSortedMapValueTy | ValueTypeInfo for                 |
    | peInfo.html "class in com.faceboo | ImmutableSortedMaps.              |
    | k.buck.rules.modern.impl")\<K,​V\> | :::                               |
    +-----------------------------------+-----------------------------------+
    | [InputsMapBuilder](Inp            | ::: block                         |
    | utsMapBuilder.html "class in com. | InputsMapBuilder is used to find  |
    | facebook.buck.rules.modern.impl") | all the input SourcePaths of a    |
    |                                   | Buildable.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [InputsMapBuilder.Data](InputsMa  | ::: block                         |
    | pBuilder.Data.html "class in com. | Holds the information derived     |
    | facebook.buck.rules.modern.impl") | from a rulekey appendable.        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | ModernBuildableSupport](ModernBui | ModernBuildableSupport provides   |
    | ldableSupport.html "class in com. | methods to make using,            |
    | facebook.buck.rules.modern.impl") | implementing and migrating to     |
    |                                   | ModernBuildRules easier.          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NonHashab                        | ::: block                         |
    | leSourcePathContainerValueTypeInf | ValueTypeInfo for a               |
    | o](NonHashableSourcePathContainer | NonHashableSourcePathContainer.   |
    | ValueTypeInfo.html "class in com. | :::                               |
    | facebook.buck.rules.modern.impl") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Nul                              | ::: block                         |
    | lableValueTypeInfo](NullableValue | ValueTypeInfo for fields marked   |
    | TypeInfo.html "class in com.faceb | \@Nullable.                       |
    | ook.buck.rules.modern.impl")\<T\> | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Outp                             | ::: block                         |
    | utLabelValueTypeInfo](OutputLabel | [`ValueTypeInfo`](..              |
    | ValueTypeInfo.html "class in com. | /ValueTypeInfo.html "interface in |
    | facebook.buck.rules.modern.impl") |  com.facebook.buck.rules.modern") |
    |                                   | for                               |
    |                                   | [`OutputLabel`](../../../co       |
    |                                   | re/model/OutputLabel.html "class  |
    |                                   | in com.facebook.buck.core.model") |
    |                                   | instances.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [OutputPathVisitor](Outp          | ::: block                         |
    | utPathVisitor.html "class in com. | Visits all the referenced         |
    | facebook.buck.rules.modern.impl") | OutputPaths.                      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PatternValueTypeInfo](Pattern    | ::: block                         |
    | ValueTypeInfo.html "class in com. | ValueTypeInfo for Pattern.        |
    | facebook.buck.rules.modern.impl") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [So                               | ::: block                         |
    | urcePathValueTypeInfo](SourcePath | ValueTypeInfo for SourcePaths.    |
    | ValueTypeInfo.html "class in com. | :::                               |
    | facebook.buck.rules.modern.impl") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Stri                             | ::: block                         |
    | ngifyingValueVisitor](Stringifyin | A ValueVisitor that can be used   |
    | gValueVisitor.html "class in com. | to construct a String             |
    | facebook.buck.rules.modern.impl") | representation of an object.      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [StringifyingValueVisitor.        |                                   |
    | ExcludeFromStringification](Strin |                                   |
    | gifyingValueVisitor.ExcludeFromSt |                                   |
    | ringification.html "class in com. |                                   |
    | facebook.buck.rules.modern.impl") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Sup                              | ::: block                         |
    | plierValueTypeInfo](SupplierValue | ValueTypeInfo for Suppliers.      |
    | TypeInfo.html "class in com.faceb | :::                               |
    | ook.buck.rules.modern.impl")\<T\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [TargetConf                       | ::: block                         |
    | igurationTypeInfo](TargetConfigur | TypeInfo for TargetConfiguration  |
    | ationTypeInfo.html "class in com. | values.                           |
    | facebook.buck.rules.modern.impl") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ToolchainTypeInfo](Toolcha       | ::: block                         |
    | inTypeInfo.html "class in com.fac | TypeInfo for all Toolchains.      |
    | ebook.buck.rules.modern.impl")\<T | :::                               |
    | extends                           |                                   |
    | [T                                |                                   |
    | oolchain](../../../core/toolchain |                                   |
    | /Toolchain.html "interface in com |                                   |
    | .facebook.buck.core.toolchain")\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [UnconfiguredBuildT               | ::: block                         |
    | argetTypeInfo](UnconfiguredBuildT | TypeInfo for BuildTarget values.  |
    | argetTypeInfo.html "class in com. | :::                               |
    | facebook.buck.rules.modern.impl") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ValueTypeInfoFactory](ValueTy    | ::: block                         |
    | peInfoFactory.html "class in com. | Creates ValueTypeInfos for given  |
    | facebook.buck.rules.modern.impl") | Types/TypeTokens.                 |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ValueTypeInfos](V                | ::: block                         |
    | alueTypeInfos.html "class in com. | Some utilities and simple         |
    | facebook.buck.rules.modern.impl") | implementations for               |
    |                                   | ValueTypeInfo.                    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ValueTypeInfos.ExcludedValue     | ::: block                         |
    | TypeInfo](ValueTypeInfos.Excluded | ValueTypeInfo for fields that are |
    | ValueTypeInfo.html "class in com. | not annotated with                |
    | facebook.buck.rules.modern.impl") | \@AddToRuleKey.                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../../../index.html)
-   Package
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

[]{#skip.navbar.bottom}
:::
