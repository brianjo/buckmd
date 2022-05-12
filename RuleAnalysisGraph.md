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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.analysis.computation](package-summary.html)
:::

## Interface RuleAnalysisGraph {#interface-ruleanalysisgraph .title title="Interface RuleAnalysisGraph"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `RuleAnalysisCompatibleDelegatingActionGraphBuilder`,
        `RuleAnalysisGraphImpl`

    ------------------------------------------------------------------------

        public interface RuleAnalysisGraph

    ::: block
    Represents the stage of buck where the
    [`TargetGraph`](../../../model/targetgraph/TargetGraph.html "class in com.facebook.buck.core.model.targetgraph")
    is analyzed and converted into its corresponding
    [`RuleAnalysisResult`](../RuleAnalysisResult.html "interface in com.facebook.buck.core.rules.analysis")
    graph, which consists of a `Provider` graph and a
    [`ActionAnalysisData`](../action/ActionAnalysisData.html "interface in com.facebook.buck.core.rules.analysis.action")
    graph.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `RuleAnalysisResult`  | `get​(RuleAn           | ::: block             |
        |                       | alysisKey lookupKey)` | Finds the             |
        |                       |                       | [`RuleAnalysisResul   |
        |                       |                       | t`](../RuleAnalysisRe |
        |                       |                       | sult.html "interface  |
        |                       |                       | in com.facebook.buck. |
        |                       |                       | core.rules.analysis") |
        |                       |                       | of the given          |
        |                       |                       | [`RuleAnal            |
        |                       |                       | ysisKey`](../RuleAnal |
        |                       |                       | ysisKey.html "class i |
        |                       |                       | n com.facebook.buck.c |
        |                       |                       | ore.rules.analysis"), |
        |                       |                       | starting computation  |
        |                       |                       | as necessary.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `getAll​(Set<RuleAnal  | ::: block             |
        | ommon.collect.Immutab | ysisKey> lookupKeys)` | same as               |
        | leMap<RuleAnalysisKey |                       | [                     |
        | ,​RuleAnalysisResult>` |                       | `get(RuleAnalysisKey) |
        |                       |                       | `](#get(com.facebook. |
        |                       |                       | buck.core.rules.analy |
        |                       |                       | sis.RuleAnalysisKey)) |
        |                       |                       | but for multiple      |
        |                       |                       | [`RuleAnal            |
        |                       |                       | ysisKey`](../RuleAnal |
        |                       |                       | ysisKey.html "class i |
        |                       |                       | n com.facebook.buck.c |
        |                       |                       | ore.rules.analysis")s |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

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

        []{#get(com.facebook.buck.core.rules.analysis.RuleAnalysisKey)}

        -   #### get

            ``` methodSignature
            RuleAnalysisResult get​(RuleAnalysisKey lookupKey)
            ```

            ::: block
            Finds the
            [`RuleAnalysisResult`](../RuleAnalysisResult.html "interface in com.facebook.buck.core.rules.analysis")
            of the given
            [`RuleAnalysisKey`](../RuleAnalysisKey.html "class in com.facebook.buck.core.rules.analysis"),
            starting computation as necessary. All dependencies required
            will also be transformed, and cached.
            :::

            [Parameters:]{.paramLabel}
            :   `lookupKey` - the
                [`RuleAnalysisKey`](../RuleAnalysisKey.html "class in com.facebook.buck.core.rules.analysis")
                to find the result for

            [Returns:]{.returnLabel}
            :   the
                [`RuleAnalysisResult`](../RuleAnalysisResult.html "interface in com.facebook.buck.core.rules.analysis")
                from analyzing the given
                [`RuleAnalysisKey`](../RuleAnalysisKey.html "class in com.facebook.buck.core.rules.analysis")

        []{#getAll(java.util.Set)}

        -   #### getAll

            ``` methodSignature
            com.google.common.collect.ImmutableMap<RuleAnalysisKey,​RuleAnalysisResult> getAll​(Set<RuleAnalysisKey> lookupKeys)
            ```

            ::: block
            same as
            [`get(RuleAnalysisKey)`](#get(com.facebook.buck.core.rules.analysis.RuleAnalysisKey))
            but for multiple
            [`RuleAnalysisKey`](../RuleAnalysisKey.html "class in com.facebook.buck.core.rules.analysis")s
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
