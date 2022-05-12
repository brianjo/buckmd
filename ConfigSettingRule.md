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

## Class ConfigSettingRule {#class-configsettingrule .title title="Class ConfigSettingRule"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.config.AbstractConfigurationRule](../config/AbstractConfigurationRule.html "class in com.facebook.buck.core.rules.config")

    -   -   com.facebook.buck.core.rules.configsetting.ConfigSettingRule

::: description
-   

    All Implemented Interfaces:
    :   `ConfigurationRule`, `ProvidesSelectable`

    ------------------------------------------------------------------------

        public class ConfigSettingRule
        extends AbstractConfigurationRule
        implements ProvidesSelectable

    ::: block
    `config_setting` rule.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                      Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `ConfigSettingRule​(BuildTarget buildTarget,                  com.google.common.collect.ImmutableMap<String,​String> values,                  com.google.common.collect.ImmutableSet<ConstraintValueRule> constraintValueRules)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Selectable`          | `getSelectable()`     | ::: block             |
        |                       |                       | Returns a             |
        |                       |                       | [`Sel                 |
        |                       |                       | ectable`](../../selec |
        |                       |                       | t/Selectable.html "in |
        |                       |                       | terface in com.facebo |
        |                       |                       | ok.buck.core.select") |
        |                       |                       | that can be used      |
        |                       |                       | during evaluation of  |
        |                       |                       | conditions in a       |
        |                       |                       | `select  ` statement. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.config.AbstractConfigurationRule}

            ### Methods inherited from class com.facebook.buck.core.rules.config.[AbstractConfigurationRule](../config/AbstractConfigurationRule.html "class in com.facebook.buck.core.rules.config")

            `getBuildTarget`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.google.common.collect.ImmutableMap,com.google.common.collect.ImmutableSet)}

        -   #### ConfigSettingRule

                public ConfigSettingRule​(BuildTarget buildTarget,
                                         com.google.common.collect.ImmutableMap<String,​String> values,
                                         com.google.common.collect.ImmutableSet<ConstraintValueRule> constraintValueRules)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getSelectable()}

        -   #### getSelectable

            ``` methodSignature
            public Selectable getSelectable()
            ```

            ::: block
            [Description copied from
            interface: `ProvidesSelectable`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns a
            [`Selectable`](../../select/Selectable.html "interface in com.facebook.buck.core.select")
            that can be used during evaluation of conditions in a
            `select  ` statement.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSelectable` in interface `ProvidesSelectable`
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
