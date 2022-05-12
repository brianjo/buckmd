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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Class ConstraintBasedAndroidNativeTargetConfigurationMatcher {#class-constraintbasedandroidnativetargetconfigurationmatcher .title title="Class ConstraintBasedAndroidNativeTargetConfigurationMatcher"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.ConstraintBasedAndroidNativeTargetConfigurationMatcher

::: description
-   

    All Implemented Interfaces:
    :   `AndroidNativeTargetConfigurationMatcher`

    ------------------------------------------------------------------------

        public class ConstraintBasedAndroidNativeTargetConfigurationMatcher
        extends Object
        implements AndroidNativeTargetConfigurationMatcher

    ::: block
    Matcher that uses constraints to figure out whether platform in
    target configuration matches the CPU type.
    It keeps a mapping that provides a list of constraint values for a
    given CPU type. When a request is made, it uses the constraints for
    the given CPU and checks whether the platform of the target matches
    the constraints.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                           Description
          --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `ConstraintBasedAndroidNativeTargetConfigurationMatcher​(ConfigurationRuleRegistry configurationRuleRegistry,                                                       com.google.common.collect.ImmutableMap<TargetCpuType,​NamedPlatform> targetCpuTypeToConstraints)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type             Method                                                                                                                                   Description
          ----------------------------- ---------------------------------------------------------------------------------------------------------------------------------------- -------------
          `ConfigurationRuleRegistry`   `getConfigurationRuleRegistry()`                                                                                                          
          `boolean`                     `nativeTargetConfigurationMatchesCpuType​(BuildTarget buildTarget,                                        TargetCpuType targetCpuType)`    

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

        []{#<init>(com.facebook.buck.core.rules.config.registry.ConfigurationRuleRegistry,com.google.common.collect.ImmutableMap)}

        -   #### ConstraintBasedAndroidNativeTargetConfigurationMatcher

                public ConstraintBasedAndroidNativeTargetConfigurationMatcher​(ConfigurationRuleRegistry configurationRuleRegistry,
                                                                              com.google.common.collect.ImmutableMap<TargetCpuType,​NamedPlatform> targetCpuTypeToConstraints)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#nativeTargetConfigurationMatchesCpuType(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.android.toolchain.ndk.TargetCpuType)}

        -   #### nativeTargetConfigurationMatchesCpuType

            ``` methodSignature
            public boolean nativeTargetConfigurationMatchesCpuType​(BuildTarget buildTarget,
                                                                   TargetCpuType targetCpuType)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `nativeTargetConfigurationMatchesCpuType` in
                interface `AndroidNativeTargetConfigurationMatcher`

            [Returns:]{.returnLabel}
            :   `true` when platform in configuration of the target
                matches the given CPU type.

        []{#getConfigurationRuleRegistry()}

        -   #### getConfigurationRuleRegistry

            ``` methodSignature
            public ConfigurationRuleRegistry getConfigurationRuleRegistry()
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
