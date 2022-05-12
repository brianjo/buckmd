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
[Package]{.packageLabelInType} [com.facebook.buck.android.toolchain.platform](package-summary.html)
:::

## Class AndroidPlatformDescription {#class-androidplatformdescription .title title="Class AndroidPlatformDescription"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.toolchain.platform.AndroidPlatformDescription

::: description
-   

    All Implemented Interfaces:
    :   `BaseDescription<AndroidPlatformArg>`,
        `ConfigurationRuleDescription<AndroidPlatformArg,​AndroidMultiPlatformRule>`

    ------------------------------------------------------------------------

        public class AndroidPlatformDescription
        extends Object
        implements ConfigurationRuleDescription<AndroidPlatformArg,​AndroidMultiPlatformRule>

    ::: block
    A description for `android_platform`.
    For example:

           android_platform(
              name = "platform",
              base_platform = "//config/platform:android",
              native_platforms = [
                  "//config/platform:cpu-x86_64",
                  "//config/platform:cpu-armv7",
              ]
           )
         
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                      Description
          -------------------------------- -------------
          `AndroidPlatformDescription()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Andr                 | `createConfiguratio   | ::: block             |
        | oidMultiPlatformRule` | nRule​(ConfigurationRu | Creates a             |
        |                       | leResolver configurat | [`ConfigurationRul    |
        |                       | ionRuleResolver,      | e`](../../../core/rul |
        |                       |                    Bu | es/config/Configurati |
        |                       | ildTarget buildTarget | onRule.html "interfac |
        |                       | ,                     | e in com.facebook.buc |
        |                       |     DependencyStack d | k.core.rules.config") |
        |                       | ependencyStack,       | :::                   |
        |                       |                   And |                       |
        |                       | roidPlatformArg arg)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `get                  |                       |
        | .common.collect.Immut | ConfigurationDeps​(And |                       |
        | ableSet<BuildTarget>` | roidPlatformArg arg)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Class                | `get                  | ::: block             |
        | <AndroidPlatformArg>` | ConstructorArgType()` | The type of the       |
        |                       |                       | constructor argument  |
        |                       |                       | that is used by this  |
        |                       |                       | description to create |
        |                       |                       | a rule                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Class<Andro          | `getRuleClass()`      | ::: block             |
        | idMultiPlatformRule>` |                       | Reified type          |
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

        -   #### AndroidPlatformDescription

                public AndroidPlatformDescription()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getConstructorArgType()}

        -   #### getConstructorArgType

            ``` methodSignature
            public Class<AndroidPlatformArg> getConstructorArgType()
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
                interface `BaseDescription<AndroidPlatformArg>`

        []{#getRuleClass()}

        -   #### getRuleClass

            ``` methodSignature
            public Class<AndroidMultiPlatformRule> getRuleClass()
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
                interface `ConfigurationRuleDescription<AndroidPlatformArg,​AndroidMultiPlatformRule>`

        []{#createConfigurationRule(com.facebook.buck.core.rules.config.ConfigurationRuleResolver,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.exceptions.DependencyStack,com.facebook.buck.android.toolchain.platform.AndroidPlatformArg)}

        -   #### createConfigurationRule

            ``` methodSignature
            public AndroidMultiPlatformRule createConfigurationRule​(ConfigurationRuleResolver configurationRuleResolver,
                                                                    BuildTarget buildTarget,
                                                                    DependencyStack dependencyStack,
                                                                    AndroidPlatformArg arg)
            ```

            ::: block
            [Description copied from
            interface: `ConfigurationRuleDescription`]{.descfrmTypeLabel}
            :::

            ::: block
            Creates a
            [`ConfigurationRule`](../../../core/rules/config/ConfigurationRule.html "interface in com.facebook.buck.core.rules.config")
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `createConfigurationRule` in
                interface `ConfigurationRuleDescription<AndroidPlatformArg,​AndroidMultiPlatformRule>`

        []{#getConfigurationDeps(com.facebook.buck.android.toolchain.platform.AndroidPlatformArg)}

        -   #### getConfigurationDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<BuildTarget> getConfigurationDeps​(AndroidPlatformArg arg)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getConfigurationDeps` in
                interface `BaseDescription<AndroidPlatformArg>`

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
