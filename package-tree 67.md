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
-   Tree
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Hierarchy For Package com.facebook.buck.httpserver {#hierarchy-for-package-com.facebook.buck.httpserver .title}

[Package Hierarchies:]{.packageHierarchyLabel}

-   [All Packages](../../../../overview-tree.html)
:::

::: contentContainer
::: {.section role="region"}
## Class Hierarchy {#class-hierarchy title="Class Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   org.eclipse.jetty.util.component.AbstractLifeCycle (implements
        org.eclipse.jetty.util.component.LifeCycle)
        -   org.eclipse.jetty.util.component.ContainerLifeCycle
            (implements org.eclipse.jetty.util.component.Container,
            org.eclipse.jetty.util.component.Destroyable,
            org.eclipse.jetty.util.component.Dumpable)
            -   org.eclipse.jetty.server.handler.AbstractHandler
                (implements org.eclipse.jetty.server.Handler)
                -   com.facebook.buck.httpserver.[[ArtifactCacheHandler]{.typeNameLink}](ArtifactCacheHandler.html "class in com.facebook.buck.httpserver")
    -   javax.servlet.GenericServlet (implements
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink},
        javax.servlet.Servlet, javax.servlet.ServletConfig)
        -   javax.servlet.http.HttpServlet
            -   org.eclipse.jetty.websocket.servlet.WebSocketServlet
                -   com.facebook.buck.httpserver.[[StreamingWebSocketServlet]{.typeNameLink}](StreamingWebSocketServlet.html "class in com.facebook.buck.httpserver")
    -   java.lang.[[Throwable]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Throwable.html?is-external=true "class or interface in java.lang"){.externalLink}
        (implements
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   java.lang.[[Exception]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Exception.html?is-external=true "class or interface in java.lang"){.externalLink}
            -   com.facebook.buck.httpserver.[[WebServer.WebServerException]{.typeNameLink}](WebServer.WebServerException.html "class in com.facebook.buck.httpserver")
    -   com.facebook.buck.httpserver.[[TraceHandlerDelegate]{.typeNameLink}](TraceHandlerDelegate.html "class in com.facebook.buck.httpserver")
        (implements
        com.facebook.buck.httpserver.[TemplateHandlerDelegate](TemplateHandlerDelegate.html "interface in com.facebook.buck.httpserver"))
    -   com.facebook.buck.httpserver.[[TracesHandlerDelegate]{.typeNameLink}](TracesHandlerDelegate.html "class in com.facebook.buck.httpserver")
        (implements
        com.facebook.buck.httpserver.[TemplateHandlerDelegate](TemplateHandlerDelegate.html "interface in com.facebook.buck.httpserver"))
    -   com.facebook.buck.httpserver.[[TracesHandlerDelegate.TraceAttrs]{.typeNameLink}](TracesHandlerDelegate.TraceAttrs.html "class in com.facebook.buck.httpserver")
    -   com.facebook.buck.httpserver.[[WebServer]{.typeNameLink}](WebServer.html "class in com.facebook.buck.httpserver")
    -   com.facebook.buck.httpserver.[[WebServerBuckEventListener]{.typeNameLink}](WebServerBuckEventListener.html "class in com.facebook.buck.httpserver")
        (implements
        com.facebook.buck.event.[BuckEventListener](../event/BuckEventListener.html "interface in com.facebook.buck.event"))
    -   org.eclipse.jetty.websocket.api.WebSocketAdapter (implements
        org.eclipse.jetty.websocket.api.WebSocketListener)
        -   com.facebook.buck.httpserver.[[StreamingWebSocketServlet.MyWebSocket]{.typeNameLink}](StreamingWebSocketServlet.MyWebSocket.html "class in com.facebook.buck.httpserver")
:::

::: {.section role="region"}
## Interface Hierarchy {#interface-hierarchy title="Interface Hierarchy"}

-   com.facebook.buck.httpserver.[[TemplateHandlerDelegate]{.typeNameLink}](TemplateHandlerDelegate.html "interface in com.facebook.buck.httpserver")
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
-   Tree
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

[]{#skip.navbar.bottom}
:::
