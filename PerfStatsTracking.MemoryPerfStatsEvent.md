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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.util.perf](package-summary.html)
:::

## Class PerfStatsTracking.MemoryPerfStatsEvent {#class-perfstatstracking.memoryperfstatsevent .title title="Class PerfStatsTracking.MemoryPerfStatsEvent"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.event.AbstractBuckEvent](../../event/AbstractBuckEvent.html "class in com.facebook.buck.event")

    -   -   [com.facebook.buck.util.perf.PerfStatsTracking.PerfStatsEvent](PerfStatsTracking.PerfStatsEvent.html "class in com.facebook.buck.util.perf")

        -   -   com.facebook.buck.util.perf.PerfStatsTracking.MemoryPerfStatsEvent

::: description
-   

    All Implemented Interfaces:
    :   `BuckEvent`, `BuckEventExternalInterface`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [PerfStatsTracking](PerfStatsTracking.html "class in com.facebook.buck.util.perf")

    ------------------------------------------------------------------------

        public static class PerfStatsTracking.MemoryPerfStatsEvent
        extends PerfStatsTracking.PerfStatsEvent

    ::: block
    Performance event that tracks current memory usage of Buck
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Fields inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](../../event/external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `BUILD_FINISHED, BUILD_REPORT, BUILD_STARTED, BUILD_STATUS_EVENT, CACHE_RATE_STATS_UPDATE_EVENT, INDIVIDUAL_TEST_AWAITING_RESULTS, INSTALL_STARTED, PARSE_FINISHED, PARSE_STARTED, PROJECT_GENERATION_FINISHED, PROJECT_GENERATION_STARTED, TEST_RUN_STARTED`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `Memory                           | ::: block                         |
        | PerfStatsEvent​(long freeMemoryByt | Construct a new memory            |
        | es,                     long tota | performance tracking object       |
        | lMemoryBytes,                     | :::                               |
        |  long maxMemoryBytes,             |                                   |
        |          long timeSpentInGcMs,    |                                   |
        |                   Map<String,​Long |                                   |
        | > currentMemoryBytesUsageByPool)` |                                   |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type    Method                                 Description
          -------------------- -------------------------------------- -------------
          `Map<String,​Long>`   `getCurrentMemoryBytesUsageByPool()`    
          `long`               `getFreeMemoryBytes()`                  
          `long`               `getMaxMemoryBytes()`                   
          `long`               `getTimeSpentInGcMs()`                  
          `long`               `getTotalMemoryBytes()`                 

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.util.perf.PerfStatsTracking.PerfStatsEvent}

            ### Methods inherited from class com.facebook.buck.util.perf.[PerfStatsTracking.PerfStatsEvent](PerfStatsTracking.PerfStatsEvent.html "class in com.facebook.buck.util.perf")

            `getEventName, getValueString`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.event.AbstractBuckEvent}

            ### Methods inherited from class com.facebook.buck.event.[AbstractBuckEvent](../../event/AbstractBuckEvent.html "class in com.facebook.buck.event")

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
        -   []{#methods.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Methods inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](../../event/external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `storeLastInstanceAndReplayForNewClients`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(long,long,long,long,java.util.Map)}

        -   #### MemoryPerfStatsEvent

                public MemoryPerfStatsEvent​(long freeMemoryBytes,
                                            long totalMemoryBytes,
                                            long maxMemoryBytes,
                                            long timeSpentInGcMs,
                                            Map<String,​Long> currentMemoryBytesUsageByPool)

            ::: block
            Construct a new memory performance tracking object
            :::

            [Parameters:]{.paramLabel}
            :   `freeMemoryBytes` - Memory in bytes available for JVM to
                use for new allocations
            :   `totalMemoryBytes` - Memory in bytes that JVM allocated
                at the moment, both used and unused
            :   `maxMemoryBytes` - Maximum amount of memory in bytes
                that JVM can allocate (-Xmx parameter)
            :   `timeSpentInGcMs` - Total amount of milliseconds spent
                doing garbage collection till now
            :   `currentMemoryBytesUsageByPool` - A map of JVM memory
                pool name to the amount of memory used by that pool
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getFreeMemoryBytes()}

        -   #### getFreeMemoryBytes

            ``` methodSignature
            public long getFreeMemoryBytes()
            ```

            [Returns:]{.returnLabel}
            :   Memory in bytes available for JVM to use for new
                allocations

        []{#getTotalMemoryBytes()}

        -   #### getTotalMemoryBytes

            ``` methodSignature
            public long getTotalMemoryBytes()
            ```

            [Returns:]{.returnLabel}
            :   Memory in bytes that JVM allocated at the moment, both
                used and unused

        []{#getMaxMemoryBytes()}

        -   #### getMaxMemoryBytes

            ``` methodSignature
            public long getMaxMemoryBytes()
            ```

            [Returns:]{.returnLabel}
            :   Maximum amount of memory in bytes that JVM can allocate
                (-Xmx parameter)

        []{#getTimeSpentInGcMs()}

        -   #### getTimeSpentInGcMs

            ``` methodSignature
            public long getTimeSpentInGcMs()
            ```

            [Returns:]{.returnLabel}
            :   Total amount of milliseconds spent doing garbage
                collection till now

        []{#getCurrentMemoryBytesUsageByPool()}

        -   #### getCurrentMemoryBytesUsageByPool

            ``` methodSignature
            public Map<String,​Long> getCurrentMemoryBytesUsageByPool()
            ```

            [Returns:]{.returnLabel}
            :   A map of JVM memory pool name to the amount of memory
                used by that pool
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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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
