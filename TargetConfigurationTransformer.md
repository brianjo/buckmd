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
[Package]{.packageLabelInType} [com.facebook.buck.core.model](package-summary.html)
:::

## Interface TargetConfigurationTransformer {#interface-targetconfigurationtransformer .title title="Interface TargetConfigurationTransformer"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `MultiPlatformTargetConfigurationTransformer`,
        `ThrowingTargetConfigurationTransformer`

    ------------------------------------------------------------------------

        public interface TargetConfigurationTransformer

    ::: block
    Interface that allows transforming target configurations.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `needsTra             |                       |
        |                       | nsformation​(TargetCon |                       |
        |                       | figuration targetConf |                       |
        |                       | iguration,            |                       |
        |                       |          DependencySt |                       |
        |                       | ack dependencyStack)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.c  | `transform            | ::: block             |
        | ollect.ImmutableList< | ​(TargetConfiguration  | Transforms a single   |
        | TargetConfiguration>` | targetConfiguration,  | target configurations |
        |                       |          DependencySt | into multiple target  |
        |                       | ack dependencyStack)` | configurations.       |
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

        []{#transform(com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.exceptions.DependencyStack)}

        -   #### transform

            ``` methodSignature
            com.google.common.collect.ImmutableList<TargetConfiguration> transform​(TargetConfiguration targetConfiguration,
                                                                                   DependencyStack dependencyStack)
            ```

            ::: block
            Transforms a single target configurations into multiple
            target configurations.
            :::

        []{#needsTransformation(com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.exceptions.DependencyStack)}

        -   #### needsTransformation

            ``` methodSignature
            boolean needsTransformation​(TargetConfiguration targetConfiguration,
                                        DependencyStack dependencyStack)
            ```

            [Returns:]{.returnLabel}
            :   `true` is the given target configuration can be
                transformed into other configurations.
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
