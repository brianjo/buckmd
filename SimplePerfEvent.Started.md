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
[Package]{.packageLabelInType} [com.facebook.buck.event](package-summary.html)
:::

## Interface SimplePerfEvent.Started {#interface-simpleperfevent.started .title title="Interface SimplePerfEvent.Started"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `BuckEvent`, `BuckEventExternalInterface`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [SimplePerfEvent](SimplePerfEvent.html "class in com.facebook.buck.event")

    ------------------------------------------------------------------------

        public static interface SimplePerfEvent.Started
        extends BuckEvent
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Fields inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `BUILD_FINISHED, BUILD_REPORT, BUILD_STARTED, BUILD_STATUS_EVENT, CACHE_RATE_STATS_UPDATE_EVENT, INDIVIDUAL_TEST_AWAITING_RESULTS, INSTALL_STARTED, PARSE_FINISHED, PARSE_STARTED, PROJECT_GENERATION_FINISHED, PROJECT_GENERATION_STARTED, TEST_RUN_STARTED`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `BuckEvent`           | `c                    | ::: block             |
        |                       | reateFinishedEvent()` | Convenience wrapper   |
        |                       |                       | for                   |
        |                       |                       | [`createFinis         |
        |                       |                       | hedEvent(String, Obje |
        |                       |                       | ct)`](#createFinished |
        |                       |                       | Event(java.lang.Strin |
        |                       |                       | g,java.lang.Object)). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `BuckEvent`           | `createFinishedEve    | ::: block             |
        |                       | nt​(com.google.common. | Creates a new event   |
        |                       | collect.ImmutableMap< | which indicates the   |
        |                       | String,​Object> info)` | end of a performance  |
        |                       |                       | event.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `BuckEvent`           | `createFinishedEvent  | ::: block             |
        |                       | ​(String k1,           | Convenience wrapper   |
        |                       |           Object v1)` | for                   |
        |                       |                       | [`createFinis         |
        |                       |                       | hedEvent(String, Obje |
        |                       |                       | ct)`](#createFinished |
        |                       |                       | Event(java.lang.Strin |
        |                       |                       | g,java.lang.Object)). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `BuckEvent`           | `createFinishedEv     | ::: block             |
        |                       | ent​(String k1,        | Convenience wrapper   |
        |                       |              Object v | for                   |
        |                       | 1,                    | [`createFinis         |
        |                       |  String k2,           | hedEvent(String, Obje |
        |                       |           Object v2)` | ct)`](#createFinished |
        |                       |                       | Event(java.lang.Strin |
        |                       |                       | g,java.lang.Object)). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `BuckEvent`           | `createUpdateEve      | ::: block             |
        |                       | nt​(com.google.common. | Creates a new event   |
        |                       | collect.ImmutableMap< | which indicates an    |
        |                       | String,​Object> info)` | update to the         |
        |                       |                       | performance data      |
        |                       |                       | being gathered.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `BuckEvent`           | `createUpdateEve      | ::: block             |
        |                       | nt​(String k1,         | Convenience wrapper   |
        |                       |           Object v1)` | for                   |
        |                       |                       | [`createU             |
        |                       |                       | pdateEvent(String, Ob |
        |                       |                       | ject)`](#createUpdate |
        |                       |                       | Event(java.lang.Strin |
        |                       |                       | g,java.lang.Object)). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `BuckEvent`           | `createUp             | ::: block             |
        |                       | dateEvent​(String k1,  | Convenience wrapper   |
        |                       |                  Obje | for                   |
        |                       | ct v1,                | [`createU             |
        |                       |    String k2,         | pdateEvent(String, Ob |
        |                       |           Object v2)` | ject)`](#createUpdate |
        |                       |                       | Event(java.lang.Strin |
        |                       |                       | g,java.lang.Object)). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.event.BuckEvent}

            ### Methods inherited from interface com.facebook.buck.event.[BuckEvent](BuckEvent.html "interface in com.facebook.buck.event")

            `configure, getBuildId, getEventKey, getNanoTime, getThreadId, getThreadUserNanoTime, isConfigured, isRelatedTo, toLogMessage`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Methods inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `getEventName, getTimestampMillis, storeLastInstanceAndReplayForNewClients`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createUpdateEvent(com.google.common.collect.ImmutableMap)}

        -   #### createUpdateEvent

            ``` methodSignature
            BuckEvent createUpdateEvent​(com.google.common.collect.ImmutableMap<String,​Object> info)
            ```

            ::: block
            Creates a new event which indicates an update to the
            performance data being gathered.
            :::

            [Parameters:]{.paramLabel}
            :   `info` - Any additional information to be saved with the
                event. This will be serialized and potentially sent over
                the wire, so please keep this small.

            [Returns:]{.returnLabel}
            :   An event which should be posted to the
                [`BuckEventBus`](BuckEventBus.html "interface in com.facebook.buck.event").

        []{#createUpdateEvent(java.lang.String,java.lang.Object)}

        -   #### createUpdateEvent

            ``` methodSignature
            BuckEvent createUpdateEvent​(String k1,
                                        Object v1)
            ```

            ::: block
            Convenience wrapper for
            [`createUpdateEvent(String, Object)`](#createUpdateEvent(java.lang.String,java.lang.Object)).
            :::

        []{#createUpdateEvent(java.lang.String,java.lang.Object,java.lang.String,java.lang.Object)}

        -   #### createUpdateEvent

            ``` methodSignature
            BuckEvent createUpdateEvent​(String k1,
                                        Object v1,
                                        String k2,
                                        Object v2)
            ```

            ::: block
            Convenience wrapper for
            [`createUpdateEvent(String, Object)`](#createUpdateEvent(java.lang.String,java.lang.Object)).
            :::

        []{#createFinishedEvent(com.google.common.collect.ImmutableMap)}

        -   #### createFinishedEvent

            ``` methodSignature
            BuckEvent createFinishedEvent​(com.google.common.collect.ImmutableMap<String,​Object> info)
            ```

            ::: block
            Creates a new event which indicates the end of a performance
            event.
            :::

            [Parameters:]{.paramLabel}
            :   `info` - Any additional information to be saved with the
                event. This will be serialized and potentially sent over
                the wire, so please keep this small.

            [Returns:]{.returnLabel}
            :   An event which should be posted to the
                [`BuckEventBus`](BuckEventBus.html "interface in com.facebook.buck.event").

        []{#createFinishedEvent()}

        -   #### createFinishedEvent

            ``` methodSignature
            BuckEvent createFinishedEvent()
            ```

            ::: block
            Convenience wrapper for
            [`createFinishedEvent(String, Object)`](#createFinishedEvent(java.lang.String,java.lang.Object)).
            :::

        []{#createFinishedEvent(java.lang.String,java.lang.Object)}

        -   #### createFinishedEvent

            ``` methodSignature
            BuckEvent createFinishedEvent​(String k1,
                                          Object v1)
            ```

            ::: block
            Convenience wrapper for
            [`createFinishedEvent(String, Object)`](#createFinishedEvent(java.lang.String,java.lang.Object)).
            :::

        []{#createFinishedEvent(java.lang.String,java.lang.Object,java.lang.String,java.lang.Object)}

        -   #### createFinishedEvent

            ``` methodSignature
            BuckEvent createFinishedEvent​(String k1,
                                          Object v1,
                                          String k2,
                                          Object v2)
            ```

            ::: block
            Convenience wrapper for
            [`createFinishedEvent(String, Object)`](#createFinishedEvent(java.lang.String,java.lang.Object)).
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
