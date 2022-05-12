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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.graph.transformation.executor](package-summary.html)
:::

## Class DepsAwareTask\<T,​Impl extends DepsAwareTask\<T,​Impl\>\> {#class-depsawaretasktimpl-extends-depsawaretasktimpl .title title="Class DepsAwareTask"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.graph.transformation.executor.DepsAwareTask\<T,​Impl\>

::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `T` - the result type of the task
    :   `Impl` - The implementation type of

    ------------------------------------------------------------------------

        public abstract class DepsAwareTask<T,​Impl extends DepsAwareTask<T,​Impl>>
        extends Object

    ::: block
    Task to be ran in a
    [`DepsAwareExecutor`](DepsAwareExecutor.html "interface in com.facebook.buck.core.graph.transformation.executor").
    This task will offer dependency discovery to the executor so that
    the executor can perform better scheduling.
    The task uses
    [`DepsAwareTask.DepsSupplier`](DepsAwareTask.DepsSupplier.html "class in com.facebook.buck.core.graph.transformation.executor")
    to mark what dependencies are needed.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `DepsAwareTas         | ::: block             |
        |                       | k.DepsSupplier<Impl>` | The dependency        |
        |                       |                       | information of a      |
        |                       |                       | task.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                  Field      Description
          ---------------------------------- ---------- -------------
          `protected CompletableFuture<T>`   `result`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                                                         Description
          -------------- --------------------------------------------------------------------------------------------------- -------------
          `protected `   `DepsAwareTask​(Callable<T> callable,              DepsAwareTask.DepsSupplier<Impl> depsSupplier)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                    Method                Description
          ------------------------------------ --------------------- -------------
          `Callable<T>`                        `getCallable()`        
          `DepsAwareTask.DepsSupplier<Impl>`   `getDepsSupplier()`    
          `Future<T>`                          `getResultFuture()`    

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
    -   []{#field.detail}

        ### Field Detail

        []{#result}

        -   #### result

                protected final CompletableFuture<T> result
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.util.concurrent.Callable,com.facebook.buck.core.graph.transformation.executor.DepsAwareTask.DepsSupplier)}

        -   #### DepsAwareTask

                protected DepsAwareTask​(Callable<T> callable,
                                        DepsAwareTask.DepsSupplier<Impl> depsSupplier)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getCallable()}

        -   #### getCallable

            ``` methodSignature
            public Callable<T> getCallable()
            ```

            [Returns:]{.returnLabel}
            :   the function to run for this task

        []{#getDepsSupplier()}

        -   #### getDepsSupplier

            ``` methodSignature
            public DepsAwareTask.DepsSupplier<Impl> getDepsSupplier()
            ```

            [Returns:]{.returnLabel}
            :   a function to generate the dependencies

        []{#getResultFuture()}

        -   #### getResultFuture

            ``` methodSignature
            public Future<T> getResultFuture()
            ```

            [Returns:]{.returnLabel}
            :   a future of the result of this task
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   [Nested](#nested.class.summary) \| 
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
