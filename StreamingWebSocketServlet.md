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
[Package]{.packageLabelInType} [com.facebook.buck.httpserver](package-summary.html)
:::

## Class StreamingWebSocketServlet {#class-streamingwebsocketservlet .title title="Class StreamingWebSocketServlet"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   javax.servlet.GenericServlet

    -   -   javax.servlet.http.HttpServlet

        -   -   org.eclipse.jetty.websocket.servlet.WebSocketServlet

            -   -   com.facebook.buck.httpserver.StreamingWebSocketServlet

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`, `javax.servlet.Servlet`,
        `javax.servlet.ServletConfig`

    ------------------------------------------------------------------------

        public class StreamingWebSocketServlet
        extends org.eclipse.jetty.websocket.servlet.WebSocketServlet

    [See Also:]{.seeLabel}
    :   [Serialized
        Form](../../../../serialized-form.html#com.facebook.buck.httpserver.StreamingWebSocketServlet)
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `class `              | `StreamingWebSocke    | ::: block             |
        |                       | tServlet.MyWebSocket` | This is the           |
        |                       |                       | httpserver component  |
        |                       |                       | of a WebSocket that   |
        |                       |                       | maintains a session   |
        |                       |                       | with one client.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                     Description
          ------------------------------- -------------
          `StreamingWebSocketServlet()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `configure​(org.ec     |                       |
        |                       | lipse.jetty.websocket |                       |
        |                       | .servlet.WebSocketSer |                       |
        |                       | vletFactory factory)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getNu                |                       |
        |                       | mActiveConnections()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `tell                 | ::: block             |
        |                       | Clients​(BuckEventExte | Sends the message to  |
        |                       | rnalInterface event)` | all WebSockets that   |
        |                       |                       | are subscribed to the |
        |                       |                       | given event.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.org.eclipse.jetty.websocket.servlet.WebSocketServlet}

            ### Methods inherited from class org.eclipse.jetty.websocket.servlet.WebSocketServlet

            `destroy, init, service`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.javax.servlet.http.HttpServlet}

            ### Methods inherited from class javax.servlet.http.HttpServlet

            `doDelete, doGet, doHead, doOptions, doPost, doPut, doTrace, getLastModified, service`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.javax.servlet.GenericServlet}

            ### Methods inherited from class javax.servlet.GenericServlet

            `getInitParameter, getInitParameterNames, getServletConfig, getServletContext, getServletInfo, getServletName, init, log, log`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### StreamingWebSocketServlet

                public StreamingWebSocketServlet()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#configure(org.eclipse.jetty.websocket.servlet.WebSocketServletFactory)}

        -   #### configure

            ``` methodSignature
            public void configure​(org.eclipse.jetty.websocket.servlet.WebSocketServletFactory factory)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `configure` in
                class `org.eclipse.jetty.websocket.servlet.WebSocketServlet`

        []{#tellClients(com.facebook.buck.event.external.events.BuckEventExternalInterface)}

        -   #### tellClients

            ``` methodSignature
            public void tellClients​(BuckEventExternalInterface event)
            ```

            ::: block
            Sends the message to all WebSockets that are subscribed to
            the given event.
            :::

        []{#getNumActiveConnections()}

        -   #### getNumActiveConnections

            ``` methodSignature
            public int getNumActiveConnections()
            ```

            [Returns:]{.returnLabel}
            :   Number of clients streaming from webserver. This may be
                called on any thread since connections is a thread-safe
                set, but beware of the usual caveat: by the time you act
                on the information returned, the number of active
                connections may have changed!
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
