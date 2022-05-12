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
-   [Nested](#nested.class.summary) \| 
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

## Class AbstractBreadthFirstThrowingTraversal\<Node,​E extends [Throwable](http://docs.oracle.com/javase/7/docs/api/java/lang/Throwable.html?is-external=true "class or interface in java.lang"){.externalLink}\> {#class-abstractbreadthfirstthrowingtraversalnodee-extends-throwable .title title="Class AbstractBreadthFirstThrowingTraversal"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.util.graph.AbstractBreadthFirstThrowingTraversal\<Node,​E\>

::: description
-   

    Direct Known Subclasses:
    :   `AbstractBreadthFirstThrowingTraversal.StaticBreadthFirstTraversal`,
        `AbstractBreadthFirstTraversal`

    ------------------------------------------------------------------------

        public abstract class AbstractBreadthFirstThrowingTraversal<Node,​E extends Throwable>
        extends Object

    ::: block
    Performs a breadth-first traversal of dependencies of a graph node.
    In cases where the cost of allocating
    [`Iterable`](http://docs.oracle.com/javase/7/docs/api/java/lang/Iterable.html?is-external=true "class or interface in java.lang"){.externalLink}s
    for node dependencies is expensive/costly,
    [`ConsumingTraverser.breadthFirst(Iterable, ForEachSuccessorFunction)`](ConsumingTraverser.html#breadthFirst(java.lang.Iterable,com.facebook.buck.core.util.graph.ForEachSuccessorFunction))
    provides a lighter-weight option.

    TODO: Implement via
    [`ConsumingTraverser`](ConsumingTraverser.html "class in com.facebook.buck.core.util.graph").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `pro                  | `AbstractB            |                       |
        | tected static class ` | readthFirstThrowingTr |                       |
        |                       | aversal.StaticBreadth |                       |
        |                       | FirstTraversal<Node>` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static interface `   | `AbstractB            | ::: block             |
        |                       | readthFirstThrowingTr | This will typically   |
        |                       | aversal.Visitor<Node, | be implemented as a   |
        |                       | ​E extends Throwable>` | lambda passed to      |
        |                       |                       | [`traverse(Object, Vi |
        |                       |                       | sitor)`](#traverse(No |
        |                       |                       | de,com.facebook.buck. |
        |                       |                       | core.util.graph.Abstr |
        |                       |                       | actBreadthFirstThrowi |
        |                       |                       | ngTraversal.Visitor)) |
        |                       |                       | or                    |
        |                       |                       | [`traverse(Itera      |
        |                       |                       | ble, Visitor)`](#trav |
        |                       |                       | erse(java.lang.Iterab |
        |                       |                       | le,com.facebook.buck. |
        |                       |                       | core.util.graph.Abstr |
        |                       |                       | actBreadthFirstThrowi |
        |                       |                       | ngTraversal.Visitor)) |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                      Description
          -------------------------------------------------------------------------------- -------------
          `AbstractBreadthFirstThrowingTraversal​(Iterable<? extends Node> initialNodes)`    
          `AbstractBreadthFirstThrowingTraversal​(Node initialNode)`                         

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected void`      | `onComplete()`        | ::: block             |
        |                       |                       | Override this method  |
        |                       |                       | with any logic that   |
        |                       |                       | should be run when    |
        |                       |                       | [`start()`](#start()) |
        |                       |                       | completes.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `start()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <Node> void`  | `traverse             | ::: block             |
        |                       | ​(Iterable<? extends N | Traverse a graph      |
        |                       | ode> initialNodes,    | without explicitly    |
        |                       |       AbstractBreadth | creating a            |
        |                       | FirstThrowingTraversa | `n                    |
        |                       | l.Visitor<Node,​Runtim | ew  AbstractBreadthFi |
        |                       | eException> visitor)` | rstThrowingTraversal` |
        |                       |                       | and overriding        |
        |                       |                       | [`visit(Ob            |
        |                       |                       | ject)`](#visit(Node)) |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static <Node> void`  | `traverse             | ::: block             |
        |                       | ​(Node initialNode,    | Traverse a graph      |
        |                       |       AbstractBreadth | without explicitly    |
        |                       | FirstThrowingTraversa | creating a            |
        |                       | l.Visitor<Node,​Runtim | `n                    |
        |                       | eException> visitor)` | ew  AbstractBreadthFi |
        |                       |                       | rstThrowingTraversal` |
        |                       |                       | and overriding        |
        |                       |                       | [`visit(Ob            |
        |                       |                       | ject)`](#visit(Node)) |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Iter        | `visit​(Node node)`    | ::: block             |
        | able<? extends Node>` |                       | To perform a full     |
        |                       |                       | traversal of the the  |
        |                       |                       | `initialNode`\'s      |
        |                       |                       | transitive            |
        |                       |                       | dependencies, this    |
        |                       |                       | function should       |
        |                       |                       | return all of         |
        |                       |                       | `node`\'s direct      |
        |                       |                       | dependencies.         |
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

        []{#<init>(java.lang.Object)} []{#<init>(Node)}

        -   #### AbstractBreadthFirstThrowingTraversal

                public AbstractBreadthFirstThrowingTraversal​(Node initialNode)

        []{#<init>(java.lang.Iterable)}

        -   #### AbstractBreadthFirstThrowingTraversal

                public AbstractBreadthFirstThrowingTraversal​(Iterable<? extends Node> initialNodes)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#start()}

        -   #### start

            ``` methodSignature
            public final void start()
                             throws E extends Throwable
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Throwable`

        []{#onComplete()}

        -   #### onComplete

            ``` methodSignature
            protected void onComplete()
                               throws E extends Throwable
            ```

            ::: block
            Override this method with any logic that should be run when
            [`start()`](#start()) completes.
            :::

            [Throws:]{.throwsLabel}
            :   `E extends Throwable`

        []{#visit(java.lang.Object)} []{#visit(Node)}

        -   #### visit

            ``` methodSignature
            public abstract Iterable<? extends Node> visit​(Node node)
                                                    throws E extends Throwable
            ```

            ::: block
            To perform a full traversal of the the `initialNode`\'s
            transitive dependencies, this function should return all of
            `node`\'s direct dependencies.
            :::

            [Parameters:]{.paramLabel}
            :   `node` - Visited graph node

            [Returns:]{.returnLabel}
            :   The set of direct dependencies to visit after visiting
                this node.

            [Throws:]{.throwsLabel}
            :   `E extends Throwable`

        []{#traverse(java.lang.Object,com.facebook.buck.core.util.graph.AbstractBreadthFirstThrowingTraversal.Visitor)}
        []{#traverse(Node,com.facebook.buck.core.util.graph.AbstractBreadthFirstThrowingTraversal.Visitor)}

        -   #### traverse

            ``` methodSignature
            public static <Node> void traverse​(Node initialNode,
                                               AbstractBreadthFirstThrowingTraversal.Visitor<Node,​RuntimeException> visitor)
            ```

            ::: block
            Traverse a graph without explicitly creating a
            `new  AbstractBreadthFirstThrowingTraversal` and overriding
            [`visit(Object)`](#visit(Node))
            :::

            [Parameters:]{.paramLabel}
            :   `visitor` - Typically a lambda expression

        []{#traverse(java.lang.Iterable,com.facebook.buck.core.util.graph.AbstractBreadthFirstThrowingTraversal.Visitor)}

        -   #### traverse

            ``` methodSignature
            public static <Node> void traverse​(Iterable<? extends Node> initialNodes,
                                               AbstractBreadthFirstThrowingTraversal.Visitor<Node,​RuntimeException> visitor)
            ```

            ::: block
            Traverse a graph without explicitly creating a
            `new  AbstractBreadthFirstThrowingTraversal` and overriding
            [`visit(Object)`](#visit(Node))
            :::

            [Parameters:]{.paramLabel}
            :   `visitor` - Typically a lambda expression
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
-   [Nested](#nested.class.summary) \| 
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
