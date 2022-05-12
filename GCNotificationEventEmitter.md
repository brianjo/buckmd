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
[Package]{.packageLabelInType} [com.facebook.buck.support.jvm](package-summary.html)
:::

## Class GCNotificationEventEmitter {#class-gcnotificationeventemitter .title title="Class GCNotificationEventEmitter"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.support.jvm.GCNotificationEventEmitter

::: description
-   

    All Implemented Interfaces:
    :   `EventListener`, `NotificationListener`

    ------------------------------------------------------------------------

        public final class GCNotificationEventEmitter
        extends Object
        implements NotificationListener

    ::: block
    JVM
    [`NotificationListener`](http://docs.oracle.com/javase/7/docs/api/javax/management/NotificationListener.html?is-external=true "class or interface in javax.management"){.externalLink}
    tuned to listen for GC events and emit GC events on the Buck event
    bus. This class receives GC events directly from the JVM and reports
    them in as high fidelity as possible to various log systems, where
    they can be used to correlate JVM GCs with other events in the Buck
    system.
    This class is expected to work the same with any GC, but Buck
    currently uses the G1 GC, so its heuristics are tuned to that.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `handleNotification   | ::: block             |
        |                       | ​(Notification notific | Handles a JMX         |
        |                       | ation,                | [`Notification`](ht   |
        |                       |     Object handback)` | tp://docs.oracle.com/ |
        |                       |                       | javase/7/docs/api/jav |
        |                       |                       | ax/management/Notific |
        |                       |                       | ation.html?is-externa |
        |                       |                       | l=true "class or inte |
        |                       |                       | rface in javax.manage |
        |                       |                       | ment"){.externalLink} |
        |                       |                       | emitted by one of the |
        |                       |                       | GC beans that we\'re  |
        |                       |                       | listening to.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `regist               | ::: block             |
        |                       | er​(BuckEventBus bus)` | Registers for GC      |
        |                       |                       | notifications to be   |
        |                       |                       | sent to the given     |
        |                       |                       | event bus.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
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
    -   []{#method.detail}

        ### Method Detail

        []{#register(com.facebook.buck.event.BuckEventBus)}

        -   #### register

            ``` methodSignature
            public static void register​(BuckEventBus bus)
            ```

            ::: block
            Registers for GC notifications to be sent to the given event
            bus.
            :::

            [Parameters:]{.paramLabel}
            :   `bus` - The event bus to send GC events to.

        []{#handleNotification(javax.management.Notification,java.lang.Object)}

        -   #### handleNotification

            ``` methodSignature
            public void handleNotification​(Notification notification,
                                           Object handback)
            ```

            ::: block
            Handles a JMX
            [`Notification`](http://docs.oracle.com/javase/7/docs/api/javax/management/Notification.html?is-external=true "class or interface in javax.management"){.externalLink}
            emitted by one of the GC beans that we\'re listening to.
            This function is called on a special runtime thread that is
            not visible to debuggers, so if you\'re trying to break in
            this method and it\'s not working, that\'s why.
            Since this is called on a special thread, it\'s important
            that it 1) not block and 2) terminate as quickly as
            possible.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `handleNotification` in interface `NotificationListener`

            [Parameters:]{.paramLabel}
            :   `notification` - The notification that we\'ve just
                received from JMX
            :   `handback` - An instance of the
                [`GarbageCollectorMXBean`](http://docs.oracle.com/javase/7/docs/api/java/lang/management/GarbageCollectorMXBean.html?is-external=true "class or interface in java.lang.management"){.externalLink}
                that triggered the event, which we passed explicitly as
                the third parameter of
                [`NotificationBroadcaster.addNotificationListener(NotificationListener, NotificationFilter,      Object)`](http://docs.oracle.com/javase/7/docs/api/javax/management/NotificationBroadcaster.html?is-external=true#addNotificationListener(javax.management.NotificationListener,javax.management.NotificationFilter,java.lang.Object) "class or interface in javax.management"){.externalLink}
                in the class constructor.
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
