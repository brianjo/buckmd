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
[Package]{.packageLabelInType} [com.facebook.buck.core.model.actiongraph.computation](package-summary.html)
:::

## Interface ActionGraphFactoryDelegate {#interface-actiongraphfactorydelegate .title title="Interface ActionGraphFactoryDelegate"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `ParallelActionGraphFactory`

    ------------------------------------------------------------------------

        public interface ActionGraphFactoryDelegate

    ::: block
    The factory in charge of creating the action graph depending on the
    construction mode.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Interface             | Description           |
        +=======================+=======================+=======================+
        | `static interface `   | `ActionGraphFa        | ::: block             |
        |                       | ctoryDelegate.ActionG | Creates the base      |
        |                       | raphBuilderDecorator` | [                     |
        |                       |                       | `ActionGraphBuilder`] |
        |                       |                       | (../../../rules/Actio |
        |                       |                       | nGraphBuilder.html "i |
        |                       |                       | nterface in com.faceb |
        |                       |                       | ook.buck.core.rules") |
        |                       |                       | with potentially a    |
        |                       |                       | decorator to be       |
        |                       |                       | compatible with the   |
        |                       |                       | new rule analysis     |
        |                       |                       | framework             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type         Method                                                                                                                                                                                                                                                                                                                                     Description
          ------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `ActionGraphAndBuilder`   `create​(TargetNodeToBuildRuleTransformer transformer,       TargetGraph targetGraph,       com.facebook.buck.core.model.actiongraph.computation.ActionGraphFactory.ActionGraphCreationLifecycleListener actionGraphCreationLifecycleListener,       ActionGraphFactoryDelegate.ActionGraphBuilderDecorator actionGraphBuilderDecorator)`    

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

        []{#create(com.facebook.buck.core.rules.transformer.TargetNodeToBuildRuleTransformer,com.facebook.buck.core.model.targetgraph.TargetGraph,com.facebook.buck.core.model.actiongraph.computation.ActionGraphFactory.ActionGraphCreationLifecycleListener,com.facebook.buck.core.model.actiongraph.computation.ActionGraphFactoryDelegate.ActionGraphBuilderDecorator)}

        -   #### create

            ``` methodSignature
            ActionGraphAndBuilder create​(TargetNodeToBuildRuleTransformer transformer,
                                         TargetGraph targetGraph,
                                         com.facebook.buck.core.model.actiongraph.computation.ActionGraphFactory.ActionGraphCreationLifecycleListener actionGraphCreationLifecycleListener,
                                         ActionGraphFactoryDelegate.ActionGraphBuilderDecorator actionGraphBuilderDecorator)
            ```
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
