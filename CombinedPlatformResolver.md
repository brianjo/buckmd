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

## Class CombinedPlatformResolver {#class-combinedplatformresolver .title title="Class CombinedPlatformResolver"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rules.platform.CombinedPlatformResolver

::: description
-   

    All Implemented Interfaces:
    :   `PlatformResolver`

    ------------------------------------------------------------------------

        public class CombinedPlatformResolver
        extends Object
        implements PlatformResolver

    ::: block
    [`PlatformResolver`](../../model/platform/PlatformResolver.html "interface in com.facebook.buck.core.model.platform")
    that supports both multiplatforms and regular platforms.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                           Description
          ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `CombinedPlatformResolver​(ConfigurationRuleResolver configurationRuleResolver,                         RuleBasedPlatformResolver ruleBasedPlatformResolver,                         RuleBasedMultiPlatformResolver ruleBasedMultiPlatformResolver)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                               Description
          ------------------- ------------------------------------------------------------------------------------ -------------
          `Platform`          `getPlatform​(BuildTarget buildTarget,            DependencyStack dependencyStack)`    

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

        []{#<init>(com.facebook.buck.core.rules.config.ConfigurationRuleResolver,com.facebook.buck.core.rules.platform.RuleBasedPlatformResolver,com.facebook.buck.core.rules.platform.RuleBasedMultiPlatformResolver)}

        -   #### CombinedPlatformResolver

                public CombinedPlatformResolver​(ConfigurationRuleResolver configurationRuleResolver,
                                                RuleBasedPlatformResolver ruleBasedPlatformResolver,
                                                RuleBasedMultiPlatformResolver ruleBasedMultiPlatformResolver)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getPlatform(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.exceptions.DependencyStack)}

        -   #### getPlatform

            ``` methodSignature
            public Platform getPlatform​(BuildTarget buildTarget,
                                        DependencyStack dependencyStack)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPlatform` in interface `PlatformResolver`

            [Returns:]{.returnLabel}
            :   [`Platform`](../../model/platform/Platform.html "interface in com.facebook.buck.core.model.platform")
                for a given build target.
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
