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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.knowntypes](package-summary.html)
:::

## Interface KnownRuleTypes {#interface-knownruletypes .title title="Interface KnownRuleTypes"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `HybridKnownRuleTypes`, `KnownNativeRuleTypes`,
        `KnownUserDefinedRuleTypes`

    ------------------------------------------------------------------------

        public interface KnownRuleTypes

    ::: block
    Provides access to rule types and descriptions for both native and
    user defined rules.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `RuleDescriptor<?>`   | `getDescripto         | ::: block             |
        |                       | rByName​(String name)` | Get rule type,        |
        |                       |                       | constructor arg and   |
        |                       |                       | description object    |
        |                       |                       | for by rule name.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default <T           | `getDesc              | ::: block             |
        |  extends ConstructorA | riptorByNameChecked​(S | Safer version of      |
        | rg>RuleDescriptor<T>` | tring name,           | [`getDesc             |
        |                       |                  Clas | riptorByName(String)` |
        |                       | s<T> constructorArg)` | ](#getDescriptorByNam |
        |                       |                       | e(java.lang.String)). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

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

        []{#getDescriptorByName(java.lang.String)}

        -   #### getDescriptorByName

            ``` methodSignature
            RuleDescriptor<?> getDescriptorByName​(String name)
            ```

            ::: block
            Get rule type, constructor arg and description object for by
            rule name.
            :::

        []{#getDescriptorByNameChecked(java.lang.String,java.lang.Class)}

        -   #### getDescriptorByNameChecked

            ``` methodSignature
            default <T extends ConstructorArg> RuleDescriptor<T> getDescriptorByNameChecked​(String name,
                                                                                            Class<T> constructorArg)
            ```

            ::: block
            Safer version of
            [`getDescriptorByName(String)`](#getDescriptorByName(java.lang.String)).
            :::
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
