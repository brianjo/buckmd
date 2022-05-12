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
[Package]{.packageLabelInType} [com.facebook.buck.core.util.graph](package-summary.html)
:::

## Class MutableDirectedGraph\<T\> {#class-mutabledirectedgrapht .title title="Class MutableDirectedGraph"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.util.graph.MutableDirectedGraph\<T\>

::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `T` - the type of object stored as nodes in this graph

    ```{=html}
    <!-- -->
    ```

    All Implemented Interfaces:
    :   `TraversableGraph<T>`

    ------------------------------------------------------------------------

        public final class MutableDirectedGraph<T>
        extends Object
        implements TraversableGraph<T>

    ::: block
    Represents a directed graph with unweighted edges. For a given
    source and sink node pair, there is at most one directed edge
    connecting them in the graph. The graph is not required to be
    connected or acyclic.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `MutableDirectedGraph()`          | ::: block                         |
        |                                   | Creates a new graph with no nodes |
        |                                   | or edges.                         |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `addEdge​(T so         | ::: block             |
        |                       | urce,        T sink)` | Adds an edge between  |
        |                       |                       | `source` and `sink`.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `addNode​(T node)`     | ::: block             |
        |                       |                       | Adds the specified    |
        |                       |                       | node to the graph.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `c                    |                       |
        |                       | ontainsEdge​(T source, |                       |
        |                       |              T sink)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `                     |                       |
        |                       | containsNode​(T node)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <T> Mut       | `createConcurrent()`  |                       |
        | ableDirectedGraph<T>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.c  | `findCycles()`        |                       |
        | ollect.ImmutableSet<c |                       |                       |
        | om.google.common.coll |                       |                       |
        | ect.ImmutableSet<T>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Set<Set<T>>`         | `findStronglyC        | ::: block             |
        |                       | onnectedComponents()` | For this graph,       |
        |                       |                       | returns the set of    |
        |                       |                       | strongly connected    |
        |                       |                       | components using      |
        |                       |                       | Tarjan\'s algorithm.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getEdgeCount()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<T>`         | `getInco              |                       |
        |                       | mingNodesFor​(T sink)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getNodeCount()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Set<T>`              | `getNodes()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<T>`         | `getNodesW            |                       |
        |                       | ithNoIncomingEdges()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<T>`         | `getNodesW            |                       |
        |                       | ithNoOutgoingEdges()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<T>`         | `getOutgoi            |                       |
        |                       | ngNodesFor​(T source)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `hasI                 |                       |
        |                       | ncomingEdges​(T node)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isAcyclic()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `removeEdge​(T sourc   | ::: block             |
        |                       | e,           T sink)` | Removes the edge      |
        |                       |                       | between `source` and  |
        |                       |                       | `sink`.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `removeNode​(T node)`  | ::: block             |
        |                       |                       | Removes the specified |
        |                       |                       | node from the graph.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
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

        []{#<init>()}

        -   #### MutableDirectedGraph

                public MutableDirectedGraph()

            ::: block
            Creates a new graph with no nodes or edges.
            :::
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createConcurrent()}

        -   #### createConcurrent

            ``` methodSignature
            public static <T> MutableDirectedGraph<T> createConcurrent()
            ```

        []{#getNodeCount()}

        -   #### getNodeCount

            ``` methodSignature
            public int getNodeCount()
            ```

            [Returns:]{.returnLabel}
            :   the number of nodes in the graph

        []{#getEdgeCount()}

        -   #### getEdgeCount

            ``` methodSignature
            public int getEdgeCount()
            ```

            [Returns:]{.returnLabel}
            :   the number of edges in the graph

        []{#containsNode(java.lang.Object)} []{#containsNode(T)}

        -   #### containsNode

            ``` methodSignature
            public boolean containsNode​(T node)
            ```

            [Returns:]{.returnLabel}
            :   whether the specified node is present in the graph

        []{#containsEdge(java.lang.Object,java.lang.Object)}
        []{#containsEdge(T,T)}

        -   #### containsEdge

            ``` methodSignature
            public boolean containsEdge​(T source,
                                        T sink)
            ```

            [Returns:]{.returnLabel}
            :   whether an edge from the source to the sink is present
                in the graph

        []{#addNode(java.lang.Object)} []{#addNode(T)}

        -   #### addNode

            ``` methodSignature
            public boolean addNode​(T node)
            ```

            ::: block
            Adds the specified node to the graph.
            :::

        []{#removeNode(java.lang.Object)} []{#removeNode(T)}

        -   #### removeNode

            ``` methodSignature
            public boolean removeNode​(T node)
            ```

            ::: block
            Removes the specified node from the graph.
            :::

        []{#addEdge(java.lang.Object,java.lang.Object)}
        []{#addEdge(T,T)}

        -   #### addEdge

            ``` methodSignature
            public void addEdge​(T source,
                                T sink)
            ```

            ::: block
            Adds an edge between `source` and `sink`. Adds the nodes to
            the graph if they are not already present.
            :::

        []{#removeEdge(java.lang.Object,java.lang.Object)}
        []{#removeEdge(T,T)}

        -   #### removeEdge

            ``` methodSignature
            public void removeEdge​(T source,
                                   T sink)
            ```

            ::: block
            Removes the edge between `source` and `sink`. This does not
            remove `source` or `sink` from the graph. Note that this may
            leave either `source` or `sink` as unconnected nodes in the
            graph.
            :::

        []{#getOutgoingNodesFor(java.lang.Object)}
        []{#getOutgoingNodesFor(T)}

        -   #### getOutgoingNodesFor

            ``` methodSignature
            public Iterable<T> getOutgoingNodesFor​(T source)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getOutgoingNodesFor` in interface `TraversableGraph<T>`

            [Returns:]{.returnLabel}
            :   [`Iterable`](http://docs.oracle.com/javase/7/docs/api/java/lang/Iterable.html?is-external=true "class or interface in java.lang"){.externalLink}
                that the caller is not allowed to mutate.

        []{#getIncomingNodesFor(java.lang.Object)}
        []{#getIncomingNodesFor(T)}

        -   #### getIncomingNodesFor

            ``` methodSignature
            public Iterable<T> getIncomingNodesFor​(T sink)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getIncomingNodesFor` in interface `TraversableGraph<T>`

            [Returns:]{.returnLabel}
            :   [`Iterable`](http://docs.oracle.com/javase/7/docs/api/java/lang/Iterable.html?is-external=true "class or interface in java.lang"){.externalLink}
                that the caller is not allowed to mutate.

        []{#hasIncomingEdges(java.lang.Object)} []{#hasIncomingEdges(T)}

        -   #### hasIncomingEdges

            ``` methodSignature
            public boolean hasIncomingEdges​(T node)
            ```

        []{#getNodes()}

        -   #### getNodes

            ``` methodSignature
            public Set<T> getNodes()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNodes` in interface `TraversableGraph<T>`

            [Returns:]{.returnLabel}
            :   an unmodifiable view of the nodes in this graph

        []{#isAcyclic()}

        -   #### isAcyclic

            ``` methodSignature
            public boolean isAcyclic()
            ```

        []{#findCycles()}

        -   #### findCycles

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<com.google.common.collect.ImmutableSet<T>> findCycles()
            ```

        []{#findStronglyConnectedComponents()}

        -   #### findStronglyConnectedComponents

            ``` methodSignature
            public Set<Set<T>> findStronglyConnectedComponents()
            ```

            ::: block
            For this graph, returns the set of strongly connected
            components using Tarjan\'s algorithm. Note this is
            `O(|V| + |E|)`.
            :::

            [Returns:]{.returnLabel}
            :   an unmodifiable
                [`Set`](http://docs.oracle.com/javase/7/docs/api/java/util/Set.html?is-external=true "class or interface in java.util"){.externalLink}
                of sets, each of which is also an unmodifiable
                [`Set`](http://docs.oracle.com/javase/7/docs/api/java/util/Set.html?is-external=true "class or interface in java.util"){.externalLink}
                and represents a strongly connected component.

        []{#getNodesWithNoIncomingEdges()}

        -   #### getNodesWithNoIncomingEdges

            ``` methodSignature
            public Iterable<T> getNodesWithNoIncomingEdges()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNodesWithNoIncomingEdges` in
                interface `TraversableGraph<T>`

            [Returns:]{.returnLabel}
            :   [`Iterable`](http://docs.oracle.com/javase/7/docs/api/java/lang/Iterable.html?is-external=true "class or interface in java.lang"){.externalLink}
                that the caller is not allowed to mutate.

        []{#getNodesWithNoOutgoingEdges()}

        -   #### getNodesWithNoOutgoingEdges

            ``` methodSignature
            public Iterable<T> getNodesWithNoOutgoingEdges()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNodesWithNoOutgoingEdges` in
                interface `TraversableGraph<T>`

            [Returns:]{.returnLabel}
            :   [`Iterable`](http://docs.oracle.com/javase/7/docs/api/java/lang/Iterable.html?is-external=true "class or interface in java.lang"){.externalLink}
                that the caller is not allowed to mutate.
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
