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
-   Nested \| 
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   Method

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

## Class ConcurrencyLimit {#class-concurrencylimit .title title="Class ConcurrencyLimit"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.concurrent.ConcurrencyLimit

::: description
-   

    ------------------------------------------------------------------------

        public class ConcurrencyLimit
        extends Object

    ::: block
    Amalgamation of parameters that control how many jobs we can run at
    once.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `ResourceAmounts`     | `defaultAmounts`      | ::: block             |
        |                       |                       | Default resource      |
        |                       |                       | amounts that job      |
        |                       |                       | would require.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `managedThreadCount`  | ::: block             |
        |                       |                       | Number of threads     |
        |                       |                       | that Buck can manage  |
        |                       |                       | and use them as       |
        |                       |                       | worker threads.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ResourceAmounts`     | `maximumAmounts`      | ::: block             |
        |                       |                       | Maximum resource      |
        |                       |                       | amounts that are      |
        |                       |                       | available on the      |
        |                       |                       | system for all jobs   |
        |                       |                       | to share.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Resour               | `resour               |                       |
        | ceAllocationFairness` | ceAllocationFairness` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `threadLimit`         | ::: block             |
        |                       |                       | Considered as number  |
        |                       |                       | of build threads that |
        |                       |                       | are available for     |
        |                       |                       | extensive             |
        |                       |                       | computations.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                          Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `ConcurrencyLimit​(int threadLimit,                 ResourceAllocationFairness resourceAllocationFairness,                 int managedThreadCount,                 ResourceAmounts defaultAmounts,                 ResourceAmounts maximumAmounts)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#threadLimit}

        -   #### threadLimit

                public final int threadLimit

            ::: block
            Considered as number of build threads that are available for
            extensive computations.
            :::

        []{#resourceAllocationFairness}

        -   #### resourceAllocationFairness

                public final ResourceAllocationFairness resourceAllocationFairness

        []{#managedThreadCount}

        -   #### managedThreadCount

                public final int managedThreadCount

            ::: block
            Number of threads that Buck can manage and use them as
            worker threads. This number includes
            [`threadLimit`](#threadLimit) value. The rest of the threads
            may be used for lightweight tasks, I/O blocking tasks, etc.
            :::

        []{#defaultAmounts}

        -   #### defaultAmounts

                public final ResourceAmounts defaultAmounts

            ::: block
            Default resource amounts that job would require.
            :::

        []{#maximumAmounts}

        -   #### maximumAmounts

                public final ResourceAmounts maximumAmounts

            ::: block
            Maximum resource amounts that are available on the system
            for all jobs to share.
            :::
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(int,com.facebook.buck.util.concurrent.ResourceAllocationFairness,int,com.facebook.buck.util.concurrent.ResourceAmounts,com.facebook.buck.util.concurrent.ResourceAmounts)}

        -   #### ConcurrencyLimit

                public ConcurrencyLimit​(int threadLimit,
                                        ResourceAllocationFairness resourceAllocationFairness,
                                        int managedThreadCount,
                                        ResourceAmounts defaultAmounts,
                                        ResourceAmounts maximumAmounts)
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
-   Nested \| 
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   Method

</div>

[]{#skip.navbar.bottom}
:::
