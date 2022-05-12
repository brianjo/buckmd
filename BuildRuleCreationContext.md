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

## Interface BuildRuleCreationContext {#interface-buildrulecreationcontext .title title="Interface BuildRuleCreationContext"}
:::

::: contentContainer
::: description
-   

    All Known Subinterfaces:
    :   `BuildRuleCreationContextWithTargetGraph`

    ------------------------------------------------------------------------

        public interface BuildRuleCreationContext

    ::: block
    Common objects used during
    [`BuildRule`](BuildRule.html "interface in com.facebook.buck.core.rules")
    creation, without a reference to
    [`TargetGraph`](../model/targetgraph/TargetGraph.html "class in com.facebook.buck.core.model.targetgraph")
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type             Method                             Description
          ----------------------------- ---------------------------------- -------------
          `ActionGraphBuilder`          `getActionGraphBuilder()`           
          `CellPathResolver`            `getCellPathResolver()`             
          `ConfigurationRuleRegistry`   `getConfigurationRuleRegistry()`    
          `ProjectFilesystem`           `getProjectFilesystem()`            
          `ToolchainProvider`           `getToolchainProvider()`            

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getActionGraphBuilder()}

        -   #### getActionGraphBuilder

            ``` methodSignature
            ActionGraphBuilder getActionGraphBuilder()
            ```

        []{#getProjectFilesystem()}

        -   #### getProjectFilesystem

            ``` methodSignature
            ProjectFilesystem getProjectFilesystem()
            ```

        []{#getCellPathResolver()}

        -   #### getCellPathResolver

            ``` methodSignature
            CellPathResolver getCellPathResolver()
            ```

        []{#getToolchainProvider()}

        -   #### getToolchainProvider

            ``` methodSignature
            ToolchainProvider getToolchainProvider()
            ```

        []{#getConfigurationRuleRegistry()}

        -   #### getConfigurationRuleRegistry

            ``` methodSignature
            ConfigurationRuleRegistry getConfigurationRuleRegistry()
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
