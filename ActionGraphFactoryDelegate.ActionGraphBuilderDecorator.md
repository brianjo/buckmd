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
[Package]{.packageLabelInType} [com.facebook.buck.core.model.actiongraph.computation](package-summary.html)
:::

## Interface ActionGraphFactoryDelegate.ActionGraphBuilderDecorator {#interface-actiongraphfactorydelegate.actiongraphbuilderdecorator .title title="Interface ActionGraphFactoryDelegate.ActionGraphBuilderDecorator"}
:::

::: contentContainer
::: description
-   

    Enclosing interface:
    :   [ActionGraphFactoryDelegate](ActionGraphFactoryDelegate.html "interface in com.facebook.buck.core.model.actiongraph.computation")

    ```{=html}
    <!-- -->
    ```

    Functional Interface:
    :   This is a functional interface and can therefore be used as the
        assignment target for a lambda expression or method reference.

    ------------------------------------------------------------------------

        @FunctionalInterface
        public static interface ActionGraphFactoryDelegate.ActionGraphBuilderDecorator

    ::: block
    Creates the base
    [`ActionGraphBuilder`](../../../rules/ActionGraphBuilder.html "interface in com.facebook.buck.core.rules")
    with potentially a decorator to be compatible with the new rule
    analysis framework
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type      Method                                                                                                                     Description
          ---------------------- -------------------------------------------------------------------------------------------------------------------------- -------------
          `ActionGraphBuilder`   `create​(java.util.function.Function<TargetNodeToBuildRuleTransformer,​ActionGraphBuilder> actionGraphBuilderConstructor)`    

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

        []{#create(java.util.function.Function)}

        -   #### create

            ``` methodSignature
            ActionGraphBuilder create​(java.util.function.Function<TargetNodeToBuildRuleTransformer,​ActionGraphBuilder> actionGraphBuilderConstructor)
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
