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
[Package]{.packageLabelInType} [com.facebook.buck.core.toolchain](package-summary.html)
:::

## Interface RuleAnalysisLegacyToolchain {#interface-ruleanalysislegacytoolchain .title title="Interface RuleAnalysisLegacyToolchain"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface RuleAnalysisLegacyToolchain

    ::: block
    Allows legacy
    [`Toolchain`](Toolchain.html "interface in com.facebook.buck.core.toolchain")s
    to be exposed in a generic way to the rule analysis graph via
    providers.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Pr                   | `getP                 |                       |
        | oviderInfoCollection` | roviders​(DependencyOn |                       |
        |                       | lyRuleAnalysisContext |                       |
        |                       |  context,             |                       |
        |                       |  TargetConfiguration  |                       |
        |                       | targetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `visitToo             | ::: block             |
        |                       | lDependencies​(TargetC | Add the dependencies  |
        |                       | onfiguration targetCo | for this toolchain to |
        |                       | nfiguration,          | the graph.            |
        |                       |              java.uti | :::                   |
        |                       | l.function.Consumer<B |                       |
        |                       | uildTarget> builder)` |                       |
        +-----------------------+-----------------------+-----------------------+

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

        []{#getProviders(com.facebook.buck.core.rules.analysis.context.DependencyOnlyRuleAnalysisContext,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getProviders

            ``` methodSignature
            ProviderInfoCollection getProviders​(DependencyOnlyRuleAnalysisContext context,
                                                TargetConfiguration targetConfiguration)
            ```

            [Returns:]{.returnLabel}
            :   the providers that describe this specific toolchain.
                e.g. A C++ toolchain might return a C++ToolchainInfo
                object that has a compiler, and default compiler flags

        []{#visitToolDependencies(com.facebook.buck.core.model.TargetConfiguration,java.util.function.Consumer)}

        -   #### visitToolDependencies

            ``` methodSignature
            void visitToolDependencies​(TargetConfiguration targetConfiguration,
                                       java.util.function.Consumer<BuildTarget> builder)
            ```

            ::: block
            Add the dependencies for this toolchain to the graph. This
            includes things like build targets for a compiler or linker,
            etc.
            :::

            [Parameters:]{.paramLabel}
            :   `targetConfiguration` - the configuration this toolchain
                will be used in
            :   `builder` - the builder to add dependencies to
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
