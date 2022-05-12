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
[Package]{.packageLabelInType} [com.facebook.buck.core.toolchain.impl](package-summary.html)
:::

## Class DefaultToolchainProviderFactory {#class-defaulttoolchainproviderfactory .title title="Class DefaultToolchainProviderFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.toolchain.impl.DefaultToolchainProviderFactory

::: description
-   

    All Implemented Interfaces:
    :   `ToolchainProviderFactory`

    ------------------------------------------------------------------------

        public class DefaultToolchainProviderFactory
        extends Object
        implements ToolchainProviderFactory
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                   Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `DefaultToolchainProviderFactory​(org.pf4j.PluginManager pluginManager,                                com.google.common.collect.ImmutableMap<String,​String> environment,                                ProcessExecutor processExecutor,                                ExecutableFinder executableFinder)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type     Method                                                                                                                        Description
          --------------------- ----------------------------------------------------------------------------------------------------------------------------- -------------
          `ToolchainProvider`   `create​(BuckConfig buckConfig,       ProjectFilesystem projectFilesystem,       RuleKeyConfiguration ruleKeyConfiguration)`    

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

        []{#<init>(org.pf4j.PluginManager,com.google.common.collect.ImmutableMap,com.facebook.buck.util.ProcessExecutor,com.facebook.buck.io.ExecutableFinder)}

        -   #### DefaultToolchainProviderFactory

                public DefaultToolchainProviderFactory​(org.pf4j.PluginManager pluginManager,
                                                       com.google.common.collect.ImmutableMap<String,​String> environment,
                                                       ProcessExecutor processExecutor,
                                                       ExecutableFinder executableFinder)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#create(com.facebook.buck.core.config.BuckConfig,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.rules.keys.config.RuleKeyConfiguration)}

        -   #### create

            ``` methodSignature
            public ToolchainProvider create​(BuckConfig buckConfig,
                                            ProjectFilesystem projectFilesystem,
                                            RuleKeyConfiguration ruleKeyConfiguration)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `create` in interface `ToolchainProviderFactory`
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
