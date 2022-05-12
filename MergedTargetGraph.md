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
[Package]{.packageLabelInType} [com.facebook.buck.core.model.targetgraph](package-summary.html)
:::

## Class MergedTargetGraph {#class-mergedtargetgraph .title title="Class MergedTargetGraph"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.util.graph.DirectedAcyclicGraph](../../util/graph/DirectedAcyclicGraph.html "class in com.facebook.buck.core.util.graph")\<[MergedTargetNode](MergedTargetNode.html "class in com.facebook.buck.core.model.targetgraph")\>

    -   -   com.facebook.buck.core.model.targetgraph.MergedTargetGraph

::: description
-   

    All Implemented Interfaces:
    :   `TraversableGraph<MergedTargetNode>`

    ------------------------------------------------------------------------

        public class MergedTargetGraph
        extends DirectedAcyclicGraph<MergedTargetNode>

    ::: block
    Target graph version where node is a set of all nodes with the same
    [`UnflavoredBuildTarget`](../UnflavoredBuildTarget.html "class in com.facebook.buck.core.model").
    This utility exists to support legacy configured `buck query`, and
    should not be used for anything else.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.google.commo     | `getIndex()`          |                       |
        | n.collect.ImmutableMa |                       |                       |
        | p<UnflavoredBuildTarg |                       |                       |
        | et,​MergedTargetNode>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `merge​(Directe        | ::: block             |
        | ic MergedTargetGraph` | dAcyclicGraph<TargetN | Group notes by        |
        |                       | ode<?>> targetGraph)` | [`UnflavoredB         |
        |                       |                       | uildTarget`](../Unfla |
        |                       |                       | voredBuildTarget.html |
        |                       |                       |  "class in com.facebo |
        |                       |                       | ok.buck.core.model"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.util.graph.DirectedAcyclicGraph}

            ### Methods inherited from class com.facebook.buck.core.util.graph.[DirectedAcyclicGraph](../../util/graph/DirectedAcyclicGraph.html "class in com.facebook.buck.core.util.graph")

            `equals, getIncomingNodesFor, getNodes, getNodesWithNoIncomingEdges, getNodesWithNoOutgoingEdges, getOutgoingEdges, getOutgoingNodesFor, hashCode`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getIndex()}

        -   #### getIndex

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<UnflavoredBuildTarget,​MergedTargetNode> getIndex()
            ```

        []{#merge(com.facebook.buck.core.util.graph.DirectedAcyclicGraph)}

        -   #### merge

            ``` methodSignature
            public static MergedTargetGraph merge​(DirectedAcyclicGraph<TargetNode<?>> targetGraph)
            ```

            ::: block
            Group notes by
            [`UnflavoredBuildTarget`](../UnflavoredBuildTarget.html "class in com.facebook.buck.core.model").
            :::
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
