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
-   [Field](#field.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.features.python.toolchain.impl](package-summary.html)
:::

## Class DefaultPexToolProvider {#class-defaultpextoolprovider .title title="Class DefaultPexToolProvider"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.python.toolchain.impl.DefaultPexToolProvider

::: description
-   

    All Implemented Interfaces:
    :   `Toolchain`, `PexToolProvider`

    ------------------------------------------------------------------------

        public class DefaultPexToolProvider
        extends Object
        implements PexToolProvider
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.features.python.toolchain.PexToolProvider}

            ### Fields inherited from interface com.facebook.buck.features.python.toolchain.[PexToolProvider](../PexToolProvider.html "interface in com.facebook.buck.features.python.toolchain")

            `DEFAULT_NAME`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                               Description
          ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `DefaultPexToolProvider​(ToolchainProvider toolchainProvider,                       PythonBuckConfig pythonBuckConfig,                       RuleKeyConfiguration ruleKeyConfiguration)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                        Description
          ------------------- --------------------------------------------------------------------------------------------- -------------
          `Tool`              `getPexTool​(BuildRuleResolver resolver,           TargetConfiguration targetConfiguration)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.features.python.toolchain.PexToolProvider}

            ### Methods inherited from interface com.facebook.buck.features.python.toolchain.[PexToolProvider](../PexToolProvider.html "interface in com.facebook.buck.features.python.toolchain")

            `getName`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.toolchain.ToolchainProvider,com.facebook.buck.features.python.PythonBuckConfig,com.facebook.buck.rules.keys.config.RuleKeyConfiguration)}

        -   #### DefaultPexToolProvider

                public DefaultPexToolProvider​(ToolchainProvider toolchainProvider,
                                              PythonBuckConfig pythonBuckConfig,
                                              RuleKeyConfiguration ruleKeyConfiguration)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getPexTool(com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getPexTool

            ``` methodSignature
            public Tool getPexTool​(BuildRuleResolver resolver,
                                   TargetConfiguration targetConfiguration)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPexTool` in interface `PexToolProvider`
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
-   [Field](#field.summary) \| 
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
