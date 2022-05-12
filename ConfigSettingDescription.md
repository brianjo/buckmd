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

## Class ConfigSettingDescription {#class-configsettingdescription .title title="Class ConfigSettingDescription"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rules.configsetting.ConfigSettingDescription

::: description
-   

    All Implemented Interfaces:
    :   `BaseDescription<ConfigSettingArg>`,
        `ConfigurationRuleDescription<ConfigSettingArg,​ConfigSettingRule>`

    ------------------------------------------------------------------------

        public class ConfigSettingDescription
        extends Object
        implements ConfigurationRuleDescription<ConfigSettingArg,​ConfigSettingRule>

    ::: block
    A description for `config_setting`.
    This rule should be used to create conditions for `select`
    statements.

    The `values` parameter is used to list configuration keys
    (configuration options from `.buckconfig` in the form
    `section.option`) with expected values.

    For example:

           config_setting(
              name = "a",
              values = {
                "section.option": "expected_value",
              }
           )
         
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                    Description
          ------------------------------ -------------
          `ConfigSettingDescription()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `ConfigSettingRule`   | `createConfigurat     | ::: block             |
        |                       | ionRule​(Configuration | Creates a             |
        |                       | RuleResolver configur | [                     |
        |                       | ationRuleResolver,    | `ConfigurationRule`]( |
        |                       |                       | ../config/Configurati |
        |                       | BuildTarget buildTarg | onRule.html "interfac |
        |                       | et,                   | e in com.facebook.buc |
        |                       |       DependencyStack | k.core.rules.config") |
        |                       |  dependencyStack,     | :::                   |
        |                       |                     C |                       |
        |                       | onfigSettingArg arg)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `g                    |                       |
        | .common.collect.Immut | etConfigurationDeps​(C |                       |
        | ableSet<BuildTarget>` | onfigSettingArg arg)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Cla                  | `get                  | ::: block             |
        | ss<ConfigSettingArg>` | ConstructorArgType()` | The type of the       |
        |                       |                       | constructor argument  |
        |                       |                       | that is used by this  |
        |                       |                       | description to create |
        |                       |                       | a rule                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Clas                 | `getRuleClass()`      | ::: block             |
        | s<ConfigSettingRule>` |                       | Reified type          |
        |                       |                       | parameter             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### ConfigSettingDescription

                public ConfigSettingDescription()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getConstructorArgType()}

        -   #### getConstructorArgType

            ``` methodSignature
            public Class<ConfigSettingArg> getConstructorArgType()
            ```

            ::: block
            [Description copied from
            interface: `BaseDescription`]{.descfrmTypeLabel}
            :::

            ::: block
            The type of the constructor argument that is used by this
            description to create a rule
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getConstructorArgType` in
                interface `BaseDescription<ConfigSettingArg>`

        []{#getRuleClass()}

        -   #### getRuleClass

            ``` methodSignature
            public Class<ConfigSettingRule> getRuleClass()
            ```

            ::: block
            [Description copied from
            interface: `ConfigurationRuleDescription`]{.descfrmTypeLabel}
            :::

            ::: block
            Reified type parameter
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRuleClass` in
                interface `ConfigurationRuleDescription<ConfigSettingArg,​ConfigSettingRule>`

        []{#createConfigurationRule(com.facebook.buck.core.rules.config.ConfigurationRuleResolver,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.exceptions.DependencyStack,com.facebook.buck.core.rules.configsetting.ConfigSettingArg)}

        -   #### createConfigurationRule

            ``` methodSignature
            public ConfigSettingRule createConfigurationRule​(ConfigurationRuleResolver configurationRuleResolver,
                                                             BuildTarget buildTarget,
                                                             DependencyStack dependencyStack,
                                                             ConfigSettingArg arg)
            ```

            ::: block
            [Description copied from
            interface: `ConfigurationRuleDescription`]{.descfrmTypeLabel}
            :::

            ::: block
            Creates a
            [`ConfigurationRule`](../config/ConfigurationRule.html "interface in com.facebook.buck.core.rules.config")
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `createConfigurationRule` in
                interface `ConfigurationRuleDescription<ConfigSettingArg,​ConfigSettingRule>`

        []{#getConfigurationDeps(com.facebook.buck.core.rules.configsetting.ConfigSettingArg)}

        -   #### getConfigurationDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<BuildTarget> getConfigurationDeps​(ConfigSettingArg arg)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getConfigurationDeps` in
                interface `BaseDescription<ConfigSettingArg>`

            [Returns:]{.returnLabel}
            :   a set of configuration targets declared in a given
                constructor argument.
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
