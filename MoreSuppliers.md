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

## Class MoreSuppliers {#class-moresuppliers .title title="Class MoreSuppliers"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.MoreSuppliers

::: description
-   

    ------------------------------------------------------------------------

        public final class MoreSuppliers
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static <T,           | `memoize​(T            | ::: block             |
        | ​E extends Exception>T | hrowingSupplier<T,​E>  | Returns a             |
        | hrowingSupplier<T,​E>` | delegate,        Clas | [`ThrowingSuppl       |
        |                       | s<E> exceptionClass)` | ier`](function/Throwi |
        |                       |                       | ngSupplier.html "inte |
        |                       |                       | rface in com.facebook |
        |                       |                       | .buck.util.function") |
        |                       |                       | that caches the       |
        |                       |                       | result or the         |
        |                       |                       | exception during the  |
        |                       |                       | first call to         |
        |                       |                       | `get()`, and returns  |
        |                       |                       | or throws on          |
        |                       |                       | subsequent calls to   |
        |                       |                       | `get()`               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `memoize              | ::: block             |
        | static <T> java.util. | ​(java.util.function.S | Returns a supplier    |
        | function.Supplier<T>` | upplier<T> delegate)` | which caches the      |
        |                       |                       | instance retrieved    |
        |                       |                       | during the first call |
        |                       |                       | to `get()` and        |
        |                       |                       | returns that value on |
        |                       |                       | subsequent calls to   |
        |                       |                       | `get()`.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `weakMemoize          |                       |
        | static <T> java.util. | ​(java.util.function.S |                       |
        | function.Supplier<T>` | upplier<T> delegate)` |                       |
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

        []{#memoize(java.util.function.Supplier)}

        -   #### memoize

            ``` methodSignature
            public static <T> java.util.function.Supplier<T> memoize​(java.util.function.Supplier<T> delegate)
            ```

            ::: block
            Returns a supplier which caches the instance retrieved
            during the first call to `get()` and returns that value on
            subsequent calls to `get()`.
            Unlike Guava\'s
            `Suppliers.memoize(com.google.common.base.Supplier)`, this
            version removes the reference to the underlying Supplier
            once the value is computed. This frees up memory used in
            lambda captures, at the cost of causing the supplier to be
            not Serializable.
            :::

        []{#memoize(com.facebook.buck.util.function.ThrowingSupplier,java.lang.Class)}

        -   #### memoize

            ``` methodSignature
            public static <T,​E extends Exception> ThrowingSupplier<T,​E> memoize​(ThrowingSupplier<T,​E> delegate,
                                                                                            Class<E> exceptionClass)
            ```

            ::: block
            Returns a
            [`ThrowingSupplier`](function/ThrowingSupplier.html "interface in com.facebook.buck.util.function")
            that caches the result or the exception during the first
            call to `get()`, and returns or throws on subsequent calls
            to `get()`
            :::

        []{#weakMemoize(java.util.function.Supplier)}

        -   #### weakMemoize

            ``` methodSignature
            public static <T> java.util.function.Supplier<T> weakMemoize​(java.util.function.Supplier<T> delegate)
            ```
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
