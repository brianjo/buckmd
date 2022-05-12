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

## Class DirectedAcyclicGraph\<T\> {#class-directedacyclicgrapht .title title="Class DirectedAcyclicGraph"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.util.graph.DirectedAcyclicGraph\<T\>

::: description
-   

    All Implemented Interfaces:
    :   `TraversableGraph<T>`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `MergedTargetGraph`, `TargetGraph`

    ------------------------------------------------------------------------

        public class DirectedAcyclicGraph<T>
        extends Object
        implements TraversableGraph<T>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                             Description
          ------------------------------------------------------- -------------
          `DirectedAcyclicGraph​(MutableDirectedGraph<T> graph)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                       Method                            Description
          ------------------------------------------------------- --------------------------------- -------------
          `boolean`                                               `equals​(Object other)`             
          `com.google.common.collect.ImmutableSet<T>`             `getIncomingNodesFor​(T sink)`      
          `com.google.common.collect.ImmutableSet<T>`             `getNodes()`                       
          `com.google.common.collect.ImmutableSet<T>`             `getNodesWithNoIncomingEdges()`    
          `com.google.common.collect.ImmutableSet<T>`             `getNodesWithNoOutgoingEdges()`    
          `com.google.common.collect.ImmutableSetMultimap<T,​T>`   `getOutgoingEdges()`               
          `com.google.common.collect.ImmutableSet<T>`             `getOutgoingNodesFor​(T source)`    
          `int`                                                   `hashCode()`                       

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.util.graph.MutableDirectedGraph)}

        -   #### DirectedAcyclicGraph

                public DirectedAcyclicGraph​(MutableDirectedGraph<T> graph)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getOutgoingNodesFor(java.lang.Object)}
        []{#getOutgoingNodesFor(T)}

        -   #### getOutgoingNodesFor

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<T> getOutgoingNodesFor​(T source)
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
            public com.google.common.collect.ImmutableSet<T> getIncomingNodesFor​(T sink)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getIncomingNodesFor` in interface `TraversableGraph<T>`

            [Returns:]{.returnLabel}
            :   [`Iterable`](http://docs.oracle.com/javase/7/docs/api/java/lang/Iterable.html?is-external=true "class or interface in java.lang"){.externalLink}
                that the caller is not allowed to mutate.

        []{#getNodesWithNoOutgoingEdges()}

        -   #### getNodesWithNoOutgoingEdges

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<T> getNodesWithNoOutgoingEdges()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNodesWithNoOutgoingEdges` in
                interface `TraversableGraph<T>`

            [Returns:]{.returnLabel}
            :   [`Iterable`](http://docs.oracle.com/javase/7/docs/api/java/lang/Iterable.html?is-external=true "class or interface in java.lang"){.externalLink}
                that the caller is not allowed to mutate.

        []{#getNodesWithNoIncomingEdges()}

        -   #### getNodesWithNoIncomingEdges

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<T> getNodesWithNoIncomingEdges()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNodesWithNoIncomingEdges` in
                interface `TraversableGraph<T>`

            [Returns:]{.returnLabel}
            :   [`Iterable`](http://docs.oracle.com/javase/7/docs/api/java/lang/Iterable.html?is-external=true "class or interface in java.lang"){.externalLink}
                that the caller is not allowed to mutate.

        []{#getNodes()}

        -   #### getNodes

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<T> getNodes()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNodes` in interface `TraversableGraph<T>`

            [Returns:]{.returnLabel}
            :   an unmodifiable view of the nodes in this graph

        []{#getOutgoingEdges()}

        -   #### getOutgoingEdges

            ``` methodSignature
            public com.google.common.collect.ImmutableSetMultimap<T,​T> getOutgoingEdges()
            ```

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object other)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`
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
