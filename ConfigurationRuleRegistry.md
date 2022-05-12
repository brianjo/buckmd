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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.config.registry](package-summary.html)
:::

## Interface ConfigurationRuleRegistry {#interface-configurationruleregistry .title title="Interface ConfigurationRuleRegistry"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface ConfigurationRuleRegistry

    ::: block
    Provides centralized access to various configuration rules.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Confi                | `getConfigu           | ::: block             |
        | gurationRuleResolver` | rationRuleResolver()` | Provides generic      |
        |                       |                       | access to             |
        |                       |                       | configuration rules.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ConstraintResolver`  | `get                  | ::: block             |
        |                       | ConstraintResolver()` | Allows to get access  |
        |                       |                       | to configuration      |
        |                       |                       | rules that represent  |
        |                       |                       | `constraint_setting`  |
        |                       |                       | and                   |
        |                       |                       | `constraint_value`    |
        |                       |                       | rules.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Ta                   | `getTarg              | ::: block             |
        | rgetPlatformResolver` | etPlatformResolver()` | Resolves target       |
        |                       |                       | configuration to a    |
        |                       |                       | platform.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Confi         | `of​(ConfigurationRule |                       |
        | gurationRuleRegistry` | Resolver configuratio |                       |
        |                       | nRuleResolver,   Cons |                       |
        |                       | traintResolver constr |                       |
        |                       | aintResolver,   Targe |                       |
        |                       | tPlatformResolver tar |                       |
        |                       | getPlatformResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getConfigurationRuleResolver()}

        -   #### getConfigurationRuleResolver

            ``` methodSignature
            ConfigurationRuleResolver getConfigurationRuleResolver()
            ```

            ::: block
            Provides generic access to configuration rules.
            :::

        []{#getConstraintResolver()}

        -   #### getConstraintResolver

            ``` methodSignature
            ConstraintResolver getConstraintResolver()
            ```

            ::: block
            Allows to get access to configuration rules that represent
            `constraint_setting` and `constraint_value` rules.
            :::

        []{#getTargetPlatformResolver()}

        -   #### getTargetPlatformResolver

            ``` methodSignature
            TargetPlatformResolver getTargetPlatformResolver()
            ```

            ::: block
            Resolves target configuration to a platform.
            :::

        []{#of(com.facebook.buck.core.rules.config.ConfigurationRuleResolver,com.facebook.buck.core.model.platform.ConstraintResolver,com.facebook.buck.core.model.platform.TargetPlatformResolver)}

        -   #### of

            ``` methodSignature
            static ConfigurationRuleRegistry of​(ConfigurationRuleResolver configurationRuleResolver,
                                                ConstraintResolver constraintResolver,
                                                TargetPlatformResolver targetPlatformResolver)
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
