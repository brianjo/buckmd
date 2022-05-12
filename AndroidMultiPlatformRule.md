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

## Class AndroidMultiPlatformRule {#class-androidmultiplatformrule .title title="Class AndroidMultiPlatformRule"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.config.AbstractConfigurationRule](../../../core/rules/config/AbstractConfigurationRule.html "class in com.facebook.buck.core.rules.config")

    -   -   com.facebook.buck.android.toolchain.platform.AndroidMultiPlatformRule

::: description
-   

    All Implemented Interfaces:
    :   `ConfigurationRule`, `MultiPlatformRule`

    ------------------------------------------------------------------------

        public class AndroidMultiPlatformRule
        extends AbstractConfigurationRule
        implements MultiPlatformRule

    ::: block
    Buck rule representing Android multiplatform definition
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                              Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `AndroidMultiPlatformRule​(BuildTarget buildTarget,                         BuildTarget basePlatform,                         com.google.common.collect.ImmutableSortedMap<TargetCpuType,​BuildTarget> nestedPlatforms)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                                 Description
          ------------------- ---------------------------------------------------------------------------------------------------------------------- -------------
          `Platform`          `createPlatform​(RuleBasedPlatformResolver ruleBasedPlatformResolver,               DependencyStack dependencyStack)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.config.AbstractConfigurationRule}

            ### Methods inherited from class com.facebook.buck.core.rules.config.[AbstractConfigurationRule](../../../core/rules/config/AbstractConfigurationRule.html "class in com.facebook.buck.core.rules.config")

            `getBuildTarget`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.config.ConfigurationRule}

            ### Methods inherited from interface com.facebook.buck.core.rules.config.[ConfigurationRule](../../../core/rules/config/ConfigurationRule.html "interface in com.facebook.buck.core.rules.config")

            `getBuildTarget`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.model.BuildTarget,com.google.common.collect.ImmutableSortedMap)}

        -   #### AndroidMultiPlatformRule

                public AndroidMultiPlatformRule​(BuildTarget buildTarget,
                                                BuildTarget basePlatform,
                                                com.google.common.collect.ImmutableSortedMap<TargetCpuType,​BuildTarget> nestedPlatforms)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createPlatform(com.facebook.buck.core.rules.platform.RuleBasedPlatformResolver,com.facebook.buck.core.exceptions.DependencyStack)}

        -   #### createPlatform

            ``` methodSignature
            public Platform createPlatform​(RuleBasedPlatformResolver ruleBasedPlatformResolver,
                                           DependencyStack dependencyStack)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createPlatform` in interface `MultiPlatformRule`
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
