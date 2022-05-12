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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.model.targetgraph.impl](package-summary.html)
:::

## Class TargetNodes {#class-targetnodes .title title="Class TargetNodes"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.model.targetgraph.impl.TargetNodes

::: description
-   

    ------------------------------------------------------------------------

        public class TargetNodes
        extends Object

    ::: block
    Utility class to work with
    [`TargetNode`](../TargetNode.html "interface in com.facebook.buck.core.model.targetgraph")
    objects.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static <V exten      | `castArg              | ::: block             |
        | ds ConstructorArg>Opt | ​(TargetNode<?> node,  | Type safe checked     |
        | ional<TargetNode<V>>` |        Class<V> cls)` | cast of the           |
        |                       |                       | constructor arg.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `                     | ::: block             |
        | atic com.google.commo | getTestTargetsForNode | If `node` refers to a |
        | n.collect.ImmutableSo | ​(TargetNode<?> node)` | node which contains   |
        | rtedSet<BuildTarget>` |                       | references to its     |
        |                       |                       | tests, returns the    |
        |                       |                       | tests associated with |
        |                       |                       | that node.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static com.google    | `getTestTarge         |                       |
        | .common.collect.Immut | tsForNodes​(Iterator<T |                       |
        | ableSet<BuildTarget>` | argetNode<?>> nodes)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getTestTargetsForNode(com.facebook.buck.core.model.targetgraph.TargetNode)}

        -   #### getTestTargetsForNode

            ``` methodSignature
            public static com.google.common.collect.ImmutableSortedSet<BuildTarget> getTestTargetsForNode​(TargetNode<?> node)
            ```

            ::: block
            If `node` refers to a node which contains references to its
            tests, returns the tests associated with that node.
            Otherwise, returns an empty set.
            :::

        []{#getTestTargetsForNodes(java.util.Iterator)}

        -   #### getTestTargetsForNodes

            ``` methodSignature
            public static com.google.common.collect.ImmutableSet<BuildTarget> getTestTargetsForNodes​(Iterator<TargetNode<?>> nodes)
            ```

            [Parameters:]{.paramLabel}
            :   `nodes` - Nodes whose test targets we would like to find

            [Returns:]{.returnLabel}
            :   A set of all test targets that test the targets in
                `nodes`.

        []{#castArg(com.facebook.buck.core.model.targetgraph.TargetNode,java.lang.Class)}

        -   #### castArg

            ``` methodSignature
            public static <V extends ConstructorArg> Optional<TargetNode<V>> castArg​(TargetNode<?> node,
                                                                                     Class<V> cls)
            ```

            ::: block
            Type safe checked cast of the constructor arg.
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
