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

## Class ArtifactCacheEvent {#class-artifactcacheevent .title title="Class ArtifactCacheEvent"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.event.AbstractBuckEvent](../event/AbstractBuckEvent.html "class in com.facebook.buck.event")

    -   -   com.facebook.buck.artifact_cache.ArtifactCacheEvent

::: description
-   

    All Implemented Interfaces:
    :   `BuckEvent`, `BuckEventExternalInterface`, `LeafEvent`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `ArtifactCacheEvent.Finished`, `ArtifactCacheEvent.Started`,
        `HttpArtifactCacheEvent`

    ------------------------------------------------------------------------

        public abstract class ArtifactCacheEvent
        extends AbstractBuckEvent
        implements LeafEvent
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `Artifact             |                       |
        |                       | CacheEvent.CacheMode` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `Artifac              |                       |
        |                       | tCacheEvent.Finished` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `ArtifactCache        |                       |
        |                       | Event.InvocationType` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `Artifact             |                       |
        |                       | CacheEvent.Operation` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `Artifa               |                       |
        |                       | ctCacheEvent.Started` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `Artifact             | ::: block             |
        |                       | CacheEvent.StoreType` | For                   |
        |                       |                       | [`Art                 |
        |                       |                       | ifactCacheEvent.Opera |
        |                       |                       | tion`](ArtifactCacheE |
        |                       |                       | vent.Operation.html " |
        |                       |                       | enum in com.facebook. |
        |                       |                       | buck.artifact_cache") |
        |                       |                       | STORE there are       |
        |                       |                       | different store       |
        |                       |                       | types, storing the    |
        |                       |                       | actual artifact or    |
        |                       |                       | the manifest of it.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
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

          Modifier       Constructor                                                                                                                                                                                                                                                                                                                                                                                                             Description
          -------------- ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `protected `   `ArtifactCacheEvent​(EventKey eventKey,                   ArtifactCacheEvent.CacheMode cacheMode,                   ArtifactCacheEvent.Operation operation,                   Optional<BuildTarget> target,                   com.google.common.collect.ImmutableSet<RuleKey> ruleKeys,                   ArtifactCacheEvent.InvocationType invocationType,                   ArtifactCacheEvent.StoreType storeType)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                   Method                  Description
          --------------------------------------------------- ----------------------- -------------
          `String`                                            `getCategory()`          
          `abstract String`                                   `getEventName()`         
          `ArtifactCacheEvent.InvocationType`                 `getInvocationType()`    
          `ArtifactCacheEvent.Operation`                      `getOperation()`         
          `com.google.common.collect.ImmutableSet<RuleKey>`   `getRuleKeys()`          
          `ArtifactCacheEvent.StoreType`                      `getStoreType()`         
          `Optional<BuildTarget>`                             `getTarget()`            
          `protected String`                                  `getValueString()`       

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

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

        []{#<init>(com.facebook.buck.event.EventKey,com.facebook.buck.artifact_cache.ArtifactCacheEvent.CacheMode,com.facebook.buck.artifact_cache.ArtifactCacheEvent.Operation,java.util.Optional,com.google.common.collect.ImmutableSet,com.facebook.buck.artifact_cache.ArtifactCacheEvent.InvocationType,com.facebook.buck.artifact_cache.ArtifactCacheEvent.StoreType)}

        -   #### ArtifactCacheEvent

                protected ArtifactCacheEvent​(EventKey eventKey,
                                             ArtifactCacheEvent.CacheMode cacheMode,
                                             ArtifactCacheEvent.Operation operation,
                                             Optional<BuildTarget> target,
                                             com.google.common.collect.ImmutableSet<RuleKey> ruleKeys,
                                             ArtifactCacheEvent.InvocationType invocationType,
                                             ArtifactCacheEvent.StoreType storeType)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getValueString()}

        -   #### getValueString

            ``` methodSignature
            protected String getValueString()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getValueString` in class `AbstractBuckEvent`

        []{#getCategory()}

        -   #### getCategory

            ``` methodSignature
            public String getCategory()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCategory` in interface `LeafEvent`

            [Returns:]{.returnLabel}
            :   The category time spent in this event should be
                accounted under.

        []{#getOperation()}

        -   #### getOperation

            ``` methodSignature
            public ArtifactCacheEvent.Operation getOperation()
            ```

        []{#getRuleKeys()}

        -   #### getRuleKeys

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<RuleKey> getRuleKeys()
            ```

        []{#getTarget()}

        -   #### getTarget

            ``` methodSignature
            public Optional<BuildTarget> getTarget()
            ```

        []{#getInvocationType()}

        -   #### getInvocationType

            ``` methodSignature
            public ArtifactCacheEvent.InvocationType getInvocationType()
            ```

        []{#getStoreType()}

        -   #### getStoreType

            ``` methodSignature
            public ArtifactCacheEvent.StoreType getStoreType()
            ```

        []{#getEventName()}

        -   #### getEventName

            ``` methodSignature
            public abstract String getEventName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getEventName` in interface `BuckEventExternalInterface`

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
