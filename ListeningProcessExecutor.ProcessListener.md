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
[Package]{.packageLabelInType} [com.facebook.buck.util](package-summary.html)
:::

## Interface ListeningProcessExecutor.ProcessListener {#interface-listeningprocessexecutor.processlistener .title title="Interface ListeningProcessExecutor.ProcessListener"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `ForwardingProcessListener`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [ListeningProcessExecutor](ListeningProcessExecutor.html "class in com.facebook.buck.util")

    ------------------------------------------------------------------------

        public static interface ListeningProcessExecutor.ProcessListener

    ::: block
    Callback API to notify the caller on a background thread when a
    process starts, exits, has stdout or stderr bytes to read, or is
    ready to receive bytes on stdin.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `                     | ::: block             |
        |                       | onExit​(int exitCode)` | Called just after the |
        |                       |                       | process exits.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `onStart​(Listenin     | ::: block             |
        |                       | gProcessExecutor.Laun | Called just after the |
        |                       | chedProcess process)` | process starts.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `onStderr​(B           | ::: block             |
        |                       | yteBuffer buffer,     | Called when the       |
        |                       |      boolean closed)` | process writes bytes  |
        |                       |                       | to stderr.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `onStdinRead          | ::: block             |
        |                       | y​(ByteBuffer buffer)` | Called when the       |
        |                       |                       | process is ready to   |
        |                       |                       | receive bytes on      |
        |                       |                       | stdin.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `onStdout​(B           | ::: block             |
        |                       | yteBuffer buffer,     | Called when the       |
        |                       |      boolean closed)` | process writes bytes  |
        |                       |                       | to stdout.            |
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

        []{#onStart(com.facebook.buck.util.ListeningProcessExecutor.LaunchedProcess)}

        -   #### onStart

            ``` methodSignature
            void onStart​(ListeningProcessExecutor.LaunchedProcess process)
            ```

            ::: block
            Called just after the process starts.
            :::

        []{#onExit(int)}

        -   #### onExit

            ``` methodSignature
            void onExit​(int exitCode)
            ```

            ::: block
            Called just after the process exits.
            :::

        []{#onStdout(java.nio.ByteBuffer,boolean)}

        -   #### onStdout

            ``` methodSignature
            void onStdout​(ByteBuffer buffer,
                          boolean closed)
            ```

            ::: block
            Called when the process writes bytes to stdout.
            Before this method returns, you must set `buffer.position()`
            to indicate how many bytes you have consumed.

            If you do not consume the entire buffer, any remaining bytes
            will be passed back to you upon the next invocation (for
            example, when implementing a UTF-8 decoder which might
            contain a byte sequence spanning multiple reads).

            If `closed` is `true`, then stdout has been closed and no
            more bytes will be received.
            :::

        []{#onStderr(java.nio.ByteBuffer,boolean)}

        -   #### onStderr

            ``` methodSignature
            void onStderr​(ByteBuffer buffer,
                          boolean closed)
            ```

            ::: block
            Called when the process writes bytes to stderr.
            Before this method returns, you must set `buffer.position()`
            to indicate how many bytes you have consumed.

            If you do not consume the entire buffer, any remaining bytes
            will be passed back to you upon the next invocation (for
            example, when implementing a UTF-8 decoder which might
            contain a byte sequence spanning multiple reads).

            If `closed` is `true`, then stdout has been closed and no
            more bytes will be received.
            :::

        []{#onStdinReady(java.nio.ByteBuffer)}

        -   #### onStdinReady

            ``` methodSignature
            boolean onStdinReady​(ByteBuffer buffer)
            ```

            ::: block
            Called when the process is ready to receive bytes on stdin.
            Before this method returns, you must set the `buffer`\'s
            [`position`](http://docs.oracle.com/javase/7/docs/api/java/nio/Buffer.html?is-external=true#position() "class or interface in java.nio"){.externalLink}
            and
            [`limit`](http://docs.oracle.com/javase/7/docs/api/java/nio/Buffer.html?is-external=true#limit() "class or interface in java.nio"){.externalLink}
            (for example, by invoking
            [`ByteBuffer.flip()`](http://docs.oracle.com/javase/7/docs/api/java/nio/ByteBuffer.html?is-external=true#flip() "class or interface in java.nio"){.externalLink})
            to indicate how much data is in the buffer before returning
            from this method.

            You must first call
            [`ListeningProcessExecutor.LaunchedProcess.wantWrite()`](ListeningProcessExecutor.LaunchedProcess.html#wantWrite())
            at least once before this method will be invoked.

            If not all of the data needed to be written will fit in
            `buffer`, you can return `true` to indicate that you would
            like to write more data.

            Otherwise, return `false` if you have no more data to write
            to stdin. (You can always invoke
            [`ListeningProcessExecutor.LaunchedProcess.wantWrite()`](ListeningProcessExecutor.LaunchedProcess.html#wantWrite())
            any time in the future.
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
