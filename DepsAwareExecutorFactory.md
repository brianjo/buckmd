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

-   [Overview](../../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../../index-all.html)
-   [Help](../../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.graph.transformation.executor.factory](package-summary.html)
:::

## Class DepsAwareExecutorFactory {#class-depsawareexecutorfactory .title title="Class DepsAwareExecutorFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.graph.transformation.executor.factory.DepsAwareExecutorFactory

::: description
-   

    ------------------------------------------------------------------------

        public class DepsAwareExecutorFactory
        extends Object

    ::: block
    A factory for
    [`DepsAwareExecutor`](../DepsAwareExecutor.html "interface in com.facebook.buck.core.graph.transformation.executor")s.
    This factory uses
    [`DepsAwareExecutorType`](DepsAwareExecutorType.html "enum in com.facebook.buck.core.graph.transformation.executor.factory")
    to determine which implementation of the
    [`DepsAwareExecutor`](../DepsAwareExecutor.html "interface in com.facebook.buck.core.graph.transformation.executor")s
    to use.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                     Method                                                        Description
          ------------------------------------- ------------------------------------------------------------- -------------
          `static <U> DepsAwareExecutor<U,​?>`   `create​(DepsAwareExecutorType type,       int parallelism)`    

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

        []{#create(com.facebook.buck.core.graph.transformation.executor.factory.DepsAwareExecutorType,int)}

        -   #### create

            ``` methodSignature
            public static <U> DepsAwareExecutor<U,​?> create​(DepsAwareExecutorType type,
                                                                  int parallelism)
            ```

            [Type Parameters:]{.paramLabel}
            :   `U` - the type supported by the
                [`DepsAwareExecutor`](../DepsAwareExecutor.html "interface in com.facebook.buck.core.graph.transformation.executor")

            [Parameters:]{.paramLabel}
            :   `type` - the
                [`DepsAwareExecutorType`](DepsAwareExecutorType.html "enum in com.facebook.buck.core.graph.transformation.executor.factory")
                used to indicate which specific implementation of
                [`DepsAwareExecutor`](../DepsAwareExecutor.html "interface in com.facebook.buck.core.graph.transformation.executor")
                to return
            :   `parallelism` - the number of threads in parallel

            [Returns:]{.returnLabel}
            :   a
                [`DepsAwareExecutor`](../DepsAwareExecutor.html "interface in com.facebook.buck.core.graph.transformation.executor")
                of the given parallelism with the specific
                implementation based on
                [`DepsAwareExecutorType`](DepsAwareExecutorType.html "enum in com.facebook.buck.core.graph.transformation.executor.factory")
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

-   [Overview](../../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../../index-all.html)
-   [Help](../../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../../allclasses.html)

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
