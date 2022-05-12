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

## Class PlatformDescription {#class-platformdescription .title title="Class PlatformDescription"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rules.platform.PlatformDescription

::: description
-   

    All Implemented Interfaces:
    :   `BaseDescription<PlatformArg>`,
        `ConfigurationRuleDescription<PlatformArg,​com.facebook.buck.core.rules.platform.PlatformDescription.PlatformRule>`

    ------------------------------------------------------------------------

        public class PlatformDescription
        extends Object
        implements ConfigurationRuleDescription<PlatformArg,​com.facebook.buck.core.rules.platform.PlatformDescription.PlatformRule>

    ::: block
    A description for `platform`.
    A platform is a set of constraints.

    For example:

           platform(
              name = "platform",
              constraint_values = [
                  ":constraint1",
                  ":constraint2",
              ]
           )
         
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor               Description
          ------------------------- -------------
          `PlatformDescription()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.face             | `createConfi          | ::: block             |
        | book.buck.core.rules. | gurationRule​(Configur | Creates a             |
        | platform.PlatformDesc | ationRuleResolver con | [                     |
        | ription.PlatformRule` | figurationRuleResolve | `ConfigurationRule`]( |
        |                       | r,                    | ../config/Configurati |
        |                       |      BuildTarget buil | onRule.html "interfac |
        |                       | dTarget,              | e in com.facebook.buc |
        |                       |            Dependency | k.core.rules.config") |
        |                       | Stack dependencyStack | :::                   |
        |                       | ,                     |                       |
        |                       |     PlatformArg arg)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getConfigurationD    |                       |
        | .common.collect.Immut | eps​(PlatformArg arg)` |                       |
        | ableSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Class<PlatformArg>`  | `get                  | ::: block             |
        |                       | ConstructorArgType()` | The type of the       |
        |                       |                       | constructor argument  |
        |                       |                       | that is used by this  |
        |                       |                       | description to create |
        |                       |                       | a rule                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Class<com.faceb      | `getRuleClass()`      | ::: block             |
        | ook.buck.core.rules.p |                       | Reified type          |
        | latform.PlatformDescr |                       | parameter             |
        | iption.PlatformRule>` |                       | :::                   |
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

        -   #### PlatformDescription

                public PlatformDescription()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getConstructorArgType()}

        -   #### getConstructorArgType

            ``` methodSignature
            public Class<PlatformArg> getConstructorArgType()
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
                interface `BaseDescription<PlatformArg>`

        []{#getRuleClass()}

        -   #### getRuleClass

            ``` methodSignature
            public Class<com.facebook.buck.core.rules.platform.PlatformDescription.PlatformRule> getRuleClass()
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
                interface `ConfigurationRuleDescription<PlatformArg,​com.facebook.buck.core.rules.platform.PlatformDescription.PlatformRule>`

        []{#createConfigurationRule(com.facebook.buck.core.rules.config.ConfigurationRuleResolver,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.exceptions.DependencyStack,com.facebook.buck.core.rules.platform.PlatformArg)}

        -   #### createConfigurationRule

            ``` methodSignature
            public com.facebook.buck.core.rules.platform.PlatformDescription.PlatformRule createConfigurationRule​(ConfigurationRuleResolver configurationRuleResolver,
                                                                                                                  BuildTarget buildTarget,
                                                                                                                  DependencyStack dependencyStack,
                                                                                                                  PlatformArg arg)
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
                interface `ConfigurationRuleDescription<PlatformArg,​com.facebook.buck.core.rules.platform.PlatformDescription.PlatformRule>`

        []{#getConfigurationDeps(com.facebook.buck.core.rules.platform.PlatformArg)}

        -   #### getConfigurationDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<BuildTarget> getConfigurationDeps​(PlatformArg arg)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getConfigurationDeps` in
                interface `BaseDescription<PlatformArg>`

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
