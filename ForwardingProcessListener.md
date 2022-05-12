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
[Package]{.packageLabelInType} [com.facebook.buck.util](package-summary.html)
:::

## Class ForwardingProcessListener {#class-forwardingprocesslistener .title title="Class ForwardingProcessListener"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.ForwardingProcessListener

::: description
-   

    All Implemented Interfaces:
    :   `ListeningProcessExecutor.ProcessListener`

    ------------------------------------------------------------------------

        public class ForwardingProcessListener
        extends Object
        implements ListeningProcessExecutor.ProcessListener
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                      Description
          ------------------------------------------------------------------------------------------------ -------------
          `ForwardingProcessListener​(OutputStream stdout,                          OutputStream stderr)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
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

        []{#<init>(java.io.OutputStream,java.io.OutputStream)}

        -   #### ForwardingProcessListener

                public ForwardingProcessListener​(OutputStream stdout,
                                                 OutputStream stderr)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#onStart(com.facebook.buck.util.ListeningProcessExecutor.LaunchedProcess)}

        -   #### onStart

            ``` methodSignature
            public void onStart​(ListeningProcessExecutor.LaunchedProcess process)
            ```

            ::: block
            [Description copied from
            interface: `ListeningProcessExecutor.ProcessListener`]{.descfrmTypeLabel}
            :::

            ::: block
            Called just after the process starts.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `onStart` in
                interface `ListeningProcessExecutor.ProcessListener`

        []{#onExit(int)}

        -   #### onExit

            ``` methodSignature
            public void onExit​(int exitCode)
            ```

            ::: block
            [Description copied from
            interface: `ListeningProcessExecutor.ProcessListener`]{.descfrmTypeLabel}
            :::

            ::: block
            Called just after the process exits.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `onExit` in
                interface `ListeningProcessExecutor.ProcessListener`

        []{#onStdout(java.nio.ByteBuffer,boolean)}

        -   #### onStdout

            ``` methodSignature
            public void onStdout​(ByteBuffer buffer,
                                 boolean closed)
            ```

            ::: block
            [Description copied from
            interface: `ListeningProcessExecutor.ProcessListener`]{.descfrmTypeLabel}
            :::

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

            [Specified by:]{.overrideSpecifyLabel}
            :   `onStdout` in
                interface `ListeningProcessExecutor.ProcessListener`

        []{#onStderr(java.nio.ByteBuffer,boolean)}

        -   #### onStderr

            ``` methodSignature
            public void onStderr​(ByteBuffer buffer,
                                 boolean closed)
            ```

            ::: block
            [Description copied from
            interface: `ListeningProcessExecutor.ProcessListener`]{.descfrmTypeLabel}
            :::

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

            [Specified by:]{.overrideSpecifyLabel}
            :   `onStderr` in
                interface `ListeningProcessExecutor.ProcessListener`

        []{#onStdinReady(java.nio.ByteBuffer)}

        -   #### onStdinReady

            ``` methodSignature
            public boolean onStdinReady​(ByteBuffer buffer)
            ```

            ::: block
            [Description copied from
            interface: `ListeningProcessExecutor.ProcessListener`]{.descfrmTypeLabel}
            :::

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

            [Specified by:]{.overrideSpecifyLabel}
            :   `onStdinReady` in
                interface `ListeningProcessExecutor.ProcessListener`
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
