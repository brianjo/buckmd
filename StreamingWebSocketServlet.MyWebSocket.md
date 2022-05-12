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
[Package]{.packageLabelInType} [com.facebook.buck.httpserver](package-summary.html)
:::

## Class StreamingWebSocketServlet.MyWebSocket {#class-streamingwebsocketservlet.mywebsocket .title title="Class StreamingWebSocketServlet.MyWebSocket"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   org.eclipse.jetty.websocket.api.WebSocketAdapter

    -   -   com.facebook.buck.httpserver.StreamingWebSocketServlet.MyWebSocket

::: description
-   

    All Implemented Interfaces:
    :   `org.eclipse.jetty.websocket.api.WebSocketConnectionListener`,
        `org.eclipse.jetty.websocket.api.WebSocketListener`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [StreamingWebSocketServlet](StreamingWebSocketServlet.html "class in com.facebook.buck.httpserver")

    ------------------------------------------------------------------------

        public class StreamingWebSocketServlet.MyWebSocket
        extends org.eclipse.jetty.websocket.api.WebSocketAdapter

    ::: block
    This is the httpserver component of a WebSocket that maintains a
    session with one client.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor       Description
          ----------------- -------------
          `MyWebSocket()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                  Description
          ------------------- ----------------------------------------------------------------------- -------------
          `boolean`           `isSubscribedTo​(String eventName)`                                       
          `void`              `onWebSocketClose​(int statusCode,                 String reason)`        
          `void`              `onWebSocketConnect​(org.eclipse.jetty.websocket.api.Session session)`    
          `void`              `onWebSocketText​(String message)`                                        

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.org.eclipse.jetty.websocket.api.WebSocketAdapter}

            ### Methods inherited from class org.eclipse.jetty.websocket.api.WebSocketAdapter

            `getRemote, getSession, isConnected, isNotConnected, onWebSocketBinary, onWebSocketError`

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

        -   #### MyWebSocket

                public MyWebSocket()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#onWebSocketConnect(org.eclipse.jetty.websocket.api.Session)}

        -   #### onWebSocketConnect

            ``` methodSignature
            public void onWebSocketConnect​(org.eclipse.jetty.websocket.api.Session session)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `onWebSocketConnect` in
                interface `org.eclipse.jetty.websocket.api.WebSocketConnectionListener`

            [Overrides:]{.overrideSpecifyLabel}
            :   `onWebSocketConnect` in
                class `org.eclipse.jetty.websocket.api.WebSocketAdapter`

        []{#onWebSocketClose(int,java.lang.String)}

        -   #### onWebSocketClose

            ``` methodSignature
            public void onWebSocketClose​(int statusCode,
                                         String reason)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `onWebSocketClose` in
                interface `org.eclipse.jetty.websocket.api.WebSocketConnectionListener`

            [Overrides:]{.overrideSpecifyLabel}
            :   `onWebSocketClose` in
                class `org.eclipse.jetty.websocket.api.WebSocketAdapter`

        []{#onWebSocketText(java.lang.String)}

        -   #### onWebSocketText

            ``` methodSignature
            public void onWebSocketText​(String message)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `onWebSocketText` in
                interface `org.eclipse.jetty.websocket.api.WebSocketListener`

            [Overrides:]{.overrideSpecifyLabel}
            :   `onWebSocketText` in
                class `org.eclipse.jetty.websocket.api.WebSocketAdapter`

        []{#isSubscribedTo(java.lang.String)}

        -   #### isSubscribedTo

            ``` methodSignature
            public boolean isSubscribedTo​(String eventName)
            ```

            [Returns:]{.returnLabel}
            :   true if client is subscribed to given event
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
