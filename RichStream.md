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
[Package]{.packageLabelInType} [com.facebook.buck.util.stream](package-summary.html)
:::

## Interface RichStream\<T\> {#interface-richstreamt .title title="Interface RichStream"}
:::

::: contentContainer
::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `T` - the type of the stream elements.

    ```{=html}
    <!-- -->
    ```

    All Superinterfaces:
    :   `AutoCloseable`,
        `java.util.stream.BaseStream<T,​java.util.stream.Stream<T>>`,
        `java.util.stream.Stream<T>`

    ------------------------------------------------------------------------

        public interface RichStream<T>
        extends java.util.stream.Stream<T>

    ::: block
    Java 8 streams with \"rich\" API (convenience methods).
    The default Java 8 Stream implementation is deliberately spartan in
    API methods in order to avoid dependencies on Collections, and to
    focus on parallelism. This wrapper adds common operations to the
    Stream API, mostly inspired by Guava\'s `FluentIterable`.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.java.util.stream.Stream}

            ### Nested classes/interfaces inherited from interface java.util.stream.Stream

            `java.util.stream.Stream.Builder<T extends Object>`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `d                    | `concat​(ja            |                       |
        | efault RichStream<T>` | va.util.stream.Stream |                       |
        |                       | <? extends T> other)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `RichStream<T>`       | `distinct()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `empty()`             |                       |
        | ic <T> RichStream<T>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `defau                | `                     | ::: block             |
        | lt <U> RichStream<U>` | filter​(Class<U> cls)` | Filter stream         |
        |                       |                       | elements, returning   |
        |                       |                       | only those that is an |
        |                       |                       | instance of the given |
        |                       |                       | class.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RichStream<T>`       | `filter​(java.util     |                       |
        |                       | .function.Predicate<? |                       |
        |                       |  super T> predicate)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `<R> RichStream<R>`   | `flatMap​(java.util.   |                       |
        |                       | function.Function<? s |                       |
        |                       | uper T,​? extends java |                       |
        |                       | .util.stream.Stream<? |                       |
        |                       |  extends R>> mapper)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `<E ex                | `forEachOrderedThrow  | ::: block             |
        | tends Exception>void` | ing​(ThrowingConsumer< | A variant of          |
        |                       | ? super T,​E> action)` | `Stream.forEachOrdere |
        |                       |                       | d(java.util.function. |
        |                       |                       | Consumer<? super T>)` |
        |                       |                       | that can safely throw |
        |                       |                       | a checked exception.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `<E ex                | `forEachThrow         | ::: block             |
        | tends Exception>void` | ing​(ThrowingConsumer< | A variant of          |
        |                       | ? super T,​E> action)` | `Stream.forEac        |
        |                       |                       | h(java.util.function. |
        |                       |                       | Consumer<? super T>)` |
        |                       |                       | that can safely throw |
        |                       |                       | a checked exception.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `from​(I               |                       |
        | ic <T> RichStream<T>` | terable<T> iterable)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `from​(I               |                       |
        | ic <T> RichStream<T>` | terator<T> iterator)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `from​(O               |                       |
        | ic <T> RichStream<T>` | ptional<T> optional)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `from​(java.util.stre  |                       |
        | ic <T> RichStream<T>` | am.Stream<T> stream)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `from​(T[] array)`     |                       |
        | ic <T> RichStream<T>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `                     |                       |
        | ic <T> RichStream<T>` | fromSupplierOfIterabl |                       |
        |                       | e​(java.util.function. |                       |
        |                       | Supplier<? extends It |                       |
        |                       | erable<T>> supplier)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `RichStream<T>`       | `limit​(long maxSize)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `<R> RichStream<R>`   | `                     |                       |
        |                       | map​(java.util.functio |                       |
        |                       | n.Function<? super T, |                       |
        |                       | ​? extends R> mapper)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `of​(T value)`         |                       |
        | ic <T> RichStream<T>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `of​(T... values)`     |                       |
        | ic <T> RichStream<T>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `RichStream<T>`       | `onClose​(Ru           |                       |
        |                       | nnable closeHandler)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `RichStream<T>`       | `parallel()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `RichStream<T>`       | `peek​(java.           |                       |
        |                       | util.function.Consume |                       |
        |                       | r<? super T> action)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `RichStream<T>`       | `sequential()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `RichStream<T>`       | `skip​(long n)`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `RichStream<T>`       | `sorted()`            |                       |
        +-----------------------+-----------------------+-----------------------+
        | `RichStream<T>`       | `sorted​(Comparator<?  |                       |
        |                       | super T> comparator)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default c            | `toImmutableList()`   |                       |
        | om.google.common.coll |                       |                       |
        | ect.ImmutableList<T>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default              | `toImmutableSet()`    |                       |
        | com.google.common.col |                       |                       |
        | lect.ImmutableSet<T>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default com.go       | `toImmutable          |                       |
        | ogle.common.collect.I | SortedSet​(Comparator< |                       |
        | mmutableSortedSet<T>` | ? super T> ordering)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default Iterable<T>` | `toOnceIterable()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `RichStream<T>`       | `unordered()`         |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}

        -   []{#methods.inherited.from.class.java.util.stream.BaseStream}

            ### Methods inherited from interface java.util.stream.BaseStream

            `close, isParallel, iterator, spliterator`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.util.stream.Stream}

            ### Methods inherited from interface java.util.stream.Stream

            `allMatch, anyMatch, collect, collect, count, dropWhile, findAny, findFirst, flatMapToDouble, flatMapToInt, flatMapToLong, forEach, forEachOrdered, mapToDouble, mapToInt, mapToLong, max, min, noneMatch, reduce, reduce, reduce, takeWhile, toArray, toArray`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#empty()}

        -   #### empty

            ``` methodSignature
            static <T> RichStream<T> empty()
            ```

        []{#of(java.lang.Object)} []{#of(T)}

        -   #### of

            ``` methodSignature
            static <T> RichStream<T> of​(T value)
            ```

        []{#of(java.lang.Object[])} []{#of(T...)}

        -   #### of

            ``` methodSignature
            @SafeVarargs
            static <T> RichStream<T> of​(T... values)
            ```

        []{#from(java.lang.Object[])} []{#from(T[])}

        -   #### from

            ``` methodSignature
            static <T> RichStream<T> from​(T[] array)
            ```

        []{#from(java.lang.Iterable)}

        -   #### from

            ``` methodSignature
            static <T> RichStream<T> from​(Iterable<T> iterable)
            ```

        []{#from(java.util.Iterator)}

        -   #### from

            ``` methodSignature
            static <T> RichStream<T> from​(Iterator<T> iterator)
            ```

        []{#from(java.util.Optional)}

        -   #### from

            ``` methodSignature
            static <T> RichStream<T> from​(Optional<T> optional)
            ```

        []{#fromSupplierOfIterable(java.util.function.Supplier)}

        -   #### fromSupplierOfIterable

            ``` methodSignature
            static <T> RichStream<T> fromSupplierOfIterable​(java.util.function.Supplier<? extends Iterable<T>> supplier)
            ```

        []{#from(java.util.stream.Stream)}

        -   #### from

            ``` methodSignature
            static <T> RichStream<T> from​(java.util.stream.Stream<T> stream)
            ```

        []{#concat(java.util.stream.Stream)}

        -   #### concat

            ``` methodSignature
            default RichStream<T> concat​(java.util.stream.Stream<? extends T> other)
            ```

            [Parameters:]{.paramLabel}
            :   `other` - Stream to concatenate into the current one.

            [Returns:]{.returnLabel}
            :   Stream containing the elements of the current stream
                followed by that of the given stream.

        []{#filter(java.lang.Class)}

        -   #### filter

            ``` methodSignature
            default <U> RichStream<U> filter​(Class<U> cls)
            ```

            ::: block
            Filter stream elements, returning only those that is an
            instance of the given class.
            :::

            [Type Parameters:]{.paramLabel}
            :   `U` - Class to cast to.

            [Parameters:]{.paramLabel}
            :   `cls` - Class instance of the class to cast to.

            [Returns:]{.returnLabel}
            :   Filtered stream of instances of `cls`.

        []{#toImmutableList()}

        -   #### toImmutableList

            ``` methodSignature
            default com.google.common.collect.ImmutableList<T> toImmutableList()
            ```

        []{#toImmutableSet()}

        -   #### toImmutableSet

            ``` methodSignature
            default com.google.common.collect.ImmutableSet<T> toImmutableSet()
            ```

        []{#toImmutableSortedSet(java.util.Comparator)}

        -   #### toImmutableSortedSet

            ``` methodSignature
            default com.google.common.collect.ImmutableSortedSet<T> toImmutableSortedSet​(Comparator<? super T> ordering)
            ```

        []{#toOnceIterable()}

        -   #### toOnceIterable

            ``` methodSignature
            default Iterable<T> toOnceIterable()
            ```

        []{#forEachThrowing(com.facebook.buck.util.function.ThrowingConsumer)}

        -   #### forEachThrowing

            ``` methodSignature
            <E extends Exception> void forEachThrowing​(ThrowingConsumer<? super T,​E> action)
                                                throws E extends Exception
            ```

            ::: block
            A variant of
            `Stream.forEach(java.util.function.Consumer<? super T>)`
            that can safely throw a checked exception.
            :::

            [Type Parameters:]{.paramLabel}
            :   `E` - Exception that may be thrown by the action.

            [Throws:]{.throwsLabel}
            :   `E` - Exception thrown by the action.
            :   `E extends Exception`

        []{#forEachOrderedThrowing(com.facebook.buck.util.function.ThrowingConsumer)}

        -   #### forEachOrderedThrowing

            ``` methodSignature
            <E extends Exception> void forEachOrderedThrowing​(ThrowingConsumer<? super T,​E> action)
                                                       throws E extends Exception
            ```

            ::: block
            A variant of
            `Stream.forEachOrdered(java.util.function.Consumer<? super T>)`
            that can safely throw a checked exception.
            :::

            [Type Parameters:]{.paramLabel}
            :   `E` - Exception that may be thrown by the action.

            [Throws:]{.throwsLabel}
            :   `E` - Exception thrown by the action.
            :   `E extends Exception`

        []{#filter(java.util.function.Predicate)}

        -   #### filter

            ``` methodSignature
            RichStream<T> filter​(java.util.function.Predicate<? super T> predicate)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `filter` in interface `java.util.stream.Stream<T>`

        []{#map(java.util.function.Function)}

        -   #### map

            ``` methodSignature
            <R> RichStream<R> map​(java.util.function.Function<? super T,​? extends R> mapper)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `map` in interface `java.util.stream.Stream<T>`

        []{#flatMap(java.util.function.Function)}

        -   #### flatMap

            ``` methodSignature
            <R> RichStream<R> flatMap​(java.util.function.Function<? super T,​? extends java.util.stream.Stream<? extends R>> mapper)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `flatMap` in interface `java.util.stream.Stream<T>`

        []{#distinct()}

        -   #### distinct

            ``` methodSignature
            RichStream<T> distinct()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `distinct` in interface `java.util.stream.Stream<T>`

        []{#sorted()}

        -   #### sorted

            ``` methodSignature
            RichStream<T> sorted()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `sorted` in interface `java.util.stream.Stream<T>`

        []{#sorted(java.util.Comparator)}

        -   #### sorted

            ``` methodSignature
            RichStream<T> sorted​(Comparator<? super T> comparator)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `sorted` in interface `java.util.stream.Stream<T>`

        []{#peek(java.util.function.Consumer)}

        -   #### peek

            ``` methodSignature
            RichStream<T> peek​(java.util.function.Consumer<? super T> action)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `peek` in interface `java.util.stream.Stream<T>`

        []{#limit(long)}

        -   #### limit

            ``` methodSignature
            RichStream<T> limit​(long maxSize)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `limit` in interface `java.util.stream.Stream<T>`

        []{#skip(long)}

        -   #### skip

            ``` methodSignature
            RichStream<T> skip​(long n)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `skip` in interface `java.util.stream.Stream<T>`

        []{#sequential()}

        -   #### sequential

            ``` methodSignature
            RichStream<T> sequential()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `sequential` in
                interface `java.util.stream.BaseStream<T,​java.util.stream.Stream<T>>`

        []{#parallel()}

        -   #### parallel

            ``` methodSignature
            RichStream<T> parallel()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `parallel` in
                interface `java.util.stream.BaseStream<T,​java.util.stream.Stream<T>>`

        []{#unordered()}

        -   #### unordered

            ``` methodSignature
            RichStream<T> unordered()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `unordered` in
                interface `java.util.stream.BaseStream<T,​java.util.stream.Stream<T>>`

        []{#onClose(java.lang.Runnable)}

        -   #### onClose

            ``` methodSignature
            RichStream<T> onClose​(Runnable closeHandler)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `onClose` in
                interface `java.util.stream.BaseStream<T,​java.util.stream.Stream<T>>`
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
