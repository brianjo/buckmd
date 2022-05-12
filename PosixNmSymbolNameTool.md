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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain](package-summary.html)
:::

## Class PosixNmSymbolNameTool {#class-posixnmsymbolnametool .title title="Class PosixNmSymbolNameTool"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.toolchain.PosixNmSymbolNameTool

::: description
-   

    All Implemented Interfaces:
    :   `SymbolNameTool`

    ------------------------------------------------------------------------

        public class PosixNmSymbolNameTool
        extends Object
        implements SymbolNameTool

    ::: block
    A
    [`SymbolNameTool`](SymbolNameTool.html "interface in com.facebook.buck.cxx.toolchain")
    implementation using a POSIX-compliant \`nm\` utility
    (http://pubs.opengroup.org/onlinepubs/009696699/utilities/nm.html).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                Description
          ------------------------------------------ -------------
          `PosixNmSymbolNameTool​(ToolProvider nm)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
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

        []{#<init>(com.facebook.buck.core.toolchain.toolprovider.ToolProvider)}

        -   #### PosixNmSymbolNameTool

                public PosixNmSymbolNameTool​(ToolProvider nm)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createUndefinedSymbolsFile(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.model.BuildTarget,java.lang.Iterable)}

        -   #### createUndefinedSymbolsFile

            ``` methodSignature
            public SourcePath createUndefinedSymbolsFile​(ProjectFilesystem projectFilesystem,
                                                         BuildRuleParams baseParams,
                                                         ActionGraphBuilder graphBuilder,
                                                         TargetConfiguration targetConfiguration,
                                                         BuildTarget target,
                                                         Iterable<? extends SourcePath> linkerInputs)
            ```

            ::: block
            [Description copied from
            interface: `SymbolNameTool`]{.descfrmTypeLabel}
            :::

            ::: block
            Creates a
            [`BuildRule`](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
            which extracts all undefined symbols from the given inputs.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `createUndefinedSymbolsFile` in
                interface `SymbolNameTool`
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
            public Iterable<BuildTarget> getParseTimeDeps​(TargetConfiguration targetConfiguration)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getParseTimeDeps` in interface `SymbolNameTool`

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
