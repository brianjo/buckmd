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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.util](package-summary.html)
:::

## Interface ListeningProcessExecutor.LaunchedProcess {#interface-listeningprocessexecutor.launchedprocess .title title="Interface ListeningProcessExecutor.LaunchedProcess"}
:::

::: contentContainer
::: description
-   

    Enclosing class:
    :   [ListeningProcessExecutor](ListeningProcessExecutor.html "class in com.facebook.buck.util")

    ------------------------------------------------------------------------

        public static interface ListeningProcessExecutor.LaunchedProcess

    ::: block
    Represents a process which was launched by a
    [`ListeningProcessExecutor`](ListeningProcessExecutor.html "class in com.facebook.buck.util").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `static int`          | `BUFFER_CAPACITY`     | ::: block             |
        |                       |                       | The capacity of each  |
        |                       |                       | I/O buffer, in bytes. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `close                | ::: block             |
        |                       | Stdin​(boolean force)` | Closes the stdin of   |
        |                       |                       | the process.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `hasPendingWrites()`  | ::: block             |
        |                       |                       | Returns `true` if the |
        |                       |                       | process has any data  |
        |                       |                       | queued to write to    |
        |                       |                       | stdin, `false`        |
        |                       |                       | otherwise.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isRunning()`         | ::: block             |
        |                       |                       | Returns `true` if the |
        |                       |                       | process is running,   |
        |                       |                       | `false` otherwise.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `wantWrite()`         | ::: block             |
        |                       |                       | Invoke this to        |
        |                       |                       | indicate you wish to  |
        |                       |                       | write to the launched |
        |                       |                       | process\'s stdin.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `writeStdi            | ::: block             |
        |                       | n​(ByteBuffer buffer)` | Invoke this to        |
        |                       |                       | directly write data   |
        |                       |                       | to the launched       |
        |                       |                       | process\'s stdin.     |
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
    -   []{#field.detail}

        ### Field Detail

        []{#BUFFER_CAPACITY}

        -   #### BUFFER_CAPACITY

                static final int BUFFER_CAPACITY

            ::: block
            The capacity of each I/O buffer, in bytes.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.util.ListeningProcessExecutor.LaunchedProcess.BUFFER_CAPACITY)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#wantWrite()}

        -   #### wantWrite

            ``` methodSignature
            void wantWrite()
            ```

            ::: block
            Invoke this to indicate you wish to write to the launched
            process\'s stdin.
            Your
            [`ListeningProcessExecutor.ProcessListener.onStdinReady(ByteBuffer)`](ListeningProcessExecutor.ProcessListener.html#onStdinReady(java.nio.ByteBuffer))
            method will be invoked asynchronously when the process is
            ready to receive data on stdin.
            :::

        []{#writeStdin(java.nio.ByteBuffer)}

        -   #### writeStdin

            ``` methodSignature
            void writeStdin​(ByteBuffer buffer)
            ```

            ::: block
            Invoke this to directly write data to the launched
            process\'s stdin. This method does not block, and will
            enqueue the buffer to be written to the launched process\'s
            stdin at a later date.
            If you need to be notified when the write to stdin
            completes, use [`wantWrite()`](#wantWrite()) and
            [`ListeningProcessExecutor.ProcessListener.onStdinReady(ByteBuffer)`](ListeningProcessExecutor.ProcessListener.html#onStdinReady(java.nio.ByteBuffer))
            instead.
            :::

        []{#closeStdin(boolean)}

        -   #### closeStdin

            ``` methodSignature
            void closeStdin​(boolean force)
            ```

            ::: block
            Closes the stdin of the process. Call this if the process
            expects stdin to be closed before it writes to stdout.
            If `force` is `true`, then pending writes to stdin are
            discarded. Otherwise, waits for pending writes to flush,
            then closes stdin.
            :::

        []{#hasPendingWrites()}

        -   #### hasPendingWrites

            ``` methodSignature
            boolean hasPendingWrites()
            ```

            ::: block
            Returns `true` if the process has any data queued to write
            to stdin, `false` otherwise.
            :::

        []{#isRunning()}

        -   #### isRunning

            ``` methodSignature
            boolean isRunning()
            ```

            ::: block
            Returns `true` if the process is running, `false` otherwise.
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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
