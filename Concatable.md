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
-   [Package](package-summary.html)
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
[Package]{.packageLabelInType} [com.facebook.buck.rules.coercer.concat](package-summary.html)
:::

## Interface Concatable\<T\> {#interface-concatablet .title title="Interface Concatable"}
:::

::: contentContainer
::: description
-   

    All Known Subinterfaces:
    :   `TypeCoercer<U,​T>`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `BuildConfigFieldsTypeCoercer`, `BuildTargetTypeCoercer`,
        `BuildTargetWithOutputsTypeCoercer`, `CollectionTypeCoercer`,
        `ConstraintTypeCoercer`, `CxxLinkGroupMappingCoercer`,
        `CxxLinkGroupMappingTargetCoercer`,
        `CxxLinkGroupMappingTargetTraversalCoercer`,
        `EitherTypeCoercer`, `EnumTypeCoercer`, `FlavorTypeCoercer`,
        `FrameworkPathTypeCoercer`, `IdentityTypeCoercer`,
        `ImmutableListConcatable`, `ImmutableTypeCoercer`,
        `JsonTypeConcatenatingCoercer`, `LeafTypeCoercer`,
        `LeafTypeNewCoercer`, `LeafUnconfiguredOnlyCoercer`,
        `ListTypeCoercer`, `LogLevelTypeCoercer`,
        `ManifestEntriesTypeCoercer`, `MapTypeCoercer`,
        `NeededCoverageSpecTypeCoercer`, `NumberTypeCoercer`,
        `OptionalTypeCoercer`, `PairTypeCoercer`, `PathTypeCoercer`,
        `PatternMatchedCollectionTypeCoercer`, `PatternTypeCoercer`,
        `QueryCoercer`, `SetTypeCoercer`,
        `SingleElementJsonTypeConcatenatingCoercer`,
        `SortedMapTypeCoercer`, `SortedSetConcatable`,
        `SortedSetTypeCoercer`, `SourcePathTypeCoercer`,
        `SourceSetConcatable`, `SourceSetTypeCoercer`,
        `SourceSortedSetConcatable`, `SourceSortedSetTypeCoercer`,
        `SourceWithFlagsListTypeCoercer`, `SourceWithFlagsTypeCoercer`,
        `StringTypeCoercer`, `StringWithMacrosTypeCoercer`,
        `TestRunnerSpecCoercer`, `UnconfiguredBuildTargetTypeCoercer`,
        `UnconfiguredBuildTargetWithOutputsTypeCoercer`,
        `VersionMatchedCollectionTypeCoercer`

    ------------------------------------------------------------------------

        public interface Concatable<T>

    ::: block
    Indicates that a class provides concatenation operation (which can
    either perform concatenation or indicate that the type doesn\'t
    support concatenation).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                           Description
          ------------------- -------------------------------- -------------
          `T`                 `concat​(Iterable<T> elements)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#concat(java.lang.Iterable)}

        -   #### concat

            ``` methodSignature
            @Nullable
            T concat​(Iterable<T> elements)
            ```

            [Returns:]{.returnLabel}
            :   an instance with concatenated elements or `null` if
                concatenation is not supported for the type
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
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
