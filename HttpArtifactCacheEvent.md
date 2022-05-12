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
[Package]{.packageLabelInType} [com.facebook.buck.artifact_cache](package-summary.html)
:::

## Class HttpArtifactCacheEvent {#class-httpartifactcacheevent .title title="Class HttpArtifactCacheEvent"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.event.AbstractBuckEvent](../event/AbstractBuckEvent.html "class in com.facebook.buck.event")

    -   -   [com.facebook.buck.artifact_cache.ArtifactCacheEvent](ArtifactCacheEvent.html "class in com.facebook.buck.artifact_cache")

        -   -   com.facebook.buck.artifact_cache.HttpArtifactCacheEvent

::: description
-   

    All Implemented Interfaces:
    :   `BuckEvent`, `BuckEventExternalInterface`, `LeafEvent`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `HttpArtifactCacheEvent.Scheduled`

    ------------------------------------------------------------------------

        public abstract class HttpArtifactCacheEvent
        extends ArtifactCacheEvent

    ::: block
    Event produced for HttpArtifactCache operations containing different
    stats.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type     Class                                                      Description
          --------------------- ---------------------------------------------------------- -------------
          `static class `       `HttpArtifactCacheEvent.Finished`                           
          `static interface `   `HttpArtifactCacheEvent.HttpArtifactCacheEventFetchData`    
          `static interface `   `HttpArtifactCacheEvent.HttpArtifactCacheEventStoreData`    
          `static class `       `HttpArtifactCacheEvent.Scheduled`                          
          `static class `       `HttpArtifactCacheEvent.Shutdown`                           
          `static class `       `HttpArtifactCacheEvent.Started`                            

          : Nested Classes[ ]{.tabEnd}

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.artifact_cache.ArtifactCacheEvent}

            ### Nested classes/interfaces inherited from class com.facebook.buck.artifact_cache.[ArtifactCacheEvent](ArtifactCacheEvent.html "class in com.facebook.buck.artifact_cache")

            `ArtifactCacheEvent.CacheMode, ArtifactCacheEvent.InvocationType, ArtifactCacheEvent.Operation, ArtifactCacheEvent.StoreType`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                       Field          Description
          --------------------------------------- -------------- -------------
          `static ArtifactCacheEvent.CacheMode`   `CACHE_MODE`    

          : Fields[ ]{.tabEnd}

        -   []{#fields.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Fields inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](../event/external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `BUILD_FINISHED, BUILD_REPORT, BUILD_STARTED, BUILD_STATUS_EVENT, CACHE_RATE_STATS_UPDATE_EVENT, INDIVIDUAL_TEST_AWAITING_RESULTS, INSTALL_STARTED, PARSE_FINISHED, PARSE_STARTED, PROJECT_GENERATION_FINISHED, PROJECT_GENERATION_STARTED, TEST_RUN_STARTED`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                                                                                                                                                                                                                                                                                                                                           Description
          -------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `protected `   `HttpArtifactCacheEvent​(EventKey eventKey,                       ArtifactCacheEvent.Operation operation,                       Optional<BuildTarget> target,                       com.google.common.collect.ImmutableSet<RuleKey> ruleKeys,                       ArtifactCacheEvent.InvocationType invocationType,                       ArtifactCacheEvent.StoreType storeType)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                    Method                                                                                                                                                                                                 Description
          ------------------------------------------------------------------------------------ ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `static HttpArtifactCacheEvent.Started`                                              `newFetchStartedEvent​(BuildTarget target,                     RuleKey ruleKey)`                                                                                                                         
          `static HttpArtifactCacheEvent.Finished.Builder`                                     `newFinishedEventBuilder​(HttpArtifactCacheEvent.Started event)`                                                                                                                                         
          `static com.facebook.buck.artifact_cache.HttpArtifactCacheEvent.MultiFetchStarted`   `newMultiFetchStartedEvent​(com.google.common.collect.ImmutableList<BuildTarget> targets,                          com.google.common.collect.ImmutableList<RuleKey> ruleKeys)`                           
          `static HttpArtifactCacheEvent.Shutdown`                                             `newShutdownEvent()`                                                                                                                                                                                    
          `static HttpArtifactCacheEvent.Scheduled`                                            `newStoreScheduledEvent​(Optional<BuildTarget> target,                       com.google.common.collect.ImmutableSet<RuleKey> ruleKeys,                       ArtifactCacheEvent.StoreType storeType)`    
          `static HttpArtifactCacheEvent.Started`                                              `newStoreStartedEvent​(HttpArtifactCacheEvent.Scheduled scheduled)`                                                                                                                                      

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.artifact_cache.ArtifactCacheEvent}

            ### Methods inherited from class com.facebook.buck.artifact_cache.[ArtifactCacheEvent](ArtifactCacheEvent.html "class in com.facebook.buck.artifact_cache")

            `getCategory, getEventName, getInvocationType, getOperation, getRuleKeys, getStoreType, getTarget, getValueString`

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
    -   []{#field.detail}

        ### Field Detail

        []{#CACHE_MODE}

        -   #### CACHE_MODE

                public static final ArtifactCacheEvent.CacheMode CACHE_MODE
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.event.EventKey,com.facebook.buck.artifact_cache.ArtifactCacheEvent.Operation,java.util.Optional,com.google.common.collect.ImmutableSet,com.facebook.buck.artifact_cache.ArtifactCacheEvent.InvocationType,com.facebook.buck.artifact_cache.ArtifactCacheEvent.StoreType)}

        -   #### HttpArtifactCacheEvent

                protected HttpArtifactCacheEvent​(EventKey eventKey,
                                                 ArtifactCacheEvent.Operation operation,
                                                 Optional<BuildTarget> target,
                                                 com.google.common.collect.ImmutableSet<RuleKey> ruleKeys,
                                                 ArtifactCacheEvent.InvocationType invocationType,
                                                 ArtifactCacheEvent.StoreType storeType)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#newFetchStartedEvent(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rulekey.RuleKey)}

        -   #### newFetchStartedEvent

            ``` methodSignature
            public static HttpArtifactCacheEvent.Started newFetchStartedEvent​(@Nullable
                                                                              BuildTarget target,
                                                                              RuleKey ruleKey)
            ```

        []{#newStoreStartedEvent(com.facebook.buck.artifact_cache.HttpArtifactCacheEvent.Scheduled)}

        -   #### newStoreStartedEvent

            ``` methodSignature
            public static HttpArtifactCacheEvent.Started newStoreStartedEvent​(HttpArtifactCacheEvent.Scheduled scheduled)
            ```

        []{#newStoreScheduledEvent(java.util.Optional,com.google.common.collect.ImmutableSet,com.facebook.buck.artifact_cache.ArtifactCacheEvent.StoreType)}

        -   #### newStoreScheduledEvent

            ``` methodSignature
            public static HttpArtifactCacheEvent.Scheduled newStoreScheduledEvent​(Optional<BuildTarget> target,
                                                                                  com.google.common.collect.ImmutableSet<RuleKey> ruleKeys,
                                                                                  ArtifactCacheEvent.StoreType storeType)
            ```

        []{#newShutdownEvent()}

        -   #### newShutdownEvent

            ``` methodSignature
            public static HttpArtifactCacheEvent.Shutdown newShutdownEvent()
            ```

        []{#newFinishedEventBuilder(com.facebook.buck.artifact_cache.HttpArtifactCacheEvent.Started)}

        -   #### newFinishedEventBuilder

            ``` methodSignature
            public static HttpArtifactCacheEvent.Finished.Builder newFinishedEventBuilder​(HttpArtifactCacheEvent.Started event)
            ```

        []{#newMultiFetchStartedEvent(com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableList)}

        -   #### newMultiFetchStartedEvent

            ``` methodSignature
            public static com.facebook.buck.artifact_cache.HttpArtifactCacheEvent.MultiFetchStarted newMultiFetchStartedEvent​(com.google.common.collect.ImmutableList<BuildTarget> targets,
                                                                                                                              com.google.common.collect.ImmutableList<RuleKey> ruleKeys)
            ```
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
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
