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

## Class SimplePerfEvent {#class-simpleperfevent .title title="Class SimplePerfEvent"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.event.AbstractBuckEvent](AbstractBuckEvent.html "class in com.facebook.buck.event")

    -   -   com.facebook.buck.event.SimplePerfEvent

::: description
-   

    All Implemented Interfaces:
    :   `BuckEvent`, `BuckEventExternalInterface`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `SimplePerfEvent.Finished`

    ------------------------------------------------------------------------

        public abstract class SimplePerfEvent
        extends AbstractBuckEvent

    ::: block
    An implementation of
    [`BuckEvent`](BuckEvent.html "interface in com.facebook.buck.event")s
    used for gathering performance statistics. These are only intended
    to be used with the trace viewer and should not be used to
    communicate information between parts of the system.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `Simp                 |                       |
        |                       | lePerfEvent.Finished` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `SimpleP              |                       |
        |                       | erfEvent.PerfEventId` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static interface `   | `S                    | ::: block             |
        |                       | implePerfEvent.Scope` | Represents the scope  |
        |                       |                       | within which a        |
        |                       |                       | particular            |
        |                       |                       | performance operation |
        |                       |                       | is taking place.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static interface `   | `Sim                  |                       |
        |                       | plePerfEvent.Started` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `                     |                       |
        |                       | SimplePerfEvent.Type` |                       |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Fields inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `BUILD_FINISHED, BUILD_REPORT, BUILD_STARTED, BUILD_STATUS_EVENT, CACHE_RATE_STATS_UPDATE_EVENT, INDIVIDUAL_TEST_AWAITING_RESULTS, INSTALL_STARTED, PARSE_FINISHED, PARSE_STARTED, PROJECT_GENERATION_FINISHED, PROJECT_GENERATION_STARTED, TEST_RUN_STARTED`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                            Description
          -------------------------------------- -------------
          `SimplePerfEvent​(EventKey eventKey)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `abstract SimpleP     | `getEventId()`        |                       |
        | erfEvent.PerfEventId` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getEventInfo()`      |                       |
        | abstract com.google.c |                       |                       |
        | ommon.collect.Immutab |                       |                       |
        | leMap<String,​Object>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract             | `getEventType()`      |                       |
        | SimplePerfEvent.Type` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static S             | `scope​(B              | ::: block             |
        | implePerfEvent.Scope` | uckEventBus bus,      | Convenience wrapper   |
        |                       |  SimplePerfEvent.Perf | for                   |
        |                       | EventId perfEventId)` | [`scope(BuckEventBus  |
        |                       |                       | , PerfEventId, Immuta |
        |                       |                       | bleMap)`](#scope(com. |
        |                       |                       | facebook.buck.event.B |
        |                       |                       | uckEventBus,com.faceb |
        |                       |                       | ook.buck.event.Simple |
        |                       |                       | PerfEvent.PerfEventId |
        |                       |                       | ,com.google.common.co |
        |                       |                       | llect.ImmutableMap)). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static S             | `scope​(Buc            | ::: block             |
        | implePerfEvent.Scope` | kEventBus bus,      S | Creates a scope       |
        |                       | implePerfEvent.PerfEv | within which the      |
        |                       | entId perfEventId,    | measured operation    |
        |                       |    com.google.common. | takes place.          |
        |                       | collect.ImmutableMap< | :::                   |
        |                       | String,​Object> info)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static S             | `scope​(BuckEventBus   | ::: block             |
        | implePerfEvent.Scope` |  bus,      SimplePerf | Convenience wrapper   |
        |                       | Event.PerfEventId per | for                   |
        |                       | fEventId,      String | [`scope(BuckEventBus  |
        |                       |  k1,      Object v1)` | , PerfEventId, Immuta |
        |                       |                       | bleMap)`](#scope(com. |
        |                       |                       | facebook.buck.event.B |
        |                       |                       | uckEventBus,com.faceb |
        |                       |                       | ook.buck.event.Simple |
        |                       |                       | PerfEvent.PerfEventId |
        |                       |                       | ,com.google.common.co |
        |                       |                       | llect.ImmutableMap)). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static S             | `scope​(Bu             | ::: block             |
        | implePerfEvent.Scope` | ckEventBus bus,       | Convenience wrapper   |
        |                       | SimplePerfEvent.PerfE | for                   |
        |                       | ventId perfEventId,   | [`scope(BuckEventBus  |
        |                       |     String k1,      O | , PerfEventId, Immuta |
        |                       | bject v1,      String | bleMap)`](#scope(com. |
        |                       |  k2,      Object v2)` | facebook.buck.event.B |
        |                       |                       | uckEventBus,com.faceb |
        |                       |                       | ook.buck.event.Simple |
        |                       |                       | PerfEvent.PerfEventId |
        |                       |                       | ,com.google.common.co |
        |                       |                       | llect.ImmutableMap)). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static S             | `scope​(Buc            | ::: block             |
        | implePerfEvent.Scope` | kEventBus bus,      S | Convenience wrapper   |
        |                       | tring perfEventName)` | for                   |
        |                       |                       | [`scope(BuckEventBus  |
        |                       |                       | , PerfEventId, Immuta |
        |                       |                       | bleMap)`](#scope(com. |
        |                       |                       | facebook.buck.event.B |
        |                       |                       | uckEventBus,com.faceb |
        |                       |                       | ook.buck.event.Simple |
        |                       |                       | PerfEvent.PerfEventId |
        |                       |                       | ,com.google.common.co |
        |                       |                       | llect.ImmutableMap)). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static S             | `scope​(Optional<Bu    | ::: block             |
        | implePerfEvent.Scope` | ckEventBus> bus,      | Convenience wrapper   |
        |                       |  SimplePerfEvent.Perf | for                   |
        |                       | EventId perfEventId)` | [`scope(BuckEventBus  |
        |                       |                       | , PerfEventId, Immuta |
        |                       |                       | bleMap)`](#scope(com. |
        |                       |                       | facebook.buck.event.B |
        |                       |                       | uckEventBus,com.faceb |
        |                       |                       | ook.buck.event.Simple |
        |                       |                       | PerfEvent.PerfEventId |
        |                       |                       | ,com.google.common.co |
        |                       |                       | llect.ImmutableMap)). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static S             | `scope​(Optional<Buck  | ::: block             |
        | implePerfEvent.Scope` | EventBus> bus,      S | Convenience wrapper   |
        |                       | implePerfEvent.PerfEv | for                   |
        |                       | entId perfEventId,    | [`scope(BuckEventBus  |
        |                       |    com.google.common. | , PerfEventId, Immuta |
        |                       | collect.ImmutableMap< | bleMap)`](#scope(com. |
        |                       | String,​Object> info)` | facebook.buck.event.B |
        |                       |                       | uckEventBus,com.faceb |
        |                       |                       | ook.buck.event.Simple |
        |                       |                       | PerfEvent.PerfEventId |
        |                       |                       | ,com.google.common.co |
        |                       |                       | llect.ImmutableMap)). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static S             | `scope                | ::: block             |
        | implePerfEvent.Scope` | ​(Optional<BuckEventBu | Convenience wrapper   |
        |                       | s> bus,      SimplePe | for                   |
        |                       | rfEvent.PerfEventId p | [`scope(BuckEventBus  |
        |                       | erfEventId,      Stri | , PerfEventId, Immuta |
        |                       | ng k,      Object v)` | bleMap)`](#scope(com. |
        |                       |                       | facebook.buck.event.B |
        |                       |                       | uckEventBus,com.faceb |
        |                       |                       | ook.buck.event.Simple |
        |                       |                       | PerfEvent.PerfEventId |
        |                       |                       | ,com.google.common.co |
        |                       |                       | llect.ImmutableMap)). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static S             | `scope​(Optional<B     | ::: block             |
        | implePerfEvent.Scope` | uckEventBus> bus,     | Convenience wrapper   |
        |                       |   SimplePerfEvent.Per | for                   |
        |                       | fEventId perfEventId, | [`scope(BuckEventBus  |
        |                       |       String k,       | , PerfEventId, Immuta |
        |                       | Object v,      String | bleMap)`](#scope(com. |
        |                       |  k2,      Object v2)` | facebook.buck.event.B |
        |                       |                       | uckEventBus,com.faceb |
        |                       |                       | ook.buck.event.Simple |
        |                       |                       | PerfEvent.PerfEventId |
        |                       |                       | ,com.google.common.co |
        |                       |                       | llect.ImmutableMap)). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static S             | `                     | ::: block             |
        | implePerfEvent.Scope` | scopeIgnoringShortEve | Convenience wrapper   |
        |                       | nts​(BuckEventBus bus, | for                   |
        |                       |                       | [`scope(BuckEventBus  |
        |                       |     SimplePerfEvent.P | , PerfEventId, Immuta |
        |                       | erfEventId perfEventI | bleMap)`](#scope(com. |
        |                       | d,                    | facebook.buck.event.B |
        |                       |       SimplePerfEvent | uckEventBus,com.faceb |
        |                       | .Scope parentScope,   | ook.buck.event.Simple |
        |                       |                       | PerfEvent.PerfEventId |
        |                       |   long minimumTime,   | ,com.google.common.co |
        |                       |                       | llect.ImmutableMap)). |
        |                       |   TimeUnit timeUnit)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static S             | `                     | ::: block             |
        | implePerfEvent.Scope` | scopeIgnoringShortEve | Like                  |
        |                       | nts​(BuckEventBus bus, | [`scope(BuckEventBus  |
        |                       |                       | , PerfEventId, Immuta |
        |                       |     SimplePerfEvent.P | bleMap)`](#scope(com. |
        |                       | erfEventId perfEventI | facebook.buck.event.B |
        |                       | d,                    | uckEventBus,com.faceb |
        |                       |       com.google.comm | ook.buck.event.Simple |
        |                       | on.collect.ImmutableM | PerfEvent.PerfEventId |
        |                       | ap<String,​Object> inf | ,com.google.common.co |
        |                       | o,                    | llect.ImmutableMap)), |
        |                       |       SimplePerfEvent | but doesn\'t post the |
        |                       | .Scope parentScope,   | events if the         |
        |                       |                       | duration of the scope |
        |                       |   long minimumTime,   | is below a certain    |
        |                       |                       | threshold.            |
        |                       |   TimeUnit timeUnit)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static S             | `scopeIg              | ::: block             |
        | implePerfEvent.Scope` | noringShortEvents​(Buc | Convenience wrapper   |
        |                       | kEventBus bus,        | for                   |
        |                       |                   Sim | [`scope(BuckEventBus  |
        |                       | plePerfEvent.PerfEven | , PerfEventId, Immuta |
        |                       | tId perfEventId,      | bleMap)`](#scope(com. |
        |                       |                     S | facebook.buck.event.B |
        |                       | tring k1,             | uckEventBus,com.faceb |
        |                       |              Object v | ook.buck.event.Simple |
        |                       | 1,                    | PerfEvent.PerfEventId |
        |                       |       SimplePerfEvent | ,com.google.common.co |
        |                       | .Scope parentScope,   | llect.ImmutableMap)). |
        |                       |                       | :::                   |
        |                       |   long minimumTime,   |                       |
        |                       |                       |                       |
        |                       |   TimeUnit timeUnit)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static S             | `scopeIgnoringS       | ::: block             |
        | implePerfEvent.Scope` | hortEvents​(BuckEventB | Convenience wrapper   |
        |                       | us bus,               | for                   |
        |                       |            SimplePerf | [`scope(BuckEventBus  |
        |                       | Event.PerfEventId per | , PerfEventId, Immuta |
        |                       | fEventId,             | bleMap)`](#scope(com. |
        |                       |              String k | facebook.buck.event.B |
        |                       | 1,                    | uckEventBus,com.faceb |
        |                       |       Object v1,      | ook.buck.event.Simple |
        |                       |                     S | PerfEvent.PerfEventId |
        |                       | tring k2,             | ,com.google.common.co |
        |                       |              Object v | llect.ImmutableMap)). |
        |                       | 2,                    | :::                   |
        |                       |       SimplePerfEvent |                       |
        |                       | .Scope parentScope,   |                       |
        |                       |                       |                       |
        |                       |   long minimumTime,   |                       |
        |                       |                       |                       |
        |                       |   TimeUnit timeUnit)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Sim           | `started              | ::: block             |
        | plePerfEvent.Started` | ​(SimplePerfEvent.Perf | Convenience wrapper   |
        |                       | EventId perfEventId)` | around                |
        |                       |                       | [`started(PerfE       |
        |                       |                       | ventId, ImmutableMap) |
        |                       |                       | `](#started(com.faceb |
        |                       |                       | ook.buck.event.Simple |
        |                       |                       | PerfEvent.PerfEventId |
        |                       |                       | ,com.google.common.co |
        |                       |                       | llect.ImmutableMap)). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Sim           | `started​(Sim          | ::: block             |
        | plePerfEvent.Started` | plePerfEvent.PerfEven | Prefer using          |
        |                       | tId perfEventId,      | [`scope(BuckEventBu   |
        |                       |    com.google.common. | s, PerfEventId, Immut |
        |                       | collect.ImmutableMap< | ableMap)`](#scope(com |
        |                       | String,​Object> info)` | .facebook.buck.event. |
        |                       |                       | BuckEventBus,com.face |
        |                       |                       | book.buck.event.Simpl |
        |                       |                       | ePerfEvent.PerfEventI |
        |                       |                       | d,com.google.common.c |
        |                       |                       | ollect.ImmutableMap)) |
        |                       |                       | when possible.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Sim           | `s                    | ::: block             |
        | plePerfEvent.Started` | tarted​(SimplePerfEven | Convenience wrapper   |
        |                       | t.PerfEventId perfEve | around                |
        |                       | ntId,        String k | [`started(PerfE       |
        |                       | 1,        Object v1)` | ventId, ImmutableMap) |
        |                       |                       | `](#started(com.faceb |
        |                       |                       | ook.buck.event.Simple |
        |                       |                       | PerfEvent.PerfEventId |
        |                       |                       | ,com.google.common.co |
        |                       |                       | llect.ImmutableMap)). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Sim           | `started​(SimplePe     | ::: block             |
        | plePerfEvent.Started` | rfEvent.PerfEventId p | Convenience wrapper   |
        |                       | erfEventId,        St | around                |
        |                       | ring k1,        Objec | [`started(PerfE       |
        |                       | t v1,        String k | ventId, ImmutableMap) |
        |                       | 2,        Object v2)` | `](#started(com.faceb |
        |                       |                       | ook.buck.event.Simple |
        |                       |                       | PerfEvent.PerfEventId |
        |                       |                       | ,com.google.common.co |
        |                       |                       | llect.ImmutableMap)). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.event.AbstractBuckEvent}

            ### Methods inherited from class com.facebook.buck.event.[AbstractBuckEvent](AbstractBuckEvent.html "class in com.facebook.buck.event")

            `configure, equals, getBuildId, getEventKey, getNanoTime, getThreadId, getThreadUserNanoTime, getTimestampMillis, getValueString, hashCode, isConfigured, isRelatedTo, toLogMessage, toString`

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

            `getEventName, storeLastInstanceAndReplayForNewClients`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.event.EventKey)}

        -   #### SimplePerfEvent

                public SimplePerfEvent​(EventKey eventKey)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getEventId()}

        -   #### getEventId

            ``` methodSignature
            public abstract SimplePerfEvent.PerfEventId getEventId()
            ```

            [Returns:]{.returnLabel}
            :   event identifier.

        []{#getEventType()}

        -   #### getEventType

            ``` methodSignature
            public abstract SimplePerfEvent.Type getEventType()
            ```

            [Returns:]{.returnLabel}
            :   event type.

        []{#getEventInfo()}

        -   #### getEventInfo

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<String,​Object> getEventInfo()
            ```

            [Returns:]{.returnLabel}
            :   information associated with the event.

        []{#started(com.facebook.buck.event.SimplePerfEvent.PerfEventId,com.google.common.collect.ImmutableMap)}

        -   #### started

            ``` methodSignature
            public static SimplePerfEvent.Started started​(SimplePerfEvent.PerfEventId perfEventId,
                                                          com.google.common.collect.ImmutableMap<String,​Object> info)
            ```

            ::: block
            Prefer using
            [`scope(BuckEventBus, PerfEventId, ImmutableMap)`](#scope(com.facebook.buck.event.BuckEventBus,com.facebook.buck.event.SimplePerfEvent.PerfEventId,com.google.common.collect.ImmutableMap))
            when possible.
            Create an event that indicates the start of a particular
            operation.
            :::

            [Parameters:]{.paramLabel}
            :   `perfEventId` - identifier of the operation (Upload,
                CacheFetch, Parse, etc..).
            :   `info` - Any additional information to be saved with the
                event. This will be serialized and potentially sent over
                the wire, so please keep this small.

            [Returns:]{.returnLabel}
            :   an object that should be used to create the
                corresponding update and finished event.

        []{#started(com.facebook.buck.event.SimplePerfEvent.PerfEventId)}

        -   #### started

            ``` methodSignature
            public static SimplePerfEvent.Started started​(SimplePerfEvent.PerfEventId perfEventId)
            ```

            ::: block
            Convenience wrapper around
            [`started(PerfEventId, ImmutableMap)`](#started(com.facebook.buck.event.SimplePerfEvent.PerfEventId,com.google.common.collect.ImmutableMap)).
            :::

            [Parameters:]{.paramLabel}
            :   `perfEventId` - identifier of the operation (Upload,
                CacheFetch, Parse, etc..).

            [Returns:]{.returnLabel}
            :   an object that should be used to create the
                corresponding update and finished event.

        []{#started(com.facebook.buck.event.SimplePerfEvent.PerfEventId,java.lang.String,java.lang.Object)}

        -   #### started

            ``` methodSignature
            public static SimplePerfEvent.Started started​(SimplePerfEvent.PerfEventId perfEventId,
                                                          String k1,
                                                          Object v1)
            ```

            ::: block
            Convenience wrapper around
            [`started(PerfEventId, ImmutableMap)`](#started(com.facebook.buck.event.SimplePerfEvent.PerfEventId,com.google.common.collect.ImmutableMap)).
            :::

            [Parameters:]{.paramLabel}
            :   `perfEventId` - identifier of the operation (Upload,
                CacheFetch, Parse, etc..).
            :   `k1` - name of the value to be stored with the event.
            :   `v1` - value to be stored. This will be serialized and
                potentially sent over the wire, so please keep this
                small.

            [Returns:]{.returnLabel}
            :   an object that should be used to create the
                corresponding update and finished event.

        []{#started(com.facebook.buck.event.SimplePerfEvent.PerfEventId,java.lang.String,java.lang.Object,java.lang.String,java.lang.Object)}

        -   #### started

            ``` methodSignature
            public static SimplePerfEvent.Started started​(SimplePerfEvent.PerfEventId perfEventId,
                                                          String k1,
                                                          Object v1,
                                                          String k2,
                                                          Object v2)
            ```

            ::: block
            Convenience wrapper around
            [`started(PerfEventId, ImmutableMap)`](#started(com.facebook.buck.event.SimplePerfEvent.PerfEventId,com.google.common.collect.ImmutableMap)).
            :::

            [Parameters:]{.paramLabel}
            :   `perfEventId` - identifier of the operation (Upload,
                CacheFetch, Parse, etc..).
            :   `k1` - name of the value to be stored with the event.
            :   `v1` - value to be stored. This will be serialized and
                potentially sent over the wire, so please keep this
                small.
            :   `k2` - name of the value to be stored with the event.
            :   `v2` - value to be stored. This will be serialized and
                potentially sent over the wire, so please keep this
                small.

            [Returns:]{.returnLabel}
            :   an object that should be used to create the
                corresponding update and finished event.

        []{#scope(com.facebook.buck.event.BuckEventBus,com.facebook.buck.event.SimplePerfEvent.PerfEventId,com.google.common.collect.ImmutableMap)}

        -   #### scope

            ``` methodSignature
            public static SimplePerfEvent.Scope scope​(BuckEventBus bus,
                                                      SimplePerfEvent.PerfEventId perfEventId,
                                                      com.google.common.collect.ImmutableMap<String,​Object> info)
            ```

            ::: block
            Creates a scope within which the measured operation takes
            place.
                 try (perfEvent = SimplePerfEvent.scope(bus, PerfEventId.of("BurnCpu"))) {
                   int bitsFlopped = 0;
                   for (int i = 0; i < 1000; i++) {
                     bitsFlopped += invokeExpensiveOp();
                     if (bitsFlopped % 100 == 0) {
                       // Some of these events are of special interest.
                       perfEvent.update("noFlopIteration", i);
                     }
                   }
                   perfEvent.appendFinishedInfo("totalBitsFlopped", bitsFlopped);
                 }
                 
            :::

            [Parameters:]{.paramLabel}
            :   `bus` - the
                [`BuckEventBus`](BuckEventBus.html "interface in com.facebook.buck.event")
                to post update and finished events to.
            :   `perfEventId` - identifier of the operation (Upload,
                CacheFetch, Parse, etc..).
            :   `info` - Any additional information to be saved with the
                event. This will be serialized and potentially sent over
                the wire, so please keep this small.

            [Returns:]{.returnLabel}
            :   an AutoCloseable which will send the finished event as
                soon as control flow exits the scope.

        []{#scope(com.facebook.buck.event.BuckEventBus,com.facebook.buck.event.SimplePerfEvent.PerfEventId)}

        -   #### scope

            ``` methodSignature
            public static SimplePerfEvent.Scope scope​(BuckEventBus bus,
                                                      SimplePerfEvent.PerfEventId perfEventId)
            ```

            ::: block
            Convenience wrapper for
            [`scope(BuckEventBus, PerfEventId, ImmutableMap)`](#scope(com.facebook.buck.event.BuckEventBus,com.facebook.buck.event.SimplePerfEvent.PerfEventId,com.google.common.collect.ImmutableMap)).
            :::

        []{#scope(com.facebook.buck.event.BuckEventBus,com.facebook.buck.event.SimplePerfEvent.PerfEventId,java.lang.String,java.lang.Object)}

        -   #### scope

            ``` methodSignature
            public static SimplePerfEvent.Scope scope​(BuckEventBus bus,
                                                      SimplePerfEvent.PerfEventId perfEventId,
                                                      String k1,
                                                      Object v1)
            ```

            ::: block
            Convenience wrapper for
            [`scope(BuckEventBus, PerfEventId, ImmutableMap)`](#scope(com.facebook.buck.event.BuckEventBus,com.facebook.buck.event.SimplePerfEvent.PerfEventId,com.google.common.collect.ImmutableMap)).
            :::

        []{#scope(com.facebook.buck.event.BuckEventBus,com.facebook.buck.event.SimplePerfEvent.PerfEventId,java.lang.String,java.lang.Object,java.lang.String,java.lang.Object)}

        -   #### scope

            ``` methodSignature
            public static SimplePerfEvent.Scope scope​(BuckEventBus bus,
                                                      SimplePerfEvent.PerfEventId perfEventId,
                                                      String k1,
                                                      Object v1,
                                                      String k2,
                                                      Object v2)
            ```

            ::: block
            Convenience wrapper for
            [`scope(BuckEventBus, PerfEventId, ImmutableMap)`](#scope(com.facebook.buck.event.BuckEventBus,com.facebook.buck.event.SimplePerfEvent.PerfEventId,com.google.common.collect.ImmutableMap)).
            :::

        []{#scope(java.util.Optional,com.facebook.buck.event.SimplePerfEvent.PerfEventId,com.google.common.collect.ImmutableMap)}

        -   #### scope

            ``` methodSignature
            public static SimplePerfEvent.Scope scope​(Optional<BuckEventBus> bus,
                                                      SimplePerfEvent.PerfEventId perfEventId,
                                                      com.google.common.collect.ImmutableMap<String,​Object> info)
            ```

            ::: block
            Convenience wrapper for
            [`scope(BuckEventBus, PerfEventId, ImmutableMap)`](#scope(com.facebook.buck.event.BuckEventBus,com.facebook.buck.event.SimplePerfEvent.PerfEventId,com.google.common.collect.ImmutableMap)).
            :::

        []{#scope(java.util.Optional,com.facebook.buck.event.SimplePerfEvent.PerfEventId)}

        -   #### scope

            ``` methodSignature
            public static SimplePerfEvent.Scope scope​(Optional<BuckEventBus> bus,
                                                      SimplePerfEvent.PerfEventId perfEventId)
            ```

            ::: block
            Convenience wrapper for
            [`scope(BuckEventBus, PerfEventId, ImmutableMap)`](#scope(com.facebook.buck.event.BuckEventBus,com.facebook.buck.event.SimplePerfEvent.PerfEventId,com.google.common.collect.ImmutableMap)).
            :::

        []{#scope(java.util.Optional,com.facebook.buck.event.SimplePerfEvent.PerfEventId,java.lang.String,java.lang.Object)}

        -   #### scope

            ``` methodSignature
            public static SimplePerfEvent.Scope scope​(Optional<BuckEventBus> bus,
                                                      SimplePerfEvent.PerfEventId perfEventId,
                                                      String k,
                                                      Object v)
            ```

            ::: block
            Convenience wrapper for
            [`scope(BuckEventBus, PerfEventId, ImmutableMap)`](#scope(com.facebook.buck.event.BuckEventBus,com.facebook.buck.event.SimplePerfEvent.PerfEventId,com.google.common.collect.ImmutableMap)).
            :::

        []{#scope(java.util.Optional,com.facebook.buck.event.SimplePerfEvent.PerfEventId,java.lang.String,java.lang.Object,java.lang.String,java.lang.Object)}

        -   #### scope

            ``` methodSignature
            public static SimplePerfEvent.Scope scope​(Optional<BuckEventBus> bus,
                                                      SimplePerfEvent.PerfEventId perfEventId,
                                                      String k,
                                                      Object v,
                                                      String k2,
                                                      Object v2)
            ```

            ::: block
            Convenience wrapper for
            [`scope(BuckEventBus, PerfEventId, ImmutableMap)`](#scope(com.facebook.buck.event.BuckEventBus,com.facebook.buck.event.SimplePerfEvent.PerfEventId,com.google.common.collect.ImmutableMap)).
            :::

        []{#scope(com.facebook.buck.event.BuckEventBus,java.lang.String)}

        -   #### scope

            ``` methodSignature
            public static SimplePerfEvent.Scope scope​(BuckEventBus bus,
                                                      String perfEventName)
            ```

            ::: block
            Convenience wrapper for
            [`scope(BuckEventBus, PerfEventId, ImmutableMap)`](#scope(com.facebook.buck.event.BuckEventBus,com.facebook.buck.event.SimplePerfEvent.PerfEventId,com.google.common.collect.ImmutableMap)).
            :::

        []{#scopeIgnoringShortEvents(com.facebook.buck.event.BuckEventBus,com.facebook.buck.event.SimplePerfEvent.PerfEventId,com.google.common.collect.ImmutableMap,com.facebook.buck.event.SimplePerfEvent.Scope,long,java.util.concurrent.TimeUnit)}

        -   #### scopeIgnoringShortEvents

            ``` methodSignature
            public static SimplePerfEvent.Scope scopeIgnoringShortEvents​(BuckEventBus bus,
                                                                         SimplePerfEvent.PerfEventId perfEventId,
                                                                         com.google.common.collect.ImmutableMap<String,​Object> info,
                                                                         SimplePerfEvent.Scope parentScope,
                                                                         long minimumTime,
                                                                         TimeUnit timeUnit)
            ```

            ::: block
            Like
            [`scope(BuckEventBus, PerfEventId, ImmutableMap)`](#scope(com.facebook.buck.event.BuckEventBus,com.facebook.buck.event.SimplePerfEvent.PerfEventId,com.google.common.collect.ImmutableMap)),
            but doesn\'t post the events if the duration of the scope is
            below a certain threshold. NOTE: The events are buffered
            before being posted. The longer they are buffered, the more
            likely any logging code will be confused. Ideally the
            threshold should not exceed 100ms.
            :::

            [Parameters:]{.paramLabel}
            :   `bus` - the
                [`BuckEventBus`](BuckEventBus.html "interface in com.facebook.buck.event")
                to post update and finished events to.
            :   `perfEventId` - identifier of the operation (Upload,
                CacheFetch, Parse, etc..).
            :   `info` - Any additional information to be saved with the
                event. This will be serialized and potentially sent over
                the wire, so please keep this small.
            :   `minimumTime` - the scope must take at least this long
                for the event to be posted.
            :   `timeUnit` - time unit for minimumTime.

            [Returns:]{.returnLabel}
            :   an AutoCloseable which will send the finished event as
                soon as control flow exits the scope.

        []{#scopeIgnoringShortEvents(com.facebook.buck.event.BuckEventBus,com.facebook.buck.event.SimplePerfEvent.PerfEventId,com.facebook.buck.event.SimplePerfEvent.Scope,long,java.util.concurrent.TimeUnit)}

        -   #### scopeIgnoringShortEvents

            ``` methodSignature
            public static SimplePerfEvent.Scope scopeIgnoringShortEvents​(BuckEventBus bus,
                                                                         SimplePerfEvent.PerfEventId perfEventId,
                                                                         SimplePerfEvent.Scope parentScope,
                                                                         long minimumTime,
                                                                         TimeUnit timeUnit)
            ```

            ::: block
            Convenience wrapper for
            [`scope(BuckEventBus, PerfEventId, ImmutableMap)`](#scope(com.facebook.buck.event.BuckEventBus,com.facebook.buck.event.SimplePerfEvent.PerfEventId,com.google.common.collect.ImmutableMap)).
            :::

        []{#scopeIgnoringShortEvents(com.facebook.buck.event.BuckEventBus,com.facebook.buck.event.SimplePerfEvent.PerfEventId,java.lang.String,java.lang.Object,com.facebook.buck.event.SimplePerfEvent.Scope,long,java.util.concurrent.TimeUnit)}

        -   #### scopeIgnoringShortEvents

            ``` methodSignature
            public static SimplePerfEvent.Scope scopeIgnoringShortEvents​(BuckEventBus bus,
                                                                         SimplePerfEvent.PerfEventId perfEventId,
                                                                         String k1,
                                                                         Object v1,
                                                                         SimplePerfEvent.Scope parentScope,
                                                                         long minimumTime,
                                                                         TimeUnit timeUnit)
            ```

            ::: block
            Convenience wrapper for
            [`scope(BuckEventBus, PerfEventId, ImmutableMap)`](#scope(com.facebook.buck.event.BuckEventBus,com.facebook.buck.event.SimplePerfEvent.PerfEventId,com.google.common.collect.ImmutableMap)).
            :::

        []{#scopeIgnoringShortEvents(com.facebook.buck.event.BuckEventBus,com.facebook.buck.event.SimplePerfEvent.PerfEventId,java.lang.String,java.lang.Object,java.lang.String,java.lang.Object,com.facebook.buck.event.SimplePerfEvent.Scope,long,java.util.concurrent.TimeUnit)}

        -   #### scopeIgnoringShortEvents

            ``` methodSignature
            public static SimplePerfEvent.Scope scopeIgnoringShortEvents​(BuckEventBus bus,
                                                                         SimplePerfEvent.PerfEventId perfEventId,
                                                                         String k1,
                                                                         Object v1,
                                                                         String k2,
                                                                         Object v2,
                                                                         SimplePerfEvent.Scope parentScope,
                                                                         long minimumTime,
                                                                         TimeUnit timeUnit)
            ```

            ::: block
            Convenience wrapper for
            [`scope(BuckEventBus, PerfEventId, ImmutableMap)`](#scope(com.facebook.buck.event.BuckEventBus,com.facebook.buck.event.SimplePerfEvent.PerfEventId,com.google.common.collect.ImmutableMap)).
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
-   [Nested](#nested.class.summary) \| 
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
