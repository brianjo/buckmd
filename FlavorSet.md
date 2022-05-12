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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.model](package-summary.html)
:::

## Class FlavorSet {#class-flavorset .title title="Class FlavorSet"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.model.FlavorSet

::: description
-   

    All Implemented Interfaces:
    :   `Comparable<FlavorSet>`

    ------------------------------------------------------------------------

        public class FlavorSet
        extends Object
        implements Comparable<FlavorSet>

    ::: block
    Set of
    [`Flavor`](Flavor.html "interface in com.facebook.buck.core.model")s.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `static c             | `FLAVOR_ORDERING`     | ::: block             |
        | om.google.common.coll |                       | Flavors passed to     |
        | ect.Ordering<Flavor>` |                       | this object should be |
        |                       |                       | sorted using this     |
        |                       |                       | ordering              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static FlavorSet`    | `NO_FLAVORS`          |                       |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `int`                 | `co                   |                       |
        |                       | mpareTo​(FlavorSet o)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `con                  | ::: block             |
        |                       | tains​(Flavor flavor)` | Does this set contain |
        |                       |                       | given flavor?         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `containsAl           | ::: block             |
        |                       | l​(FlavorSet flavors)` | Does this set contain |
        |                       |                       | all given flavors?    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `containsAll​(Collect  | ::: block             |
        |                       | ion<Flavor> flavors)` | Does this set contain |
        |                       |                       | all given flavors?    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static FlavorSet`    | `copyOf               | ::: block             |
        |                       | ​(com.google.common.co | Constructor.          |
        |                       | llect.ImmutableSorted | :::                   |
        |                       | Set<Flavor> flavors)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static FlavorSet`    | `c                    | ::: block             |
        |                       | opyOf​(Iterable<? exte | Constructor.          |
        |                       | nds Flavor> flavors)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `equals​(Object that)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getSet()`            |                       |
        | common.collect.Immuta |                       |                       |
        | bleSortedSet<Flavor>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isEmpty()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static FlavorSet`    | `o                    |                       |
        |                       | f​(Flavor... flavors)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toCo                 | ::: block             |
        |                       | mmaSeparatedString()` | Just comma separated. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static java.         | `toFlavorSet()`       | ::: block             |
        | util.stream.Collector |                       | Stream collector.     |
        | <Flavor,​?,​FlavorSet>` |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toPostfixString()`   | ::: block             |
        |                       |                       | Flavors list as       |
        |                       |                       | string in the end of  |
        |                       |                       | build target.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static FlavorSet`    | `union​(FlavorSet      | ::: block             |
        |                       | a,      FlavorSet b)` | Return a flavor set   |
        |                       |                       | with flavors in first |
        |                       |                       | or second given set.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `FlavorSet`           | `withAdded​(           | ::: block             |
        |                       | Set<Flavor> flavors)` | Create a flavor set   |
        |                       |                       | with union of this    |
        |                       |                       | and that flavors.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `FlavorSet`           | `without​(             | ::: block             |
        |                       | Set<Flavor> flavors)` | Flavors in this set,  |
        |                       |                       | but not in that set.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#NO_FLAVORS}

        -   #### NO_FLAVORS

                public static final FlavorSet NO_FLAVORS

        []{#FLAVOR_ORDERING}

        -   #### FLAVOR_ORDERING

                public static final com.google.common.collect.Ordering<Flavor> FLAVOR_ORDERING

            ::: block
            Flavors passed to this object should be sorted using this
            ordering
            :::
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#of(com.facebook.buck.core.model.Flavor...)}

        -   #### of

            ``` methodSignature
            public static FlavorSet of​(Flavor... flavors)
            ```

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object that)
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

        []{#compareTo(com.facebook.buck.core.model.FlavorSet)}

        -   #### compareTo

            ``` methodSignature
            public int compareTo​(FlavorSet o)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `compareTo` in interface `Comparable<FlavorSet>`

        []{#getSet()}

        -   #### getSet

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<Flavor> getSet()
            ```

        []{#isEmpty()}

        -   #### isEmpty

            ``` methodSignature
            public boolean isEmpty()
            ```

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#toCommaSeparatedString()}

        -   #### toCommaSeparatedString

            ``` methodSignature
            public String toCommaSeparatedString()
            ```

            ::: block
            Just comma separated.
            :::

        []{#toPostfixString()}

        -   #### toPostfixString

            ``` methodSignature
            public String toPostfixString()
            ```

            ::: block
            Flavors list as string in the end of build target.
            :::

        []{#copyOf(java.lang.Iterable)}

        -   #### copyOf

            ``` methodSignature
            public static FlavorSet copyOf​(Iterable<? extends Flavor> flavors)
            ```

            ::: block
            Constructor.
            :::

        []{#copyOf(com.google.common.collect.ImmutableSortedSet)}

        -   #### copyOf

            ``` methodSignature
            public static FlavorSet copyOf​(com.google.common.collect.ImmutableSortedSet<Flavor> flavors)
            ```

            ::: block
            Constructor.
            :::

        []{#union(com.facebook.buck.core.model.FlavorSet,com.facebook.buck.core.model.FlavorSet)}

        -   #### union

            ``` methodSignature
            public static FlavorSet union​(FlavorSet a,
                                          FlavorSet b)
            ```

            ::: block
            Return a flavor set with flavors in first or second given
            set.
            :::

        []{#toFlavorSet()}

        -   #### toFlavorSet

            ``` methodSignature
            public static java.util.stream.Collector<Flavor,​?,​FlavorSet> toFlavorSet()
            ```

            ::: block
            Stream collector.
            :::

        []{#without(java.util.Set)}

        -   #### without

            ``` methodSignature
            public FlavorSet without​(Set<Flavor> flavors)
            ```

            ::: block
            Flavors in this set, but not in that set.
            :::

        []{#withAdded(java.util.Set)}

        -   #### withAdded

            ``` methodSignature
            public FlavorSet withAdded​(Set<Flavor> flavors)
            ```

            ::: block
            Create a flavor set with union of this and that flavors.
            :::

        []{#contains(com.facebook.buck.core.model.Flavor)}

        -   #### contains

            ``` methodSignature
            public boolean contains​(Flavor flavor)
            ```

            ::: block
            Does this set contain given flavor?
            :::

        []{#containsAll(com.facebook.buck.core.model.FlavorSet)}

        -   #### containsAll

            ``` methodSignature
            public boolean containsAll​(FlavorSet flavors)
            ```

            ::: block
            Does this set contain all given flavors?
            :::

        []{#containsAll(java.util.Collection)}

        -   #### containsAll

            ``` methodSignature
            public boolean containsAll​(Collection<Flavor> flavors)
            ```

            ::: block
            Does this set contain all given flavors?
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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   Nested \| 
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
