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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.configsetting](package-summary.html)
:::

## Class ConfigSettingSelectable {#class-configsettingselectable .title title="Class ConfigSettingSelectable"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rules.configsetting.ConfigSettingSelectable

::: description
-   

    All Implemented Interfaces:
    :   `Selectable`

    ------------------------------------------------------------------------

        public class ConfigSettingSelectable
        extends Object
        implements Selectable

    ::: block
    `Selectable` created by
    [`ConfigSettingRule`](ConfigSettingRule.html "class in com.facebook.buck.core.rules.configsetting")
    for integration with
    [`SelectableResolver`](../../select/SelectableResolver.html "interface in com.facebook.buck.core.select").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `ConfigSettingSelectable​(BuildTarget buildTarget,                        com.google.common.collect.ImmutableMap<String,​String> values,                        com.google.common.collect.ImmutableSet<ConstraintValue> constraintValues)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `BuildTarget`         | `getBuildTarget()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `matches​(Selectabl    |                       |
        |                       | eConfigurationContext |                       |
        |                       |  configurationContext |                       |
        |                       | ,        DependencySt |                       |
        |                       | ack dependencyStack)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `matches              |                       |
        |                       | Platform​(Platform pla |                       |
        |                       | tform,                |                       |
        |                       |  ConstraintResolver c |                       |
        |                       | onstraintResolver,    |                       |
        |                       |              Dependen |                       |
        |                       | cyStack dependencySta |                       |
        |                       | ck,                Bu |                       |
        |                       | ckConfig buckConfig)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `refin                | ::: block             |
        |                       | es​(Selectable other)` | A                     |
        |                       |                       | [`Conf                |
        |                       |                       | igSettingSelectable`] |
        |                       |                       | (ConfigSettingSelecta |
        |                       |                       | ble.html "class in co |
        |                       |                       | m.facebook.buck.core. |
        |                       |                       | rules.configsetting") |
        |                       |                       | refines another       |
        |                       |                       | [`Conf                |
        |                       |                       | igSettingSelectable`] |
        |                       |                       | (ConfigSettingSelecta |
        |                       |                       | ble.html "class in co |
        |                       |                       | m.facebook.buck.core. |
        |                       |                       | rules.configsetting") |
        |                       |                       | when                  |
        |                       |                       | [`values`](#values)   |
        |                       |                       | or                    |
        |                       |                       | [`constraintValues    |
        |                       |                       | `](#constraintValues) |
        |                       |                       | or both are strict    |
        |                       |                       | supersets of          |
        |                       |                       | corresponding sets of |
        |                       |                       | the other selectable. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.google.common.collect.ImmutableMap,com.google.common.collect.ImmutableSet)}

        -   #### ConfigSettingSelectable

                public ConfigSettingSelectable​(BuildTarget buildTarget,
                                               com.google.common.collect.ImmutableMap<String,​String> values,
                                               com.google.common.collect.ImmutableSet<ConstraintValue> constraintValues)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#matches(com.facebook.buck.core.select.SelectableConfigurationContext,com.facebook.buck.core.exceptions.DependencyStack)}

        -   #### matches

            ``` methodSignature
            public boolean matches​(SelectableConfigurationContext configurationContext,
                                   DependencyStack dependencyStack)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `matches` in interface `Selectable`

            [Returns:]{.returnLabel}
            :   `true` if this condition matches the configuration

        []{#matchesPlatform(com.facebook.buck.core.model.platform.Platform,com.facebook.buck.core.model.platform.ConstraintResolver,com.facebook.buck.core.exceptions.DependencyStack,com.facebook.buck.core.config.BuckConfig)}

        -   #### matchesPlatform

            ``` methodSignature
            public boolean matchesPlatform​(Platform platform,
                                           ConstraintResolver constraintResolver,
                                           DependencyStack dependencyStack,
                                           BuckConfig buckConfig)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `matchesPlatform` in interface `Selectable`

            [Returns:]{.returnLabel}
            :   `true` if this condition matches the platform

        []{#refines(com.facebook.buck.core.select.Selectable)}

        -   #### refines

            ``` methodSignature
            public boolean refines​(Selectable other)
            ```

            ::: block
            A
            [`ConfigSettingSelectable`](ConfigSettingSelectable.html "class in com.facebook.buck.core.rules.configsetting")
            refines another
            [`ConfigSettingSelectable`](ConfigSettingSelectable.html "class in com.facebook.buck.core.rules.configsetting")
            when [`values`](#values) or
            [`constraintValues`](#constraintValues) or both are strict
            supersets of corresponding sets of the other selectable.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `refines` in interface `Selectable`

            [Returns:]{.returnLabel}
            :   `true` for given `this` selectable and `other`
                selectable when one of this conditions is true:
                -   `this.values` is a strict superset of `other.values`
                    and `            this.constraintValues` is a strict
                    superset of `other.constraintValues`
                -   `this.values` is equal to `other.values` and
                    `            this.constraintValues` is a strict
                    superset of `other.constraintValues`
                -   `this.values` is a strict superset of `other.values`
                    and `            this.constraintValues` is equal to
                    `other.constraintValues`

        []{#getBuildTarget()}

        -   #### getBuildTarget

            ``` methodSignature
            public BuildTarget getBuildTarget()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildTarget` in interface `Selectable`

            [Returns:]{.returnLabel}
            :   build target of this condition

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`
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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
