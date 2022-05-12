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
[Package]{.packageLabelInType} [com.facebook.buck.util.concurrent](package-summary.html)
:::

## Class ResourcePool\<R extends [AutoCloseable](http://docs.oracle.com/javase/7/docs/api/java/lang/AutoCloseable.html?is-external=true "class or interface in java.lang"){.externalLink}\> {#class-resourcepoolr-extends-autocloseable .title title="Class ResourcePool"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.concurrent.ResourcePool\<R\>

::: description
-   

    All Implemented Interfaces:
    :   `AutoCloseable`

    ------------------------------------------------------------------------

        public class ResourcePool<R extends AutoCloseable>
        extends Object
        implements AutoCloseable

    ::: block
    Allows multiple concurrently executing futures to share a
    constrained number of resources.
    Resources are lazily created up till a fixed maximum. If more than
    max resources are requested the associated \'requests\' are queued
    up in the resourceRequests field. As soon as a resource is returned
    it will be used to satisfy the first pending request, otherwise it
    is stored in the parkedResources queue.

    If the resourceSupplier throws a RuntimeException the Future
    associated with the failed attempt to create the resource will
    contain the relevant exception. Any subsequent requests the pool
    will get will attempt to create a new resource.

    If the
    [`ResourcePool.ResourceUsageErrorPolicy.RECYCLE`](ResourcePool.ResourceUsageErrorPolicy.html#RECYCLE)
    error usage policy is specified then, in case of errors when
    \"using\" a resource it is assumed to be defective, will be retired
    and a new resource will be requested from the supplier. The Future
    associated with the failed attempt to use the resource will contain
    the relevant exception.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `ResourcePool.Reso    | ::: block             |
        |                       | urceUsageErrorPolicy` | Describes how to      |
        |                       |                       | handle errors that    |
        |                       |                       | take place during     |
        |                       |                       | resource usage.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static interface `   | `ResourcePool.T       |                       |
        |                       | hrowingFunction<T,​R>` |                       |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                 Description
          --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `ResourcePool​(int maxResources,             ResourcePool.ResourceUsageErrorPolicy resourceUsageErrorPolicy,             java.util.function.Supplier<R> resourceSupplier)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                             Method                                                                                                                                                                                      Description
          ------------------------------------------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `void`                                                        `callOnEachResource​(java.util.function.Consumer<R> withResource)`                                                                                                                            
          `void`                                                        `close()`                                                                                                                                                                                    
          `com.google.common.util.concurrent.ListenableFuture<Unit>`    `getShutdownFullyCompleteFuture()`                                                                                                                                                           
          `<T> com.google.common.util.concurrent.ListenableFuture<T>`   `scheduleOperationWithResource​(ResourcePool.ThrowingFunction<R,​T> withResource,                              com.google.common.util.concurrent.ListeningExecutorService executorService)`    

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

        []{#<init>(int,com.facebook.buck.util.concurrent.ResourcePool.ResourceUsageErrorPolicy,java.util.function.Supplier)}

        -   #### ResourcePool

                public ResourcePool​(int maxResources,
                                    ResourcePool.ResourceUsageErrorPolicy resourceUsageErrorPolicy,
                                    java.util.function.Supplier<R> resourceSupplier)

            [Parameters:]{.paramLabel}
            :   `maxResources` - maximum number of resources to use
                concurrently.
            :   `resourceSupplier` - function used to create a new
                resource. It should never block, it may be called more
                than maxResources times if processing resources throws
                exceptions.
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#callOnEachResource(java.util.function.Consumer)}

        -   #### callOnEachResource

            ``` methodSignature
            public void callOnEachResource​(java.util.function.Consumer<R> withResource)
            ```

        []{#scheduleOperationWithResource(com.facebook.buck.util.concurrent.ResourcePool.ThrowingFunction,com.google.common.util.concurrent.ListeningExecutorService)}

        -   #### scheduleOperationWithResource

            ``` methodSignature
            public <T> com.google.common.util.concurrent.ListenableFuture<T> scheduleOperationWithResource​(ResourcePool.ThrowingFunction<R,​T> withResource,
                                                                                                           com.google.common.util.concurrent.ListeningExecutorService executorService)
            ```

            [Parameters:]{.paramLabel}
            :   `executorService` - where to perform the resource
                processing. Should really be a \"real\" executor (not a
                directExecutor).

            [Returns:]{.returnLabel}
            :   a `ListenableFuture` containing the result of the
                processing. The future will be cancelled if the
                [`close()`](#close()) method is called.

        []{#getShutdownFullyCompleteFuture()}

        -   #### getShutdownFullyCompleteFuture

            ``` methodSignature
            @Nullable
            public com.google.common.util.concurrent.ListenableFuture<Unit> getShutdownFullyCompleteFuture()
            ```

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`
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
