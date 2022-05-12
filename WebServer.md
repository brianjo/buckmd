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

## Class WebServer {#class-webserver .title title="Class WebServer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.httpserver.WebServer

::: description
-   

    ------------------------------------------------------------------------

        public class WebServer
        extends Object

    ::: block
    A WebSocket server that reports events of buck.
    The WebServer can be modeled as: a) a network listener/dispatcher
    which sits on the port and listens for incoming http requests. b)
    static handlers - list of handlers that are bound to the current
    process (list of traces/logs/socket), c) \'normal\' handlers, bound
    to the daemon state.

    We would like the server to go down as infrequently as possible
    (this makes it simpler for /ws users who would otherwise need to
    reconnect and potentially lose state) which is the reason for
    section c) above.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                            Description
          ------------------- -------------------------------- -------------
          `static class `     `WebServer.WebServerException`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                 Description
          ------------------------------------------------------------------------------------------- -------------
          `WebServer​(int port,          ProjectFilesystem projectFilesystem,          Clock clock)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `WebSer               | `createListener()`    |                       |
        | verBuckEventListener` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getNu                |                       |
        |                       | mActiveConnections()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getPort()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `stop()`              |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `updateAndStartIfNeed | ::: block             |
        |                       | ed​(Optional<ArtifactC | Update state and      |
        |                       | ache> artifactCache)` | start the server if   |
        |                       |                       | necessary.            |
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

        []{#<init>(int,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.util.timing.Clock)}

        -   #### WebServer

                public WebServer​(int port,
                                 ProjectFilesystem projectFilesystem,
                                 Clock clock)

            [Parameters:]{.paramLabel}
            :   `port` - If 0, then an [ephemeral
                port](http://en.wikipedia.org/wiki/Ephemeral_port) will
                be assigned. Use [`getPort()`](#getPort()) to find out
                which port is being used.
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getPort()}

        -   #### getPort

            ``` methodSignature
            public int getPort()
            ```

            [Returns:]{.returnLabel}
            :   The port that web server is listening on.

        []{#createListener()}

        -   #### createListener

            ``` methodSignature
            public WebServerBuckEventListener createListener()
            ```

        []{#getNumActiveConnections()}

        -   #### getNumActiveConnections

            ``` methodSignature
            public int getNumActiveConnections()
            ```

            [Returns:]{.returnLabel}
            :   Number of clients streaming from webserver

        []{#updateAndStartIfNeeded(java.util.Optional)}

        -   #### updateAndStartIfNeeded

            ``` methodSignature
            public void updateAndStartIfNeeded​(Optional<ArtifactCache> artifactCache)
                                        throws WebServer.WebServerException
            ```

            ::: block
            Update state and start the server if necessary.
            :::

            [Parameters:]{.paramLabel}
            :   `artifactCache` - cache to serve.

            [Throws:]{.throwsLabel}
            :   `WebServer.WebServerException`

        []{#stop()}

        -   #### stop

            ``` methodSignature
            public void stop()
                      throws WebServer.WebServerException
            ```

            [Throws:]{.throwsLabel}
            :   `WebServer.WebServerException`
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
