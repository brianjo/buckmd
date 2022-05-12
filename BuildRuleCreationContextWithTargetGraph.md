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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules](package-summary.html)
:::

## Interface BuildRuleCreationContextWithTargetGraph {#interface-buildrulecreationcontextwithtargetgraph .title title="Interface BuildRuleCreationContextWithTargetGraph"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `BuildRuleCreationContext`

    ------------------------------------------------------------------------

        public interface BuildRuleCreationContextWithTargetGraph
        extends BuildRuleCreationContext

    ::: block
    Contains common objects used during
    [`BuildRule`](BuildRule.html "interface in com.facebook.buck.core.rules")
    creation in
    [`DescriptionWithTargetGraph.createBuildRule(com.facebook.buck.core.rules.BuildRuleCreationContextWithTargetGraph, com.facebook.buck.core.model.BuildTarget, com.facebook.buck.core.rules.BuildRuleParams, T)`](DescriptionWithTargetGraph.html#createBuildRule(com.facebook.buck.core.rules.BuildRuleCreationContextWithTargetGraph,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.BuildRuleParams,T)).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                  Method                                                                                                                                                                                                                                                                                              Description
          -------------------------------------------------- --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `ActionGraphBuilder`                               `getActionGraphBuilder()`                                                                                                                                                                                                                                                                            
          `CellPathResolver`                                 `getCellPathResolver()`                                                                                                                                                                                                                                                                              
          `ConfigurationRuleRegistry`                        `getConfigurationRuleRegistry()`                                                                                                                                                                                                                                                                     
          `ProjectFilesystem`                                `getProjectFilesystem()`                                                                                                                                                                                                                                                                             
          `ProviderInfoCollection`                           `getProviderInfoCollection()`                                                                                                                                                                                                                                                                        
          `TargetGraph`                                      `getTargetGraph()`                                                                                                                                                                                                                                                                                   
          `ToolchainProvider`                                `getToolchainProvider()`                                                                                                                                                                                                                                                                             
          `static BuildRuleCreationContextWithTargetGraph`   `of​(TargetGraph targetGraph,   ActionGraphBuilder actionGraphBuilder,   ProjectFilesystem projectFilesystem,   CellPathResolver cellPathResolver,   ToolchainProvider toolchainProvider,   ConfigurationRuleRegistry configurationRuleRegistry,   ProviderInfoCollection providerInfoCollection)`    

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

        []{#getTargetGraph()}

        -   #### getTargetGraph

            ``` methodSignature
            TargetGraph getTargetGraph()
            ```

        []{#getActionGraphBuilder()}

        -   #### getActionGraphBuilder

            ``` methodSignature
            ActionGraphBuilder getActionGraphBuilder()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getActionGraphBuilder` in
                interface `BuildRuleCreationContext`

        []{#getProjectFilesystem()}

        -   #### getProjectFilesystem

            ``` methodSignature
            ProjectFilesystem getProjectFilesystem()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getProjectFilesystem` in
                interface `BuildRuleCreationContext`

        []{#getCellPathResolver()}

        -   #### getCellPathResolver

            ``` methodSignature
            CellPathResolver getCellPathResolver()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCellPathResolver` in
                interface `BuildRuleCreationContext`

        []{#getToolchainProvider()}

        -   #### getToolchainProvider

            ``` methodSignature
            ToolchainProvider getToolchainProvider()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getToolchainProvider` in
                interface `BuildRuleCreationContext`

        []{#getConfigurationRuleRegistry()}

        -   #### getConfigurationRuleRegistry

            ``` methodSignature
            ConfigurationRuleRegistry getConfigurationRuleRegistry()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getConfigurationRuleRegistry` in
                interface `BuildRuleCreationContext`

        []{#getProviderInfoCollection()}

        -   #### getProviderInfoCollection

            ``` methodSignature
            ProviderInfoCollection getProviderInfoCollection()
            ```

            [Returns:]{.returnLabel}
            :   the
                [`ProviderInfoCollection`](providers/collect/ProviderInfoCollection.html "interface in com.facebook.buck.core.rules.providers.collect")
                that was created by the rules
                [`LegacyProviderCompatibleDescription.createProviders(ProviderCreationContext, BuildTarget,      BuildRuleArg)`](LegacyProviderCompatibleDescription.html#createProviders(com.facebook.buck.core.rules.ProviderCreationContext,com.facebook.buck.core.model.BuildTarget,T))

        []{#of(com.facebook.buck.core.model.targetgraph.TargetGraph,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.cell.CellPathResolver,com.facebook.buck.core.toolchain.ToolchainProvider,com.facebook.buck.core.rules.config.registry.ConfigurationRuleRegistry,com.facebook.buck.core.rules.providers.collect.ProviderInfoCollection)}

        -   #### of

            ``` methodSignature
            static BuildRuleCreationContextWithTargetGraph of​(TargetGraph targetGraph,
                                                              ActionGraphBuilder actionGraphBuilder,
                                                              ProjectFilesystem projectFilesystem,
                                                              CellPathResolver cellPathResolver,
                                                              ToolchainProvider toolchainProvider,
                                                              ConfigurationRuleRegistry configurationRuleRegistry,
                                                              ProviderInfoCollection providerInfoCollection)
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
