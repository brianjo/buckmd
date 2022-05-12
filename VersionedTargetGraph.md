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
-   [Nested](#nested.class.summary) \| 
-   [Field](#field.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.versions](package-summary.html)
:::

## Class VersionedTargetGraph {#class-versionedtargetgraph .title title="Class VersionedTargetGraph"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.util.graph.DirectedAcyclicGraph](../core/util/graph/DirectedAcyclicGraph.html "class in com.facebook.buck.core.util.graph")\<[TargetNode](../core/model/targetgraph/TargetNode.html "interface in com.facebook.buck.core.model.targetgraph")\<?\>\>

    -   -   [com.facebook.buck.core.model.targetgraph.TargetGraph](../core/model/targetgraph/TargetGraph.html "class in com.facebook.buck.core.model.targetgraph")

        -   -   com.facebook.buck.versions.VersionedTargetGraph

::: description
-   

    All Implemented Interfaces:
    :   `TraversableGraph<TargetNode<?>>`

    ------------------------------------------------------------------------

        public class VersionedTargetGraph
        extends TargetGraph
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                            Description
          ------------------- -------------------------------- -------------
          `static class `     `VersionedTargetGraph.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.core.model.targetgraph.TargetGraph}

            ### Fields inherited from class com.facebook.buck.core.model.targetgraph.[TargetGraph](../core/model/targetgraph/TargetGraph.html "class in com.facebook.buck.core.model.targetgraph")

            `EMPTY`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                       Method                              Description
          --------------------------------------- ----------------------------------- -------------
          `static VersionedTargetGraph.Builder`   `builder()`                          
          `protected TargetNode<?>`               `getInternal​(BuildTarget target)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.model.targetgraph.TargetGraph}

            ### Methods inherited from class com.facebook.buck.core.model.targetgraph.[TargetGraph](../core/model/targetgraph/TargetGraph.html "class in com.facebook.buck.core.model.targetgraph")

            `equals, get, get, getAll, getExactOptional, getOptional, getSize, getSubgraph, hashCode`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.util.graph.DirectedAcyclicGraph}

            ### Methods inherited from class com.facebook.buck.core.util.graph.[DirectedAcyclicGraph](../core/util/graph/DirectedAcyclicGraph.html "class in com.facebook.buck.core.util.graph")

            `getIncomingNodesFor, getNodes, getNodesWithNoIncomingEdges, getNodesWithNoOutgoingEdges, getOutgoingEdges, getOutgoingNodesFor`

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

        []{#getInternal(com.facebook.buck.core.model.BuildTarget)}

        -   #### getInternal

            ``` methodSignature
            @Nullable
            protected TargetNode<?> getInternal​(BuildTarget target)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `getInternal` in class `TargetGraph`

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static VersionedTargetGraph.Builder builder()
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
-   [Nested](#nested.class.summary) \| 
-   [Field](#field.summary) \| 
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
