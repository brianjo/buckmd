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
[Package]{.packageLabelInType} [com.facebook.buck.event](package-summary.html)
:::

## Class ActionGraphEvent.Cache.MissWithEmptyCache {#class-actiongraphevent.cache.misswithemptycache .title title="Class ActionGraphEvent.Cache.MissWithEmptyCache"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.event.AbstractBuckEvent](AbstractBuckEvent.html "class in com.facebook.buck.event")

    -   -   [com.facebook.buck.event.ActionGraphEvent](ActionGraphEvent.html "class in com.facebook.buck.event")

        -   -   [com.facebook.buck.event.ActionGraphEvent.Cache](ActionGraphEvent.Cache.html "class in com.facebook.buck.event")

            -   -   com.facebook.buck.event.ActionGraphEvent.Cache.MissWithEmptyCache

::: description
-   

    All Implemented Interfaces:
    :   `BuckEvent`, `BuckEventExternalInterface`, `LeafEvent`,
        `WorkAdvanceEvent`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [ActionGraphEvent.Cache](ActionGraphEvent.Cache.html "class in com.facebook.buck.event")

    ------------------------------------------------------------------------

        public static class ActionGraphEvent.Cache.MissWithEmptyCache
        extends ActionGraphEvent.Cache
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.event.ActionGraphEvent.Cache}

            ### Nested classes/interfaces inherited from class com.facebook.buck.event.[ActionGraphEvent.Cache](ActionGraphEvent.Cache.html "class in com.facebook.buck.event")

            `ActionGraphEvent.Cache.Hit, ActionGraphEvent.Cache.Miss, ActionGraphEvent.Cache.MissWithEmptyCache, ActionGraphEvent.Cache.MissWithTargetGraphDifference, ActionGraphEvent.Cache.MissWithTargetGraphHashMatch`

        ```{=html}
        <!-- -->
        ```
        -   []{#nested.classes.inherited.from.class.com.facebook.buck.event.ActionGraphEvent}

            ### Nested classes/interfaces inherited from class com.facebook.buck.event.[ActionGraphEvent](ActionGraphEvent.html "class in com.facebook.buck.event")

            `ActionGraphEvent.Cache, ActionGraphEvent.Finished, ActionGraphEvent.IncrementalLoad, ActionGraphEvent.Started`
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

          Constructor              Description
          ------------------------ -------------
          `MissWithEmptyCache()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        -   []{#methods.inherited.from.class.com.facebook.buck.event.ActionGraphEvent.Cache}

            ### Methods inherited from class com.facebook.buck.event.[ActionGraphEvent.Cache](ActionGraphEvent.Cache.html "class in com.facebook.buck.event")

            `getEventName, hit, miss, missWithEmptyCache, missWithTargetGraphDifference`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.event.ActionGraphEvent}

            ### Methods inherited from class com.facebook.buck.event.[ActionGraphEvent](ActionGraphEvent.html "class in com.facebook.buck.event")

            `finished, finished, getCategory, getValueString, started`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.event.AbstractBuckEvent}

            ### Methods inherited from class com.facebook.buck.event.[AbstractBuckEvent](AbstractBuckEvent.html "class in com.facebook.buck.event")

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

            ### Methods inherited from interface com.facebook.buck.event.[BuckEvent](BuckEvent.html "interface in com.facebook.buck.event")

            `configure, getBuildId, getEventKey, getNanoTime, getThreadId, getThreadUserNanoTime, isConfigured, isRelatedTo, toLogMessage`

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

        []{#<init>()}

        -   #### MissWithEmptyCache

                public MissWithEmptyCache()
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