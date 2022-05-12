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
[Package]{.packageLabelInType} [com.facebook.buck.artifact_cache](package-summary.html)
:::

## Class HttpArtifactCacheEvent.Finished {#class-httpartifactcacheevent.finished .title title="Class HttpArtifactCacheEvent.Finished"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.event.AbstractBuckEvent](../event/AbstractBuckEvent.html "class in com.facebook.buck.event")

    -   -   [com.facebook.buck.artifact_cache.ArtifactCacheEvent](ArtifactCacheEvent.html "class in com.facebook.buck.artifact_cache")

        -   -   [com.facebook.buck.artifact_cache.ArtifactCacheEvent.Finished](ArtifactCacheEvent.Finished.html "class in com.facebook.buck.artifact_cache")

            -   -   com.facebook.buck.artifact_cache.HttpArtifactCacheEvent.Finished

::: description
-   

    All Implemented Interfaces:
    :   `BuckEvent`, `BuckEventExternalInterface`, `LeafEvent`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [HttpArtifactCacheEvent](HttpArtifactCacheEvent.html "class in com.facebook.buck.artifact_cache")

    ------------------------------------------------------------------------

        public static class HttpArtifactCacheEvent.Finished
        extends ArtifactCacheEvent.Finished
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                                       Description
          ------------------- ------------------------------------------- -------------
          `static class `     `HttpArtifactCacheEvent.Finished.Builder`    

          : Nested Classes[ ]{.tabEnd}

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.artifact_cache.ArtifactCacheEvent}

            ### Nested classes/interfaces inherited from class com.facebook.buck.artifact_cache.[ArtifactCacheEvent](ArtifactCacheEvent.html "class in com.facebook.buck.artifact_cache")

            `ArtifactCacheEvent.CacheMode, ArtifactCacheEvent.Finished, ArtifactCacheEvent.InvocationType, ArtifactCacheEvent.Operation, ArtifactCacheEvent.Started, ArtifactCacheEvent.StoreType`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Fields inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](../event/external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `BUILD_FINISHED, BUILD_REPORT, BUILD_STARTED, BUILD_STATUS_EVENT, CACHE_RATE_STATS_UPDATE_EVENT, INDIVIDUAL_TEST_AWAITING_RESULTS, INSTALL_STARTED, PARSE_FINISHED, PARSE_STARTED, PROJECT_GENERATION_FINISHED, PROJECT_GENERATION_STARTED, TEST_RUN_STARTED`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                               Description
          --------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `Finished​(ArtifactCacheEvent.Started event,         HttpArtifactCacheEvent.HttpArtifactCacheEventStoreData data)`                                          
          `Finished​(ArtifactCacheEvent.Started event,         Optional<BuildTarget> target,         HttpArtifactCacheEvent.HttpArtifactCacheEventFetchData data)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `configure​(long       | ::: block             |
        |                       |  timestampMillis,     | Method to configure   |
        |                       |       long nanoTime,  | an event before       |
        |                       |          long userThr | posting it to the     |
        |                       | eadNanoTime,          | [`BuckEventBus`](../e |
        |                       |  long threadId,       | vent/BuckEventBus.htm |
        |                       |     BuildId buildId)` | l "interface in com.f |
        |                       |                       | acebook.buck.event"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getEventName()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `HttpArtifactC        | `getFetchData()`      |                       |
        | acheEvent.HttpArtifac |                       |                       |
        | tCacheEventFetchData` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `getReq               |                       |
        |                       | uestDurationMillis()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Artifa               | `getStartedEvent()`   |                       |
        | ctCacheEvent.Started` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `HttpArtifactC        | `getStoreData()`      |                       |
        | acheEvent.HttpArtifac |                       |                       |
        | tCacheEventStoreData` |                       |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.artifact_cache.ArtifactCacheEvent.Finished}

            ### Methods inherited from class com.facebook.buck.artifact_cache.[ArtifactCacheEvent.Finished](ArtifactCacheEvent.Finished.html "class in com.facebook.buck.artifact_cache")

            `equals, getCacheResult, hashCode, isSuccess`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.artifact_cache.ArtifactCacheEvent}

            ### Methods inherited from class com.facebook.buck.artifact_cache.[ArtifactCacheEvent](ArtifactCacheEvent.html "class in com.facebook.buck.artifact_cache")

            `getCategory, getInvocationType, getOperation, getRuleKeys, getStoreType, getTarget, getValueString`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.event.AbstractBuckEvent}

            ### Methods inherited from class com.facebook.buck.event.[AbstractBuckEvent](../event/AbstractBuckEvent.html "class in com.facebook.buck.event")

            `getBuildId, getEventKey, getNanoTime, getThreadId, getThreadUserNanoTime, getTimestampMillis, isConfigured, isRelatedTo, toLogMessage, toString`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.event.BuckEvent}

            ### Methods inherited from interface com.facebook.buck.event.[BuckEvent](../event/BuckEvent.html "interface in com.facebook.buck.event")

            `getBuildId, getEventKey, getNanoTime, getThreadId, getThreadUserNanoTime, isConfigured, isRelatedTo, toLogMessage`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Methods inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](../event/external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `getTimestampMillis, storeLastInstanceAndReplayForNewClients`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.artifact_cache.ArtifactCacheEvent.Started,java.util.Optional,com.facebook.buck.artifact_cache.HttpArtifactCacheEvent.HttpArtifactCacheEventFetchData)}

        -   #### Finished

                public Finished​(ArtifactCacheEvent.Started event,
                                Optional<BuildTarget> target,
                                HttpArtifactCacheEvent.HttpArtifactCacheEventFetchData data)

        []{#<init>(com.facebook.buck.artifact_cache.ArtifactCacheEvent.Started,com.facebook.buck.artifact_cache.HttpArtifactCacheEvent.HttpArtifactCacheEventStoreData)}

        -   #### Finished

                public Finished​(ArtifactCacheEvent.Started event,
                                HttpArtifactCacheEvent.HttpArtifactCacheEventStoreData data)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getRequestDurationMillis()}

        -   #### getRequestDurationMillis

            ``` methodSignature
            public long getRequestDurationMillis()
            ```

        []{#getFetchData()}

        -   #### getFetchData

            ``` methodSignature
            public HttpArtifactCacheEvent.HttpArtifactCacheEventFetchData getFetchData()
            ```

        []{#getStartedEvent()}

        -   #### getStartedEvent

            ``` methodSignature
            public ArtifactCacheEvent.Started getStartedEvent()
            ```

        []{#getStoreData()}

        -   #### getStoreData

            ``` methodSignature
            public HttpArtifactCacheEvent.HttpArtifactCacheEventStoreData getStoreData()
            ```

        []{#configure(long,long,long,long,com.facebook.buck.core.model.BuildId)}

        -   #### configure

            ``` methodSignature
            public void configure​(long timestampMillis,
                                  long nanoTime,
                                  long userThreadNanoTime,
                                  long threadId,
                                  BuildId buildId)
            ```

            ::: block
            [Description copied from
            class: `AbstractBuckEvent`]{.descfrmTypeLabel}
            :::

            ::: block
            Method to configure an event before posting it to the
            [`BuckEventBus`](../event/BuckEventBus.html "interface in com.facebook.buck.event").
            This method should only be invoked once per event, and only
            by the
            [`BuckEventBus`](../event/BuckEventBus.html "interface in com.facebook.buck.event")
            in production code.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `configure` in interface `BuckEvent`

            [Overrides:]{.overrideSpecifyLabel}
            :   `configure` in class `AbstractBuckEvent`

        []{#getEventName()}

        -   #### getEventName

            ``` methodSignature
            public String getEventName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getEventName` in interface `BuckEventExternalInterface`

            [Specified by:]{.overrideSpecifyLabel}
            :   `getEventName` in class `ArtifactCacheEvent`

            [Returns:]{.returnLabel}
            :   the type of the event.
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
