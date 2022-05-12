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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.config.impl](package-summary.html)
:::

## Class SameThreadConfigurationRuleResolver {#class-samethreadconfigurationruleresolver .title title="Class SameThreadConfigurationRuleResolver"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rules.config.impl.SameThreadConfigurationRuleResolver

::: description
-   

    All Implemented Interfaces:
    :   `ConfigurationRuleResolver`

    ------------------------------------------------------------------------

        public class SameThreadConfigurationRuleResolver
        extends Object
        implements ConfigurationRuleResolver

    ::: block
    Provides a mechanism for mapping between a
    [`UnconfiguredBuildTarget`](../../../model/UnconfiguredBuildTarget.html "class in com.facebook.buck.core.model")
    and the
    [`ConfigurationRule`](../ConfigurationRule.html "interface in com.facebook.buck.core.rules.config")
    it represents.
    This resolver performs all computations on the same thread
    [`ConfigurationRuleResolver.getRule(com.facebook.buck.core.model.BuildTarget, java.lang.Class<R>, com.facebook.buck.core.exceptions.DependencyStack)`](../ConfigurationRuleResolver.html#getRule(com.facebook.buck.core.model.BuildTarget,java.lang.Class,com.facebook.buck.core.exceptions.DependencyStack))
    was called from.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                          Description
          ------------------------------------------------------------------------------------------------------------------------------------ -------------
          `SameThreadConfigurationRuleResolver​(java.util.function.BiFunction<BuildTarget,​DependencyStack,​TargetNode<?>> targetNodeSupplier)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `<R extends           | `getRule​(BuildTar     | ::: block             |
        |  ConfigurationRule>R` | get buildTarget,      | Returns the           |
        |                       |    Class<R> ruleClass | [`Configuration       |
        |                       | ,        DependencySt | Rule`](../Configurati |
        |                       | ack dependencyStack)` | onRule.html "interfac |
        |                       |                       | e in com.facebook.buc |
        |                       |                       | k.core.rules.config") |
        |                       |                       | associated with the   |
        |                       |                       | given                 |
        |                       |                       | [`Bui                 |
        |                       |                       | ldTarget`](../../../m |
        |                       |                       | odel/BuildTarget.html |
        |                       |                       |  "class in com.facebo |
        |                       |                       | ok.buck.core.model"). |
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

        []{#<init>(java.util.function.BiFunction)}

        -   #### SameThreadConfigurationRuleResolver

                public SameThreadConfigurationRuleResolver​(java.util.function.BiFunction<BuildTarget,​DependencyStack,​TargetNode<?>> targetNodeSupplier)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getRule(com.facebook.buck.core.model.BuildTarget,java.lang.Class,com.facebook.buck.core.exceptions.DependencyStack)}

        -   #### getRule

            ``` methodSignature
            public <R extends ConfigurationRule> R getRule​(BuildTarget buildTarget,
                                                           Class<R> ruleClass,
                                                           DependencyStack dependencyStack)
            ```

            ::: block
            [Description copied from
            interface: `ConfigurationRuleResolver`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the
            [`ConfigurationRule`](../ConfigurationRule.html "interface in com.facebook.buck.core.rules.config")
            associated with the given
            [`BuildTarget`](../../../model/BuildTarget.html "class in com.facebook.buck.core.model").
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRule` in interface `ConfigurationRuleResolver`
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
