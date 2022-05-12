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
[Package]{.packageLabelInType} [com.facebook.buck.core.select](package-summary.html)
:::

## Class Selector\<T\> {#class-selectort .title title="Class Selector"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.select.Selector\<T\>

::: description
-   

    ------------------------------------------------------------------------

        public class Selector<T>
        extends Object

    ::: block
    Keeps mapping of a single `select` expression. The keys of a mapping
    are
    [`SelectorKey`](SelectorKey.html "class in com.facebook.buck.core.select")s
    and the values can be of an arbitrary type.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `Selector​(com.goog                | ::: block                         |
        | le.common.collect.ImmutableMap<Se | Creates a new Selector with a     |
        | lectorKey,​T> conditions,          | custom error message for a        |
        | com.google.common.collect.Immutab | situation when no conditions      |
        | leSet<SelectorKey> nullConditions | match.                            |
        | ,         String noMatchMessage)` | :::                               |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `equals​(Object o)`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `getConditions()`     |                       |
        | ommon.collect.Immutab |                       |                       |
        | leMap<SelectorKey,​T>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `T`                   | `getDef               | ::: block             |
        |                       | aultConditionValue()` | Returns the default   |
        |                       |                       | value - value to use  |
        |                       |                       | when none of the      |
        |                       |                       | conditions match.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getNoMatchMessage()` | ::: block             |
        |                       |                       | Returns a custom      |
        |                       |                       | message that needs to |
        |                       |                       | be shown to a user    |
        |                       |                       | when no condition     |
        |                       |                       | matches.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getNullConditions()` |                       |
        | .common.collect.Immut |                       |                       |
        | ableSet<SelectorKey>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `h                    | ::: block             |
        |                       | asDefaultCondition()` | Returns whether or    |
        |                       |                       | not this selector has |
        |                       |                       | a default condition.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `<U,​E extends E       | `mapValuesT           | ::: block             |
        | xception>Selector<U>` | hrowing​(ThrowingFunct | Transform all items   |
        |                       | ion<T,​U,​E> function)` | with given function.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `on                   |                       |
        | atic <T> Selector<T>` | lyDefault​(T element)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.google.common.collect.ImmutableMap,com.google.common.collect.ImmutableSet,java.lang.String)}

        -   #### Selector

                public Selector​(com.google.common.collect.ImmutableMap<SelectorKey,​T> conditions,
                                com.google.common.collect.ImmutableSet<SelectorKey> nullConditions,
                                String noMatchMessage)

            ::: block
            Creates a new Selector with a custom error message for a
            situation when no conditions match.
            :::
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#onlyDefault(java.lang.Object)} []{#onlyDefault(T)}

        -   #### onlyDefault

            ``` methodSignature
            public static <T> Selector<T> onlyDefault​(T element)
            ```

        []{#getConditions()}

        -   #### getConditions

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<SelectorKey,​T> getConditions()
            ```

        []{#getNullConditions()}

        -   #### getNullConditions

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<SelectorKey> getNullConditions()
            ```

        []{#getDefaultConditionValue()}

        -   #### getDefaultConditionValue

            ``` methodSignature
            @Nullable
            public T getDefaultConditionValue()
            ```

            ::: block
            Returns the default value - value to use when none of the
            conditions match.
            :::

            [Returns:]{.returnLabel}
            :   the value provided in the default condition or `null` if
                it wasn\'t provided.

        []{#hasDefaultCondition()}

        -   #### hasDefaultCondition

            ``` methodSignature
            public boolean hasDefaultCondition()
            ```

            ::: block
            Returns whether or not this selector has a default
            condition.
            :::

        []{#getNoMatchMessage()}

        -   #### getNoMatchMessage

            ``` methodSignature
            public String getNoMatchMessage()
            ```

            ::: block
            Returns a custom message that needs to be shown to a user
            when no condition matches.
            :::

            [Returns:]{.returnLabel}
            :   the custom message or an empty string if the message is
                not declared.

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object o)
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

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#mapValuesThrowing(com.facebook.buck.util.function.ThrowingFunction)}

        -   #### mapValuesThrowing

            ``` methodSignature
            public <U,​E extends Exception> Selector<U> mapValuesThrowing​(ThrowingFunction<T,​U,​E> function)
                                                                        throws E extends Exception
            ```

            ::: block
            Transform all items with given function.
            :::

            [Throws:]{.throwsLabel}
            :   `E extends Exception`
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
