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
[Package]{.packageLabelInType} [com.facebook.buck.rules.modern.config](package-summary.html)
:::

## Class ModernBuildRuleStrategyConfigFromSection {#class-modernbuildrulestrategyconfigfromsection .title title="Class ModernBuildRuleStrategyConfigFromSection"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.modern.config.ModernBuildRuleStrategyConfigFromSection

::: description
-   

    All Implemented Interfaces:
    :   `ModernBuildRuleStrategyConfig`

    ------------------------------------------------------------------------

        public class ModernBuildRuleStrategyConfigFromSection
        extends Object
        implements ModernBuildRuleStrategyConfig

    ::: block
    Parses the values of a buckconfig section into a
    [`ModernBuildRuleStrategyConfig`](ModernBuildRuleStrategyConfig.html "interface in com.facebook.buck.rules.modern.config").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                               Description
          ------------------------------------------------------------------------------------------------------------------------- -------------
          `ModernBuildRuleStrategyConfigFromSection​(BuckConfig delegate,                                         String section)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                  Method                                                                                                        Description
          ---------------------------------- ------------------------------------------------------------------------------------------------------------- -------------
          `ModernBuildRuleBuildStrategy`     `getBuildStrategy​(boolean remoteExecutionAutoEnabled,                 boolean forceDisableRemoteExecution)`    
          `ModernBuildRuleStrategyConfig`    `getFlavoredStrategyConfig​(String flavor)`                                                                     
          `HybridLocalBuildStrategyConfig`   `getHybridLocalConfig()`                                                                                       

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

        []{#<init>(com.facebook.buck.core.config.BuckConfig,java.lang.String)}

        -   #### ModernBuildRuleStrategyConfigFromSection

                public ModernBuildRuleStrategyConfigFromSection​(BuckConfig delegate,
                                                                String section)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildStrategy(boolean,boolean)}

        -   #### getBuildStrategy

            ``` methodSignature
            public ModernBuildRuleBuildStrategy getBuildStrategy​(boolean remoteExecutionAutoEnabled,
                                                                 boolean forceDisableRemoteExecution)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildStrategy` in
                interface `ModernBuildRuleStrategyConfig`

        []{#getHybridLocalConfig()}

        -   #### getHybridLocalConfig

            ``` methodSignature
            public HybridLocalBuildStrategyConfig getHybridLocalConfig()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getHybridLocalConfig` in
                interface `ModernBuildRuleStrategyConfig`

        []{#getFlavoredStrategyConfig(java.lang.String)}

        -   #### getFlavoredStrategyConfig

            ``` methodSignature
            public ModernBuildRuleStrategyConfig getFlavoredStrategyConfig​(String flavor)
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
