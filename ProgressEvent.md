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
[Package]{.packageLabelInType} [com.facebook.buck.event](package-summary.html)
:::

## Class ProgressEvent {#class-progressevent .title title="Class ProgressEvent"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.event.AbstractBuckEvent](AbstractBuckEvent.html "class in com.facebook.buck.event")

    -   -   com.facebook.buck.event.ProgressEvent

::: description
-   

    All Implemented Interfaces:
    :   `BuckEvent`, `BuckEventExternalInterface`,
        `ProgressEventInterface`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `ProgressEvent.BuildProgressUpdated`,
        `ProgressEvent.ParsingProgressUpdated`,
        `ProgressEvent.ProjectGenerationProgressUpdated`

    ------------------------------------------------------------------------

        public abstract class ProgressEvent
        extends AbstractBuckEvent
        implements ProgressEventInterface
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                                              Description
          ------------------- -------------------------------------------------- -------------
          `static class `     `ProgressEvent.BuildProgressUpdated`                
          `static class `     `ProgressEvent.ParsingProgressUpdated`              
          `static class `     `ProgressEvent.ProjectGenerationProgressUpdated`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type    Field             Description
          -------------------- ----------------- -------------
          `protected double`   `progressValue`    

          : Fields[ ]{.tabEnd}

        -   []{#fields.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Fields inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `BUILD_FINISHED, BUILD_REPORT, BUILD_STARTED, BUILD_STATUS_EVENT, CACHE_RATE_STATS_UPDATE_EVENT, INDIVIDUAL_TEST_AWAITING_RESULTS, INSTALL_STARTED, PARSE_FINISHED, PARSE_STARTED, PROJECT_GENERATION_FINISHED, PROJECT_GENERATION_STARTED, TEST_RUN_STARTED`

        ```{=html}
        <!-- -->
        ```
        -   []{#fields.inherited.from.class.com.facebook.buck.event.external.events.ProgressEventInterface}

            ### Fields inherited from interface com.facebook.buck.event.external.events.[ProgressEventInterface](external/events/ProgressEventInterface.html "interface in com.facebook.buck.event.external.events")

            `BUILD_PROGRESS_UPDATED, PARSING_PROGRESS_UPDATED, PROJECT_GENERATION_PROGRESS_UPDATED`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                             Description
          -------------- --------------------------------------- -------------
          `protected `   `ProgressEvent​(double progressValue)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                         Method                                         Description
          --------------------------------------------------------- ---------------------------------------------- -------------
          `static ProgressEvent.BuildProgressUpdated`               `buildProgressUpdated​(double v)`                
          `double`                                                  `getProgressValue()`                            
          `protected String`                                        `getValueString()`                              
          `static ProgressEvent.ParsingProgressUpdated`             `parsingProgressUpdated​(double v)`              
          `static ProgressEvent.ProjectGenerationProgressUpdated`   `projectGenerationProgressUpdated​(double v)`    

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
        -   []{#methods.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Methods inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `getEventName, getTimestampMillis, storeLastInstanceAndReplayForNewClients`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#progressValue}

        -   #### progressValue

                protected final double progressValue
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(double)}

        -   #### ProgressEvent

                protected ProgressEvent​(double progressValue)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#parsingProgressUpdated(double)}

        -   #### parsingProgressUpdated

            ``` methodSignature
            public static ProgressEvent.ParsingProgressUpdated parsingProgressUpdated​(double v)
            ```

        []{#projectGenerationProgressUpdated(double)}

        -   #### projectGenerationProgressUpdated

            ``` methodSignature
            public static ProgressEvent.ProjectGenerationProgressUpdated projectGenerationProgressUpdated​(double v)
            ```

        []{#buildProgressUpdated(double)}

        -   #### buildProgressUpdated

            ``` methodSignature
            public static ProgressEvent.BuildProgressUpdated buildProgressUpdated​(double v)
            ```

        []{#getValueString()}

        -   #### getValueString

            ``` methodSignature
            protected String getValueString()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getValueString` in class `AbstractBuckEvent`

        []{#getProgressValue()}

        -   #### getProgressValue

            ``` methodSignature
            public double getProgressValue()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getProgressValue` in interface `ProgressEventInterface`

            [Returns:]{.returnLabel}
            :   the current progress value for any of the build, parse
                or project generation events
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
