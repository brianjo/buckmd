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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.graph.transformation.model](package-summary.html)
:::

## Interface ComputeKey\<ResultType extends [ComputeResult](ComputeResult.html "interface in com.facebook.buck.core.graph.transformation.model")\> {#interface-computekeyresulttype-extends-computeresult .title title="Interface ComputeKey"}
:::

::: contentContainer
::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `ResultType` - should be the corresponding result type of
        performing the transformation in the
        [`GraphComputation`](../GraphComputation.html "interface in com.facebook.buck.core.graph.transformation")

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `BuildPackagePathToBuildFileManifestKey`,
        `BuildPackagePathToUnconfiguredTargetNodePackageKey`,
        `BuildTargetPatternToBuildPackagePathKey`,
        `BuildTargetToUnconfiguredTargetNodeKey`, `ComposedKey`,
        `DirectoryListKey`, `FileTreeKey`, `RuleAnalysisKey`,
        `UnconfiguredTargetNodeToUnconfiguredTargetNodeWithDepsKey`

    ------------------------------------------------------------------------

        public interface ComputeKey<ResultType extends ComputeResult>

    ::: block
    This is an interface for all keys to be used in
    [`GraphComputation`](../GraphComputation.html "interface in com.facebook.buck.core.graph.transformation").
    Implementation should define a static to expose
    [`getIdentifier()`](#getIdentifier()) statically for users and for
    avoiding recomputation.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                     Method              Description
          ------------------------------------- ------------------- -------------
          `ComputationIdentifier<ResultType>`   `getIdentifier()`    

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

        []{#getIdentifier()}

        -   #### getIdentifier

            ``` methodSignature
            ComputationIdentifier<ResultType> getIdentifier()
            ```

            [Returns:]{.returnLabel}
            :   the identifier of this key. This identifier is used to
                map all keys of the same
                [`ComputationIdentifier`](ComputationIdentifier.html "interface in com.facebook.buck.core.graph.transformation.model")
                to the same
                [`GraphComputation`](../GraphComputation.html "interface in com.facebook.buck.core.graph.transformation").
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
