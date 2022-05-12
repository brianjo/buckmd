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
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.remoteexecution.grpc](package-summary.html)
:::

## Class GrpcRemoteExecutionServiceClient {#class-grpcremoteexecutionserviceclient .title title="Class GrpcRemoteExecutionServiceClient"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.remoteexecution.grpc.GrpcRemoteExecutionServiceClient

::: description
-   

    All Implemented Interfaces:
    :   `RemoteExecutionServiceClient`

    ------------------------------------------------------------------------

        public class GrpcRemoteExecutionServiceClient
        extends Object
        implements RemoteExecutionServiceClient

    ::: block
    Implementation of the GRPC client for the Remote Execution service.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.remoteexecution.RemoteExecutionServiceClient}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.remoteexecution.[RemoteExecutionServiceClient](../RemoteExecutionServiceClient.html "interface in com.facebook.buck.remoteexecution")

            `RemoteExecutionServiceClient.ExecutionHandle, RemoteExecutionServiceClient.ExecutionResult`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                  Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `GrpcRemoteExecutionServiceClient​(build.bazel.remote.execution.v2.ExecutionGrpc.ExecutionStub executionStub,                                 com.google.bytestream.ByteStreamGrpc.ByteStreamStub byteStreamStub,                                 String instanceName,                                 Protocol protocol,                                 int casDeadline)`    

          : Constructors[ ]{.tabEnd}
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

        []{#<init>(build.bazel.remote.execution.v2.ExecutionGrpc.ExecutionStub,com.google.bytestream.ByteStreamGrpc.ByteStreamStub,java.lang.String,com.facebook.buck.remoteexecution.interfaces.Protocol,int)}

        -   #### GrpcRemoteExecutionServiceClient

                public GrpcRemoteExecutionServiceClient​(build.bazel.remote.execution.v2.ExecutionGrpc.ExecutionStub executionStub,
                                                        com.google.bytestream.ByteStreamGrpc.ByteStreamStub byteStreamStub,
                                                        String instanceName,
                                                        Protocol protocol,
                                                        int casDeadline)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#execute(com.facebook.buck.remoteexecution.interfaces.Protocol.Digest,java.lang.String,com.facebook.buck.remoteexecution.interfaces.MetadataProvider)}

        -   #### execute

            ``` methodSignature
            public RemoteExecutionServiceClient.ExecutionHandle execute​(Protocol.Digest actionDigest,
                                                                        String ruleName,
                                                                        MetadataProvider metadataProvider)
                                                                 throws IOException,
                                                                        InterruptedException
            ```

            ::: block
            [Description copied from
            interface: `RemoteExecutionServiceClient`]{.descfrmTypeLabel}
            :::

            ::: block
            This should run the command with the provided environment
            and inputs.
            Returns an ActionResult with exit code, outputs,
            stdout/stderr, etc.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `execute` in interface `RemoteExecutionServiceClient`

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
-   [Nested](#nested.class.summary) \| 
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
