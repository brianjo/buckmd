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

## Interface RemoteExecutionServiceClient.ExecutionResult {#interface-remoteexecutionserviceclient.executionresult .title title="Interface RemoteExecutionServiceClient.ExecutionResult"}
:::

::: contentContainer
::: description
-   

    Enclosing interface:
    :   [RemoteExecutionServiceClient](RemoteExecutionServiceClient.html "interface in com.facebook.buck.remoteexecution")

    ------------------------------------------------------------------------

        public static interface RemoteExecutionServiceClient.ExecutionResult

    ::: block
    Represents the result of remote execution.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                   Method                           Description
          ------------------------------------------------------------------- -------------------------------- -------------
          `build.bazel.remote.execution.v2.ExecutedActionMetadata`            `getActionMetadata()`             
          `Protocol.Digest`                                                   `getActionResultDigest()`         
          `int`                                                               `getExitCode()`                   
          `List<Protocol.OutputDirectory>`                                    `getOutputDirectories()`          
          `List<Protocol.OutputFile>`                                         `getOutputFiles()`                
          `com.facebook.buck.remoteexecution.proto.RemoteExecutionMetadata`   `getRemoteExecutionMetadata()`    
          `Optional<String>`                                                  `getStderr()`                     
          `Optional<String>`                                                  `getStdout()`                     

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

        []{#getRemoteExecutionMetadata()}

        -   #### getRemoteExecutionMetadata

            ``` methodSignature
            com.facebook.buck.remoteexecution.proto.RemoteExecutionMetadata getRemoteExecutionMetadata()
            ```

        []{#getOutputDirectories()}

        -   #### getOutputDirectories

            ``` methodSignature
            List<Protocol.OutputDirectory> getOutputDirectories()
            ```

        []{#getOutputFiles()}

        -   #### getOutputFiles

            ``` methodSignature
            List<Protocol.OutputFile> getOutputFiles()
            ```

        []{#getExitCode()}

        -   #### getExitCode

            ``` methodSignature
            int getExitCode()
            ```

        []{#getStdout()}

        -   #### getStdout

            ``` methodSignature
            Optional<String> getStdout()
            ```

        []{#getStderr()}

        -   #### getStderr

            ``` methodSignature
            Optional<String> getStderr()
            ```

        []{#getActionResultDigest()}

        -   #### getActionResultDigest

            ``` methodSignature
            Protocol.Digest getActionResultDigest()
            ```

        []{#getActionMetadata()}

        -   #### getActionMetadata

            ``` methodSignature
            build.bazel.remote.execution.v2.ExecutedActionMetadata getActionMetadata()
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
