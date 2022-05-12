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

## Class ConsumingTraverser\<N\> {#class-consumingtraversern .title title="Class ConsumingTraverser"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.util.graph.ConsumingTraverser\<N\>

::: description
-   

    ------------------------------------------------------------------------

        public abstract class ConsumingTraverser<N>
        extends Object

    ::: block
    `Consumer`-based graph traversers.
    Implements various graph traversals for graphs represented by
    [`ForEachSuccessorFunction`](ForEachSuccessorFunction.html "interface in com.facebook.buck.core.util.graph").
    This may be desirable to use instead of `Abstract*Traversal`s in
    cases where the overhead of buffering node dependencies in
    streams/iterables/collections needs to be avoided (as node
    dependencies are discovered/consumed without per-node buffering).

    The traversals generally avoid extra bookkeeping to detect graph
    cycles, and so may silently produce undefined results in this case.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor              Description
          ------------------------ -------------
          `ConsumingTraverser()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static <N> C         | `breadthFirst​(It      | ::: block             |
        | onsumingTraverser<N>` | erable<? extends N> s | Consume nodes via     |
        |                       | tartNodes,            | `consumer`, starting  |
        |                       |   ForEachSuccessorFun | from `startNodes`, in |
        |                       | ction<N> successors)` | a breadth-first walk  |
        |                       |                       | of the graph.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract void`       | `forEach              |                       |
        |                       | ​(java.util.function.C |                       |
        |                       | onsumer<N> consumer)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `<E ex                | `forEac               |                       |
        | tends Exception>void` | hThrowing​(ThrowingCon |                       |
        |                       | sumer<N,​E> consumer)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <N> C         | `topologi             | ::: block             |
        | onsumingTraverser<N>` | callySorted​(Iterable< | Consume nodes via     |
        |                       | ? extends N> startNod | `consumer`, starting  |
        |                       | es,                   | from `startNodes`, in |
        |                       |   ForEachSuccessorFun | a topologically       |
        |                       | ction<N> successors)` | sorted order.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

        -   #### ConsumingTraverser

                public ConsumingTraverser()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#forEach(java.util.function.Consumer)}

        -   #### forEach

            ``` methodSignature
            public abstract void forEach​(java.util.function.Consumer<N> consumer)
            ```

        []{#forEachThrowing(com.facebook.buck.util.function.ThrowingConsumer)}

        -   #### forEachThrowing

            ``` methodSignature
            public final <E extends Exception> void forEachThrowing​(ThrowingConsumer<N,​E> consumer)
                                                             throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#breadthFirst(java.lang.Iterable,com.facebook.buck.core.util.graph.ForEachSuccessorFunction)}

        -   #### breadthFirst

            ``` methodSignature
            public static <N> ConsumingTraverser<N> breadthFirst​(Iterable<? extends N> startNodes,
                                                                 ForEachSuccessorFunction<N> successors)
            ```

            ::: block
            Consume nodes via `consumer`, starting from `startNodes`, in
            a breadth-first walk of the graph.
            Allocates a set of O(#nodes) to record visited nodes and a
            queue of O(width).
            :::

        []{#topologicallySorted(java.lang.Iterable,com.facebook.buck.core.util.graph.ForEachSuccessorFunction)}

        -   #### topologicallySorted

            ``` methodSignature
            public static <N> ConsumingTraverser<N> topologicallySorted​(Iterable<? extends N> startNodes,
                                                                        ForEachSuccessorFunction<N> successors)
            ```

            ::: block
            Consume nodes via `consumer`, starting from `startNodes`, in
            a topologically sorted order.
            :::

            [Returns:]{.returnLabel}

            :   a
                [`ConsumingTraverser`](ConsumingTraverser.html "class in com.facebook.buck.core.util.graph")
                for a graph represented by the given
                [`ForEachSuccessorFunction`](ForEachSuccessorFunction.html "interface in com.facebook.buck.core.util.graph").

                Allocates a set of O(#nodes) to record visited nodes, a
                map of (#nodes) to count incoming edges, and a queue of
                nodes to process. Calls each node\'s successor consumer
                function twice.
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
