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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.event](package-summary.html)
:::

## Class DefaultBuckEventBus {#class-defaultbuckeventbus .title title="Class DefaultBuckEventBus"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.event.DefaultBuckEventBus

::: description
-   

    All Implemented Interfaces:
    :   `BuckEventBus`, `EventDispatcher`, `Closeable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class DefaultBuckEventBus
        extends Object
        implements BuckEventBus

    ::: block
    Thin wrapper around guava event bus.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                           Description
          ------------------- ------------------------------- -------------
          `static int`        `DEFAULT_SHUTDOWN_TIMEOUT_MS`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `DefaultBuckEventBus​(Clock clock,                    boolean async,                    BuildId buildId,                    int shutdownTimeoutMillis)`                      
          `DefaultBuckEventBus​(Clock clock,                    BuildId buildId)`                                                                                                      
          `DefaultBuckEventBus​(Clock clock,                    BuildId buildId,                    int shutdownTimeoutMillis,                    ExecutorService executorService)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `close()`             | ::: block             |
        |                       |                       | [`ExecutorServ        |
        |                       |                       | ice.awaitTermination( |
        |                       |                       | long, java.util.concu |
        |                       |                       | rrent.TimeUnit)`](htt |
        |                       |                       | p://docs.oracle.com/j |
        |                       |                       | avase/7/docs/api/java |
        |                       |                       | /util/concurrent/Exec |
        |                       |                       | utorService.html?is-e |
        |                       |                       | xternal=true#awaitTer |
        |                       |                       | mination(long,java.ut |
        |                       |                       | il.concurrent.TimeUni |
        |                       |                       | t) "class or interfac |
        |                       |                       | e in java.util.concur |
        |                       |                       | rent"){.externalLink} |
        |                       |                       | is called to wait for |
        |                       |                       | events which have     |
        |                       |                       | been posted, but      |
        |                       |                       | which have been       |
        |                       |                       | queued by the         |
        |                       |                       | `EventBus`, to be     |
        |                       |                       | delivered.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `BuildId`             | `getBuildId()`        | ::: block             |
        |                       |                       | An id that every      |
        |                       |                       | event posted to this  |
        |                       |                       | event bus will share. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `p                    |                       |
        |                       | ost​(BuckEvent event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `po                   | ::: block             |
        |                       | st​(BuckEvent event,   | Post event to the     |
        |                       |    BuckEvent atTime)` | EventBus using the    |
        |                       |                       | timestamp given by    |
        |                       |                       | atTime.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `postWithoutConfigur  |                       |
        |                       | ing​(BuckEvent event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `reg                  | ::: block             |
        |                       | ister​(Object object)` | Register a listener   |
        |                       |                       | to process events     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `timest               | ::: block             |
        |                       | amp​(BuckEvent event)` | Timestamp event.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `unreg                | ::: block             |
        |                       | ister​(Object object)` | Remove a listener     |
        |                       |                       | previously specified  |
        |                       |                       | with `register()`     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `wait                 | ::: block             |
        |                       | Events​(long timeout)` | Wait for all          |
        |                       |                       | currently running     |
        |                       |                       | events to dispatch    |
        |                       |                       | and finish executing  |
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
    -   []{#field.detail}

        ### Field Detail

        []{#DEFAULT_SHUTDOWN_TIMEOUT_MS}

        -   #### DEFAULT_SHUTDOWN_TIMEOUT_MS

                public static final int DEFAULT_SHUTDOWN_TIMEOUT_MS

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.event.DefaultBuckEventBus.DEFAULT_SHUTDOWN_TIMEOUT_MS)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.util.timing.Clock,com.facebook.buck.core.model.BuildId)}

        -   #### DefaultBuckEventBus

                public DefaultBuckEventBus​(Clock clock,
                                           BuildId buildId)

        []{#<init>(com.facebook.buck.util.timing.Clock,boolean,com.facebook.buck.core.model.BuildId,int)}

        -   #### DefaultBuckEventBus

                public DefaultBuckEventBus​(Clock clock,
                                           boolean async,
                                           BuildId buildId,
                                           int shutdownTimeoutMillis)

        []{#<init>(com.facebook.buck.util.timing.Clock,com.facebook.buck.core.model.BuildId,int,java.util.concurrent.ExecutorService)}

        -   #### DefaultBuckEventBus

                public DefaultBuckEventBus​(Clock clock,
                                           BuildId buildId,
                                           int shutdownTimeoutMillis,
                                           ExecutorService executorService)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#post(com.facebook.buck.event.BuckEvent)}

        -   #### post

            ``` methodSignature
            public void post​(BuckEvent event)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `post` in interface `EventDispatcher`

        []{#post(com.facebook.buck.event.BuckEvent,com.facebook.buck.event.BuckEvent)}

        -   #### post

            ``` methodSignature
            public void post​(BuckEvent event,
                             BuckEvent atTime)
            ```

            ::: block
            Post event to the EventBus using the timestamp given by
            atTime.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `post` in interface `EventDispatcher`

        []{#register(java.lang.Object)}

        -   #### register

            ``` methodSignature
            public void register​(Object object)
            ```

            ::: block
            [Description copied from
            interface: `BuckEventBus`]{.descfrmTypeLabel}
            :::

            ::: block
            Register a listener to process events
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `register` in interface `BuckEventBus`

        []{#unregister(java.lang.Object)}

        -   #### unregister

            ``` methodSignature
            public void unregister​(Object object)
            ```

            ::: block
            [Description copied from
            interface: `BuckEventBus`]{.descfrmTypeLabel}
            :::

            ::: block
            Remove a listener previously specified with `register()`
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `unregister` in interface `BuckEventBus`

        []{#postWithoutConfiguring(com.facebook.buck.event.BuckEvent)}

        -   #### postWithoutConfiguring

            ``` methodSignature
            public void postWithoutConfiguring​(BuckEvent event)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `postWithoutConfiguring` in interface `EventDispatcher`

        []{#getBuildId()}

        -   #### getBuildId

            ``` methodSignature
            public BuildId getBuildId()
            ```

            ::: block
            An id that every event posted to this event bus will share.
            For long-running processes, like the daemon, the build id
            makes it possible to distinguish when events come from
            different invocations of Buck.
            In practice, this should be a short string, because it may
            be sent over the wire frequently.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildId` in interface `BuckEventBus`

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
            ```

            ::: block
            [`ExecutorService.awaitTermination(long, java.util.concurrent.TimeUnit)`](http://docs.oracle.com/javase/7/docs/api/java/util/concurrent/ExecutorService.html?is-external=true#awaitTermination(long,java.util.concurrent.TimeUnit) "class or interface in java.util.concurrent"){.externalLink}
            is called to wait for events which have been posted, but
            which have been queued by the `EventBus`, to be delivered.
            This allows listeners to record or report as much
            information as possible. This aids debugging when close is
            called during exception processing.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `Closeable`

        []{#waitEvents(long)}

        -   #### waitEvents

            ``` methodSignature
            public boolean waitEvents​(long timeout)
            ```

            ::: block
            [Description copied from
            interface: `BuckEventBus`]{.descfrmTypeLabel}
            :::

            ::: block
            Wait for all currently running events to dispatch and finish
            executing
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `waitEvents` in interface `BuckEventBus`

            [Parameters:]{.paramLabel}
            :   `timeout` - Time in milliseconds to wait for completion,
                if timeout is not greater than 0 then it will wait
                indefinitely

            [Returns:]{.returnLabel}
            :   true if all events were handled and false if timeout was
                hit

        []{#timestamp(com.facebook.buck.event.BuckEvent)}

        -   #### timestamp

            ``` methodSignature
            public void timestamp​(BuckEvent event)
            ```

            ::: block
            Timestamp event. A timestamped event cannot subsequently
            being posted and is useful only to pass its timestamp on to
            another posted event.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `timestamp` in interface `EventDispatcher`
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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
