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

## Class AcyclicDepthFirstPostOrderTraversal\<T\> {#class-acyclicdepthfirstpostordertraversalt .title title="Class AcyclicDepthFirstPostOrderTraversal"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.util.graph.AcyclicDepthFirstPostOrderTraversal\<T\>

::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `T` - the type of node in the graph

    ------------------------------------------------------------------------

        public class AcyclicDepthFirstPostOrderTraversal<T>
        extends Object

    ::: block
    Performs a depth-first, post-order traversal over a DAG.
    If a cycle is encountered, a
    [`CycleException`](CycleException.html "class in com.facebook.buck.core.util.graph")
    is thrown by [`traverse(Iterable)`](#traverse(java.lang.Iterable)).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                              Description
          ------------------------------------------------------------------------ -------------
          `AcyclicDepthFirstPostOrderTraversal​(GraphTraversable<T> traversable)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Iterable<T>`         | `tra                  |                       |
        |                       | verse​(Iterable<? exte |                       |
        |                       | nds T> initialNodes)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<T>`         | `tra                  | ::: block             |
        |                       | verse​(Iterable<? exte | Performs a            |
        |                       | nds T> initialNodes,  | depth-first,          |
        |                       |         java.util.fun | post-order traversal  |
        |                       | ction.Predicate<T> sh | over a DAG.           |
        |                       | ouldExploreChildren)` | :::                   |
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

        []{#<init>(com.facebook.buck.core.util.graph.GraphTraversable)}

        -   #### AcyclicDepthFirstPostOrderTraversal

                public AcyclicDepthFirstPostOrderTraversal​(GraphTraversable<T> traversable)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#traverse(java.lang.Iterable)}

        -   #### traverse

            ``` methodSignature
            public Iterable<T> traverse​(Iterable<? extends T> initialNodes)
                                 throws CycleException
            ```

            [Throws:]{.throwsLabel}
            :   `CycleException`

        []{#traverse(java.lang.Iterable,java.util.function.Predicate)}

        -   #### traverse

            ``` methodSignature
            public Iterable<T> traverse​(Iterable<? extends T> initialNodes,
                                        java.util.function.Predicate<T> shouldExploreChildren)
                                 throws CycleException
            ```

            ::: block
            Performs a depth-first, post-order traversal over a DAG.
            :::

            [Parameters:]{.paramLabel}
            :   `initialNodes` - The nodes from which to perform the
                traversal. Not allowed to contain `null`.
            :   `shouldExploreChildren` - Whether or not to explore a
                particular node\'s children. Used to support short
                circuiting in the traversal.

            [Throws:]{.throwsLabel}
            :   `CycleException` - if a cycle is found while performing
                the traversal.
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
