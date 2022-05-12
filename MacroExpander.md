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
[Package]{.packageLabelInType} [com.facebook.buck.rules.macros](package-summary.html)
:::

## Interface MacroExpander\<T,​P\> {#interface-macroexpandertp .title title="Interface MacroExpander"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `AbsoluteOutputMacroExpander`, `AbstractLocationMacroExpander`,
        `AbstractMacroExpanderWithoutPrecomputedWork`, `ArgExpander`,
        `BuildTargetMacroExpander`, `ClasspathAbiMacroExpander`,
        `ClasspathMacroExpander`, `CxxLocationMacroExpander`,
        `EnvironmentVariableMacroExpander`, `ExecutableMacroExpander`,
        `LocationMacroExpander`, `LocationPlatformMacroExpander`,
        `MavenCoordinatesMacroExpander`, `OutputMacroExpander`,
        `QueryMacroExpander`, `QueryOutputsMacroExpander`,
        `QueryPathsMacroExpander`,
        `QueryTargetsAndOutputsMacroExpander`,
        `QueryTargetsMacroExpander`, `SimpleMacroExpander`,
        `StringExpander`, `WorkerMacroExpander`

    ------------------------------------------------------------------------

        public interface MacroExpander<T,​P>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                                                                                 Description
          ------------------- ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `Arg`               `expandFrom​(BuildTarget target,           ActionGraphBuilder graphBuilder,           T input,           P precomputedWork)`                                             
          `Class<T>`          `getInputClass()`                                                                                                                                                       
          `P`                 `precomputeWorkFrom​(BuildTarget target,                   CellNameResolver cellNames,                   ActionGraphBuilder graphBuilder,                   T input)`    

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

        []{#getInputClass()}

        -   #### getInputClass

            ``` methodSignature
            Class<T> getInputClass()
            ```

            [Returns:]{.returnLabel}
            :   the class for the parsed macro input type.

        []{#precomputeWorkFrom(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.core.rules.ActionGraphBuilder,java.lang.Object)}
        []{#precomputeWorkFrom(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.core.rules.ActionGraphBuilder,T)}

        -   #### precomputeWorkFrom

            ``` methodSignature
            P precomputeWorkFrom​(BuildTarget target,
                                 CellNameResolver cellNames,
                                 ActionGraphBuilder graphBuilder,
                                 T input)
                          throws MacroException
            ```

            [Returns:]{.returnLabel}
            :   the precomputed work that can be re-used between
                invocations

            [Throws:]{.throwsLabel}
            :   `MacroException`

        []{#expandFrom(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder,java.lang.Object,java.lang.Object)}
        []{#expandFrom(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder,T,P)}

        -   #### expandFrom

            ``` methodSignature
            Arg expandFrom​(BuildTarget target,
                           ActionGraphBuilder graphBuilder,
                           T input,
                           P precomputedWork)
                    throws MacroException
            ```

            [Throws:]{.throwsLabel}
            :   `MacroException`
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
