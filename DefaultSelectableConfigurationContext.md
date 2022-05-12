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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.parser](package-summary.html)
:::

## Class DefaultSelectableConfigurationContext {#class-defaultselectableconfigurationcontext .title title="Class DefaultSelectableConfigurationContext"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.parser.DefaultSelectableConfigurationContext

::: description
-   

    All Implemented Interfaces:
    :   `ConfigSettingSelectableConfigurationContext`,
        `SelectableConfigurationContext`

    ------------------------------------------------------------------------

        public abstract class DefaultSelectableConfigurationContext
        extends Object
        implements ConfigSettingSelectableConfigurationContext

    ::: block
    An implementation of
    [`SelectableConfigurationContext`](../core/select/SelectableConfigurationContext.html "interface in com.facebook.buck.core.select")
    that is used in parser implementation.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                 Description
          ------------------------------------------- -------------
          `DefaultSelectableConfigurationContext()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                Method                                                                                                              Description
          ------------------------------------------------ ------------------------------------------------------------------------------------------------------------------- -------------
          `abstract BuckConfig`                            `getBuckConfig()`                                                                                                    
          `abstract TargetPlatformResolver`                `getPlatformProvider()`                                                                                              
          `abstract TargetConfiguration`                   `getTargetConfiguration()`                                                                                           
          `static DefaultSelectableConfigurationContext`   `of​(BuckConfig buckConfig,   TargetConfiguration targetConfiguration,   TargetPlatformResolver platformProvider)`    
          `SelectableConfigurationContext`                 `withTargetConfiguration​(TargetConfiguration value)`                                                                 

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

        -   #### DefaultSelectableConfigurationContext

                public DefaultSelectableConfigurationContext()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuckConfig()}

        -   #### getBuckConfig

            ``` methodSignature
            public abstract BuckConfig getBuckConfig()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuckConfig` in
                interface `ConfigSettingSelectableConfigurationContext`

        []{#getTargetConfiguration()}

        -   #### getTargetConfiguration

            ``` methodSignature
            public abstract TargetConfiguration getTargetConfiguration()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTargetConfiguration` in
                interface `ConfigSettingSelectableConfigurationContext`

        []{#getPlatformProvider()}

        -   #### getPlatformProvider

            ``` methodSignature
            public abstract TargetPlatformResolver getPlatformProvider()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPlatformProvider` in
                interface `ConfigSettingSelectableConfigurationContext`

        []{#withTargetConfiguration(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### withTargetConfiguration

            ``` methodSignature
            public SelectableConfigurationContext withTargetConfiguration​(TargetConfiguration value)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `withTargetConfiguration` in
                interface `SelectableConfigurationContext`

        []{#of(com.facebook.buck.core.config.BuckConfig,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.model.platform.TargetPlatformResolver)}

        -   #### of

            ``` methodSignature
            public static DefaultSelectableConfigurationContext of​(BuckConfig buckConfig,
                                                                   TargetConfiguration targetConfiguration,
                                                                   TargetPlatformResolver platformProvider)
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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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