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

## Class AbstractBreadthFirstThrowingTraversal.StaticBreadthFirstTraversal\<Node\> {#class-abstractbreadthfirstthrowingtraversal.staticbreadthfirsttraversalnode .title title="Class AbstractBreadthFirstThrowingTraversal.StaticBreadthFirstTraversal"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.util.graph.AbstractBreadthFirstThrowingTraversal](AbstractBreadthFirstThrowingTraversal.html "class in com.facebook.buck.core.util.graph")\<Node,​[RuntimeException](http://docs.oracle.com/javase/7/docs/api/java/lang/RuntimeException.html?is-external=true "class or interface in java.lang"){.externalLink}\>

    -   -   com.facebook.buck.core.util.graph.AbstractBreadthFirstThrowingTraversal.StaticBreadthFirstTraversal\<Node\>

::: description
-   

    Enclosing class:
    :   [AbstractBreadthFirstThrowingTraversal](AbstractBreadthFirstThrowingTraversal.html "class in com.facebook.buck.core.util.graph")\<[Node](AbstractBreadthFirstThrowingTraversal.html "type parameter in AbstractBreadthFirstThrowingTraversal"),​[E](AbstractBreadthFirstThrowingTraversal.html "type parameter in AbstractBreadthFirstThrowingTraversal")
        extends
        [Throwable](http://docs.oracle.com/javase/7/docs/api/java/lang/Throwable.html?is-external=true "class or interface in java.lang"){.externalLink}\>

    ------------------------------------------------------------------------

        protected static class AbstractBreadthFirstThrowingTraversal.StaticBreadthFirstTraversal<Node>
        extends AbstractBreadthFirstThrowingTraversal<Node,​RuntimeException>
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

          Modifier       Constructor                                                                                                                                                                     Description
          -------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `protected `   `StaticBreadthFirstTraversal​(Iterable<? extends Node> initialNodes,                            AbstractBreadthFirstThrowingTraversal.Visitor<Node,​RuntimeException> visitor)`    
          `protected `   `StaticBreadthFirstTraversal​(Node initialNode,                            AbstractBreadthFirstThrowingTraversal.Visitor<Node,​RuntimeException> visitor)`                         

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Iterable<Node>`      | `visit​(Node node)`    | ::: block             |
        |                       |                       | To perform a full     |
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

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.util.graph.AbstractBreadthFirstThrowingTraversal}

            ### Methods inherited from class com.facebook.buck.core.util.graph.[AbstractBreadthFirstThrowingTraversal](AbstractBreadthFirstThrowingTraversal.html "class in com.facebook.buck.core.util.graph")

            `onComplete, start, traverse, traverse`

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

        []{#<init>(java.lang.Object,com.facebook.buck.core.util.graph.AbstractBreadthFirstThrowingTraversal.Visitor)}
        []{#<init>(Node,com.facebook.buck.core.util.graph.AbstractBreadthFirstThrowingTraversal.Visitor)}

        -   #### StaticBreadthFirstTraversal

                protected StaticBreadthFirstTraversal​(Node initialNode,
                                                      AbstractBreadthFirstThrowingTraversal.Visitor<Node,​RuntimeException> visitor)

        []{#<init>(java.lang.Iterable,com.facebook.buck.core.util.graph.AbstractBreadthFirstThrowingTraversal.Visitor)}

        -   #### StaticBreadthFirstTraversal

                protected StaticBreadthFirstTraversal​(Iterable<? extends Node> initialNodes,
                                                      AbstractBreadthFirstThrowingTraversal.Visitor<Node,​RuntimeException> visitor)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#visit(java.lang.Object)} []{#visit(Node)}

        -   #### visit

            ``` methodSignature
            public Iterable<Node> visit​(Node node)
                                 throws RuntimeException
            ```

            ::: block
            [Description copied from
            class: `AbstractBreadthFirstThrowingTraversal`]{.descfrmTypeLabel}
            :::

            ::: block
            To perform a full traversal of the the `initialNode`\'s
            transitive dependencies, this function should return all of
            `node`\'s direct dependencies.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `visit` in
                class `AbstractBreadthFirstThrowingTraversal<Node,​RuntimeException>`

            [Parameters:]{.paramLabel}
            :   `node` - Visited graph node

            [Returns:]{.returnLabel}
            :   The set of direct dependencies to visit after visiting
                this node.

            [Throws:]{.throwsLabel}
            :   `RuntimeException`
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
