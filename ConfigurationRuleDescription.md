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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.config](package-summary.html)
:::

## Interface ConfigurationRuleDescription\<T extends [ConfigurationRuleArg](ConfigurationRuleArg.html "interface in com.facebook.buck.core.rules.config"),​R extends [ConfigurationRule](ConfigurationRule.html "interface in com.facebook.buck.core.rules.config")\> {#interface-configurationruledescriptiont-extends-configurationruleargr-extends-configurationrule .title title="Interface ConfigurationRuleDescription"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `BaseDescription<T>`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AndroidPlatformDescription`, `ConfigSettingDescription`,
        `ConstraintSettingDescription`, `ConstraintValueDescription`,
        `PlatformDescription`

    ------------------------------------------------------------------------

        public interface ConfigurationRuleDescription<T extends ConfigurationRuleArg,​R extends ConfigurationRule>
        extends BaseDescription<T>

    ::: block
    This class describe a configuration rule - a rule that can be used
    during configuration of a target graph.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `R`                   | `c                    | ::: block             |
        |                       | reateConfigurationRul | Creates a             |
        |                       | e​(ConfigurationRuleRe | [`Configurat          |
        |                       | solver configurationR | ionRule`](Configurati |
        |                       | uleResolver,          | onRule.html "interfac |
        |                       |                BuildT | e in com.facebook.buc |
        |                       | arget buildTarget,    | k.core.rules.config") |
        |                       |                       | :::                   |
        |                       | DependencyStack depen |                       |
        |                       | dencyStack,           |                       |
        |                       |               T arg)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Class<R>`            | `getRuleClass()`      | ::: block             |
        |                       |                       | Reified type          |
        |                       |                       | parameter             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.BaseDescription}

            ### Methods inherited from interface com.facebook.buck.core.description.[BaseDescription](../../description/BaseDescription.html "interface in com.facebook.buck.core.description")

            `getConfigurationDeps, getConstructorArgType`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getRuleClass()}

        -   #### getRuleClass

            ``` methodSignature
            Class<R> getRuleClass()
            ```

            ::: block
            Reified type parameter
            :::

        []{#createConfigurationRule(com.facebook.buck.core.rules.config.ConfigurationRuleResolver,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.exceptions.DependencyStack,com.facebook.buck.core.rules.config.ConfigurationRuleArg)}
        []{#createConfigurationRule(com.facebook.buck.core.rules.config.ConfigurationRuleResolver,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.exceptions.DependencyStack,T)}

        -   #### createConfigurationRule

            ``` methodSignature
            R createConfigurationRule​(ConfigurationRuleResolver configurationRuleResolver,
                                      BuildTarget buildTarget,
                                      DependencyStack dependencyStack,
                                      T arg)
            ```

            ::: block
            Creates a
            [`ConfigurationRule`](ConfigurationRule.html "interface in com.facebook.buck.core.rules.config")
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
