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

## Class ListeningMultiSemaphore {#class-listeningmultisemaphore .title title="Class ListeningMultiSemaphore"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.concurrent.ListeningMultiSemaphore

::: description
-   

    ------------------------------------------------------------------------

        public class ListeningMultiSemaphore
        extends Object

    ::: block
    A semaphore using `ListenableFuture`s for acquisition of different
    resource types rather than blocking.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                 Description
          --------------------------------------------------------------------------------------------------------------------------- -------------
          `ListeningMultiSemaphore​(ResourceAmounts availableResources,                        ResourceAllocationFairness fairness)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.google.comm      | `acquire​(Resour       | ::: block             |
        | on.util.concurrent.Li | ceAmounts resources)` | Returns the future    |
        | stenableFuture<Unit>` |                       | which will be         |
        |                       |                       | completed by the      |
        |                       |                       | moment when resources |
        |                       |                       | will be acquired.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ResourceAmounts`     | `get                  |                       |
        |                       | AvailableResources()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ResourceAmounts`     | `getMaximumValues()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getQueueLength()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `release​(Resour       | ::: block             |
        |                       | ceAmounts resources)` | Releases previously   |
        |                       |                       | acquired resources.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

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

        []{#<init>(com.facebook.buck.util.concurrent.ResourceAmounts,com.facebook.buck.util.concurrent.ResourceAllocationFairness)}

        -   #### ListeningMultiSemaphore

                public ListeningMultiSemaphore​(ResourceAmounts availableResources,
                                               ResourceAllocationFairness fairness)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#acquire(com.facebook.buck.util.concurrent.ResourceAmounts)}

        -   #### acquire

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<Unit> acquire​(ResourceAmounts resources)
            ```

            ::: block
            Returns the future which will be completed by the moment
            when resources will be acquired. Future may be returned
            already completed. You should subscribe to the future and
            perform your resource requiring job once the future will be
            completed and not cancelled. When you finish your job, you
            must release acquired resources by calling release() method
            below.
            :::

            [Parameters:]{.paramLabel}
            :   `resources` - Resource amounts that need to be acquired.
                If they are higher than maximum amounts, they will be
                capped to them.

            [Returns:]{.returnLabel}
            :   Future that will be completed once resource will be
                acquired.

        []{#release(com.facebook.buck.util.concurrent.ResourceAmounts)}

        -   #### release

            ``` methodSignature
            public void release​(ResourceAmounts resources)
            ```

            ::: block
            Releases previously acquired resources.
            :::

            [Parameters:]{.paramLabel}
            :   `resources` - Resource amounts that need to be released.
                This argument should match one you used during resource
                acquiring.

        []{#getAvailableResources()}

        -   #### getAvailableResources

            ``` methodSignature
            public ResourceAmounts getAvailableResources()
            ```

        []{#getMaximumValues()}

        -   #### getMaximumValues

            ``` methodSignature
            public ResourceAmounts getMaximumValues()
            ```

        []{#getQueueLength()}

        -   #### getQueueLength

            ``` methodSignature
            public int getQueueLength()
            ```
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
