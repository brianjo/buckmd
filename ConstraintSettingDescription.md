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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.platform](package-summary.html)
:::

## Class ConstraintSettingDescription {#class-constraintsettingdescription .title title="Class ConstraintSettingDescription"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rules.platform.ConstraintSettingDescription

::: description
-   

    All Implemented Interfaces:
    :   `BaseDescription<ConstraintSettingArg>`,
        `ConfigurationRuleDescription<ConstraintSettingArg,​ConstraintSettingRule>`

    ------------------------------------------------------------------------

        public class ConstraintSettingDescription
        extends Object
        implements ConfigurationRuleDescription<ConstraintSettingArg,​ConstraintSettingRule>

    ::: block
    A description for `constraint_setting`.
    Constraint setting define a type of a constraint that can be used to
    define platforms.

    For example:

           constraint_setting(
              name = "constraint"
           )
         
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                        Description
          ---------------------------------- -------------
          `ConstraintSettingDescription()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `C                    | `createConfigurationR | ::: block             |
        | onstraintSettingRule` | ule​(ConfigurationRule | Creates a             |
        |                       | Resolver configuratio | [                     |
        |                       | nRuleResolver,        | `ConfigurationRule`]( |
        |                       |                  Buil | ../config/Configurati |
        |                       | dTarget buildTarget,  | onRule.html "interfac |
        |                       |                       | e in com.facebook.buc |
        |                       |   DependencyStack dep | k.core.rules.config") |
        |                       | endencyStack,         | :::                   |
        |                       |                 Const |                       |
        |                       | raintSettingArg arg)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getCo                |                       |
        | .common.collect.Immut | nfigurationDeps​(Const |                       |
        | ableSet<BuildTarget>` | raintSettingArg arg)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Class<C              | `get                  | ::: block             |
        | onstraintSettingArg>` | ConstructorArgType()` | The type of the       |
        |                       |                       | constructor argument  |
        |                       |                       | that is used by this  |
        |                       |                       | description to create |
        |                       |                       | a rule                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Class<Co             | `getRuleClass()`      | ::: block             |
        | nstraintSettingRule>` |                       | Reified type          |
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

        -   #### ConstraintSettingDescription

                public ConstraintSettingDescription()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getConstructorArgType()}

        -   #### getConstructorArgType

            ``` methodSignature
            public Class<ConstraintSettingArg> getConstructorArgType()
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
                interface `BaseDescription<ConstraintSettingArg>`

        []{#getRuleClass()}

        -   #### getRuleClass

            ``` methodSignature
            public Class<ConstraintSettingRule> getRuleClass()
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
                interface `ConfigurationRuleDescription<ConstraintSettingArg,​ConstraintSettingRule>`

        []{#createConfigurationRule(com.facebook.buck.core.rules.config.ConfigurationRuleResolver,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.exceptions.DependencyStack,com.facebook.buck.core.rules.platform.ConstraintSettingArg)}

        -   #### createConfigurationRule

            ``` methodSignature
            public ConstraintSettingRule createConfigurationRule​(ConfigurationRuleResolver configurationRuleResolver,
                                                                 BuildTarget buildTarget,
                                                                 DependencyStack dependencyStack,
                                                                 ConstraintSettingArg arg)
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
                interface `ConfigurationRuleDescription<ConstraintSettingArg,​ConstraintSettingRule>`

        []{#getConfigurationDeps(com.facebook.buck.core.rules.platform.ConstraintSettingArg)}

        -   #### getConfigurationDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<BuildTarget> getConfigurationDeps​(ConstraintSettingArg arg)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getConfigurationDeps` in
                interface `BaseDescription<ConstraintSettingArg>`

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
