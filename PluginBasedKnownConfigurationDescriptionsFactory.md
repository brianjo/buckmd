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

## Class PluginBasedKnownConfigurationDescriptionsFactory {#class-pluginbasedknownconfigurationdescriptionsfactory .title title="Class PluginBasedKnownConfigurationDescriptionsFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rules.config.impl.PluginBasedKnownConfigurationDescriptionsFactory

::: description
-   

    ------------------------------------------------------------------------

        public class PluginBasedKnownConfigurationDescriptionsFactory
        extends Object

    ::: block
    This factory creates a list of
    [`ConfigurationRuleDescription`](../ConfigurationRuleDescription.html "interface in com.facebook.buck.core.rules.config")
    by loading instances of
    [`ConfigurationRuleDescriptionProvider`](../ConfigurationRuleDescriptionProvider.html "interface in com.facebook.buck.core.rules.config")
    using plugin framework and collecting
    [`ConfigurationRuleDescription`](../ConfigurationRuleDescription.html "interface in com.facebook.buck.core.rules.config")
    from the loaded providers.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                            Description
          ------------------------------------------------------ -------------
          `PluginBasedKnownConfigurationDescriptionsFactory()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static com.google.c  | `createFromPlug       | ::: block             |
        | ommon.collect.Immutab | ins​(org.pf4j.PluginMa | Create rule           |
        | leList<ConfigurationR | nager pluginManager)` | descriptors using     |
        | uleDescription<?,​?>>` |                       | provided plugin       |
        |                       |                       | manager               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
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

        -   #### PluginBasedKnownConfigurationDescriptionsFactory

                public PluginBasedKnownConfigurationDescriptionsFactory()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createFromPlugins(org.pf4j.PluginManager)}

        -   #### createFromPlugins

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<ConfigurationRuleDescription<?,​?>> createFromPlugins​(org.pf4j.PluginManager pluginManager)
            ```

            ::: block
            Create rule descriptors using provided plugin manager
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
