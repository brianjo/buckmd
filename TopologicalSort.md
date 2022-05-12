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

## Class TopologicalSort {#class-topologicalsort .title title="Class TopologicalSort"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.util.graph.TopologicalSort

::: description
-   

    ------------------------------------------------------------------------

        public class TopologicalSort
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static interface `   | `Topologica           | ::: block             |
        |                       | lSort.Traversable<T>` | User provider         |
        |                       |                       | callback used for     |
        |                       |                       | walking the graph     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `s                    | `snowflakeSort        | ::: block             |
        | tatic <T> com.google. | ​(Iterable<? extends T | [Deprecate            |
        | common.collect.Immuta | > roots,              | d.]{.deprecatedLabel} |
        | bleList<? extends T>` |  TopologicalSort.Trav |                       |
        |                       | ersable<T> traversabl | :                     |
        |                       | e,              Compa | :: deprecationComment |
        |                       | rator<T> comparator)` | This is silly.        |
        |                       |                       | :::                   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static <T> c         | `sort​(Traver          | ::: block             |
        | om.google.common.coll | sableGraph<T> graph)` | Returns a             |
        | ect.ImmutableList<T>` |                       | topologically sorted  |
        |                       |                       | list of the nodes in  |
        |                       |                       | the graph.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `s                    | `sort​(Iterable<? ext  | ::: block             |
        | tatic <T> com.google. | ends T> roots,     To | Returns a             |
        | common.collect.Immuta | pologicalSort.Travers | topologically sorted  |
        | bleList<? extends T>` | able<T> traversable)` | list of all nodes in  |
        |                       |                       | the graph.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4
        .tableTab}[[Deprecated
        Methods](javascript:show(32);)[ ]{.tabEnd}]{#t6 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#sort(com.facebook.buck.core.util.graph.TraversableGraph)}

        -   #### sort

            ``` methodSignature
            public static <T> com.google.common.collect.ImmutableList<T> sort​(TraversableGraph<T> graph)
            ```

            ::: block
            Returns a topologically sorted list of the nodes in the
            graph.
            :::

        []{#sort(java.lang.Iterable,com.facebook.buck.core.util.graph.TopologicalSort.Traversable)}

        -   #### sort

            ``` methodSignature
            public static <T> com.google.common.collect.ImmutableList<? extends T> sort​(Iterable<? extends T> roots,
                                                                                        TopologicalSort.Traversable<T> traversable)
            ```

            ::: block
            Returns a topologically sorted list of all nodes in the
            graph.
            :::

        []{#snowflakeSort(java.lang.Iterable,com.facebook.buck.core.util.graph.TopologicalSort.Traversable,java.util.Comparator)}

        -   #### snowflakeSort

            ``` methodSignature
            @Deprecated
            public static <T> com.google.common.collect.ImmutableList<? extends T> snowflakeSort​(Iterable<? extends T> roots,
                                                                                                 TopologicalSort.Traversable<T> traversable,
                                                                                                 Comparator<T> comparator)
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}

            ::: deprecationComment
            This is silly. You should just use the normal sort. This is
            here because c/c++ link command lines are sensitive to
            argument order, but aren\'t strict about it being correct.
            Since they aren\'t strict, code has evolved to depend on the
            specific order that Buck has been ordering link lines, and
            so this preserves that legacy behavior until code that
            depends on it is fixed.
            :::
            :::

            ::: block
            This special form of topological sort returns items with
            each \"level\" sorted. The algorithm is basically this:
            identify all the leaves of the graph, sort them, add them to
            the list, remove them from the graph and proceed.
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
