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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.util](package-summary.html)
:::

## Class MoreIterables {#class-moreiterables .title title="Class MoreIterables"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.MoreIterables

::: description
-   

    ------------------------------------------------------------------------

        public class MoreIterables
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static <T> Set<T>`   | `dedupKeepLast​(       | ::: block             |
        |                       | Iterable<T> toDedup)` | Returns a deduped     |
        |                       |                       | version of toDedup    |
        |                       |                       | and keeps the order   |
        |                       |                       | of elements If a key  |
        |                       |                       | is contained more     |
        |                       |                       | than once (that is,   |
        |                       |                       | there are multiple    |
        |                       |                       | elements e1, e2\...   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static <T> Itera     | `enumerat             |                       |
        | ble<Pair<Integer,​T>>` | e​(Iterable<T> items)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <L,​R>void`    | `forEac               | ::: block             |
        |                       | hPair​(Iterable<L> lef | Provides convenient   |
        |                       | t,            Iterabl | consumption of a pair |
        |                       | e<R> right,           | of Iterables of the   |
        |                       |   java.util.function. | same length.          |
        |                       | BiConsumer<? super L, | :::                   |
        |                       | ​? super R> consumer)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `zipAndConcat​(It      | ::: block             |
        | atic <T> Iterable<T>` | erable<T>... inputs)` | Combine the given     |
        |                       |                       | iterables by peeling  |
        |                       |                       | off items one at a    |
        |                       |                       | time from each of the |
        |                       |                       | input iterables until |
        |                       |                       | any one of the        |
        |                       |                       | iterables are         |
        |                       |                       | exhausted.            |
        |                       |                       | :::                   |
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

        []{#zipAndConcat(java.lang.Iterable...)}

        -   #### zipAndConcat

            ``` methodSignature
            @SafeVarargs
            public static <T> Iterable<T> zipAndConcat​(Iterable<T>... inputs)
            ```

            ::: block
            Combine the given iterables by peeling off items one at a
            time from each of the input iterables until any one of the
            iterables are exhausted.
            :::

        []{#forEachPair(java.lang.Iterable,java.lang.Iterable,java.util.function.BiConsumer)}

        -   #### forEachPair

            ``` methodSignature
            public static <L,​R> void forEachPair​(Iterable<L> left,
                                                       Iterable<R> right,
                                                       java.util.function.BiConsumer<? super L,​? super R> consumer)
            ```

            ::: block
            Provides convenient consumption of a pair of Iterables of
            the same length.
            :::

        []{#dedupKeepLast(java.lang.Iterable)}

        -   #### dedupKeepLast

            ``` methodSignature
            public static <T> Set<T> dedupKeepLast​(Iterable<T> toDedup)
            ```

            ::: block
            Returns a deduped version of toDedup and keeps the order of
            elements If a key is contained more than once (that is,
            there are multiple elements e1, e2\... en, such that
            ei.equals(ej)) then the last one will be kept in the
            ordering
            :::

        []{#enumerate(java.lang.Iterable)}

        -   #### enumerate

            ``` methodSignature
            public static <T> Iterable<Pair<Integer,​T>> enumerate​(Iterable<T> items)
            ```

            [Returns:]{.returnLabel}
            :   a new
                [`Iterable`](http://docs.oracle.com/javase/7/docs/api/java/lang/Iterable.html?is-external=true "class or interface in java.lang"){.externalLink}
                containing pairs of the original items along with the
                index of the current item.
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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
