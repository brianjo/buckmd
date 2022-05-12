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
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.rules.keys](package-summary.html)
:::

## Interface RuleKeyAppendable {#interface-rulekeyappendable .title title="Interface RuleKeyAppendable"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AddsToRuleKey`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `CxxSymlinkTreeHeaders`

    ------------------------------------------------------------------------

        @Deprecated
        public interface RuleKeyAppendable
        extends AddsToRuleKey

    ::: deprecationBlock
    [Deprecated.]{.deprecatedLabel}
    :::

    ::: block
    Deprecated. Implement
    [`AddsToRuleKey`](../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey")
    instead, and use
    [`AddToRuleKey`](../../core/rulekey/AddToRuleKey.html "annotation in com.facebook.buck.core.rulekey")
    annotations on fields to indicate which ones should be part of the
    rule key.
    TODO(t6430785): Delete this class once no more usages exist
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Interface             | Description           |
        +=======================+=======================+=======================+
        | `static interface `   | `RuleKeyAppendable.R  | ::: block             |
        |                       | uleKeyAppendableSink` | [Deprecate            |
        |                       |                       | d.]{.deprecatedLabel} |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `appendToRuleKey​(Rule | ::: block             |
        |                       | KeyAppendable.RuleKey | [Deprecate            |
        |                       | AppendableSink sink)` | d.]{.deprecatedLabel} |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Deprecated
        Methods](javascript:show(32);)[ ]{.tabEnd}]{#t6 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#appendToRuleKey(com.facebook.buck.rules.keys.RuleKeyAppendable.RuleKeyAppendableSink)}

        -   #### appendToRuleKey

            ``` methodSignature
            @Deprecated
            void appendToRuleKey​(RuleKeyAppendable.RuleKeyAppendableSink sink)
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            ::: block
            Deprecated. Add additional custom things to the rulekey
            builder.
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
-   [Nested](#nested.class.summary) \| 
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
