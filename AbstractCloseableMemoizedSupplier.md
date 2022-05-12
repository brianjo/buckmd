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
[Package]{.packageLabelInType} [com.facebook.buck.util](package-summary.html)
:::

## Class AbstractCloseableMemoizedSupplier\<T,​E extends [Exception](http://docs.oracle.com/javase/7/docs/api/java/lang/Exception.html?is-external=true "class or interface in java.lang"){.externalLink}\> {#class-abstractcloseablememoizedsupplierte-extends-exception .title title="Class AbstractCloseableMemoizedSupplier"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.AbstractCloseableMemoizedSupplier\<T,​E\>

::: description
-   

    All Implemented Interfaces:
    :   `AutoCloseable`, `java.util.function.Supplier<T>`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `CloseableMemoizedSupplier`, `ThrowingCloseableMemoizedSupplier`

    ------------------------------------------------------------------------

        public class AbstractCloseableMemoizedSupplier<T,​E extends Exception>
        extends Object
        implements AutoCloseable, java.util.function.Supplier<T>

    ::: block
    Base class for
    [`CloseableMemoizedSupplier`](CloseableMemoizedSupplier.html "class in com.facebook.buck.util")
    and
    [`ThrowingCloseableMemoizedSupplier`](ThrowingCloseableMemoizedSupplier.html "class in com.facebook.buck.util")
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                                                                                                   Description
          -------------- --------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `protected `   `AbstractCloseableMemoizedSupplier​(java.util.function.Supplier<T> supplier,                                  ThrowingConsumer<T,​E> closer)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method      Description
          ------------------- ----------- -------------
          `void`              `close()`    
          `T`                 `get()`      

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.util.function.Supplier,com.facebook.buck.util.function.ThrowingConsumer)}

        -   #### AbstractCloseableMemoizedSupplier

                protected AbstractCloseableMemoizedSupplier​(java.util.function.Supplier<T> supplier,
                                                            ThrowingConsumer<T,​E> closer)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#get()}

        -   #### get

            ``` methodSignature
            public T get()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `get` in interface `java.util.function.Supplier<T>`

            [Returns:]{.returnLabel}
            :   the resource from the supplier

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
                       throws E extends Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

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
