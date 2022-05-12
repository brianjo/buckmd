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
[Package]{.packageLabelInType} [com.facebook.buck.logd.server](package-summary.html)
:::

## Class LogdServer {#class-logdserver .title title="Class LogdServer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.logd.server.LogdServer

::: description
-   

    All Implemented Interfaces:
    :   `LogDaemonServer`

    ------------------------------------------------------------------------

        public class LogdServer
        extends Object
        implements LogDaemonServer

    ::: block
    Given a port number, logD server is responsible for handling log
    writing to a filesystem and to storage.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `LogdServer​(int port)`            | ::: block                         |
        |                                   | Construct a logD server at        |
        |                                   | requested port number.            |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `LogdS                            | ::: block                         |
        | erver​(int port,           io.grpc | Default to log streaming service. |
        | .ServerBuilder<?> serverBuilder)` | :::                               |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `start()`             | ::: block             |
        |                       |                       | Starts logD server    |
        |                       |                       | listening on provided |
        |                       |                       | port in constructor.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `stop()`              | ::: block             |
        |                       |                       | Shuts down logD       |
        |                       |                       | server.               |
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

        []{#<init>(int)}

        -   #### LogdServer

                public LogdServer​(int port)

            ::: block
            Construct a logD server at requested port number.
            :::

            [Parameters:]{.paramLabel}
            :   `port` - port number

        []{#<init>(int,io.grpc.ServerBuilder)}

        -   #### LogdServer

                public LogdServer​(int port,
                                  io.grpc.ServerBuilder<?> serverBuilder)

            ::: block
            Default to log streaming service.
            :::

            [Parameters:]{.paramLabel}
            :   `port` - port number
            :   `serverBuilder` - server created at requested port
                number
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#start()}

        -   #### start

            ``` methodSignature
            public void start()
                       throws IOException
            ```

            ::: block
            Starts logD server listening on provided port in
            constructor.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `start` in interface `LogDaemonServer`

            [Throws:]{.throwsLabel}
            :   `IOException` - if unable to bind

        []{#stop()}

        -   #### stop

            ``` methodSignature
            public void stop()
            ```

            ::: block
            Shuts down logD server.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `stop` in interface `LogDaemonServer`
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
