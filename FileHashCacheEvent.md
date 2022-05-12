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

## Class FileHashCacheEvent {#class-filehashcacheevent .title title="Class FileHashCacheEvent"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.event.AbstractBuckEvent](AbstractBuckEvent.html "class in com.facebook.buck.event")

    -   -   com.facebook.buck.event.FileHashCacheEvent

::: description
-   

    All Implemented Interfaces:
    :   `BuckEvent`, `BuckEventExternalInterface`, `LeafEvent`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `FileHashCacheEvent.InvalidationFinished`,
        `FileHashCacheEvent.InvalidationStarted`

    ------------------------------------------------------------------------

        public class FileHashCacheEvent
        extends AbstractBuckEvent
        implements LeafEvent
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                                       Description
          ------------------- ------------------------------------------- -------------
          `static class `     `FileHashCacheEvent.InvalidationFinished`    
          `static class `     `FileHashCacheEvent.InvalidationStarted`     

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

          Constructor                                                                                                                                                    Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `FileHashCacheEvent​(EventKey eventKey)`                                                                                                                         
          `FileHashCacheEvent​(String subCategory,                   long amortizedNanoTime,                   long totalTime,                   long dataPointsCount)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                  Method                                                                   Description
          -------------------------------------------------- ------------------------------------------------------------------------ -------------
          `long`                                             `getAmortizedNanoTime()`                                                  
          `String`                                           `getCategory()`                                                           
          `long`                                             `getDataPointsCount()`                                                    
          `String`                                           `getEventName()`                                                          
          `long`                                             `getTotalNanoTime()`                                                      
          `protected String`                                 `getValueString()`                                                        
          `static FileHashCacheEvent.InvalidationFinished`   `invalidationFinished​(FileHashCacheEvent.InvalidationStarted started)`    
          `static FileHashCacheEvent.InvalidationStarted`    `invalidationStarted()`                                                   
          `void`                                             `setCategory​(String category)`                                            

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

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

        []{#<init>(java.lang.String,long,long,long)}

        -   #### FileHashCacheEvent

                public FileHashCacheEvent​(String subCategory,
                                          long amortizedNanoTime,
                                          long totalTime,
                                          long dataPointsCount)

        []{#<init>(com.facebook.buck.event.EventKey)}

        -   #### FileHashCacheEvent

                public FileHashCacheEvent​(EventKey eventKey)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

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

        []{#setCategory(java.lang.String)}

        -   #### setCategory

            ``` methodSignature
            public void setCategory​(String category)
            ```

        []{#getAmortizedNanoTime()}

        -   #### getAmortizedNanoTime

            ``` methodSignature
            public long getAmortizedNanoTime()
            ```

        []{#getTotalNanoTime()}

        -   #### getTotalNanoTime

            ``` methodSignature
            public long getTotalNanoTime()
            ```

        []{#getDataPointsCount()}

        -   #### getDataPointsCount

            ``` methodSignature
            public long getDataPointsCount()
            ```

        []{#getEventName()}

        -   #### getEventName

            ``` methodSignature
            public String getEventName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getEventName` in interface `BuckEventExternalInterface`

            [Returns:]{.returnLabel}
            :   the type of the event.

        []{#getValueString()}

        -   #### getValueString

            ``` methodSignature
            protected String getValueString()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getValueString` in class `AbstractBuckEvent`

        []{#invalidationStarted()}

        -   #### invalidationStarted

            ``` methodSignature
            public static FileHashCacheEvent.InvalidationStarted invalidationStarted()
            ```

        []{#invalidationFinished(com.facebook.buck.event.FileHashCacheEvent.InvalidationStarted)}

        -   #### invalidationFinished

            ``` methodSignature
            public static FileHashCacheEvent.InvalidationFinished invalidationFinished​(FileHashCacheEvent.InvalidationStarted started)
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
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
