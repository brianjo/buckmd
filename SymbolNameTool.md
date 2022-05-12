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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain](package-summary.html)
:::

## Interface SymbolNameTool {#interface-symbolnametool .title title="Interface SymbolNameTool"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `PosixNmSymbolNameTool`

    ------------------------------------------------------------------------

        public interface SymbolNameTool

    ::: block
    Provides methods to extract symbol names from native formats (e.g.
    binaries, shared libraries, object files).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `SourcePath`          | `crea                 | ::: block             |
        |                       | teUndefinedSymbolsFil | Creates a             |
        |                       | e​(ProjectFilesystem p | [`Buil                |
        |                       | rojectFilesystem,     | dRule`](../../core/ru |
        |                       |                       | les/BuildRule.html "i |
        |                       |   BuildRuleParams bas | nterface in com.faceb |
        |                       | eParams,              | ook.buck.core.rules") |
        |                       |               ActionG | which extracts all    |
        |                       | raphBuilder graphBuil | undefined symbols     |
        |                       | der,                  | from the given        |
        |                       |           TargetConfi | inputs.               |
        |                       | guration targetConfig | :::                   |
        |                       | uration,              |                       |
        |                       |               BuildTa |                       |
        |                       | rget target,          |                       |
        |                       |                   Ite |                       |
        |                       | rable<? extends Sourc |                       |
        |                       | ePath> linkerInputs)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `I                    | `getParseTimeDeps     |                       |
        | terable<BuildTarget>` | ​(TargetConfiguration  |                       |
        |                       | targetConfiguration)` |                       |
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

        []{#createUndefinedSymbolsFile(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.model.BuildTarget,java.lang.Iterable)}

        -   #### createUndefinedSymbolsFile

            ``` methodSignature
            SourcePath createUndefinedSymbolsFile​(ProjectFilesystem projectFilesystem,
                                                  BuildRuleParams baseParams,
                                                  ActionGraphBuilder graphBuilder,
                                                  TargetConfiguration targetConfiguration,
                                                  BuildTarget target,
                                                  Iterable<? extends SourcePath> linkerInputs)
            ```

            ::: block
            Creates a
            [`BuildRule`](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
            which extracts all undefined symbols from the given inputs.
            :::

            [Parameters:]{.paramLabel}
            :   `target` - the name to use when creating the rule which
                extracts the symbols.

            [Returns:]{.returnLabel}
            :   a
                [`SourcePath`](../../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
                referring to a file containing all undefined symbols,
                one per line, in the given inputs.

        []{#getParseTimeDeps(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getParseTimeDeps

            ``` methodSignature
            Iterable<BuildTarget> getParseTimeDeps​(TargetConfiguration targetConfiguration)
            ```

            [Returns:]{.returnLabel}
            :   any dependencies required at parse time to support the
                provided tool.
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
