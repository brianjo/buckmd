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
[Package]{.packageLabelInType} [com.facebook.buck.core.select](package-summary.html)
:::

## Interface Selectable {#interface-selectable .title title="Interface Selectable"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `ConfigSettingSelectable`

    ------------------------------------------------------------------------

        public interface Selectable

    ::: block
    A condition in `select` statements.
    Such condition is referenced from keys in a `select` statement by a
    [`BuildTarget`](../model/BuildTarget.html "class in com.facebook.buck.core.model")
    which should point to an instance that implements
    [`ProvidesSelectable`](ProvidesSelectable.html "interface in com.facebook.buck.core.select")
    which is used to obtain the
    [`Selectable`](Selectable.html "interface in com.facebook.buck.core.select").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                                                                                             Description
          ------------------- ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `BuildTarget`       `getBuildTarget()`                                                                                                                                                                  
          `boolean`           `matches​(SelectableConfigurationContext configurationContext,        DependencyStack dependencyStack)`                                                                              
          `boolean`           `matchesPlatform​(Platform platform,                ConstraintResolver constraintResolver,                DependencyStack dependencyStack,                BuckConfig buckConfig)`    
          `boolean`           `refines​(Selectable other)`                                                                                                                                                         

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

        []{#matches(com.facebook.buck.core.select.SelectableConfigurationContext,com.facebook.buck.core.exceptions.DependencyStack)}

        -   #### matches

            ``` methodSignature
            boolean matches​(SelectableConfigurationContext configurationContext,
                            DependencyStack dependencyStack)
            ```

            [Returns:]{.returnLabel}
            :   `true` if this condition matches the configuration

        []{#matchesPlatform(com.facebook.buck.core.model.platform.Platform,com.facebook.buck.core.model.platform.ConstraintResolver,com.facebook.buck.core.exceptions.DependencyStack,com.facebook.buck.core.config.BuckConfig)}

        -   #### matchesPlatform

            ``` methodSignature
            boolean matchesPlatform​(Platform platform,
                                    ConstraintResolver constraintResolver,
                                    DependencyStack dependencyStack,
                                    BuckConfig buckConfig)
            ```

            [Returns:]{.returnLabel}
            :   `true` if this condition matches the platform

        []{#refines(com.facebook.buck.core.select.Selectable)}

        -   #### refines

            ``` methodSignature
            boolean refines​(Selectable other)
            ```

            [Returns:]{.returnLabel}
            :   `true` if this condition is more specialized than the
                given one

        []{#getBuildTarget()}

        -   #### getBuildTarget

            ``` methodSignature
            BuildTarget getBuildTarget()
            ```

            [Returns:]{.returnLabel}
            :   build target of this condition
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
