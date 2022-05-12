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

## Class CompilerPluginDurationEvent {#class-compilerplugindurationevent .title title="Class CompilerPluginDurationEvent"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.event.AbstractBuckEvent](AbstractBuckEvent.html "class in com.facebook.buck.event")

    -   -   com.facebook.buck.event.CompilerPluginDurationEvent

::: description
-   

    All Implemented Interfaces:
    :   `BuckEvent`, `BuckEventExternalInterface`, `WorkAdvanceEvent`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `CompilerPluginDurationEvent.Finished`,
        `CompilerPluginDurationEvent.Started`

    ------------------------------------------------------------------------

        public abstract class CompilerPluginDurationEvent
        extends AbstractBuckEvent
        implements WorkAdvanceEvent

    ::: block
    Base class for events being reported by plugins to in-process
    compilers such as JSR199 javac.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                                    Description
          ------------------- ---------------------------------------- -------------
          `static class `     `CompilerPluginDurationEvent.Finished`    
          `static class `     `CompilerPluginDurationEvent.Started`     

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

          Modifier       Constructor                                                                                                                                                                                                                                                                                 Description
          -------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `protected `   `CompilerPluginDurationEvent​(EventKey eventKey,                            BuildTarget buildTarget,                            String pluginName,                            String durationName,                            com.google.common.collect.ImmutableMap<String,​String> args)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                         Method                                                                                                                                                        Description
          --------------------------------------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `static CompilerPluginDurationEvent.Finished`             `finished​(CompilerPluginDurationEvent.Started startedEvent,         com.google.common.collect.ImmutableMap<String,​String> args)`                               
          `com.google.common.collect.ImmutableMap<String,​String>`   `getArgs()`                                                                                                                                                    
          `BuildTarget`                                             `getBuildTarget()`                                                                                                                                             
          `String`                                                  `getDurationName()`                                                                                                                                            
          `String`                                                  `getPluginName()`                                                                                                                                              
          `protected String`                                        `getValueString()`                                                                                                                                             
          `static CompilerPluginDurationEvent.Started`              `started​(BuildTarget buildTarget,        String pluginName,        String durationName,        com.google.common.collect.ImmutableMap<String,​String> args)`    

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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.event.EventKey,com.facebook.buck.core.model.BuildTarget,java.lang.String,java.lang.String,com.google.common.collect.ImmutableMap)}

        -   #### CompilerPluginDurationEvent

                protected CompilerPluginDurationEvent​(EventKey eventKey,
                                                      BuildTarget buildTarget,
                                                      String pluginName,
                                                      String durationName,
                                                      com.google.common.collect.ImmutableMap<String,​String> args)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildTarget()}

        -   #### getBuildTarget

            ``` methodSignature
            public BuildTarget getBuildTarget()
            ```

        []{#getPluginName()}

        -   #### getPluginName

            ``` methodSignature
            public String getPluginName()
            ```

        []{#getDurationName()}

        -   #### getDurationName

            ``` methodSignature
            public String getDurationName()
            ```

        []{#getArgs()}

        -   #### getArgs

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​String> getArgs()
            ```

        []{#getValueString()}

        -   #### getValueString

            ``` methodSignature
            protected String getValueString()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getValueString` in class `AbstractBuckEvent`

        []{#started(com.facebook.buck.core.model.BuildTarget,java.lang.String,java.lang.String,com.google.common.collect.ImmutableMap)}

        -   #### started

            ``` methodSignature
            public static CompilerPluginDurationEvent.Started started​(BuildTarget buildTarget,
                                                                      String pluginName,
                                                                      String durationName,
                                                                      com.google.common.collect.ImmutableMap<String,​String> args)
            ```

        []{#finished(com.facebook.buck.event.CompilerPluginDurationEvent.Started,com.google.common.collect.ImmutableMap)}

        -   #### finished

            ``` methodSignature
            public static CompilerPluginDurationEvent.Finished finished​(CompilerPluginDurationEvent.Started startedEvent,
                                                                        com.google.common.collect.ImmutableMap<String,​String> args)
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
