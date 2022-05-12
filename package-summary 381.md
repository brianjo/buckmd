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
-   Package
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Package com.facebook.buck.util.concurrent {#package-com.facebook.buck.util.concurrent .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [AssertScopeExclusiveAc           |                                   |
    | cess.Scope](AssertScopeExclusiveA |                                   |
    | ccess.Scope.html "interface in co |                                   |
    | m.facebook.buck.util.concurrent") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Common                           |                                   |
    | ThreadFactoryState](CommonThreadF |                                   |
    | actoryState.html "interface in co |                                   |
    | m.facebook.buck.util.concurrent") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Parallelizer](P                  | ::: block                         |
    | arallelizer.html "interface in co | Interface to transform high level |
    | m.facebook.buck.util.concurrent") | constructs to potentially         |
    |                                   | parallel ones.                    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ResourcePool.ThrowingFu          |                                   |
    | nction](ResourcePool.ThrowingFunc |                                   |
    | tion.html "interface in com.faceb |                                   |
    | ook.buck.util.concurrent")\<T,​R\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [ThreadId                         |                                   |
    | ToCommandIdMapper](ThreadIdToComm |                                   |
    | andIdMapper.html "interface in co |                                   |
    | m.facebook.buck.util.concurrent") |                                   |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [Assert                           | ::: block                         |
    | ScopeExclusiveAccess](AssertScope | Makes it simple to assert that    |
    | ExclusiveAccess.html "class in co | access to a piece of code should  |
    | m.facebook.buck.util.concurrent") | be done from one thread at a time |
    |                                   | in a non-reentrant manner.        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AutoCloseableLock](Au            |                                   |
    | toCloseableLock.html "class in co |                                   |
    | m.facebook.buck.util.concurrent") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AutoCl                           | ::: block                         |
    | oseableReadWriteLock](AutoCloseab | Convenience wrapper around        |
    | leReadWriteLock.html "class in co | [`Reentr                          |
    | m.facebook.buck.util.concurrent") | antReadWriteLock`](http://docs.or |
    |                                   | acle.com/javase/7/docs/api/java/u |
    |                                   | til/concurrent/locks/ReentrantRea |
    |                                   | dWriteLock.html?is-external=true  |
    |                                   | "class or interface in java.util. |
    |                                   | concurrent.locks"){.externalLink} |
    |                                   | that, when combined with          |
    |                                   | try-with-resources pattern,       |
    |                                   | automatically unlocks the lock    |
    |                                   | once the `try` section is         |
    |                                   | completed.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AutoCloseableReadW               |                                   |
    | riteUpdateLock](AutoCloseableRead |                                   |
    | WriteUpdateLock.html "class in co |                                   |
    | m.facebook.buck.util.concurrent") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CommandThreadFactory](Comma      | ::: block                         |
    | ndThreadFactory.html "class in co | A ThreadFactory which associates  |
    | m.facebook.buck.util.concurrent") | created threads with the same     |
    |                                   | command associated with the       |
    |                                   | thread which creates the          |
    |                                   | CommandThreadFactory.             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ConcurrencyLimit](C              | ::: block                         |
    | oncurrencyLimit.html "class in co | Amalgamation of parameters that   |
    | m.facebook.buck.util.concurrent") | control how many jobs we can run  |
    |                                   | at once.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JobLimi                          | ::: block                         |
    | ter](JobLimiter.html "class in co | JobLimiter is a simple mechanism  |
    | m.facebook.buck.util.concurrent") | for queuing asynchronous work     |
    |                                   | such that only a certain number   |
    |                                   | of items are active at a time.    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [LinkedBlockingStack](LinkedBlo   | ::: block                         |
    | ckingStack.html "class in com.fac | An implementation of              |
    | ebook.buck.util.concurrent")\<E\> | [`BlockingQ                       |
    |                                   | ueue`](http://docs.oracle.com/jav |
    |                                   | ase/7/docs/api/java/util/concurre |
    |                                   | nt/BlockingQueue.html?is-external |
    |                                   | =true "class or interface in java |
    |                                   | .util.concurrent"){.externalLink} |
    |                                   | interface returning elements in   |
    |                                   | LIFO order.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | ListeningMultiSemaphore](Listenin | A semaphore using                 |
    | gMultiSemaphore.html "class in co | `ListenableFuture`s for           |
    | m.facebook.buck.util.concurrent") | acquisition of different resource |
    |                                   | types rather than blocking.       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [MoreAtomi                        | ::: block                         |
    | cs](MoreAtomics.html "class in co | Utility methods for common        |
    | m.facebook.buck.util.concurrent") | routines with atomic variables    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [MoreFutur                        |                                   |
    | es](MoreFutures.html "class in co |                                   |
    | m.facebook.buck.util.concurrent") |                                   |
    +-----------------------------------+-----------------------------------+
    | [MostExecutors                    |                                   |
    | ](MostExecutors.html "class in co |                                   |
    | m.facebook.buck.util.concurrent") |                                   |
    +-----------------------------------+-----------------------------------+
    | [MostExecutors.Name               | ::: block                         |
    | dThreadFactory](MostExecutors.Nam | A ThreadFactory which gives each  |
    | edThreadFactory.html "class in co | thread a meaningful and distinct  |
    | m.facebook.buck.util.concurrent") | name.                             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ResourceAmounts](                |                                   |
    | ResourceAmounts.html "class in co |                                   |
    | m.facebook.buck.util.concurrent") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Re                               |                                   |
    | sourceAmountsEstimator](ResourceA |                                   |
    | mountsEstimator.html "class in co |                                   |
    | m.facebook.buck.util.concurrent") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ResourcePool](                   | ::: block                         |
    | ResourcePool.html "class in com.f | Allows multiple concurrently      |
    | acebook.buck.util.concurrent")\<R | executing futures to share a      |
    | extends                           | constrained number of resources.  |
    | [AutoCloseable](http:/            | :::                               |
    | /docs.oracle.com/javase/7/docs/ap |                                   |
    | i/java/lang/AutoCloseable.html?is |                                   |
    | -external=true "class or interfac |                                   |
    | e in java.lang"){.externalLink}\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [WeightedListeningE               | ::: block                         |
    | xecutorService](WeightedListening | A `ListeningExecutorService`      |
    | ExecutorService.html "class in co | which gates execution using a     |
    | m.facebook.buck.util.concurrent") | [`L                               |
    |                                   | isteningMultiSemaphore`](Listenin |
    |                                   | gMultiSemaphore.html "class in co |
    |                                   | m.facebook.buck.util.concurrent") |
    |                                   | and allows resources to be        |
    |                                   | assigned to submitted tasks.      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Wor                              | ::: block                         |
    | kThreadTrackingTask](WorkThreadTr | A                                 |
    | ackingTask.html "class in com.fac | [`ForkJoi                         |
    | ebook.buck.util.concurrent")\<T\> | nTask`](http://docs.oracle.com/ja |
    |                                   | vase/7/docs/api/java/util/concurr |
    |                                   | ent/ForkJoinTask.html?is-external |
    |                                   | =true "class or interface in java |
    |                                   | .util.concurrent"){.externalLink} |
    |                                   | which keeps track of the thread   |
    |                                   | running its computation.          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Enum                              | Description                       |
    +===================================+===================================+
    | [ExecutorPo                       |                                   |
    | ol](ExecutorPool.html "enum in co |                                   |
    | m.facebook.buck.util.concurrent") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Resou                            | ::: block                         |
    | rceAllocationFairness](ResourceAl | How to handle fairness when       |
    | locationFairness.html "enum in co | acquiring the semaphore.          |
    | m.facebook.buck.util.concurrent") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ResourcePool.ResourceUsageE      | ::: block                         |
    | rrorPolicy](ResourcePool.Resource | Describes how to handle errors    |
    | UsageErrorPolicy.html "enum in co | that take place during resource   |
    | m.facebook.buck.util.concurrent") | usage.                            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Enum Summary[ ]{.tabEnd}
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../../index.html)
-   Package
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

[]{#skip.navbar.bottom}
:::
