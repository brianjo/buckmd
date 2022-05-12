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
-   Tree
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Hierarchy For Package com.facebook.buck.util.concurrent {#hierarchy-for-package-com.facebook.buck.util.concurrent .title}

[Package Hierarchies:]{.packageHierarchyLabel}

-   [All Packages](../../../../../overview-tree.html)
:::

::: contentContainer
::: {.section role="region"}
## Class Hierarchy {#class-hierarchy title="Class Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   java.util.concurrent.[[AbstractExecutorService]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/util/concurrent/AbstractExecutorService.html?is-external=true "class or interface in java.util.concurrent"){.externalLink}
        (implements
        java.util.concurrent.[ExecutorService](http://docs.oracle.com/javase/7/docs/api/java/util/concurrent/ExecutorService.html?is-external=true "class or interface in java.util.concurrent"){.externalLink})
        -   com.google.common.util.concurrent.AbstractListeningExecutorService
            (implements
            com.google.common.util.concurrent.ListeningExecutorService)
            -   com.facebook.buck.util.concurrent.[[WeightedListeningExecutorService]{.typeNameLink}](WeightedListeningExecutorService.html "class in com.facebook.buck.util.concurrent")
    -   com.facebook.buck.util.concurrent.[[AssertScopeExclusiveAccess]{.typeNameLink}](AssertScopeExclusiveAccess.html "class in com.facebook.buck.util.concurrent")
    -   com.facebook.buck.util.concurrent.[[AutoCloseableLock]{.typeNameLink}](AutoCloseableLock.html "class in com.facebook.buck.util.concurrent")
        (implements
        java.lang.[AutoCloseable](http://docs.oracle.com/javase/7/docs/api/java/lang/AutoCloseable.html?is-external=true "class or interface in java.lang"){.externalLink},
        java.util.concurrent.locks.[Lock](http://docs.oracle.com/javase/7/docs/api/java/util/concurrent/locks/Lock.html?is-external=true "class or interface in java.util.concurrent.locks"){.externalLink})
    -   com.facebook.buck.util.concurrent.[[AutoCloseableReadWriteLock]{.typeNameLink}](AutoCloseableReadWriteLock.html "class in com.facebook.buck.util.concurrent")
        (implements
        java.util.concurrent.locks.[ReadWriteLock](http://docs.oracle.com/javase/7/docs/api/java/util/concurrent/locks/ReadWriteLock.html?is-external=true "class or interface in java.util.concurrent.locks"){.externalLink})
    -   com.facebook.buck.util.concurrent.[[AutoCloseableReadWriteUpdateLock]{.typeNameLink}](AutoCloseableReadWriteUpdateLock.html "class in com.facebook.buck.util.concurrent")
        (implements com.googlecode.concurentlocks.ReadWriteUpdateLock)
    -   com.facebook.buck.util.concurrent.[[CommandThreadFactory]{.typeNameLink}](CommandThreadFactory.html "class in com.facebook.buck.util.concurrent")
        (implements
        java.util.concurrent.[ThreadFactory](http://docs.oracle.com/javase/7/docs/api/java/util/concurrent/ThreadFactory.html?is-external=true "class or interface in java.util.concurrent"){.externalLink})
    -   com.facebook.buck.util.concurrent.[[ConcurrencyLimit]{.typeNameLink}](ConcurrencyLimit.html "class in com.facebook.buck.util.concurrent")
    -   java.util.concurrent.[[ForkJoinTask]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/util/concurrent/ForkJoinTask.html?is-external=true "class or interface in java.util.concurrent"){.externalLink}\<V\>
        (implements
        java.util.concurrent.[Future](http://docs.oracle.com/javase/7/docs/api/java/util/concurrent/Future.html?is-external=true "class or interface in java.util.concurrent"){.externalLink}\<V\>,
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   com.facebook.buck.util.concurrent.[[WorkThreadTrackingTask]{.typeNameLink}](WorkThreadTrackingTask.html "class in com.facebook.buck.util.concurrent")\<T\>
    -   com.facebook.buck.util.concurrent.[[JobLimiter]{.typeNameLink}](JobLimiter.html "class in com.facebook.buck.util.concurrent")
    -   com.facebook.buck.util.concurrent.[[LinkedBlockingStack]{.typeNameLink}](LinkedBlockingStack.html "class in com.facebook.buck.util.concurrent")\<E\>
        (implements
        java.util.concurrent.[BlockingQueue](http://docs.oracle.com/javase/7/docs/api/java/util/concurrent/BlockingQueue.html?is-external=true "class or interface in java.util.concurrent"){.externalLink}\<E\>)
    -   com.facebook.buck.util.concurrent.[[ListeningMultiSemaphore]{.typeNameLink}](ListeningMultiSemaphore.html "class in com.facebook.buck.util.concurrent")
    -   com.facebook.buck.util.concurrent.[[MoreAtomics]{.typeNameLink}](MoreAtomics.html "class in com.facebook.buck.util.concurrent")
    -   com.facebook.buck.util.concurrent.[[MoreFutures]{.typeNameLink}](MoreFutures.html "class in com.facebook.buck.util.concurrent")
    -   com.facebook.buck.util.concurrent.[[MostExecutors]{.typeNameLink}](MostExecutors.html "class in com.facebook.buck.util.concurrent")
    -   com.facebook.buck.util.concurrent.[[MostExecutors.NamedThreadFactory]{.typeNameLink}](MostExecutors.NamedThreadFactory.html "class in com.facebook.buck.util.concurrent")
        (implements
        java.util.concurrent.[ThreadFactory](http://docs.oracle.com/javase/7/docs/api/java/util/concurrent/ThreadFactory.html?is-external=true "class or interface in java.util.concurrent"){.externalLink})
    -   com.facebook.buck.util.concurrent.[[ResourceAmounts]{.typeNameLink}](ResourceAmounts.html "class in com.facebook.buck.util.concurrent")
    -   com.facebook.buck.util.concurrent.[[ResourceAmountsEstimator]{.typeNameLink}](ResourceAmountsEstimator.html "class in com.facebook.buck.util.concurrent")
    -   com.facebook.buck.util.concurrent.[[ResourcePool]{.typeNameLink}](ResourcePool.html "class in com.facebook.buck.util.concurrent")\<R\>
        (implements
        java.lang.[AutoCloseable](http://docs.oracle.com/javase/7/docs/api/java/lang/AutoCloseable.html?is-external=true "class or interface in java.lang"){.externalLink})
:::

::: {.section role="region"}
## Interface Hierarchy {#interface-hierarchy title="Interface Hierarchy"}

-   java.lang.[[AutoCloseable]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/AutoCloseable.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   com.facebook.buck.util.concurrent.[[AssertScopeExclusiveAccess.Scope]{.typeNameLink}](AssertScopeExclusiveAccess.Scope.html "interface in com.facebook.buck.util.concurrent")
-   com.facebook.buck.util.concurrent.[[Parallelizer]{.typeNameLink}](Parallelizer.html "interface in com.facebook.buck.util.concurrent")
-   com.facebook.buck.util.concurrent.[[ResourcePool.ThrowingFunction]{.typeNameLink}](ResourcePool.ThrowingFunction.html "interface in com.facebook.buck.util.concurrent")\<T,​R\>
-   com.facebook.buck.util.concurrent.[[ThreadIdToCommandIdMapper]{.typeNameLink}](ThreadIdToCommandIdMapper.html "interface in com.facebook.buck.util.concurrent")
    -   com.facebook.buck.util.concurrent.[[CommonThreadFactoryState]{.typeNameLink}](CommonThreadFactoryState.html "interface in com.facebook.buck.util.concurrent")
:::

::: {.section role="region"}
## Enum Hierarchy {#enum-hierarchy title="Enum Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   java.lang.[[Enum]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<E\>
        (implements
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   com.facebook.buck.util.concurrent.[[ExecutorPool]{.typeNameLink}](ExecutorPool.html "enum in com.facebook.buck.util.concurrent")
        -   com.facebook.buck.util.concurrent.[[ResourceAllocationFairness]{.typeNameLink}](ResourceAllocationFairness.html "enum in com.facebook.buck.util.concurrent")
        -   com.facebook.buck.util.concurrent.[[ResourcePool.ResourceUsageErrorPolicy]{.typeNameLink}](ResourcePool.ResourceUsageErrorPolicy.html "enum in com.facebook.buck.util.concurrent")
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
-   Tree
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

[]{#skip.navbar.bottom}
:::
