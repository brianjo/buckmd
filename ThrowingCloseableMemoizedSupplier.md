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

## Class ThrowingCloseableMemoizedSupplier\<T,​E extends [Exception](http://docs.oracle.com/javase/7/docs/api/java/lang/Exception.html?is-external=true "class or interface in java.lang"){.externalLink}\> {#class-throwingcloseablememoizedsupplierte-extends-exception .title title="Class ThrowingCloseableMemoizedSupplier"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.util.AbstractCloseableMemoizedSupplier](AbstractCloseableMemoizedSupplier.html "class in com.facebook.buck.util")\<T,​E\>

    -   -   com.facebook.buck.util.ThrowingCloseableMemoizedSupplier\<T,​E\>

::: description
-   

    All Implemented Interfaces:
    :   `AutoCloseable`, `java.util.function.Supplier<T>`

    ------------------------------------------------------------------------

        public class ThrowingCloseableMemoizedSupplier<T,​E extends Exception>
        extends AbstractCloseableMemoizedSupplier<T,​E>

    ::: block
    Convenience wrapper class to attach closeable functionality to
    suppliers of resources to be closed. Suppliers will be memoized such
    that the resources are only closed if we have requested them.
    Example:

         class Main {
          public static void main() {
            try (ThrowingCloseableMemoizedSupplier<Resource, Exception> closeableSupplier =
                ThrowingCloseableMemoizedSupplier.of(Resource::new, resource::shutDown)) {
              if (condition) {
                useResource(closeableSupplier.get())
              }
            }
          }
         }

         

    The above will only construct the Resource if condition is true, and
    close the constructed resource appropriately.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static               | `of​(java.util.        | ::: block             |
        |  <T,​E extends Excepti | function.Supplier<T>  | Wrap a supplier with  |
        | on>ThrowingCloseableM | supplier,   ThrowingC | `AutoCloseable`       |
        | emoizedSupplier<T,​E>` | onsumer<T,​E> closer)` | interface and close   |
        |                       |                       | only if the supplier  |
        |                       |                       | has been used.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.util.AbstractCloseableMemoizedSupplier}

            ### Methods inherited from class com.facebook.buck.util.[AbstractCloseableMemoizedSupplier](AbstractCloseableMemoizedSupplier.html "class in com.facebook.buck.util")

            `close, get`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#of(java.util.function.Supplier,com.facebook.buck.util.function.ThrowingConsumer)}

        -   #### of

            ``` methodSignature
            public static <T,​E extends Exception> ThrowingCloseableMemoizedSupplier<T,​E> of​(java.util.function.Supplier<T> supplier,
                                                                                                        ThrowingConsumer<T,​E> closer)
            ```

            ::: block
            Wrap a supplier with `AutoCloseable` interface and close
            only if the supplier has been used. Close is idempotent.
            :::

            [Parameters:]{.paramLabel}
            :   `supplier` - the Supplier of a resource to be closed
            :   `closer` - the method to close the resource
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