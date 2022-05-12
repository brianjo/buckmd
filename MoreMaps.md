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

## Class MoreMaps {#class-moremaps .title title="Class MoreMaps"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.MoreMaps

::: description
-   

    ------------------------------------------------------------------------

        public class MoreMaps
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static <K extends Co | `con                  |                       |
        | mparable<?>,​V>com.goo | vertMultimapToMapOfLi |                       |
        | gle.common.collect.Im | sts​(com.google.common |                       |
        | mutableSortedMap<K,​co | .collect.ImmutableMul |                       |
        | m.google.common.colle | timap<K,​V> multimap)` |                       |
        | ct.ImmutableList<V>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <K,​V>co       | `f                    | ::: block             |
        | m.google.common.colle | ilterValues​(Map<K,​V>  | Version of            |
        | ct.ImmutableMap<K,​V>` | unfiltered,           | `Maps.filterVa        |
        |                       |    com.google.common. | lues(Map, Predicate)` |
        |                       | base.Predicate<? supe | that collects the     |
        |                       | r V> valuePredicate)` | results in an         |
        |                       |                       | immutable map.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static <K,​V>co       | `me                   |                       |
        | m.google.common.colle | rge​(Map<K,​V> first,   |                       |
        | ct.ImmutableMap<K,​V>` |     Map<K,​V> second)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <K,​V>com.goog | `mergeSorted​(Ma       |                       |
        | le.common.collect.Imm | p<K,​V> first,         |                       |
        | utableSortedMap<K,​V>` |     Map<K,​V> second)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `putCheckEq           |                       |
        | static <K,​V>Map<K,​V>` | uals​(Map<K,​V> map,    |                       |
        |                       |             K key,    |                       |
        |                       |             V value)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `pu                   | ::: block             |
        | static <K,​V>Map<K,​V>` | tIfAbsentCheckEquals​( | Inserts the given     |
        |                       | ConcurrentMap<K,​V> ma | value if nothing was  |
        |                       | p,                    | already set for the   |
        |                       |     K key,            | key.                  |
        |                       |             V value)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static <K1,​K2,​V>com  | `transformKeys​(       | ::: block             |
        | .google.common.collec | Map<K1,​V> map,        | Transform a map to    |
        | t.ImmutableMap<K2,​V>` |        java.util.func | another immutable map |
        |                       | tion.Function<? super | by changing keys and  |
        |                       |  K1,​K2> transformer)` | keeping values        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `stati                | `transfo              |                       |
        | c <K1,​K2 extends Comp | rmKeysAndSort​(Map<K1, |                       |
        | arable<?>,​V>com.googl | ​V> map,               |                       |
        | e.common.collect.Immu |        java.util.func |                       |
        | tableSortedMap<K2,​V>` | tion.Function<? super |                       |
        |                       |  K1,​K2> transformer)` |                       |
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

        []{#putCheckEquals(java.util.Map,java.lang.Object,java.lang.Object)}
        []{#putCheckEquals(java.util.Map,K,V)}

        -   #### putCheckEquals

            ``` methodSignature
            public static <K,​V> Map<K,​V> putCheckEquals​(Map<K,​V> map,
                                                                    K key,
                                                                    @Nullable
                                                                    V value)
            ```

        []{#putIfAbsentCheckEquals(java.util.concurrent.ConcurrentMap,java.lang.Object,java.lang.Object)}
        []{#putIfAbsentCheckEquals(java.util.concurrent.ConcurrentMap,K,V)}

        -   #### putIfAbsentCheckEquals

            ``` methodSignature
            public static <K,​V> Map<K,​V> putIfAbsentCheckEquals​(ConcurrentMap<K,​V> map,
                                                                            K key,
                                                                            @Nullable
                                                                            V value)
            ```

            ::: block
            Inserts the given value if nothing was already set for the
            key. If a value already existed for this key, ensures it is
            the same as the one being inserted, otherwise throws an
            IllegalStateException.
            :::

        []{#transformKeys(java.util.Map,java.util.function.Function)}

        -   #### transformKeys

            ``` methodSignature
            public static <K1,​K2,​V> com.google.common.collect.ImmutableMap<K2,​V> transformKeys​(Map<K1,​V> map,
                                                                                                                 java.util.function.Function<? super K1,​K2> transformer)
            ```

            ::: block
            Transform a map to another immutable map by changing keys
            and keeping values
            :::

            [Parameters:]{.paramLabel}
            :   `map` - Source map to transform
            :   `transformer` - Function to apply to source map key to
                infer resulting map key

            [Returns:]{.returnLabel}
            :   New immutable map with new keys and corresponding values

        []{#transformKeysAndSort(java.util.Map,java.util.function.Function)}

        -   #### transformKeysAndSort

            ``` methodSignature
            public static <K1,​K2 extends Comparable<?>,​V> com.google.common.collect.ImmutableSortedMap<K2,​V> transformKeysAndSort​(Map<K1,​V> map,
                                                                                                                                                    java.util.function.Function<? super K1,​K2> transformer)
            ```

        []{#merge(java.util.Map,java.util.Map)}

        -   #### merge

            ``` methodSignature
            public static <K,​V> com.google.common.collect.ImmutableMap<K,​V> merge​(Map<K,​V> first,
                                                                                              Map<K,​V> second)
            ```

        []{#mergeSorted(java.util.Map,java.util.Map)}

        -   #### mergeSorted

            ``` methodSignature
            public static <K,​V> com.google.common.collect.ImmutableSortedMap<K,​V> mergeSorted​(Map<K,​V> first,
                                                                                                          Map<K,​V> second)
            ```

        []{#convertMultimapToMapOfLists(com.google.common.collect.ImmutableMultimap)}

        -   #### convertMultimapToMapOfLists

            ``` methodSignature
            public static <K extends Comparable<?>,​V> com.google.common.collect.ImmutableSortedMap<K,​com.google.common.collect.ImmutableList<V>> convertMultimapToMapOfLists​(com.google.common.collect.ImmutableMultimap<K,​V> multimap)
            ```

        []{#filterValues(java.util.Map,com.google.common.base.Predicate)}

        -   #### filterValues

            ``` methodSignature
            public static <K,​V> com.google.common.collect.ImmutableMap<K,​V> filterValues​(Map<K,​V> unfiltered,
                                                                                                     com.google.common.base.Predicate<? super V> valuePredicate)
            ```

            ::: block
            Version of `Maps.filterValues(Map, Predicate)` that collects
            the results in an immutable map.
            :::

            [See Also:]{.seeLabel}
            :   `Maps.filterValues(Map, Predicate)`
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
