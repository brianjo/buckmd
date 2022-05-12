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

## Class CloseableMemoizedSupplier\<T\> {#class-closeablememoizedsuppliert .title title="Class CloseableMemoizedSupplier"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.util.AbstractCloseableMemoizedSupplier](AbstractCloseableMemoizedSupplier.html "class in com.facebook.buck.util")\<T,​[RuntimeException](http://docs.oracle.com/javase/7/docs/api/java/lang/RuntimeException.html?is-external=true "class or interface in java.lang"){.externalLink}\>

    -   -   com.facebook.buck.util.CloseableMemoizedSupplier\<T\>

::: description
-   

    All Implemented Interfaces:
    :   `AutoCloseable`, `java.util.function.Supplier<T>`

    ------------------------------------------------------------------------

        public class CloseableMemoizedSupplier<T>
        extends AbstractCloseableMemoizedSupplier<T,​RuntimeException>

    ::: block
    Convenience wrapper class to attach closeable functionality to
    suppliers of resources to be closed. Suppliers will be memoized such
    that the resources are only closed if we have requested them.
    Example:

         class Main {
          public static void main() {
            try (CloseableMemoizedSupplier<Resource> closeableSupplier =
                CloseableMemoizedSupplier.of(Resource::new, resource::shutDown)) {
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
        | `static <T,​E exten    | `o                    | ::: block             |
        | ds Exception>Closeabl | f​(java.util.function. | Wrap a supplier with  |
        | eMemoizedSupplier<T>` | Supplier<T> supplier, | `AutoCloseable`       |
        |                       |    java.util.function | interface and close   |
        |                       | .Consumer<T> closer)` | only if the supplier  |
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

        []{#of(java.util.function.Supplier,java.util.function.Consumer)}

        -   #### of

            ``` methodSignature
            public static <T,​E extends Exception> CloseableMemoizedSupplier<T> of​(java.util.function.Supplier<T> supplier,
                                                                                        java.util.function.Consumer<T> closer)
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
