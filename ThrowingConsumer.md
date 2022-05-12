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
[Package]{.packageLabelInType} [com.facebook.buck.util.function](package-summary.html)
:::

## Interface ThrowingConsumer\<T,​E extends [Exception](http://docs.oracle.com/javase/7/docs/api/java/lang/Exception.html?is-external=true "class or interface in java.lang"){.externalLink}\> {#interface-throwingconsumerte-extends-exception .title title="Interface ThrowingConsumer"}
:::

::: contentContainer
::: description
-   

    Functional Interface:
    :   This is a functional interface and can therefore be used as the
        assignment target for a lambda expression or method reference.

    ------------------------------------------------------------------------

        @FunctionalInterface
        public interface ThrowingConsumer<T,​E extends Exception>

    ::: block
    The version of `Consumer<T>` that can throw an exception.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Interface             | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `ThrowingConsum       | ::: block             |
        |                       | er.TunneledException` | An exception used to  |
        |                       |                       | tunnel checked        |
        |                       |                       | exceptions through a  |
        |                       |                       | non-throwing          |
        |                       |                       | interface.            |
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
        | `void`                | `accept​(T t)`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <T,​E ex       | `wrapAsUnchecked      | ::: block             |
        | tends Exception>void` | ​(java.util.function.C | Helper to package a   |
        |                       | onsumer<java.util.fun | [`Thro                |
        |                       | ction.Consumer<T>> co | wingConsumer`](Throwi |
        |                       | nsumerConsumer,       | ngConsumer.html "inte |
        |                       |           ThrowingCon | rface in com.facebook |
        |                       | sumer<T,​E> consumer)` | .buck.util.function") |
        |                       |                       | as a `Consumer` and   |
        |                       |                       | apply it on action    |
        |                       |                       | expecting the latter. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#accept(java.lang.Object)} []{#accept(T)}

        -   #### accept

            ``` methodSignature
            void accept​(T t)
                 throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#wrapAsUnchecked(java.util.function.Consumer,com.facebook.buck.util.function.ThrowingConsumer)}

        -   #### wrapAsUnchecked

            ``` methodSignature
            static <T,​E extends Exception> void wrapAsUnchecked​(java.util.function.Consumer<java.util.function.Consumer<T>> consumerConsumer,
                                                                      ThrowingConsumer<T,​E> consumer)
                                                               throws E extends Exception
            ```

            ::: block
            Helper to package a
            [`ThrowingConsumer`](ThrowingConsumer.html "interface in com.facebook.buck.util.function")
            as a `Consumer` and apply it on action expecting the latter.
            Checked exceptions thrown by the former are tunneled inside
            unchecked exceptions and re-raised.
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
