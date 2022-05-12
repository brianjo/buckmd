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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.util.concurrent](package-summary.html)
:::

## Class ResourceAmountsEstimator {#class-resourceamountsestimator .title title="Class ResourceAmountsEstimator"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.concurrent.ResourceAmountsEstimator

::: description
-   

    ------------------------------------------------------------------------

        public class ResourceAmountsEstimator
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `st                   | `DEFAULT_AMOUNTS`     |                       |
        | atic ResourceAmounts` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static int`          | `DEFAULT_CPU_AMOUNT`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static int`          | `DEFAULT_CPU_CAP`     | ::: block             |
        |                       |                       | CPU resource amount   |
        |                       |                       | is considered as      |
        |                       |                       | number of cores.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static int`          | `DE                   |                       |
        |                       | FAULT_DISK_IO_AMOUNT` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static int`          | `DEFAULT_DISK_IO_CAP` | ::: block             |
        |                       |                       | Disk IO resource unit |
        |                       |                       | size has been chosen  |
        |                       |                       | arbitrarily.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static int`          | `DEFAULT_             | ::: block             |
        |                       | MANAGED_THREAD_COUNT` | Total number of       |
        |                       |                       | threads Buck can use  |
        |                       |                       | to schedule various   |
        |                       |                       | work.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `DEF                  |                       |
        | atic ResourceAmounts` | AULT_MAXIMUM_AMOUNTS` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static int`          | `D                    |                       |
        |                       | EFAULT_MEMORY_AMOUNT` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static int`          | `DEFAULT_MEMORY_CAP`  | ::: block             |
        |                       |                       | Memory resource unit  |
        |                       |                       | size has been chosen  |
        |                       |                       | arbitrarily.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static int`          | `DEFAU                |                       |
        |                       | LT_NETWORK_IO_AMOUNT` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static int`          | `DE                   | ::: block             |
        |                       | FAULT_NETWORK_IO_CAP` | Network IO resource   |
        |                       |                       | unit size has been    |
        |                       |                       | chosen arbitrarily.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type          Method                    Description
          -------------------------- ------------------------- -------------
          `static ResourceAmounts`   `getEstimatedAmounts()`    

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
    -   []{#field.detail}

        ### Field Detail

        []{#DEFAULT_CPU_CAP}

        -   #### DEFAULT_CPU_CAP

                public static final int DEFAULT_CPU_CAP

            ::: block
            CPU resource amount is considered as number of cores. Each
            core can perform a single job.
            :::

        []{#DEFAULT_MEMORY_CAP}

        -   #### DEFAULT_MEMORY_CAP

                public static final int DEFAULT_MEMORY_CAP

            ::: block
            Memory resource unit size has been chosen arbitrarily. We
            can tune the value if we need.
            :::

        []{#DEFAULT_DISK_IO_CAP}

        -   #### DEFAULT_DISK_IO_CAP

                public static final int DEFAULT_DISK_IO_CAP

            ::: block
            Disk IO resource unit size has been chosen arbitrarily.
            Since most of the jobs are light, we think disk can handle
            this amount of light jobs: reading/writing some small data.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.concurrent.ResourceAmountsEstimator.DEFAULT_DISK_IO_CAP)

        []{#DEFAULT_NETWORK_IO_CAP}

        -   #### DEFAULT_NETWORK_IO_CAP

                public static final int DEFAULT_NETWORK_IO_CAP

            ::: block
            Network IO resource unit size has been chosen arbitrarily.
            Since most of the jobs are light, we think network can
            handle this amount of light jobs: sending/receiving some
            small data.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.concurrent.ResourceAmountsEstimator.DEFAULT_NETWORK_IO_CAP)

        []{#DEFAULT_MAXIMUM_AMOUNTS}

        -   #### DEFAULT_MAXIMUM_AMOUNTS

                public static final ResourceAmounts DEFAULT_MAXIMUM_AMOUNTS

        []{#DEFAULT_MANAGED_THREAD_COUNT}

        -   #### DEFAULT_MANAGED_THREAD_COUNT

                public static final int DEFAULT_MANAGED_THREAD_COUNT

            ::: block
            Total number of threads Buck can use to schedule various
            work.
            :::

        []{#DEFAULT_CPU_AMOUNT}

        -   #### DEFAULT_CPU_AMOUNT

                public static final int DEFAULT_CPU_AMOUNT

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.concurrent.ResourceAmountsEstimator.DEFAULT_CPU_AMOUNT)

        []{#DEFAULT_MEMORY_AMOUNT}

        -   #### DEFAULT_MEMORY_AMOUNT

                public static final int DEFAULT_MEMORY_AMOUNT

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.concurrent.ResourceAmountsEstimator.DEFAULT_MEMORY_AMOUNT)

        []{#DEFAULT_DISK_IO_AMOUNT}

        -   #### DEFAULT_DISK_IO_AMOUNT

                public static final int DEFAULT_DISK_IO_AMOUNT

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.concurrent.ResourceAmountsEstimator.DEFAULT_DISK_IO_AMOUNT)

        []{#DEFAULT_NETWORK_IO_AMOUNT}

        -   #### DEFAULT_NETWORK_IO_AMOUNT

                public static final int DEFAULT_NETWORK_IO_AMOUNT

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.concurrent.ResourceAmountsEstimator.DEFAULT_NETWORK_IO_AMOUNT)

        []{#DEFAULT_AMOUNTS}

        -   #### DEFAULT_AMOUNTS

                public static final ResourceAmounts DEFAULT_AMOUNTS
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getEstimatedAmounts()}

        -   #### getEstimatedAmounts

            ``` methodSignature
            public static ResourceAmounts getEstimatedAmounts()
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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
