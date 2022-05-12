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
[Package]{.packageLabelInType} [com.facebook.buck.core.description](package-summary.html)
:::

## Interface RuleDescriptionWithInstanceName\<T extends [BuildRuleArg](arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")\> {#interface-ruledescriptionwithinstancenamet-extends-buildrulearg .title title="Interface RuleDescriptionWithInstanceName"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `BaseDescription<T>`, `Description<T>`, `RuleDescription<T>`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `SkylarkDescription`

    ------------------------------------------------------------------------

        public interface RuleDescriptionWithInstanceName<T extends BuildRuleArg>
        extends RuleDescription<T>

    ::: block
    An instance
    [`RuleDescription`](RuleDescription.html "interface in com.facebook.buck.core.description")
    that has a more complicated name. The common use case is
    [`SkylarkDescription`](../starlark/rule/SkylarkDescription.html "class in com.facebook.buck.core.starlark.rule")
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                  Description
          ------------------- ----------------------- -------------
          `String`            `getRuleName​(T args)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.BaseDescription}

            ### Methods inherited from interface com.facebook.buck.core.description.[BaseDescription](BaseDescription.html "interface in com.facebook.buck.core.description")

            `getConfigurationDeps, getConstructorArgType`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.RuleDescription}

            ### Methods inherited from interface com.facebook.buck.core.description.[RuleDescription](RuleDescription.html "interface in com.facebook.buck.core.description")

            `producesCacheableSubgraph, ruleImpl`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getRuleName(com.facebook.buck.core.description.arg.BuildRuleArg)}
        []{#getRuleName(T)}

        -   #### getRuleName

            ``` methodSignature
            String getRuleName​(T args)
            ```

            [Returns:]{.returnLabel}
            :   The user friendly name of a rule. e.g. cxx_binary, or
                //foo:baz.bzl:some_rule. See
                [`DescriptionCache.getRuleType(BaseDescription)`](impl/DescriptionCache.html#getRuleType(com.facebook.buck.core.description.BaseDescription))
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
