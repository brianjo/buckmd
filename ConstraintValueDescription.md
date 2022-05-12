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

## Class ConstraintValueDescription {#class-constraintvaluedescription .title title="Class ConstraintValueDescription"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rules.platform.ConstraintValueDescription

::: description
-   

    All Implemented Interfaces:
    :   `BaseDescription<ConstraintValueArg>`,
        `ConfigurationRuleDescription<ConstraintValueArg,​ConstraintValueRule>`

    ------------------------------------------------------------------------

        public class ConstraintValueDescription
        extends Object
        implements ConfigurationRuleDescription<ConstraintValueArg,​ConstraintValueRule>

    ::: block
    A description for `constraint_value`.
    Constraint value define a constraint that can be used to define
    platforms.

    For example:

           constraint_value(
              name = "constraint_value",
              constraint_setting = ":constraint",
           )
         
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                      Description
          -------------------------------- -------------
          `ConstraintValueDescription()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `ConstraintValueRule` | `createConfiguratio   | ::: block             |
        |                       | nRule​(ConfigurationRu | Creates a             |
        |                       | leResolver configurat | [                     |
        |                       | ionRuleResolver,      | `ConfigurationRule`]( |
        |                       |                    Bu | ../config/Configurati |
        |                       | ildTarget buildTarget | onRule.html "interfac |
        |                       | ,                     | e in com.facebook.buc |
        |                       |     DependencyStack d | k.core.rules.config") |
        |                       | ependencyStack,       | :::                   |
        |                       |                   Con |                       |
        |                       | straintValueArg arg)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `get                  |                       |
        | .common.collect.Immut | ConfigurationDeps​(Con |                       |
        | ableSet<BuildTarget>` | straintValueArg arg)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Class                | `get                  | ::: block             |
        | <ConstraintValueArg>` | ConstructorArgType()` | The type of the       |
        |                       |                       | constructor argument  |
        |                       |                       | that is used by this  |
        |                       |                       | description to create |
        |                       |                       | a rule                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Class<               | `getRuleClass()`      | ::: block             |
        | ConstraintValueRule>` |                       | Reified type          |
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

        -   #### ConstraintValueDescription

                public ConstraintValueDescription()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getConstructorArgType()}

        -   #### getConstructorArgType

            ``` methodSignature
            public Class<ConstraintValueArg> getConstructorArgType()
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
                interface `BaseDescription<ConstraintValueArg>`

        []{#getRuleClass()}

        -   #### getRuleClass

            ``` methodSignature
            public Class<ConstraintValueRule> getRuleClass()
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
                interface `ConfigurationRuleDescription<ConstraintValueArg,​ConstraintValueRule>`

        []{#createConfigurationRule(com.facebook.buck.core.rules.config.ConfigurationRuleResolver,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.exceptions.DependencyStack,com.facebook.buck.core.rules.platform.ConstraintValueArg)}

        -   #### createConfigurationRule

            ``` methodSignature
            public ConstraintValueRule createConfigurationRule​(ConfigurationRuleResolver configurationRuleResolver,
                                                               BuildTarget buildTarget,
                                                               DependencyStack dependencyStack,
                                                               ConstraintValueArg arg)
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
                interface `ConfigurationRuleDescription<ConstraintValueArg,​ConstraintValueRule>`

        []{#getConfigurationDeps(com.facebook.buck.core.rules.platform.ConstraintValueArg)}

        -   #### getConfigurationDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<BuildTarget> getConfigurationDeps​(ConstraintValueArg arg)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getConfigurationDeps` in
                interface `BaseDescription<ConstraintValueArg>`

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
