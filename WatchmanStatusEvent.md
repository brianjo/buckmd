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

## Class WatchmanStatusEvent {#class-watchmanstatusevent .title title="Class WatchmanStatusEvent"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.event.AbstractBuckEvent](AbstractBuckEvent.html "class in com.facebook.buck.event")

    -   -   com.facebook.buck.event.WatchmanStatusEvent

::: description
-   

    All Implemented Interfaces:
    :   `BuckEvent`, `BuckEventExternalInterface`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `WatchmanStatusEvent.FileCreation`,
        `WatchmanStatusEvent.FileDeletion`,
        `WatchmanStatusEvent.Finished`, `WatchmanStatusEvent.Overflow`,
        `WatchmanStatusEvent.Started`,
        `WatchmanStatusEvent.ZeroFileChanges`

    ------------------------------------------------------------------------

        public abstract class WatchmanStatusEvent
        extends AbstractBuckEvent
        implements BuckEvent
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `WatchmanStat         |                       |
        |                       | usEvent.FileCreation` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `WatchmanStat         |                       |
        |                       | usEvent.FileDeletion` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `Watchman             |                       |
        |                       | StatusEvent.Finished` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `Watchman             |                       |
        |                       | StatusEvent.Overflow` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `Watchma              |                       |
        |                       | nStatusEvent.Started` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `WatchmanStatusE      | ::: block             |
        |                       | vent.ZeroFileChanges` | This event is to be   |
        |                       |                       | posted when Watchman  |
        |                       |                       | does not report any   |
        |                       |                       | altered files.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

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

          Constructor                                                                     Description
          ------------------------------------------------------------------------------- -------------
          `WatchmanStatusEvent​(EventKey eventKey,                    String eventName)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                              Method                                             Description
          ---------------------------------------------- -------------------------------------------------- -------------
          `static WatchmanStatusEvent.FileCreation`      `fileCreation​(String filename)`                     
          `static WatchmanStatusEvent.FileDeletion`      `fileDeletion​(String filename)`                     
          `static WatchmanStatusEvent.Finished`          `finished()`                                        
          `String`                                       `getEventName()`                                    
          `protected String`                             `getValueString()`                                  
          `static WatchmanStatusEvent.Overflow`          `overflow​(String reason,         Path cellPath)`    
          `static WatchmanStatusEvent.Started`           `started()`                                         
          `static WatchmanStatusEvent.ZeroFileChanges`   `zeroFileChanges()`                                 

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

        []{#<init>(com.facebook.buck.event.EventKey,java.lang.String)}

        -   #### WatchmanStatusEvent

                public WatchmanStatusEvent​(EventKey eventKey,
                                           String eventName)
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

        []{#getEventName()}

        -   #### getEventName

            ``` methodSignature
            public String getEventName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getEventName` in interface `BuckEventExternalInterface`

            [Returns:]{.returnLabel}
            :   the type of the event.

        []{#started()}

        -   #### started

            ``` methodSignature
            public static WatchmanStatusEvent.Started started()
            ```

        []{#finished()}

        -   #### finished

            ``` methodSignature
            public static WatchmanStatusEvent.Finished finished()
            ```

        []{#overflow(java.lang.String,java.nio.file.Path)}

        -   #### overflow

            ``` methodSignature
            public static WatchmanStatusEvent.Overflow overflow​(String reason,
                                                                Path cellPath)
            ```

        []{#fileCreation(java.lang.String)}

        -   #### fileCreation

            ``` methodSignature
            public static WatchmanStatusEvent.FileCreation fileCreation​(String filename)
            ```

        []{#fileDeletion(java.lang.String)}

        -   #### fileDeletion

            ``` methodSignature
            public static WatchmanStatusEvent.FileDeletion fileDeletion​(String filename)
            ```

        []{#zeroFileChanges()}

        -   #### zeroFileChanges

            ``` methodSignature
            public static WatchmanStatusEvent.ZeroFileChanges zeroFileChanges()
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
