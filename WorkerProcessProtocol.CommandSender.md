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

## Interface WorkerProcessProtocol.CommandSender {#interface-workerprocessprotocol.commandsender .title title="Interface WorkerProcessProtocol.CommandSender"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AutoCloseable`, `Closeable`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `WorkerProcessProtocolZero.CommandSender`

    ```{=html}
    <!-- -->
    ```

    Enclosing interface:
    :   [WorkerProcessProtocol](WorkerProcessProtocol.html "interface in com.facebook.buck.worker")

    ------------------------------------------------------------------------

        public static interface WorkerProcessProtocol.CommandSender
        extends Closeable
:::

::: summary
-   ::: {.section role="region"}
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
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#handshake(int)}

        -   #### handshake

            ``` methodSignature
            void handshake​(int messageId)
                    throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#send(int,com.facebook.buck.worker.WorkerProcessCommand)}

        -   #### send

            ``` methodSignature
            void send​(int messageId,
                      com.facebook.buck.worker.WorkerProcessCommand command)
               throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#receiveNextCommandResponse()}

        -   #### receiveNextCommandResponse

            ``` methodSignature
            WorkerProcessProtocol.CommandResponse receiveNextCommandResponse()
                                                                      throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#close()}

        -   #### close

            ``` methodSignature
            void close()
                throws IOException
            ```

            ::: block
            Instructs the CommandReceiver to shut itself down.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `Closeable`

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
