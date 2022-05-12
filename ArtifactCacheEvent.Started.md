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
-   Method

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

## Class ArtifactCacheEvent.Started {#class-artifactcacheevent.started .title title="Class ArtifactCacheEvent.Started"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.event.AbstractBuckEvent](../event/AbstractBuckEvent.html "class in com.facebook.buck.event")

    -   -   [com.facebook.buck.artifact_cache.ArtifactCacheEvent](ArtifactCacheEvent.html "class in com.facebook.buck.artifact_cache")

        -   -   com.facebook.buck.artifact_cache.ArtifactCacheEvent.Started

::: description
-   

    All Implemented Interfaces:
    :   `BuckEvent`, `BuckEventExternalInterface`, `LeafEvent`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `DirArtifactCacheEvent.Started`,
        `HttpArtifactCacheEvent.Started`,
        `SQLiteArtifactCacheEvent.Started`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [ArtifactCacheEvent](ArtifactCacheEvent.html "class in com.facebook.buck.artifact_cache")

    ------------------------------------------------------------------------

        public abstract static class ArtifactCacheEvent.Started
        extends ArtifactCacheEvent
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

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

          Modifier       Constructor                                                                                                                                                                                                                                                                                                                                Description
          -------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `protected `   `Started​(EventKey eventKey,        ArtifactCacheEvent.CacheMode cacheMode,        ArtifactCacheEvent.Operation operation,        Optional<BuildTarget> target,        com.google.common.collect.ImmutableSet<RuleKey> ruleKeys,        ArtifactCacheEvent.InvocationType invocationType)`                                                   
          `protected `   `Started​(EventKey eventKey,        ArtifactCacheEvent.CacheMode cacheMode,        ArtifactCacheEvent.Operation operation,        Optional<BuildTarget> target,        com.google.common.collect.ImmutableSet<RuleKey> ruleKeys,        ArtifactCacheEvent.InvocationType invocationType,        ArtifactCacheEvent.StoreType storeType)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.event.EventKey,com.facebook.buck.artifact_cache.ArtifactCacheEvent.CacheMode,com.facebook.buck.artifact_cache.ArtifactCacheEvent.Operation,java.util.Optional,com.google.common.collect.ImmutableSet,com.facebook.buck.artifact_cache.ArtifactCacheEvent.InvocationType)}

        -   #### Started

                protected Started​(EventKey eventKey,
                                  ArtifactCacheEvent.CacheMode cacheMode,
                                  ArtifactCacheEvent.Operation operation,
                                  Optional<BuildTarget> target,
                                  com.google.common.collect.ImmutableSet<RuleKey> ruleKeys,
                                  ArtifactCacheEvent.InvocationType invocationType)

        []{#<init>(com.facebook.buck.event.EventKey,com.facebook.buck.artifact_cache.ArtifactCacheEvent.CacheMode,com.facebook.buck.artifact_cache.ArtifactCacheEvent.Operation,java.util.Optional,com.google.common.collect.ImmutableSet,com.facebook.buck.artifact_cache.ArtifactCacheEvent.InvocationType,com.facebook.buck.artifact_cache.ArtifactCacheEvent.StoreType)}

        -   #### Started

                protected Started​(EventKey eventKey,
                                  ArtifactCacheEvent.CacheMode cacheMode,
                                  ArtifactCacheEvent.Operation operation,
                                  Optional<BuildTarget> target,
                                  com.google.common.collect.ImmutableSet<RuleKey> ruleKeys,
                                  ArtifactCacheEvent.InvocationType invocationType,
                                  ArtifactCacheEvent.StoreType storeType)
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
-   Method

</div>

[]{#skip.navbar.bottom}
:::
