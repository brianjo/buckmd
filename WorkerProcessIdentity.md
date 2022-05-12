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
[Package]{.packageLabelInType} [com.facebook.buck.worker](package-summary.html)
:::

## Interface WorkerProcessIdentity {#interface-workerprocessidentity .title title="Interface WorkerProcessIdentity"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface WorkerProcessIdentity
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `String`              | `getP                 | ::: block             |
        |                       | ersistentWorkerKey()` | If the current        |
        |                       |                       | invocation allows to  |
        |                       |                       | have persisted worker |
        |                       |                       | pools (buck is        |
        |                       |                       | running as daemon),   |
        |                       |                       | it will be used to    |
        |                       |                       | obtain the instance   |
        |                       |                       | of the persisted      |
        |                       |                       | worker process pool.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getWorkerHash()`     | ::: block             |
        | common.hash.HashCode` |                       | Hash to identify the  |
        |                       |                       | specific worker pool  |
        |                       |                       | and kind of a         |
        |                       |                       | mechanism for         |
        |                       |                       | invalidating existing |
        |                       |                       | pools.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static W             | `of​(String pers       |                       |
        | orkerProcessIdentity` | istentWorkerKey,   co |                       |
        |                       | m.google.common.hash. |                       |
        |                       | HashCode workerHash)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getPersistentWorkerKey()}

        -   #### getPersistentWorkerKey

            ``` methodSignature
            String getPersistentWorkerKey()
            ```

            ::: block
            If the current invocation allows to have persisted worker
            pools (buck is running as daemon), it will be used to obtain
            the instance of the persisted worker process pool.
            :::

        []{#getWorkerHash()}

        -   #### getWorkerHash

            ``` methodSignature
            com.google.common.hash.HashCode getWorkerHash()
            ```

            ::: block
            Hash to identify the specific worker pool and kind of a
            mechanism for invalidating existing pools. If this value for
            the given persistent worker key changes, old pool will be
            destroyed and the new pool will be recreated.
            :::

        []{#of(java.lang.String,com.google.common.hash.HashCode)}

        -   #### of

            ``` methodSignature
            static WorkerProcessIdentity of​(String persistentWorkerKey,
                                            com.google.common.hash.HashCode workerHash)
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
