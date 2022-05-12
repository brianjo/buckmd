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
-   Method

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
[Package]{.packageLabelInType} [com.facebook.buck.features.js](package-summary.html)
:::

## Interface JsBundleOutputsDescription\<T extends [BuildRuleArg](../../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")\> {#interface-jsbundleoutputsdescriptiont-extends-buildrulearg .title title="Interface JsBundleOutputsDescription"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `BaseDescription<T>`, `Description<T>`,
        `DescriptionWithTargetGraph<T>`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `JsBundleDescription`, `JsBundleGenruleDescription`

    ------------------------------------------------------------------------

        public interface JsBundleOutputsDescription<T extends BuildRuleArg>
        extends DescriptionWithTargetGraph<T>

    ::: block
    Empty interface to mark
    [`DescriptionWithTargetGraph`](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")
    subclasses that return
    [`JsBundleOutputs`](JsBundleOutputs.html "interface in com.facebook.buck.features.js")
    instances from their
    [`DescriptionWithTargetGraph.createBuildRule(com.facebook.buck.core.rules.BuildRuleCreationContextWithTargetGraph, com.facebook.buck.core.model.BuildTarget, com.facebook.buck.core.rules.BuildRuleParams, T)`](../../core/rules/DescriptionWithTargetGraph.html#createBuildRule(com.facebook.buck.core.rules.BuildRuleCreationContextWithTargetGraph,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.BuildRuleParams,T))
    method.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.BaseDescription}

            ### Methods inherited from interface com.facebook.buck.core.description.[BaseDescription](../../core/description/BaseDescription.html "interface in com.facebook.buck.core.description")

            `getConfigurationDeps, getConstructorArgType`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.DescriptionWithTargetGraph}

            ### Methods inherited from interface com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")

            `createBuildRule, producesCacheableSubgraph`
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
-   Method

</div>

[]{#skip.navbar.bottom}
:::
