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
[Package]{.packageLabelInType} [com.facebook.buck.parser](package-summary.html)
:::

## Interface ParserTargetNodeFromAttrMapFactory {#interface-parsertargetnodefromattrmapfactory .title title="Interface ParserTargetNodeFromAttrMapFactory"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface ParserTargetNodeFromAttrMapFactory

    ::: block
    Creates
    [`TargetNode`](../core/model/targetgraph/TargetNode.html "interface in com.facebook.buck.core.model.targetgraph")
    instances from raw attribute map returned by the parser. This is a
    legacy interface which is used only for configuration targets, and
    should be removed.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                                                                                                                                                                                                                          Description
          ------------------- --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `TargetNode<?>`     `createTargetNode​(Cell cell,                 Path buildFile,                 BuildTarget target,                 DependencyStack dependencyStack,                 Map<String,​Object> rawNode,                 java.util.function.Function<SimplePerfEvent.PerfEventId,​SimplePerfEvent.Scope> perfEventScope)`    

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

        []{#createTargetNode(com.facebook.buck.core.cell.Cell,java.nio.file.Path,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.exceptions.DependencyStack,java.util.Map,java.util.function.Function)}

        -   #### createTargetNode

            ``` methodSignature
            TargetNode<?> createTargetNode​(Cell cell,
                                           Path buildFile,
                                           BuildTarget target,
                                           DependencyStack dependencyStack,
                                           Map<String,​Object> rawNode,
                                           java.util.function.Function<SimplePerfEvent.PerfEventId,​SimplePerfEvent.Scope> perfEventScope)
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
