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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.starlark.eventhandler](package-summary.html)
:::

## Class ConsoleEventHandler {#class-consoleeventhandler .title title="Class ConsoleEventHandler"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.starlark.eventhandler.ConsoleEventHandler

::: description
-   

    All Implemented Interfaces:
    :   `com.google.devtools.build.lib.events.EventHandler`

    ------------------------------------------------------------------------

        public class ConsoleEventHandler
        extends Object
        implements com.google.devtools.build.lib.events.EventHandler

    ::: block
    A simple class that posts log events from skylark as
    [`ConsoleEvent`](../../../event/ConsoleEvent.html "class in com.facebook.buck.event")
    the provided event bus
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `ConsoleEven                      | ::: block                         |
        | tHandler​(BuckEventBus eventBus,   | Create an instance of             |
        |                   Set<com.google. | [`Cons                            |
        | devtools.build.lib.events.EventKi | oleEventHandler`](ConsoleEventHan |
        | nd> supportedEvents,              | dler.html "class in com.facebook. |
        |        com.google.common.collect. | buck.core.starlark.eventhandler") |
        | ImmutableSet<String> nativeModule | that posts to `eventBus`          |
        | FunctionNames,                    | :::                               |
        |  HumanReadableExceptionAugmentor  |                                   |
        | humanReadableExceptionAugmentor)` |                                   |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                       Description
          ------------------- ------------------------------------------------------------ -------------
          `void`              `handle​(com.google.devtools.build.lib.events.Event event)`    

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

        []{#<init>(com.facebook.buck.event.BuckEventBus,java.util.Set,com.google.common.collect.ImmutableSet,com.facebook.buck.core.exceptions.HumanReadableExceptionAugmentor)}

        -   #### ConsoleEventHandler

                public ConsoleEventHandler​(BuckEventBus eventBus,
                                           Set<com.google.devtools.build.lib.events.EventKind> supportedEvents,
                                           com.google.common.collect.ImmutableSet<String> nativeModuleFunctionNames,
                                           HumanReadableExceptionAugmentor humanReadableExceptionAugmentor)

            ::: block
            Create an instance of
            [`ConsoleEventHandler`](ConsoleEventHandler.html "class in com.facebook.buck.core.starlark.eventhandler")
            that posts to `eventBus`
            :::

            [Parameters:]{.paramLabel}
            :   `eventBus` - The event bus to post
                [`ConsoleEvent`](../../../event/ConsoleEvent.html "class in com.facebook.buck.event")
                to
            :   `supportedEvents` - The events that should post to the
                event bus
            :   `humanReadableExceptionAugmentor` -
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#handle(com.google.devtools.build.lib.events.Event)}

        -   #### handle

            ``` methodSignature
            public void handle​(com.google.devtools.build.lib.events.Event event)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `handle` in
                interface `com.google.devtools.build.lib.events.EventHandler`
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
