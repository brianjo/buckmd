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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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

## Class ModernBuildRuleConfig {#class-modernbuildruleconfig .title title="Class ModernBuildRuleConfig"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.modern.config.ModernBuildRuleConfig

::: description
-   

    All Implemented Interfaces:
    :   `ConfigView<BuckConfig>`, `ModernBuildRuleStrategyConfig`

    ------------------------------------------------------------------------

        public abstract class ModernBuildRuleConfig
        extends Object
        implements ConfigView<BuckConfig>, ModernBuildRuleStrategyConfig

    ::: block
    Various configuration for ModernBuildRule behavior.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field       Description
          ------------------- ----------- -------------
          `static String`     `SECTION`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                 Description
          --------------------------- -------------
          `ModernBuildRuleConfig()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                  Method                                                                                                        Description
          ---------------------------------- ------------------------------------------------------------------------------------------------------------- -------------
          `ModernBuildRuleBuildStrategy`     `getBuildStrategy​(boolean remoteExecutionAutoEnabled,                 boolean forceDisableRemoteExecution)`    
          `ModernBuildRuleStrategyConfig`    `getDefaultStrategyConfig()`                                                                                   
          `HybridLocalBuildStrategyConfig`   `getHybridLocalConfig()`                                                                                       
          `static ModernBuildRuleConfig`     `of​(BuckConfig delegate)`                                                                                      

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.config.ConfigView}

            ### Methods inherited from interface com.facebook.buck.core.config.[ConfigView](../../../core/config/ConfigView.html "interface in com.facebook.buck.core.config")

            `getDelegate`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#SECTION}

        -   #### SECTION

                public static final String SECTION

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.rules.modern.config.ModernBuildRuleConfig.SECTION)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### ModernBuildRuleConfig

                public ModernBuildRuleConfig()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#of(com.facebook.buck.core.config.BuckConfig)}

        -   #### of

            ``` methodSignature
            public static ModernBuildRuleConfig of​(BuckConfig delegate)
            ```

        []{#getDefaultStrategyConfig()}

        -   #### getDefaultStrategyConfig

            ``` methodSignature
            @Derived
            public ModernBuildRuleStrategyConfig getDefaultStrategyConfig()
            ```

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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
