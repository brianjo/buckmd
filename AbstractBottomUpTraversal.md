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

## Class AbstractBottomUpTraversal\<T,​E extends [Throwable](http://docs.oracle.com/javase/7/docs/api/java/lang/Throwable.html?is-external=true "class or interface in java.lang"){.externalLink}\> {#class-abstractbottomuptraversalte-extends-throwable .title title="Class AbstractBottomUpTraversal"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.util.graph.AbstractBottomUpTraversal\<T,​E\>

::: description
-   

    ------------------------------------------------------------------------

        public abstract class AbstractBottomUpTraversal<T,​E extends Throwable>
        extends Object

    ::: block
    Class that performs a \"bottom-up\" traversal of a DAG. For any
    given node, every node to which it has an outgoing edge will be
    visited before the given node.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                              Description
          -------------------------------------------------------- -------------
          `AbstractBottomUpTraversal​(TraversableGraph<T> graph)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `traverse()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `t                    | ::: block             |
        |                       | raverse​(java.util.fun | Perform the           |
        |                       | ction.Predicate<T> sh | traversal.            |
        |                       | ouldExploreChildren)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract void`       | `visit​(T node)`       |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
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

        []{#<init>(com.facebook.buck.core.util.graph.TraversableGraph)}

        -   #### AbstractBottomUpTraversal

                public AbstractBottomUpTraversal​(TraversableGraph<T> graph)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#traverse()}

        -   #### traverse

            ``` methodSignature
            public final void traverse()
                                throws E extends Throwable
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Throwable`

        []{#traverse(java.util.function.Predicate)}

        -   #### traverse

            ``` methodSignature
            public final void traverse​(java.util.function.Predicate<T> shouldExploreChildren)
                                throws E extends Throwable
            ```

            ::: block
            Perform the traversal.
            :::

            [Parameters:]{.paramLabel}
            :   `shouldExploreChildren` - Whether or not to explore a
                particular node\'s children. Used to support short
                circuiting in the traversal.

            [Throws:]{.throwsLabel}
            :   `E`
            :   `E extends Throwable`

        []{#visit(java.lang.Object)} []{#visit(T)}

        -   #### visit

            ``` methodSignature
            public abstract void visit​(T node)
                                throws E extends Throwable
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Throwable`
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
