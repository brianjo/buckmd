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
[Package]{.packageLabelInType} [com.facebook.buck.event](package-summary.html)
:::

## Class ThrowableConsoleEvent {#class-throwableconsoleevent .title title="Class ThrowableConsoleEvent"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.event.AbstractBuckEvent](AbstractBuckEvent.html "class in com.facebook.buck.event")

    -   -   [com.facebook.buck.event.ConsoleEvent](ConsoleEvent.html "class in com.facebook.buck.event")

        -   -   com.facebook.buck.event.ThrowableConsoleEvent

::: description
-   

    All Implemented Interfaces:
    :   `BuckEvent`, `BuckEventExternalInterface`,
        `ConsoleEventExternalInterface`

    ------------------------------------------------------------------------

        @Deprecated
        public class ThrowableConsoleEvent
        extends ConsoleEvent

    ::: deprecationBlock
    [Deprecated.]{.deprecatedLabel}
    :::

    ::: block
    Event for tracking
    [`Throwable`](http://docs.oracle.com/javase/7/docs/api/java/lang/Throwable.html?is-external=true "class or interface in java.lang"){.externalLink}.
    Deprecated, use
    [`ErrorLogger`](../util/ErrorLogger.html "class in com.facebook.buck.util").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Fields inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `BUILD_FINISHED, BUILD_REPORT, BUILD_STARTED, BUILD_STATUS_EVENT, CACHE_RATE_STATS_UPDATE_EVENT, INDIVIDUAL_TEST_AWAITING_RESULTS, INSTALL_STARTED, PARSE_FINISHED, PARSE_STARTED, PROJECT_GENERATION_FINISHED, PROJECT_GENERATION_STARTED, TEST_RUN_STARTED`

        ```{=html}
        <!-- -->
        ```
        -   []{#fields.inherited.from.class.com.facebook.buck.event.external.events.ConsoleEventExternalInterface}

            ### Fields inherited from interface com.facebook.buck.event.external.events.[ConsoleEventExternalInterface](external/events/ConsoleEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `CONSOLE_EVENT`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier              | Constructor           | Description           |
        +=======================+=======================+=======================+
        | `protected `          | `ThrowableConsoleE    | ::: block             |
        |                       | vent​(Throwable throwa | [Deprecate            |
        |                       | ble,                  | d.]{.deprecatedLabel} |
        |                       |      String message)` | :::                   |
        |                       |                       |                       |
        |                       |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected `          | `Throwable            | ::: block             |
        |                       | ConsoleEvent​(Throwabl | [Deprecate            |
        |                       | e throwable,          | d.]{.deprecatedLabel} |
        |                       |              Level le | :::                   |
        |                       | vel,                  |                       |
        |                       |      String message)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static T             | `create​(Th            | ::: block             |
        | hrowableConsoleEvent` | rowable throwable,    | [Deprecate            |
        |                       |     String message,   | d.]{.deprecatedLabel} |
        |                       |      Object... args)` | :::                   |
        |                       |                       |                       |
        |                       |                       |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4
        .tableTab}[[Deprecated
        Methods](javascript:show(32);)[ ]{.tabEnd}]{#t6 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.event.ConsoleEvent}

            ### Methods inherited from class com.facebook.buck.event.[ConsoleEvent](ConsoleEvent.html "class in com.facebook.buck.event")

            `containsAnsiEscapeCodes, create, create, createForMessageWithAnsiEscapeCodes, fine, fine, finer, finer, getEventName, getLevel, getMessage, getValueString, info, info, severe, severe, toString, warning, warning`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.event.AbstractBuckEvent}

            ### Methods inherited from class com.facebook.buck.event.[AbstractBuckEvent](AbstractBuckEvent.html "class in com.facebook.buck.event")

            `configure, equals, getBuildId, getEventKey, getNanoTime, getThreadId, getThreadUserNanoTime, getTimestampMillis, hashCode, isConfigured, isRelatedTo, toLogMessage`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Methods inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `getTimestampMillis, storeLastInstanceAndReplayForNewClients`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.lang.Throwable,java.lang.String)}

        -   #### ThrowableConsoleEvent

                protected ThrowableConsoleEvent​(Throwable throwable,
                                                String message)

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

        []{#<init>(java.lang.Throwable,java.util.logging.Level,java.lang.String)}

        -   #### ThrowableConsoleEvent

                protected ThrowableConsoleEvent​(Throwable throwable,
                                                Level level,
                                                String message)

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#create(java.lang.Throwable,java.lang.String,java.lang.Object...)}

        -   #### create

            ``` methodSignature
            public static ThrowableConsoleEvent create​(Throwable throwable,
                                                       String message,
                                                       Object... args)
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
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
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
