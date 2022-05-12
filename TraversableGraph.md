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
[Package]{.packageLabelInType} [com.facebook.buck.core.util.graph](package-summary.html)
:::

## Interface TraversableGraph\<T\> {#interface-traversablegrapht .title title="Interface TraversableGraph"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `DirectedAcyclicGraph`, `MergedTargetGraph`,
        `MutableDirectedGraph`, `TargetGraph`, `VersionedTargetGraph`

    ------------------------------------------------------------------------

        public interface TraversableGraph<T>

    ::: block
    Minimal interface needed by
    [`AbstractBottomUpTraversal`](AbstractBottomUpTraversal.html "class in com.facebook.buck.core.util.graph")
    to traverse a graph.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                            Description
          ------------------- --------------------------------- -------------
          `Iterable<T>`       `getIncomingNodesFor​(T sink)`      
          `Iterable<T>`       `getNodes()`                       
          `Iterable<T>`       `getNodesWithNoIncomingEdges()`    
          `Iterable<T>`       `getNodesWithNoOutgoingEdges()`    
          `Iterable<T>`       `getOutgoingNodesFor​(T source)`    

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

        []{#getNodesWithNoIncomingEdges()}

        -   #### getNodesWithNoIncomingEdges

            ``` methodSignature
            Iterable<T> getNodesWithNoIncomingEdges()
            ```

            [Returns:]{.returnLabel}
            :   [`Iterable`](http://docs.oracle.com/javase/7/docs/api/java/lang/Iterable.html?is-external=true "class or interface in java.lang"){.externalLink}
                that the caller is not allowed to mutate.

        []{#getNodesWithNoOutgoingEdges()}

        -   #### getNodesWithNoOutgoingEdges

            ``` methodSignature
            Iterable<T> getNodesWithNoOutgoingEdges()
            ```

            [Returns:]{.returnLabel}
            :   [`Iterable`](http://docs.oracle.com/javase/7/docs/api/java/lang/Iterable.html?is-external=true "class or interface in java.lang"){.externalLink}
                that the caller is not allowed to mutate.

        []{#getIncomingNodesFor(java.lang.Object)}
        []{#getIncomingNodesFor(T)}

        -   #### getIncomingNodesFor

            ``` methodSignature
            Iterable<T> getIncomingNodesFor​(T sink)
            ```

            [Returns:]{.returnLabel}
            :   [`Iterable`](http://docs.oracle.com/javase/7/docs/api/java/lang/Iterable.html?is-external=true "class or interface in java.lang"){.externalLink}
                that the caller is not allowed to mutate.

        []{#getOutgoingNodesFor(java.lang.Object)}
        []{#getOutgoingNodesFor(T)}

        -   #### getOutgoingNodesFor

            ``` methodSignature
            Iterable<T> getOutgoingNodesFor​(T source)
            ```

            [Returns:]{.returnLabel}
            :   [`Iterable`](http://docs.oracle.com/javase/7/docs/api/java/lang/Iterable.html?is-external=true "class or interface in java.lang"){.externalLink}
                that the caller is not allowed to mutate.

        []{#getNodes()}

        -   #### getNodes

            ``` methodSignature
            Iterable<T> getNodes()
            ```

            [Returns:]{.returnLabel}
            :   an unmodifiable view of the nodes in this graph
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
