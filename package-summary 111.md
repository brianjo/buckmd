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
-   Package
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Package com.facebook.buck.core.util.graph {#package-com.facebook.buck.core.util.graph .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [AbstractBreadthFirstThr          | ::: block                         |
    | owingTraversal.Visitor](AbstractB | This will typically be            |
    | readthFirstThrowingTraversal.Visi | implemented as a lambda passed to |
    | tor.html "interface in com.facebo | [`Abstra                          |
    | ok.buck.core.util.graph")\<Node,​E | ctBreadthFirstThrowingTraversal.t |
    | extends                           | raverse(Object, Visitor)`](Abstra |
    | [Throwable](ht                    | ctBreadthFirstThrowingTraversal.h |
    | tp://docs.oracle.com/javase/7/doc | tml#traverse(Node,com.facebook.bu |
    | s/api/java/lang/Throwable.html?is | ck.core.util.graph.AbstractBreadt |
    | -external=true "class or interfac | hFirstThrowingTraversal.Visitor)) |
    | e in java.lang"){.externalLink}\> | or                                |
    |                                   | [`AbstractBreadthFirstTh          |
    |                                   | rowingTraversal.traverse(Iterable |
    |                                   | , Visitor)`](AbstractBreadthFirst |
    |                                   | ThrowingTraversal.html#traverse(j |
    |                                   | ava.lang.Iterable,com.facebook.bu |
    |                                   | ck.core.util.graph.AbstractBreadt |
    |                                   | hFirstThrowingTraversal.Visitor)) |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ForEachSucc                      | ::: block                         |
    | essorFunction](ForEachSuccessorFu | A `Consumer`-based interface for  |
    | nction.html "interface in com.fac | graph operations/traversals       |
    | ebook.buck.core.util.graph")\<N\> | (based on Guava\'s                |
    |                                   | \`SuccessorsFunction\`).          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [GraphTraversable](GraphTrave     |                                   |
    | rsable.html "interface in com.fac |                                   |
    | ebook.buck.core.util.graph")\<T\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | GraphTraversableWithDependencySta | Callback passed to                |
    | ck](GraphTraversableWithDependenc | [`AcyclicDepthFirstPostOrderTrav  |
    | yStack.html "interface in com.fac | ersalWithDependencyStack`](Acycli |
    | ebook.buck.core.util.graph")\<T\> | cDepthFirstPostOrderTraversalWith |
    |                                   | DependencyStack.html "class in co |
    |                                   | m.facebook.buck.core.util.graph") |
    |                                   | to access following nodes.        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [GraphTraversableWit              | ::: block                         |
    | hPayload](GraphTraversableWithPay | Callback passed to                |
    | load.html "interface in com.faceb | [`AcyclicDepthFi                  |
    | ook.buck.core.util.graph")\<T,​P\> | rstPostOrderTraversalWithPayload` |
    |                                   | ](AcyclicDepthFirstPostOrderTrave |
    |                                   | rsalWithPayload.html "class in co |
    |                                   | m.facebook.buck.core.util.graph") |
    |                                   | to access current node payload    |
    |                                   | and following nodes.              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [GraphTraversableWithPa           | ::: block                         |
    | yloadAndDependencyStack](GraphTra | Callback passed to                |
    | versableWithPayloadAndDependencyS | [`AcyclicDepthFirst               |
    | tack.html "interface in com.faceb | PostOrderTraversalWithPayloadAndD |
    | ook.buck.core.util.graph")\<T,​P\> | ependencyStack`](AcyclicDepthFirs |
    |                                   | tPostOrderTraversalWithPayloadAnd |
    |                                   | DependencyStack.html "class in co |
    |                                   | m.facebook.buck.core.util.graph") |
    |                                   | to access current node payload    |
    |                                   | and following nodes.              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [TopologicalSort.T                | ::: block                         |
    | raversable](TopologicalSort.Trave | User provider callback used for   |
    | rsable.html "interface in com.fac | walking the graph                 |
    | ebook.buck.core.util.graph")\<T\> | :::                               |
    +-----------------------------------+-----------------------------------+
    | [TraversableGraph](Traversabl     | ::: block                         |
    | eGraph.html "interface in com.fac | Minimal interface needed by       |
    | ebook.buck.core.util.graph")\<T\> | [`Abstr                           |
    |                                   | actBottomUpTraversal`](AbstractBo |
    |                                   | ttomUpTraversal.html "class in co |
    |                                   | m.facebook.buck.core.util.graph") |
    |                                   | to traverse a graph.              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [AbstractB                        | ::: block                         |
    | ottomUpTraversal](AbstractBottomU | Class that performs a             |
    | pTraversal.html "class in com.fac | \"bottom-up\" traversal of a DAG. |
    | ebook.buck.core.util.graph")\<T,​E | :::                               |
    | extends                           |                                   |
    | [Throwable](ht                    |                                   |
    | tp://docs.oracle.com/javase/7/doc |                                   |
    | s/api/java/lang/Throwable.html?is |                                   |
    | -external=true "class or interfac |                                   |
    | e in java.lang"){.externalLink}\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [Abs                              | ::: block                         |
    | tractBreadthFirstThrowingTraversa | Performs a breadth-first          |
    | l](AbstractBreadthFirstThrowingTr | traversal of dependencies of a    |
    | aversal.html "class in com.facebo | graph node.                       |
    | ok.buck.core.util.graph")\<Node,​E | :::                               |
    | extends                           |                                   |
    | [Throwable](ht                    |                                   |
    | tp://docs.oracle.com/javase/7/doc |                                   |
    | s/api/java/lang/Throwable.html?is |                                   |
    | -external=true "class or interfac |                                   |
    | e in java.lang"){.externalLink}\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [AbstractBreadthFirstThrowi       |                                   |
    | ngTraversal.StaticBreadthFirstTra |                                   |
    | versal](AbstractBreadthFirstThrow |                                   |
    | ingTraversal.StaticBreadthFirstTr |                                   |
    | aversal.html "class in com.facebo |                                   |
    | ok.buck.core.util.graph")\<Node\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [AbstractBreadthFirst             | ::: block                         |
    | Traversal](AbstractBreadthFirstTr | Performs a breadth-first          |
    | aversal.html "class in com.facebo | traversal of dependencies of a    |
    | ok.buck.core.util.graph")\<Node\> | graph node.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AcyclicDepthFirstPostOrderTra    | ::: block                         |
    | versal](AcyclicDepthFirstPostOrde | Performs a depth-first,           |
    | rTraversal.html "class in com.fac | post-order traversal over a DAG.  |
    | ebook.buck.core.util.graph")\<T\> | :::                               |
    +-----------------------------------+-----------------------------------+
    | [A                                | ::: block                         |
    | cyclicDepthFirstPostOrderTraversa | Performs a depth-first,           |
    | lWithDependencyStack](AcyclicDept | post-order traversal over a DAG.  |
    | hFirstPostOrderTraversalWithDepen | :::                               |
    | dencyStack.html "class in com.fac |                                   |
    | ebook.buck.core.util.graph")\<T\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [AcyclicDepthFirstPos             | ::: block                         |
    | tOrderTraversalWithPayload](Acycl | Performs a depth-first,           |
    | icDepthFirstPostOrderTraversalWit | post-order traversal over a DAG.  |
    | hPayload.html "class in com.faceb | :::                               |
    | ook.buck.core.util.graph")\<T,​P\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [AcyclicDepthFirstPostOr          | ::: block                         |
    | derTraversalWithPayloadAndDepende | Performs a depth-first,           |
    | ncyStack](AcyclicDepthFirstPostOr | post-order traversal over a DAG.  |
    | derTraversalWithPayloadAndDepende | :::                               |
    | ncyStack.html "class in com.faceb |                                   |
    | ook.buck.core.util.graph")\<T,​P\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [ConsumingTraverser](Consumin     | ::: block                         |
    | gTraverser.html "class in com.fac | `Consumer`-based graph            |
    | ebook.buck.core.util.graph")\<N\> | traversers.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DirectedAcyclicGraph](DirectedAc |                                   |
    | yclicGraph.html "class in com.fac |                                   |
    | ebook.buck.core.util.graph")\<T\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [MutableDirectedGraph](MutableDir | ::: block                         |
    | ectedGraph.html "class in com.fac | Represents a directed graph with  |
    | ebook.buck.core.util.graph")\<T\> | unweighted edges.                 |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [TopologicalSort](                |                                   |
    | TopologicalSort.html "class in co |                                   |
    | m.facebook.buck.core.util.graph") |                                   |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Exception                         | Description                       |
    +===================================+===================================+
    | [CycleException]                  | ::: block                         |
    | (CycleException.html "class in co | Exception thrown when graph       |
    | m.facebook.buck.core.util.graph") | traveral finds a cycle            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Exception Summary[ ]{.tabEnd}
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../../../index.html)
-   Package
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

[]{#skip.navbar.bottom}
:::
