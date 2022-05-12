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
[Package]{.packageLabelInType} [com.facebook.buck.worker](package-summary.html)
:::

## Class WorkerProcessProtocolZero.CommandSender {#class-workerprocessprotocolzero.commandsender .title title="Class WorkerProcessProtocolZero.CommandSender"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.worker.WorkerProcessProtocolZero.CommandSender

::: description
-   

    All Implemented Interfaces:
    :   `WorkerProcessProtocol.CommandSender`, `Closeable`,
        `AutoCloseable`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [WorkerProcessProtocolZero](WorkerProcessProtocolZero.html "class in com.facebook.buck.worker")

    ------------------------------------------------------------------------

        public static class WorkerProcessProtocolZero.CommandSender
        extends Object
        implements WorkerProcessProtocol.CommandSender
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                              Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `CommandSender​(OutputStream processStdin,              InputStream processStdout,              Path stdErr,              Runnable onClose,              java.util.function.Supplier<Boolean> isAlive)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `close()`             | ::: block             |
        |                       |                       | Instructs the         |
        |                       |                       | CommandReceiver to    |
        |                       |                       | shut itself down.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `hand                 |                       |
        |                       | shake​(int messageId)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `WorkerProcessProt    | `receiveN             |                       |
        | ocol.CommandResponse` | extCommandResponse()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `send​(int message     |                       |
        |                       | Id,     com.facebook. |                       |
        |                       | buck.worker.WorkerPro |                       |
        |                       | cessCommand command)` |                       |
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

        []{#<init>(java.io.OutputStream,java.io.InputStream,java.nio.file.Path,java.lang.Runnable,java.util.function.Supplier)}

        -   #### CommandSender

                public CommandSender​(OutputStream processStdin,
                                     InputStream processStdout,
                                     Path stdErr,
                                     Runnable onClose,
                                     java.util.function.Supplier<Boolean> isAlive)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#handshake(int)}

        -   #### handshake

            ``` methodSignature
            public void handshake​(int messageId)
                           throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `handshake` in
                interface `WorkerProcessProtocol.CommandSender`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#send(int,com.facebook.buck.worker.WorkerProcessCommand)}

        -   #### send

            ``` methodSignature
            public void send​(int messageId,
                             com.facebook.buck.worker.WorkerProcessCommand command)
                      throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `send` in
                interface `WorkerProcessProtocol.CommandSender`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#receiveNextCommandResponse()}

        -   #### receiveNextCommandResponse

            ``` methodSignature
            public WorkerProcessProtocol.CommandResponse receiveNextCommandResponse()
                                                                             throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `receiveNextCommandResponse` in
                interface `WorkerProcessProtocol.CommandSender`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
                       throws IOException
            ```

            ::: block
            [Description copied from
            interface: `WorkerProcessProtocol.CommandSender`]{.descfrmTypeLabel}
            :::

            ::: block
            Instructs the CommandReceiver to shut itself down.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `Closeable`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in
                interface `WorkerProcessProtocol.CommandSender`

            [Throws:]{.throwsLabel}
            :   `IOException`
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
