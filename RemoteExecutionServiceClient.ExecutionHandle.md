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
[Package]{.packageLabelInType} [com.facebook.buck.remoteexecution](package-summary.html)
:::

## Interface RemoteExecutionServiceClient.ExecutionHandle {#interface-remoteexecutionserviceclient.executionhandle .title title="Interface RemoteExecutionServiceClient.ExecutionHandle"}
:::

::: contentContainer
::: description
-   

    Enclosing interface:
    :   [RemoteExecutionServiceClient](RemoteExecutionServiceClient.html "interface in com.facebook.buck.remoteexecution")

    ------------------------------------------------------------------------

        public static interface RemoteExecutionServiceClient.ExecutionHandle

    ::: block
    Handle for an execution in progress.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                                                Method                    Description
          ---------------------------------------------------------------------------------------------------------------- ------------------------- -------------
          `void`                                                                                                           `cancel()`                 
          `com.google.common.util.concurrent.ListenableFuture<build.bazel.remote.execution.v2.ExecuteOperationMetadata>`   `getExecutionStarted()`    
          `com.google.common.util.concurrent.ListenableFuture<RemoteExecutionServiceClient.ExecutionResult>`               `getResult()`              

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getResult()}

        -   #### getResult

            ``` methodSignature
            com.google.common.util.concurrent.ListenableFuture<RemoteExecutionServiceClient.ExecutionResult> getResult()
            ```

        []{#getExecutionStarted()}

        -   #### getExecutionStarted

            ``` methodSignature
            com.google.common.util.concurrent.ListenableFuture<build.bazel.remote.execution.v2.ExecuteOperationMetadata> getExecutionStarted()
            ```

        []{#cancel()}

        -   #### cancel

            ``` methodSignature
            void cancel()
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
