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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.description](package-summary.html)
:::

## Interface DescriptionCreationContext {#interface-descriptioncreationcontext .title title="Interface DescriptionCreationContext"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface DescriptionCreationContext

    ::: block
    Contains objects that can be used during the creation of
    descriptions.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                     Method                                                                                                                                                            Description
          ------------------------------------- ----------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `BuckConfig`                          `getBuckConfig()`                                                                                                                                                  
          `org.pf4j.PluginManager`              `getPluginManager()`                                                                                                                                               
          `SandboxExecutionStrategy`            `getSandboxExecutionStrategy()`                                                                                                                                    
          `ToolchainProvider`                   `getToolchainProvider()`                                                                                                                                           
          `static DescriptionCreationContext`   `of​(BuckConfig buckConfig,   ToolchainProvider toolchainProvider,   SandboxExecutionStrategy sandboxExecutionStrategy,   org.pf4j.PluginManager pluginManager)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuckConfig()}

        -   #### getBuckConfig

            ``` methodSignature
            BuckConfig getBuckConfig()
            ```

        []{#getToolchainProvider()}

        -   #### getToolchainProvider

            ``` methodSignature
            ToolchainProvider getToolchainProvider()
            ```

        []{#getSandboxExecutionStrategy()}

        -   #### getSandboxExecutionStrategy

            ``` methodSignature
            SandboxExecutionStrategy getSandboxExecutionStrategy()
            ```

        []{#getPluginManager()}

        -   #### getPluginManager

            ``` methodSignature
            org.pf4j.PluginManager getPluginManager()
            ```

        []{#of(com.facebook.buck.core.config.BuckConfig,com.facebook.buck.core.toolchain.ToolchainProvider,com.facebook.buck.sandbox.SandboxExecutionStrategy,org.pf4j.PluginManager)}

        -   #### of

            ``` methodSignature
            static DescriptionCreationContext of​(BuckConfig buckConfig,
                                                 ToolchainProvider toolchainProvider,
                                                 SandboxExecutionStrategy sandboxExecutionStrategy,
                                                 org.pf4j.PluginManager pluginManager)
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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   Nested \| 
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
