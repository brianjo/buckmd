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
[Package]{.packageLabelInType} [com.facebook.buck.io.unixsocket](package-summary.html)
:::

## Class UnixDomainSocket {#class-unixdomainsocket .title title="Class UnixDomainSocket"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.net.Socket](http://docs.oracle.com/javase/7/docs/api/java/net/Socket.html?is-external=true "class or interface in java.net"){.externalLink}

    -   -   com.facebook.buck.io.unixsocket.UnixDomainSocket

::: description
-   

    All Implemented Interfaces:
    :   `Transport`, `Closeable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class UnixDomainSocket
        extends Socket
        implements Transport

    ::: block
    Implements a
    [`Socket`](http://docs.oracle.com/javase/7/docs/api/java/net/Socket.html?is-external=true "class or interface in java.net"){.externalLink}
    backed by a native Unix domain socket.
    Instances of this class always return `null` for
    [`Socket.getInetAddress()`](http://docs.oracle.com/javase/7/docs/api/java/net/Socket.html?is-external=true#getInetAddress() "class or interface in java.net"){.externalLink},
    [`Socket.getLocalAddress()`](http://docs.oracle.com/javase/7/docs/api/java/net/Socket.html?is-external=true#getLocalAddress() "class or interface in java.net"){.externalLink},
    [`Socket.getLocalSocketAddress()`](http://docs.oracle.com/javase/7/docs/api/java/net/Socket.html?is-external=true#getLocalSocketAddress() "class or interface in java.net"){.externalLink},
    [`Socket.getRemoteSocketAddress()`](http://docs.oracle.com/javase/7/docs/api/java/net/Socket.html?is-external=true#getRemoteSocketAddress() "class or interface in java.net"){.externalLink}.

    If not explicitly closed, will close the file descriptor when
    finalized.

    Caller is responsible for closing the streams returned from
    [`getInputStream()`](#getInputStream()) and
    [`getOutputStream()`](#getOutputStream()).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `close()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `createSocke          | ::: block             |
        | tic UnixDomainSocket` | tWithPath​(Path path)` | Creates a Unix domain |
        |                       |                       | socket bound to a     |
        |                       |                       | path.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected void`      | `finalize()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `InputStream`         | `getInputStream()`    | ::: block             |
        |                       |                       | Returns an input      |
        |                       |                       | stream for reading    |
        |                       |                       | messages              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OutputStream`        | `getOutputStream()`   | ::: block             |
        |                       |                       | Returns an input      |
        |                       |                       | stream for writing    |
        |                       |                       | messages.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isConnected()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `shutdownInput()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `shutdownOutput()`    |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.net.Socket}

            ### Methods inherited from class java.net.[Socket](http://docs.oracle.com/javase/7/docs/api/java/net/Socket.html?is-external=true "class or interface in java.net"){.externalLink}

            `bind, connect, connect, getChannel, getInetAddress, getKeepAlive, getLocalAddress, getLocalPort, getLocalSocketAddress, getOOBInline, getOption, getPort, getReceiveBufferSize, getRemoteSocketAddress, getReuseAddress, getSendBufferSize, getSoLinger, getSoTimeout, getTcpNoDelay, getTrafficClass, isBound, isClosed, isInputShutdown, isOutputShutdown, sendUrgentData, setKeepAlive, setOOBInline, setOption, setPerformancePreferences, setReceiveBufferSize, setReuseAddress, setSendBufferSize, setSocketImplFactory, setSoLinger, setSoTimeout, setTcpNoDelay, setTrafficClass, supportedOptions, toString`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, getClass, hashCode, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createSocketWithPath(java.nio.file.Path)}

        -   #### createSocketWithPath

            ``` methodSignature
            public static UnixDomainSocket createSocketWithPath​(Path path)
                                                         throws IOException
            ```

            ::: block
            Creates a Unix domain socket bound to a path.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#isConnected()}

        -   #### isConnected

            ``` methodSignature
            public boolean isConnected()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `isConnected` in class `Socket`

        []{#getInputStream()}

        -   #### getInputStream

            ``` methodSignature
            public InputStream getInputStream()
            ```

            ::: block
            [Description copied from
            interface: `Transport`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns an input stream for reading messages
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getInputStream` in interface `Transport`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getInputStream` in class `Socket`

            [Returns:]{.returnLabel}
            :   an input stream for reading messages in this IPC

        []{#getOutputStream()}

        -   #### getOutputStream

            ``` methodSignature
            public OutputStream getOutputStream()
            ```

            ::: block
            [Description copied from
            interface: `Transport`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns an input stream for writing messages.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getOutputStream` in interface `Transport`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getOutputStream` in class `Socket`

            [Returns:]{.returnLabel}
            :   an input stream for writing messages in this IPC

        []{#shutdownInput()}

        -   #### shutdownInput

            ``` methodSignature
            public void shutdownInput()
                               throws IOException
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `shutdownInput` in class `Socket`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#shutdownOutput()}

        -   #### shutdownOutput

            ``` methodSignature
            public void shutdownOutput()
                                throws IOException
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `shutdownOutput` in class `Socket`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
                       throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `Closeable`

            [Overrides:]{.overrideSpecifyLabel}
            :   `close` in class `Socket`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#finalize()}

        -   #### finalize

            ``` methodSignature
            protected void finalize()
                             throws IOException
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `finalize` in class `Object`

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
