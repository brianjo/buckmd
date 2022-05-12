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

## Class AbstractBreadthFirstTraversal\<Node\> {#class-abstractbreadthfirsttraversalnode .title title="Class AbstractBreadthFirstTraversal"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.util.graph.AbstractBreadthFirstThrowingTraversal](AbstractBreadthFirstThrowingTraversal.html "class in com.facebook.buck.core.util.graph")\<Node,​[RuntimeException](http://docs.oracle.com/javase/7/docs/api/java/lang/RuntimeException.html?is-external=true "class or interface in java.lang"){.externalLink}\>

    -   -   com.facebook.buck.core.util.graph.AbstractBreadthFirstTraversal\<Node\>

::: description
-   

    ------------------------------------------------------------------------

        public abstract class AbstractBreadthFirstTraversal<Node>
        extends AbstractBreadthFirstThrowingTraversal<Node,​RuntimeException>

    ::: block
    Performs a breadth-first traversal of dependencies of a graph node.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.core.util.graph.AbstractBreadthFirstThrowingTraversal}

            ### Nested classes/interfaces inherited from class com.facebook.buck.core.util.graph.[AbstractBreadthFirstThrowingTraversal](AbstractBreadthFirstThrowingTraversal.html "class in com.facebook.buck.core.util.graph")

            `AbstractBreadthFirstThrowingTraversal.StaticBreadthFirstTraversal<Node>, AbstractBreadthFirstThrowingTraversal.Visitor<Node,​E extends Throwable>`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                              Description
          ------------------------------------------------------------------------ -------------
          `AbstractBreadthFirstTraversal​(Iterable<? extends Node> initialNodes)`    
          `AbstractBreadthFirstTraversal​(Node initialNode)`                         

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static <Node> void`  | `traverse             | ::: block             |
        |                       | ​(Iterable<? extends N | Traverse a graph      |
        |                       | ode> initialNodes,    | without explicitly    |
        |                       |       AbstractBreadth | creating a            |
        |                       | FirstThrowingTraversa | `n                    |
        |                       | l.Visitor<Node,​Runtim | ew  AbstractBreadthFi |
        |                       | eException> visitor)` | rstThrowingTraversal` |
        |                       |                       | and overriding        |
        |                       |                       | [`Abst                |
        |                       |                       | ractBreadthFirstThrow |
        |                       |                       | ingTraversal.visit(Ob |
        |                       |                       | ject)`](AbstractBread |
        |                       |                       | thFirstThrowingTraver |
        |                       |                       | sal.html#visit(Node)) |
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
        |                       |                       | [`Abst                |
        |                       |                       | ractBreadthFirstThrow |
        |                       |                       | ingTraversal.visit(Ob |
        |                       |                       | ject)`](AbstractBread |
        |                       |                       | thFirstThrowingTraver |
        |                       |                       | sal.html#visit(Node)) |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.util.graph.AbstractBreadthFirstThrowingTraversal}

            ### Methods inherited from class com.facebook.buck.core.util.graph.[AbstractBreadthFirstThrowingTraversal](AbstractBreadthFirstThrowingTraversal.html "class in com.facebook.buck.core.util.graph")

            `onComplete, start, visit`

        ```{=html}
        <!-- -->
        ```
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

        -   #### AbstractBreadthFirstTraversal

                public AbstractBreadthFirstTraversal​(Node initialNode)

        []{#<init>(java.lang.Iterable)}

        -   #### AbstractBreadthFirstTraversal

                public AbstractBreadthFirstTraversal​(Iterable<? extends Node> initialNodes)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

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
            [`AbstractBreadthFirstThrowingTraversal.visit(Object)`](AbstractBreadthFirstThrowingTraversal.html#visit(Node))
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
            [`AbstractBreadthFirstThrowingTraversal.visit(Object)`](AbstractBreadthFirstThrowingTraversal.html#visit(Node))
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
