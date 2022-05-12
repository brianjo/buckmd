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

## Class CloseableWrapper\<T\> {#class-closeablewrappert .title title="Class CloseableWrapper"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.util.AbstractCloseableWrapper](AbstractCloseableWrapper.html "class in com.facebook.buck.util")\<T,​[RuntimeException](http://docs.oracle.com/javase/7/docs/api/java/lang/RuntimeException.html?is-external=true "class or interface in java.lang"){.externalLink}\>

    -   -   com.facebook.buck.util.CloseableWrapper\<T\>

::: description
-   

    All Implemented Interfaces:
    :   `AutoCloseable`

    ------------------------------------------------------------------------

        public class CloseableWrapper<T>
        extends AbstractCloseableWrapper<T,​RuntimeException>

    ::: block
    Convenience wrapper class to attach closeable functionality to
    non-closeable class so it can be used with try-with-resources to
    make sure resources are always released and proper exception
    suppression is used. The closer may not throw an exception.
    Example:

         class Main {
          private static void finalizeMyClass(MyClass obj) {
            obj.shutdown();
          }

          public static void main() {
            try (CloseableWrapper<MyClass> myClassWrapper =
                  CloseableWrapper.of(new MyClass(), Main::finalizeMyClass)) {
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
        | `static <T>           | `of​(T obj,            | ::: block             |
        |  CloseableWrapper<T>` |    java.util.function | Wrap an object with   |
        |                       | .Consumer<T> closer)` | `AutoCloseable`       |
        |                       |                       | interface and provide |
        |                       |                       | a function to replace |
        |                       |                       | a `  close` method.   |
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

        []{#of(java.lang.Object,java.util.function.Consumer)}
        []{#of(T,java.util.function.Consumer)}

        -   #### of

            ``` methodSignature
            public static <T> CloseableWrapper<T> of​(T obj,
                                                     java.util.function.Consumer<T> closer)
            ```

            ::: block
            Wrap an object with `AutoCloseable` interface and provide a
            function to replace a `  close` method. The wrapper is
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
