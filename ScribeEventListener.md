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
[Package]{.packageLabelInType} [com.facebook.buck.event.listener](package-summary.html)
:::

## Class ScribeEventListener {#class-scribeeventlistener .title title="Class ScribeEventListener"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.event.listener.ScribeEventListener

::: description
-   

    All Implemented Interfaces:
    :   `BuckEventListener`, `Closeable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class ScribeEventListener
        extends Object
        implements BuckEventListener

    ::: block
    [`BuckEventListener`](../BuckEventListener.html "interface in com.facebook.buck.event")
    that serializes events to JSON and sends them to Scribe.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `ScribeEve                        | ::: block                         |
        | ntListener​(ScribeEventListenerCon | Create new instance of            |
        | fig config,                    Sc | [`ScribeEventListener`](Scr       |
        | ribeLogger logger,                | ibeEventListener.html "class in c |
        |      ExecutorService dispatcher)` | om.facebook.buck.event.listener") |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `han                  |                       |
        |                       | dle​(BuckEvent event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isEnabledEv          | ::: block             |
        |                       | ent​(BuckEvent event)` | Returns true if the   |
        |                       |                       | event should be sent  |
        |                       |                       | to scribe; false      |
        |                       |                       | otherwise.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.event.BuckEventListener}

            ### Methods inherited from interface com.facebook.buck.event.[BuckEventListener](../BuckEventListener.html "interface in com.facebook.buck.event")

            `close`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.event.listener.ScribeEventListenerConfig,com.facebook.buck.util.network.ScribeLogger,java.util.concurrent.ExecutorService)}

        -   #### ScribeEventListener

                public ScribeEventListener​(ScribeEventListenerConfig config,
                                           ScribeLogger logger,
                                           ExecutorService dispatcher)

            ::: block
            Create new instance of
            [`ScribeEventListener`](ScribeEventListener.html "class in com.facebook.buck.event.listener")
            :::

            [Parameters:]{.paramLabel}
            :   `logger` - The actual scribe logger used to accept
                messages
            :   `dispatcher` - Executor service used to dispatch
                messages
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#handle(com.facebook.buck.event.BuckEvent)}

        -   #### handle

            ``` methodSignature
            public void handle​(BuckEvent event)
            ```

        []{#isEnabledEvent(com.facebook.buck.event.BuckEvent)}

        -   #### isEnabledEvent

            ``` methodSignature
            public boolean isEnabledEvent​(BuckEvent event)
            ```

            ::: block
            Returns true if the event should be sent to scribe; false
            otherwise.
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
