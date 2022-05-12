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
-   [Nested](#nested.class.summary) \| 
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

## Interface RemoteExecutionServiceClient {#interface-remoteexecutionserviceclient .title title="Interface RemoteExecutionServiceClient"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `GrpcRemoteExecutionServiceClient`

    ------------------------------------------------------------------------

        public interface RemoteExecutionServiceClient

    ::: block
    Interface for a client of the remote execution service. Used by
    RemoteExecution to build rules.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Interface             | Description           |
        +=======================+=======================+=======================+
        | `static interface `   | `Rem                  | ::: block             |
        |                       | oteExecutionServiceCl | Handle for an         |
        |                       | ient.ExecutionHandle` | execution in          |
        |                       |                       | progress.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static interface `   | `Rem                  | ::: block             |
        |                       | oteExecutionServiceCl | Represents the result |
        |                       | ient.ExecutionResult` | of remote execution.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Rem                  | `execute​(Protocol.Dig | ::: block             |
        | oteExecutionServiceCl | est actionDigest,     | This should run the   |
        | ient.ExecutionHandle` |     String ruleName,  | command with the      |
        |                       |        MetadataProvid | provided environment  |
        |                       | er metadataProvider)` | and inputs.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

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

        []{#execute(com.facebook.buck.remoteexecution.interfaces.Protocol.Digest,java.lang.String,com.facebook.buck.remoteexecution.interfaces.MetadataProvider)}

        -   #### execute

            ``` methodSignature
            RemoteExecutionServiceClient.ExecutionHandle execute​(Protocol.Digest actionDigest,
                                                                 String ruleName,
                                                                 MetadataProvider metadataProvider)
                                                          throws IOException,
                                                                 InterruptedException
            ```

            ::: block
            This should run the command with the provided environment
            and inputs.
            Returns an ActionResult with exit code, outputs,
            stdout/stderr, etc.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `InterruptedException`
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
-   [Nested](#nested.class.summary) \| 
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
