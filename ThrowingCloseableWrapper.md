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

## Class ThrowingCloseableWrapper\<T,​E extends [Exception](http://docs.oracle.com/javase/7/docs/api/java/lang/Exception.html?is-external=true "class or interface in java.lang"){.externalLink}\> {#class-throwingcloseablewrapperte-extends-exception .title title="Class ThrowingCloseableWrapper"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.util.AbstractCloseableWrapper](AbstractCloseableWrapper.html "class in com.facebook.buck.util")\<T,​E\>

    -   -   com.facebook.buck.util.ThrowingCloseableWrapper\<T,​E\>

::: description
-   

    All Implemented Interfaces:
    :   `AutoCloseable`

    ------------------------------------------------------------------------

        public class ThrowingCloseableWrapper<T,​E extends Exception>
        extends AbstractCloseableWrapper<T,​E>

    ::: block
    Convenience wrapper class to attach closeable functionality to
    non-closeable class so it can be used with try-with-resources to
    make sure resources are always released and proper exception
    suppression is used. The closer may throw an exception which type
    can be specialized.
    Example:

         class Main {
          private static void finalizeMyClass(MyClass obj) throws IOException {
            obj.shutdown();
          }

          public static void main() {
            try (ThrowingCloseableWrapper<MyClass, IOException> myClassWrapper =
                  ThrowingCloseableWrapper.of(new MyClass(), Main::finalizeMyClass)) {
              myClassWrapper.get().doSomething();
            }
          }
         }

         
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static <T,​E extend   | `                     | ::: block             |
        | s Exception>ThrowingC | of​(T obj,   ThrowingC | Wrap an object with   |
        | loseableWrapper<T,​E>` | onsumer<T,​E> closer)` | `AutoCloseable`       |
        |                       |                       | interface and provide |
        |                       |                       | a function to replace |
        |                       |                       | a `  close` method    |
        |                       |                       | The wrapper is        |
        |                       |                       | idempotent, i.e.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.util.AbstractCloseableWrapper}

            ### Methods inherited from class com.facebook.buck.util.[AbstractCloseableWrapper](AbstractCloseableWrapper.html "class in com.facebook.buck.util")

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

        []{#of(java.lang.Object,com.facebook.buck.util.function.ThrowingConsumer)}
        []{#of(T,com.facebook.buck.util.function.ThrowingConsumer)}

        -   #### of

            ``` methodSignature
            public static <T,​E extends Exception> ThrowingCloseableWrapper<T,​E> of​(T obj,
                                                                                               ThrowingConsumer<T,​E> closer)
            ```

            ::: block
            Wrap an object with `AutoCloseable` interface and provide a
            function to replace a `  close` method The wrapper is
            idempotent, i.e. it will call closer function exactly once,
            even if user calls `close` multiple times.
            :::

            [Parameters:]{.paramLabel}
            :   `obj` - Any class that does not implement AutoCloseable
                interface which is hard to extend
            :   `closer` - A function to call on close
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
