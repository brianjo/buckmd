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

## Interface WorkerJobParams {#interface-workerjobparams .title title="Interface WorkerJobParams"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface WorkerJobParams
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `String`              | `getJobArgs()`        | ::: block             |
        |                       |                       | The arguments of the  |
        |                       |                       | actual job once tool  |
        |                       |                       | has started and ready |
        |                       |                       | to accept jobs.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `WorkerProcessParams` | `getW                 |                       |
        |                       | orkerProcessParams()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `of​(String jobArgs,   |                       |
        | atic WorkerJobParams` |  WorkerProcessParams  |                       |
        |                       | workerProcessParams)` |                       |
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

        []{#getJobArgs()}

        -   #### getJobArgs

            ``` methodSignature
            String getJobArgs()
            ```

            ::: block
            The arguments of the actual job once tool has started and
            ready to accept jobs. For example, \"\--hash-file
            /path/to/file\".
            :::

        []{#getWorkerProcessParams()}

        -   #### getWorkerProcessParams

            ``` methodSignature
            WorkerProcessParams getWorkerProcessParams()
            ```

        []{#of(java.lang.String,com.facebook.buck.worker.WorkerProcessParams)}

        -   #### of

            ``` methodSignature
            static WorkerJobParams of​(String jobArgs,
                                      WorkerProcessParams workerProcessParams)
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
