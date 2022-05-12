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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.analysis](package-summary.html)
:::

## Interface RuleAnalysisResult {#interface-ruleanalysisresult .title title="Interface RuleAnalysisResult"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `ActionAnalysisDataLookUp`, `ComputeResult`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `LegacyProviderRuleAnalysisResult`

    ------------------------------------------------------------------------

        public interface RuleAnalysisResult
        extends ActionAnalysisDataLookUp, ComputeResult

    ::: block
    The result of performing rule analysis over a single
    [`BuildTarget`](../../model/BuildTarget.html "class in com.facebook.buck.core.model")
    rule.
    This is similar to Bazel\'s
    `  com.google.devtools.build.lib.skyframe.ConfiguredTargetValue`.
    {@see
    [ConfiguredTargetValue](https://github.com/bazelbuild/bazel/blob/master/src/main/java/com/google/devtools/build/lib/skyframe/ConfiguredTargetValue.java)}
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type          Method                 Description
          -------------------------- ---------------------- -------------
          `BuildTarget`              `getBuildTarget()`      
          `ProviderInfoCollection`   `getProviderInfos()`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.analysis.action.ActionAnalysisDataLookUp}

            ### Methods inherited from interface com.facebook.buck.core.rules.analysis.action.[ActionAnalysisDataLookUp](action/ActionAnalysisDataLookUp.html "interface in com.facebook.buck.core.rules.analysis.action")

            `actionExists, getActionOptional, getRegisteredActions`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildTarget()}

        -   #### getBuildTarget

            ``` methodSignature
            BuildTarget getBuildTarget()
            ```

            [Returns:]{.returnLabel}
            :   [`BuildTarget`](../../model/BuildTarget.html "class in com.facebook.buck.core.model")
                of the rule

        []{#getProviderInfos()}

        -   #### getProviderInfos

            ``` methodSignature
            ProviderInfoCollection getProviderInfos()
            ```

            [Returns:]{.returnLabel}
            :   a
                [`ProviderInfoCollection`](../providers/collect/ProviderInfoCollection.html "interface in com.facebook.buck.core.rules.providers.collect")
                exported by the rule
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
