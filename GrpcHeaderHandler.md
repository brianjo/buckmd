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
[Package]{.packageLabelInType} [com.facebook.buck.remoteexecution.grpc](package-summary.html)
:::

## Class GrpcHeaderHandler {#class-grpcheaderhandler .title title="Class GrpcHeaderHandler"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.remoteexecution.grpc.GrpcHeaderHandler

::: description
-   

    ------------------------------------------------------------------------

        public class GrpcHeaderHandler
        extends Object

    ::: block
    Provides operations over GRPC headers.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static interface `   | `Grpc                 | ::: block             |
        |                       | HeaderHandler.StubAnd | Class that contains   |
        |                       | ResponseMetadata<Stub | the GRPC stub and any |
        |                       |  extends io.grpc.stub | Re                    |
        |                       | .AbstractStub<Stub>>` | moteExecutionMetadata |
        |                       |                       | returned in the GRPC  |
        |                       |                       | response.             |
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
        | `static <Stub exte    | `wrapStubToReceiveMet | ::: block             |
        | nds io.grpc.stub.Abst | adata​(Stub grpcStub)` | Receives              |
        | ractStub<Stub>>GrpcHe |                       | Re                    |
        | aderHandler.StubAndRe |                       | moteExecutionMetadata |
        | sponseMetadata<Stub>` |                       | from the initial GRPC |
        |                       |                       | headers.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static <Stub exte    | `wrapStubToSen        | ::: block             |
        | nds io.grpc.stub.Abst | dAndReceiveMetadata​(S | Convenience function  |
        | ractStub<Stub>>GrpcHe | tub grpcStub,         | to wrap the GRPC Stub |
        | aderHandler.StubAndRe |                       | for both receiving    |
        | sponseMetadata<Stub>` |     com.facebook.buck | and sending metadata. |
        |                       | .remoteexecution.prot | :::                   |
        |                       | o.RemoteExecutionMeta |                       |
        |                       | data metadataToSend)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <Stub ext     | `wrapStub             | ::: block             |
        | ends io.grpc.stub.Abs | ToSendMetadata​(Stub g | Appends               |
        | tractStub<Stub>>Stub` | rpcStub,              | Re                    |
        |                       |           com.faceboo | moteExecutionMetadata |
        |                       | k.buck.remoteexecutio | to the GRPC headers.  |
        |                       | n.proto.RemoteExecuti | :::                   |
        |                       | onMetadata metadata)` |                       |
        +-----------------------+-----------------------+-----------------------+

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
    -   []{#method.detail}

        ### Method Detail

        []{#wrapStubToSendAndReceiveMetadata(io.grpc.stub.AbstractStub,com.facebook.buck.remoteexecution.proto.RemoteExecutionMetadata)}
        []{#wrapStubToSendAndReceiveMetadata(Stub,com.facebook.buck.remoteexecution.proto.RemoteExecutionMetadata)}

        -   #### wrapStubToSendAndReceiveMetadata

            ``` methodSignature
            public static <Stub extends io.grpc.stub.AbstractStub<Stub>> GrpcHeaderHandler.StubAndResponseMetadata<Stub> wrapStubToSendAndReceiveMetadata​(Stub grpcStub,
                                                                                                                                                          com.facebook.buck.remoteexecution.proto.RemoteExecutionMetadata metadataToSend)
            ```

            ::: block
            Convenience function to wrap the GRPC Stub for both
            receiving and sending metadata.
            :::

        []{#wrapStubToSendMetadata(io.grpc.stub.AbstractStub,com.facebook.buck.remoteexecution.proto.RemoteExecutionMetadata)}
        []{#wrapStubToSendMetadata(Stub,com.facebook.buck.remoteexecution.proto.RemoteExecutionMetadata)}

        -   #### wrapStubToSendMetadata

            ``` methodSignature
            public static <Stub extends io.grpc.stub.AbstractStub<Stub>> Stub wrapStubToSendMetadata​(Stub grpcStub,
                                                                                                     com.facebook.buck.remoteexecution.proto.RemoteExecutionMetadata metadata)
            ```

            ::: block
            Appends RemoteExecutionMetadata to the GRPC headers.
            :::

        []{#wrapStubToReceiveMetadata(io.grpc.stub.AbstractStub)}
        []{#wrapStubToReceiveMetadata(Stub)}

        -   #### wrapStubToReceiveMetadata

            ``` methodSignature
            public static <Stub extends io.grpc.stub.AbstractStub<Stub>> GrpcHeaderHandler.StubAndResponseMetadata<Stub> wrapStubToReceiveMetadata​(Stub grpcStub)
            ```

            ::: block
            Receives RemoteExecutionMetadata from the initial GRPC
            headers.
            :::
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
