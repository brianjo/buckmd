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
[Package]{.packageLabelInType} [com.facebook.buck.rules.modern](package-summary.html)
:::

## Interface ValueTypeInfo\<T\> {#interface-valuetypeinfot .title title="Interface ValueTypeInfo"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `BuildTargetTypeInfo`, `DynamicTypeInfo`, `EitherValueTypeInfo`,
        `EnumValueTypeInfo`, `HashCodeValueTypeInfo`,
        `ImmutableMapValueTypeInfo`, `ImmutableSetValueTypeInfo`,
        `ImmutableSortedMapValueTypeInfo`,
        `NonHashableSourcePathContainerValueTypeInfo`,
        `NullableValueTypeInfo`, `OutputLabelValueTypeInfo`,
        `PatternValueTypeInfo`, `SourcePathValueTypeInfo`,
        `SupplierValueTypeInfo`, `TargetConfigurationTypeInfo`,
        `ToolchainTypeInfo`, `UnconfiguredBuildTargetTypeInfo`,
        `ValueTypeInfos.ExcludedValueTypeInfo`

    ------------------------------------------------------------------------

        public interface ValueTypeInfo<T>

    ::: block
    ValueTypeInfo\<T\> provides methods to extract deps, outputs,
    rulekeys from values of type T.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                  Method                                           Description
          ---------------------------------- ------------------------------------------------ -------------
          `<E extends Exception>T`           `create​(ValueCreator<E> creator)`                 
          `default <E extends Exception>T`   `createNotNull​(ValueCreator<E> creator)`          
          `<E extends Exception>void`        `visit​(T value,      ValueVisitor<E> visitor)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
          .tableTab}[[Default
          Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#visit(java.lang.Object,com.facebook.buck.rules.modern.ValueVisitor)}
        []{#visit(T,com.facebook.buck.rules.modern.ValueVisitor)}

        -   #### visit

            ``` methodSignature
            <E extends Exception> void visit​(T value,
                                             ValueVisitor<E> visitor)
                                      throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#create(com.facebook.buck.rules.modern.ValueCreator)}

        -   #### create

            ``` methodSignature
            @Nullable
            <E extends Exception> T create​(ValueCreator<E> creator)
                                    throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#createNotNull(com.facebook.buck.rules.modern.ValueCreator)}

        -   #### createNotNull

            ``` methodSignature
            default <E extends Exception> T createNotNull​(ValueCreator<E> creator)
                                                   throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`
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
