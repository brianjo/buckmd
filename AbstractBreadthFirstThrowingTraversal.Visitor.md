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

## Interface AbstractBreadthFirstThrowingTraversal.Visitor\<Node,​E extends [Throwable](http://docs.oracle.com/javase/7/docs/api/java/lang/Throwable.html?is-external=true "class or interface in java.lang"){.externalLink}\> {#interface-abstractbreadthfirstthrowingtraversal.visitornodee-extends-throwable .title title="Interface AbstractBreadthFirstThrowingTraversal.Visitor"}
:::

::: contentContainer
::: description
-   

    Enclosing class:
    :   [AbstractBreadthFirstThrowingTraversal](AbstractBreadthFirstThrowingTraversal.html "class in com.facebook.buck.core.util.graph")\<[Node](AbstractBreadthFirstThrowingTraversal.html "type parameter in AbstractBreadthFirstThrowingTraversal"),​[E](AbstractBreadthFirstThrowingTraversal.html "type parameter in AbstractBreadthFirstThrowingTraversal")
        extends
        [Throwable](http://docs.oracle.com/javase/7/docs/api/java/lang/Throwable.html?is-external=true "class or interface in java.lang"){.externalLink}\>

    ------------------------------------------------------------------------

        public static interface AbstractBreadthFirstThrowingTraversal.Visitor<Node,​E extends Throwable>

    ::: block
    This will typically be implemented as a lambda passed to
    [`AbstractBreadthFirstThrowingTraversal.traverse(Object, Visitor)`](AbstractBreadthFirstThrowingTraversal.html#traverse(Node,com.facebook.buck.core.util.graph.AbstractBreadthFirstThrowingTraversal.Visitor))
    or
    [`AbstractBreadthFirstThrowingTraversal.traverse(Iterable, Visitor)`](AbstractBreadthFirstThrowingTraversal.html#traverse(java.lang.Iterable,com.facebook.buck.core.util.graph.AbstractBreadthFirstThrowingTraversal.Visitor))
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method               Description
          ------------------- -------------------- -------------
          `Iterable<Node>`    `visit​(Node node)`    

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

        []{#visit(java.lang.Object)} []{#visit(Node)}

        -   #### visit

            ``` methodSignature
            Iterable<Node> visit​(Node node)
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
