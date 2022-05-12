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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Class AnnotationProcessingEvent {#class-annotationprocessingevent .title title="Class AnnotationProcessingEvent"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.event.AbstractBuckEvent](../../event/AbstractBuckEvent.html "class in com.facebook.buck.event")

    -   -   com.facebook.buck.jvm.java.AnnotationProcessingEvent

::: description
-   

    All Implemented Interfaces:
    :   `BuckEvent`, `BuckEventExternalInterface`, `WorkAdvanceEvent`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `AnnotationProcessingEvent.Finished`,
        `AnnotationProcessingEvent.Started`

    ------------------------------------------------------------------------

        public abstract class AnnotationProcessingEvent
        extends AbstractBuckEvent
        implements WorkAdvanceEvent

    ::: block
    Base class for events about Java annotation processing.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                                   Description
          ------------------- --------------------------------------- -------------
          `static class `     `AnnotationProcessingEvent.Finished`     
          `static class `     `AnnotationProcessingEvent.Operation`    
          `static class `     `AnnotationProcessingEvent.Started`      

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Fields inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](../../event/external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `BUILD_FINISHED, BUILD_REPORT, BUILD_STARTED, BUILD_STATUS_EVENT, CACHE_RATE_STATS_UPDATE_EVENT, INDIVIDUAL_TEST_AWAITING_RESULTS, INSTALL_STARTED, PARSE_FINISHED, PARSE_STARTED, PROJECT_GENERATION_FINISHED, PROJECT_GENERATION_STARTED, TEST_RUN_STARTED`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                                                                                                                                                                                                                                                                           Description
          -------------- --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `protected `   `AnnotationProcessingEvent​(EventKey eventKey,                          BuildTarget buildTarget,                          String annotationProcessorName,                          AnnotationProcessingEvent.Operation operation,                          int round,                          boolean isLastRound)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                             Method                                                                                                                                                                          Description
          --------------------------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `static AnnotationProcessingEvent.Finished`   `finished​(AnnotationProcessingEvent.Started started)`                                                                                                                            
          `String`                                      `getAnnotationProcessorName()`                                                                                                                                                   
          `BuildTarget`                                 `getBuildTarget()`                                                                                                                                                               
          `String`                                      `getCategory()`                                                                                                                                                                  
          `AnnotationProcessingEvent.Operation`         `getOperation()`                                                                                                                                                                 
          `int`                                         `getRound()`                                                                                                                                                                     
          `protected String`                            `getValueString()`                                                                                                                                                               
          `boolean`                                     `isLastRound()`                                                                                                                                                                  
          `static AnnotationProcessingEvent.Started`    `started​(BuildTarget buildTarget,        String annotationProcessorName,        AnnotationProcessingEvent.Operation operation,        int round,        boolean isLastRound)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

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
        -   []{#methods.inherited.from.class.com.facebook.buck.event.BuckEvent}

            ### Methods inherited from interface com.facebook.buck.event.[BuckEvent](../../event/BuckEvent.html "interface in com.facebook.buck.event")

            `configure, getBuildId, getEventKey, getNanoTime, getThreadId, getThreadUserNanoTime, isConfigured, isRelatedTo, toLogMessage`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Methods inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](../../event/external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `getEventName, getTimestampMillis, storeLastInstanceAndReplayForNewClients`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.event.EventKey,com.facebook.buck.core.model.BuildTarget,java.lang.String,com.facebook.buck.jvm.java.AnnotationProcessingEvent.Operation,int,boolean)}

        -   #### AnnotationProcessingEvent

                protected AnnotationProcessingEvent​(EventKey eventKey,
                                                    BuildTarget buildTarget,
                                                    String annotationProcessorName,
                                                    AnnotationProcessingEvent.Operation operation,
                                                    int round,
                                                    boolean isLastRound)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildTarget()}

        -   #### getBuildTarget

            ``` methodSignature
            public BuildTarget getBuildTarget()
            ```

        []{#getAnnotationProcessorName()}

        -   #### getAnnotationProcessorName

            ``` methodSignature
            public String getAnnotationProcessorName()
            ```

        []{#getOperation()}

        -   #### getOperation

            ``` methodSignature
            public AnnotationProcessingEvent.Operation getOperation()
            ```

        []{#getRound()}

        -   #### getRound

            ``` methodSignature
            public int getRound()
            ```

        []{#isLastRound()}

        -   #### isLastRound

            ``` methodSignature
            public boolean isLastRound()
            ```

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

        []{#started(com.facebook.buck.core.model.BuildTarget,java.lang.String,com.facebook.buck.jvm.java.AnnotationProcessingEvent.Operation,int,boolean)}

        -   #### started

            ``` methodSignature
            public static AnnotationProcessingEvent.Started started​(BuildTarget buildTarget,
                                                                    String annotationProcessorName,
                                                                    AnnotationProcessingEvent.Operation operation,
                                                                    int round,
                                                                    boolean isLastRound)
            ```

        []{#finished(com.facebook.buck.jvm.java.AnnotationProcessingEvent.Started)}

        -   #### finished

            ``` methodSignature
            public static AnnotationProcessingEvent.Finished finished​(AnnotationProcessingEvent.Started started)
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
