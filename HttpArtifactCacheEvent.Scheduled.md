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

## Class HttpArtifactCacheEvent.Scheduled {#class-httpartifactcacheevent.scheduled .title title="Class HttpArtifactCacheEvent.Scheduled"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.event.AbstractBuckEvent](../event/AbstractBuckEvent.html "class in com.facebook.buck.event")

    -   -   [com.facebook.buck.artifact_cache.ArtifactCacheEvent](ArtifactCacheEvent.html "class in com.facebook.buck.artifact_cache")

        -   -   [com.facebook.buck.artifact_cache.HttpArtifactCacheEvent](HttpArtifactCacheEvent.html "class in com.facebook.buck.artifact_cache")

            -   -   com.facebook.buck.artifact_cache.HttpArtifactCacheEvent.Scheduled

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

        public static class HttpArtifactCacheEvent.Scheduled
        extends HttpArtifactCacheEvent
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.artifact_cache.HttpArtifactCacheEvent}

            ### Nested classes/interfaces inherited from class com.facebook.buck.artifact_cache.[HttpArtifactCacheEvent](HttpArtifactCacheEvent.html "class in com.facebook.buck.artifact_cache")

            `HttpArtifactCacheEvent.Finished, HttpArtifactCacheEvent.HttpArtifactCacheEventFetchData, HttpArtifactCacheEvent.HttpArtifactCacheEventStoreData, HttpArtifactCacheEvent.Scheduled, HttpArtifactCacheEvent.Shutdown, HttpArtifactCacheEvent.Started`

        ```{=html}
        <!-- -->
        ```
        -   []{#nested.classes.inherited.from.class.com.facebook.buck.artifact_cache.ArtifactCacheEvent}

            ### Nested classes/interfaces inherited from class com.facebook.buck.artifact_cache.[ArtifactCacheEvent](ArtifactCacheEvent.html "class in com.facebook.buck.artifact_cache")

            `ArtifactCacheEvent.CacheMode, ArtifactCacheEvent.InvocationType, ArtifactCacheEvent.Operation, ArtifactCacheEvent.StoreType`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.artifact_cache.HttpArtifactCacheEvent}

            ### Fields inherited from class com.facebook.buck.artifact_cache.[HttpArtifactCacheEvent](HttpArtifactCacheEvent.html "class in com.facebook.buck.artifact_cache")

            `CACHE_MODE`

        ```{=html}
        <!-- -->
        ```
        -   []{#fields.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Fields inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](../event/external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `BUILD_FINISHED, BUILD_REPORT, BUILD_STARTED, BUILD_STATUS_EVENT, CACHE_RATE_STATS_UPDATE_EVENT, INDIVIDUAL_TEST_AWAITING_RESULTS, INSTALL_STARTED, PARSE_FINISHED, PARSE_STARTED, PROJECT_GENERATION_FINISHED, PROJECT_GENERATION_STARTED, TEST_RUN_STARTED`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                      Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `Scheduled​(ArtifactCacheEvent.Operation operation,          Optional<BuildTarget> target,          com.google.common.collect.ImmutableSet<RuleKey> ruleKeys,          ArtifactCacheEvent.StoreType storeType)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method             Description
          ------------------- ------------------ -------------
          `String`            `getEventName()`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.artifact_cache.HttpArtifactCacheEvent}

            ### Methods inherited from class com.facebook.buck.artifact_cache.[HttpArtifactCacheEvent](HttpArtifactCacheEvent.html "class in com.facebook.buck.artifact_cache")

            `newFetchStartedEvent, newFinishedEventBuilder, newMultiFetchStartedEvent, newShutdownEvent, newStoreScheduledEvent, newStoreStartedEvent`

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

            `configure, equals, getBuildId, getEventKey, getNanoTime, getThreadId, getThreadUserNanoTime, getTimestampMillis, hashCode, isConfigured, isRelatedTo, toLogMessage, toString`

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

            `configure, getBuildId, getEventKey, getNanoTime, getThreadId, getThreadUserNanoTime, isConfigured, isRelatedTo, toLogMessage`

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

        []{#<init>(com.facebook.buck.artifact_cache.ArtifactCacheEvent.Operation,java.util.Optional,com.google.common.collect.ImmutableSet,com.facebook.buck.artifact_cache.ArtifactCacheEvent.StoreType)}

        -   #### Scheduled

                public Scheduled​(ArtifactCacheEvent.Operation operation,
                                 Optional<BuildTarget> target,
                                 com.google.common.collect.ImmutableSet<RuleKey> ruleKeys,
                                 ArtifactCacheEvent.StoreType storeType)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

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
