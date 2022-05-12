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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
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

## Class CommandEvent {#class-commandevent .title title="Class CommandEvent"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.event.AbstractBuckEvent](AbstractBuckEvent.html "class in com.facebook.buck.event")

    -   -   com.facebook.buck.event.CommandEvent

::: description
-   

    All Implemented Interfaces:
    :   `BuckEvent`, `BuckEventExternalInterface`, `WorkAdvanceEvent`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `CommandEvent.Finished`, `CommandEvent.Interrupted`,
        `CommandEvent.Started`

    ------------------------------------------------------------------------

        public abstract class CommandEvent
        extends AbstractBuckEvent
        implements WorkAdvanceEvent

    ::: block
    Events tracking the start and stop of a buck command.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                        Description
          ------------------- ---------------------------- -------------
          `static class `     `CommandEvent.Finished`       
          `static class `     `CommandEvent.Interrupted`    
          `static class `     `CommandEvent.Started`        

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
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                   Method                                                                                                                                                                          Description
          --------------------------------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `static CommandEvent.Finished`                      `finished​(CommandEvent.Started started,         ExitCode exitCode)`                                                                                                              
          `com.google.common.collect.ImmutableList<String>`   `getArgs()`                                                                                                                                                                      
          `String`                                            `getCommandName()`                                                                                                                                                               
          `OptionalLong`                                      `getDaemonUptime()`                                                                                                                                                              
          `long`                                              `getPid()`                                                                                                                                                                       
          `protected String`                                  `getValueString()`                                                                                                                                                               
          `static CommandEvent.Interrupted`                   `interrupted​(CommandEvent.Started started,            ExitCode exitCode)`                                                                                                        
          `boolean`                                           `isDaemon()`                                                                                                                                                                     
          `static CommandEvent.Started`                       `started​(String commandName,        com.google.common.collect.ImmutableList<String> args,        Path clientSubdirectory,        OptionalLong daemonUptime,        long pid)`    

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

            `getEventName, getTimestampMillis, storeLastInstanceAndReplayForNewClients`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getCommandName()}

        -   #### getCommandName

            ``` methodSignature
            public String getCommandName()
            ```

        []{#getArgs()}

        -   #### getArgs

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getArgs()
            ```

            [Returns:]{.returnLabel}
            :   Arguments passed to
                [`getCommandName()`](#getCommandName()).

        []{#isDaemon()}

        -   #### isDaemon

            ``` methodSignature
            public boolean isDaemon()
            ```

        []{#getDaemonUptime()}

        -   #### getDaemonUptime

            ``` methodSignature
            public OptionalLong getDaemonUptime()
            ```

        []{#getPid()}

        -   #### getPid

            ``` methodSignature
            public long getPid()
            ```

        []{#getValueString()}

        -   #### getValueString

            ``` methodSignature
            protected String getValueString()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getValueString` in class `AbstractBuckEvent`

        []{#started(java.lang.String,com.google.common.collect.ImmutableList,java.nio.file.Path,java.util.OptionalLong,long)}

        -   #### started

            ``` methodSignature
            public static CommandEvent.Started started​(String commandName,
                                                       com.google.common.collect.ImmutableList<String> args,
                                                       Path clientSubdirectory,
                                                       OptionalLong daemonUptime,
                                                       long pid)
            ```

        []{#finished(com.facebook.buck.event.CommandEvent.Started,com.facebook.buck.util.ExitCode)}

        -   #### finished

            ``` methodSignature
            public static CommandEvent.Finished finished​(CommandEvent.Started started,
                                                         ExitCode exitCode)
            ```

        []{#interrupted(com.facebook.buck.event.CommandEvent.Started,com.facebook.buck.util.ExitCode)}

        -   #### interrupted

            ``` methodSignature
            public static CommandEvent.Interrupted interrupted​(CommandEvent.Started started,
                                                               ExitCode exitCode)
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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
