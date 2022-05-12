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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.model.targetgraph](package-summary.html)
:::

## Class TargetGraph {#class-targetgraph .title title="Class TargetGraph"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.util.graph.DirectedAcyclicGraph](../../util/graph/DirectedAcyclicGraph.html "class in com.facebook.buck.core.util.graph")\<[TargetNode](TargetNode.html "interface in com.facebook.buck.core.model.targetgraph")\<?\>\>

    -   -   com.facebook.buck.core.model.targetgraph.TargetGraph

::: description
-   

    All Implemented Interfaces:
    :   `TraversableGraph<TargetNode<?>>`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `VersionedTargetGraph`

    ------------------------------------------------------------------------

        public class TargetGraph
        extends DirectedAcyclicGraph<TargetNode<?>>

    ::: block
    Represents the graph of
    [`TargetNode`](TargetNode.html "interface in com.facebook.buck.core.model.targetgraph")s
    constructed by parsing the build files.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type      Field     Description
          ---------------------- --------- -------------
          `static TargetGraph`   `EMPTY`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                    Description
          ---------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `TargetGraph​(MutableDirectedGraph<TargetNode<?>> graph,            com.google.common.collect.ImmutableMap<BuildTarget,​TargetNode<?>> index)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `equals​(Object obj)`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `TargetNode<?>`       | `get                  | ::: block             |
        |                       | ​(BuildTarget target)` | Get a target from     |
        |                       |                       | graph.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `TargetNode<?>`       | `get​(BuildTarget ta   | ::: block             |
        |                       | rget,    DependencySt | Get a target from     |
        |                       | ack dependencyStack)` | graph                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Ite                  | `getAll​(Iterable<B    |                       |
        | rable<TargetNode<?>>` | uildTarget> targets)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Opt                  | `getExactOptional     | ::: block             |
        | ional<TargetNode<?>>` | ​(BuildTarget target)` | Returns the target    |
        |                       |                       | node for the exact    |
        |                       |                       | given target, if it   |
        |                       |                       | exists in the graph.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `pro                  | `getInternal          |                       |
        | tected TargetNode<?>` | ​(BuildTarget target)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Opt                  | `getOptional          |                       |
        | ional<TargetNode<?>>` | ​(BuildTarget target)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getSize()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `<T> TargetGraph`     | `                     | ::: block             |
        |                       | getSubgraph​(Iterable< | Get the subgraph of   |
        |                       | ? extends TargetNode< | the the current graph |
        |                       | ? extends T>> roots)` | containing the passed |
        |                       |                       | in roots and all of   |
        |                       |                       | their transitive      |
        |                       |                       | dependencies as       |
        |                       |                       | nodes.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.util.graph.DirectedAcyclicGraph}

            ### Methods inherited from class com.facebook.buck.core.util.graph.[DirectedAcyclicGraph](../../util/graph/DirectedAcyclicGraph.html "class in com.facebook.buck.core.util.graph")

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
    -   []{#field.detail}

        ### Field Detail

        []{#EMPTY}

        -   #### EMPTY

                public static final TargetGraph EMPTY
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.util.graph.MutableDirectedGraph,com.google.common.collect.ImmutableMap)}

        -   #### TargetGraph

                public TargetGraph​(MutableDirectedGraph<TargetNode<?>> graph,
                                   com.google.common.collect.ImmutableMap<BuildTarget,​TargetNode<?>> index)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getInternal(com.facebook.buck.core.model.BuildTarget)}

        -   #### getInternal

            ``` methodSignature
            @Nullable
            protected TargetNode<?> getInternal​(BuildTarget target)
            ```

        []{#getOptional(com.facebook.buck.core.model.BuildTarget)}

        -   #### getOptional

            ``` methodSignature
            public Optional<TargetNode<?>> getOptional​(BuildTarget target)
            ```

        []{#get(com.facebook.buck.core.model.BuildTarget)}

        -   #### get

            ``` methodSignature
            public TargetNode<?> get​(BuildTarget target)
            ```

            ::: block
            Get a target from graph. Use of
            [`get(BuildTarget, DependencyStack)`](#get(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.exceptions.DependencyStack))
            is encouraged because it provides better diagnostics
            :::

        []{#get(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.exceptions.DependencyStack)}

        -   #### get

            ``` methodSignature
            public TargetNode<?> get​(BuildTarget target,
                                     DependencyStack dependencyStack)
            ```

            ::: block
            Get a target from graph
            :::

        []{#getExactOptional(com.facebook.buck.core.model.BuildTarget)}

        -   #### getExactOptional

            ``` methodSignature
            public Optional<TargetNode<?>> getExactOptional​(BuildTarget target)
            ```

            ::: block
            Returns the target node for the exact given target, if it
            exists in the graph.
            If given a flavored target, and the target graph doesn\'t
            contain that flavored target, this method will always return
            null, unlike `getOptional`, which may return the node for a
            differently flavored target ({@see
            VersionedTargetGraph#getInternal}).
            :::

        []{#getAll(java.lang.Iterable)}

        -   #### getAll

            ``` methodSignature
            public Iterable<TargetNode<?>> getAll​(Iterable<BuildTarget> targets)
            ```

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object obj)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `DirectedAcyclicGraph<TargetNode<?>>`

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in
                class `DirectedAcyclicGraph<TargetNode<?>>`

        []{#getSubgraph(java.lang.Iterable)}

        -   #### getSubgraph

            ``` methodSignature
            public <T> TargetGraph getSubgraph​(Iterable<? extends TargetNode<? extends T>> roots)
            ```

            ::: block
            Get the subgraph of the the current graph containing the
            passed in roots and all of their transitive dependencies as
            nodes. Edges between the included nodes are preserved.
            :::

            [Parameters:]{.paramLabel}
            :   `roots` - An iterable containing the roots of the new
                subgraph.

            [Returns:]{.returnLabel}
            :   A subgraph of the current graph.

        []{#getSize()}

        -   #### getSize

            ``` methodSignature
            public int getSize()
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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
