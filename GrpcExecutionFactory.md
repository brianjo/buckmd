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

## Class GrpcExecutionFactory {#class-grpcexecutionfactory .title title="Class GrpcExecutionFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.remoteexecution.grpc.GrpcExecutionFactory

::: description
-   

    ------------------------------------------------------------------------

        public class GrpcExecutionFactory
        extends Object

    ::: block
    Factory for creating grpc-based strategies.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                        Description
          ------------------- ---------------------------- -------------
          `static int`        `MAX_INBOUND_MESSAGE_SIZE`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                Description
          -------------------------- -------------
          `GrpcExecutionFactory()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Re            | `createInProcess​(Buck | ::: block             |
        | moteExecutionClients` | EventBus buckEventBus | The in-process        |
        |                       | ,                Remo | strategy starts up a  |
        |                       | teExecutionStrategyCo | grpc remote execution |
        |                       | nfig strategyConfig)` | service in process    |
        |                       |                       | and connects to it    |
        |                       |                       | directly.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Re            | `createRemote​(        | ::: block             |
        | moteExecutionClients` | String executionEngin | The remote strategy   |
        |                       | eHost,             in | connects to a remote  |
        |                       | t executionEnginePort | grpc remote execution |
        |                       | ,             String  | service.              |
        |                       | casHost,              | :::                   |
        |                       | int casPort,          |                       |
        |                       |     int casDeadline,  |                       |
        |                       |             boolean i |                       |
        |                       | nsecure,              |                       |
        |                       | boolean casInsecure,  |                       |
        |                       |             Optional< |                       |
        |                       | Path> certPath,       |                       |
        |                       |        Optional<Path> |                       |
        |                       |  keyPath,             |                       |
        |                       |  Optional<Path> caPat |                       |
        |                       | h,             Remote |                       |
        |                       | ExecutionStrategyConf |                       |
        |                       | ig strategyConfig,    |                       |
        |                       |           MetadataPro |                       |
        |                       | vider metadataProvide |                       |
        |                       | r,             BuckEv |                       |
        |                       | entBus buckEventBus)` |                       |
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
    -   []{#field.detail}

        ### Field Detail

        []{#MAX_INBOUND_MESSAGE_SIZE}

        -   #### MAX_INBOUND_MESSAGE_SIZE

                public static final int MAX_INBOUND_MESSAGE_SIZE

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.remoteexecution.grpc.GrpcExecutionFactory.MAX_INBOUND_MESSAGE_SIZE)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### GrpcExecutionFactory

                public GrpcExecutionFactory()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createInProcess(com.facebook.buck.event.BuckEventBus,com.facebook.buck.remoteexecution.config.RemoteExecutionStrategyConfig)}

        -   #### createInProcess

            ``` methodSignature
            public static RemoteExecutionClients createInProcess​(BuckEventBus buckEventBus,
                                                                 RemoteExecutionStrategyConfig strategyConfig)
                                                          throws IOException
            ```

            ::: block
            The in-process strategy starts up a grpc remote execution
            service in process and connects to it directly.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#createRemote(java.lang.String,int,java.lang.String,int,int,boolean,boolean,java.util.Optional,java.util.Optional,java.util.Optional,com.facebook.buck.remoteexecution.config.RemoteExecutionStrategyConfig,com.facebook.buck.remoteexecution.interfaces.MetadataProvider,com.facebook.buck.event.BuckEventBus)}

        -   #### createRemote

            ``` methodSignature
            public static RemoteExecutionClients createRemote​(String executionEngineHost,
                                                              int executionEnginePort,
                                                              String casHost,
                                                              int casPort,
                                                              int casDeadline,
                                                              boolean insecure,
                                                              boolean casInsecure,
                                                              Optional<Path> certPath,
                                                              Optional<Path> keyPath,
                                                              Optional<Path> caPath,
                                                              RemoteExecutionStrategyConfig strategyConfig,
                                                              MetadataProvider metadataProvider,
                                                              BuckEventBus buckEventBus)
                                                       throws SSLException
            ```

            ::: block
            The remote strategy connects to a remote grpc remote
            execution service.
            :::

            [Throws:]{.throwsLabel}
            :   `SSLException`
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
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
