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
[Package]{.packageLabelInType} [com.facebook.buck.core.graph.transformation.executor](package-summary.html)
:::

## Class DepsAwareTask.DepsSupplier\<Impl\> {#class-depsawaretask.depssupplierimpl .title title="Class DepsAwareTask.DepsSupplier"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.graph.transformation.executor.DepsAwareTask.DepsSupplier\<Impl\>

::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `Impl` - the task type

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [DepsAwareTask](DepsAwareTask.html "class in com.facebook.buck.core.graph.transformation.executor")\<[T](DepsAwareTask.html "type parameter in DepsAwareTask"),​[Impl](DepsAwareTask.html "type parameter in DepsAwareTask")
        extends
        [DepsAwareTask](DepsAwareTask.html "class in com.facebook.buck.core.graph.transformation.executor")\<[T](DepsAwareTask.html "type parameter in DepsAwareTask"),​[Impl](DepsAwareTask.html "type parameter in DepsAwareTask")\>\>

    ------------------------------------------------------------------------

        public static class DepsAwareTask.DepsSupplier<Impl>
        extends Object

    ::: block
    The dependency information of a task.
    The `prereqSupplier` is a supplier that returns a set of tasks
    necessary to compute `depsSupplier`. The `depsSupplier` is a
    supplier that returns the dependencies.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                Method                                                                                                                                                                            Description
          ------------------------------------------------ --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `com.google.common.collect.ImmutableSet<Impl>`   `get()`                                                                                                                                                                            
          `com.google.common.collect.ImmutableSet<Impl>`   `getPrereq()`                                                                                                                                                                      
          `static <U> DepsAwareTask.DepsSupplier<U>`       `of()`                                                                                                                                                                             
          `static <U> DepsAwareTask.DepsSupplier<U>`       `of​(ThrowingSupplier<com.google.common.collect.ImmutableSet<U>,​Exception> prereqSupplier,   ThrowingSupplier<com.google.common.collect.ImmutableSet<U>,​Exception> depSupplier)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
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
    -   []{#method.detail}

        ### Method Detail

        []{#of()}

        -   #### of

            ``` methodSignature
            public static <U> DepsAwareTask.DepsSupplier<U> of()
            ```

            [Returns:]{.returnLabel}
            :   a
                [`DepsAwareTask.DepsSupplier`](DepsAwareTask.DepsSupplier.html "class in com.facebook.buck.core.graph.transformation.executor")
                with no dependencies

        []{#of(com.facebook.buck.util.function.ThrowingSupplier,com.facebook.buck.util.function.ThrowingSupplier)}

        -   #### of

            ``` methodSignature
            public static <U> DepsAwareTask.DepsSupplier<U> of​(ThrowingSupplier<com.google.common.collect.ImmutableSet<U>,​Exception> prereqSupplier,
                                                               ThrowingSupplier<com.google.common.collect.ImmutableSet<U>,​Exception> depSupplier)
            ```

            [Returns:]{.returnLabel}
            :   a two staged
                [`DepsAwareTask.DepsSupplier`](DepsAwareTask.DepsSupplier.html "class in com.facebook.buck.core.graph.transformation.executor"),
                where `prereqSupplier` is the initial dependency
                computation, and `depSupplier` is the dependency
                computation that occurs after the tasks from the initial
                dependency computation are complete.

        []{#get()}

        -   #### get

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<Impl> get()
                                                             throws Exception
            ```

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#getPrereq()}

        -   #### getPrereq

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<Impl> getPrereq()
                                                                   throws Exception
            ```

            [Throws:]{.throwsLabel}
            :   `Exception`
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
