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
[Package]{.packageLabelInType} [com.facebook.buck.util.function](package-summary.html)
:::

## Interface ThrowingSupplier\<T,​E extends [Exception](http://docs.oracle.com/javase/7/docs/api/java/lang/Exception.html?is-external=true "class or interface in java.lang"){.externalLink}\> {#interface-throwingsupplierte-extends-exception .title title="Interface ThrowingSupplier"}
:::

::: contentContainer
::: description
-   

    Functional Interface:
    :   This is a functional interface and can therefore be used as the
        assignment target for a lambda expression or method reference.

    ------------------------------------------------------------------------

        @FunctionalInterface
        public interface ThrowingSupplier<T,​E extends Exception>

    ::: block
    This version of `Supplier<T>` can throw an exception.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `default java.util.   | `asSupplier()`        | ::: block             |
        | function.Supplier<T>` |                       | Returns a Supplier    |
        |                       |                       | that will wrap any    |
        |                       |                       | thrown exception in a |
        |                       |                       | RuntimeException.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static <T,           | `fromSupplier         | ::: block             |
        | ​E extends Exception>T | ​(java.util.function.S | Returns a             |
        | hrowingSupplier<T,​E>` | upplier<T> supplier)` | [`Thro                |
        |                       |                       | wingSupplier`](Throwi |
        |                       |                       | ngSupplier.html "inte |
        |                       |                       | rface in com.facebook |
        |                       |                       | .buck.util.function") |
        |                       |                       | from a `Supplier`     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `T`                   | `get()`               |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#get()}

        -   #### get

            ``` methodSignature
            T get()
            throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#asSupplier()}

        -   #### asSupplier

            ``` methodSignature
            default java.util.function.Supplier<T> asSupplier()
            ```

            ::: block
            Returns a Supplier that will wrap any thrown exception in a
            RuntimeException.
            :::

        []{#fromSupplier(java.util.function.Supplier)}

        -   #### fromSupplier

            ``` methodSignature
            static <T,​E extends Exception> ThrowingSupplier<T,​E> fromSupplier​(java.util.function.Supplier<T> supplier)
            ```

            ::: block
            Returns a
            [`ThrowingSupplier`](ThrowingSupplier.html "interface in com.facebook.buck.util.function")
            from a `Supplier`
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
