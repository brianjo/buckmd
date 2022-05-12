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
[Package]{.packageLabelInType} [com.facebook.buck.event](package-summary.html)
:::

## Class ConsoleEvent {#class-consoleevent .title title="Class ConsoleEvent"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.event.AbstractBuckEvent](AbstractBuckEvent.html "class in com.facebook.buck.event")

    -   -   com.facebook.buck.event.ConsoleEvent

::: description
-   

    All Implemented Interfaces:
    :   `BuckEvent`, `BuckEventExternalInterface`,
        `ConsoleEventExternalInterface`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `ThrowableConsoleEvent`

    ------------------------------------------------------------------------

        public class ConsoleEvent
        extends AbstractBuckEvent
        implements ConsoleEventExternalInterface

    ::: block
    Event for messages. Post ConsoleEvents to the event bus where you
    would normally use `  java.util.logging`.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Fields inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `BUILD_FINISHED, BUILD_REPORT, BUILD_STARTED, BUILD_STATUS_EVENT, CACHE_RATE_STATS_UPDATE_EVENT, INDIVIDUAL_TEST_AWAITING_RESULTS, INSTALL_STARTED, PARSE_FINISHED, PARSE_STARTED, PROJECT_GENERATION_FINISHED, PROJECT_GENERATION_STARTED, TEST_RUN_STARTED`

        ```{=html}
        <!-- -->
        ```
        -   []{#fields.inherited.from.class.com.facebook.buck.event.external.events.ConsoleEventExternalInterface}

            ### Fields inherited from interface com.facebook.buck.event.external.events.[ConsoleEventExternalInterface](external/events/ConsoleEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `CONSOLE_EVENT`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                                                            Description
          -------------- ------------------------------------------------------------------------------------------------------ -------------
          `protected `   `ConsoleEvent​(Level level,             boolean containsAnsiEscapeCodes,             String message)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type       Method                                                                                                  Description
          ----------------------- ------------------------------------------------------------------------------------------------------- -------------
          `boolean`               `containsAnsiEscapeCodes()`                                                                              
          `static ConsoleEvent`   `create​(Level level,       String message)`                                                              
          `static ConsoleEvent`   `create​(Level level,       String message,       Object... args)`                                        
          `static ConsoleEvent`   `createForMessageWithAnsiEscapeCodes​(Level level,                                    String message)`    
          `static ConsoleEvent`   `fine​(String message)`                                                                                   
          `static ConsoleEvent`   `fine​(String message,     Object... args)`                                                               
          `static ConsoleEvent`   `finer​(String message)`                                                                                  
          `static ConsoleEvent`   `finer​(String message,      Object... args)`                                                             
          `String`                `getEventName()`                                                                                         
          `Level`                 `getLevel()`                                                                                             
          `String`                `getMessage()`                                                                                           
          `protected String`      `getValueString()`                                                                                       
          `static ConsoleEvent`   `info​(String message)`                                                                                   
          `static ConsoleEvent`   `info​(String message,     Object... args)`                                                               
          `static ConsoleEvent`   `severe​(String message)`                                                                                 
          `static ConsoleEvent`   `severe​(String message,       Object... args)`                                                           
          `String`                `toString()`                                                                                             
          `static ConsoleEvent`   `warning​(String message)`                                                                                
          `static ConsoleEvent`   `warning​(String message,        Object... args)`                                                         

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.event.AbstractBuckEvent}

            ### Methods inherited from class com.facebook.buck.event.[AbstractBuckEvent](AbstractBuckEvent.html "class in com.facebook.buck.event")

            `configure, equals, getBuildId, getEventKey, getNanoTime, getThreadId, getThreadUserNanoTime, getTimestampMillis, hashCode, isConfigured, isRelatedTo, toLogMessage`

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

            `getTimestampMillis, storeLastInstanceAndReplayForNewClients`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.util.logging.Level,boolean,java.lang.String)}

        -   #### ConsoleEvent

                protected ConsoleEvent​(Level level,
                                       boolean containsAnsiEscapeCodes,
                                       String message)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getLevel()}

        -   #### getLevel

            ``` methodSignature
            public Level getLevel()
            ```

        []{#containsAnsiEscapeCodes()}

        -   #### containsAnsiEscapeCodes

            ``` methodSignature
            public boolean containsAnsiEscapeCodes()
            ```

        []{#getMessage()}

        -   #### getMessage

            ``` methodSignature
            public String getMessage()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getMessage` in
                interface `ConsoleEventExternalInterface`

            [Returns:]{.returnLabel}
            :   the message of the event that occurred.

        []{#create(java.util.logging.Level,java.lang.String)}

        -   #### create

            ``` methodSignature
            public static ConsoleEvent create​(Level level,
                                              String message)
            ```

        []{#create(java.util.logging.Level,java.lang.String,java.lang.Object...)}

        -   #### create

            ``` methodSignature
            public static ConsoleEvent create​(Level level,
                                              String message,
                                              Object... args)
            ```

        []{#createForMessageWithAnsiEscapeCodes(java.util.logging.Level,java.lang.String)}

        -   #### createForMessageWithAnsiEscapeCodes

            ``` methodSignature
            public static ConsoleEvent createForMessageWithAnsiEscapeCodes​(Level level,
                                                                           String message)
            ```

        []{#finer(java.lang.String)}

        -   #### finer

            ``` methodSignature
            public static ConsoleEvent finer​(String message)
            ```

        []{#finer(java.lang.String,java.lang.Object...)}

        -   #### finer

            ``` methodSignature
            public static ConsoleEvent finer​(String message,
                                             Object... args)
            ```

        []{#fine(java.lang.String)}

        -   #### fine

            ``` methodSignature
            public static ConsoleEvent fine​(String message)
            ```

        []{#fine(java.lang.String,java.lang.Object...)}

        -   #### fine

            ``` methodSignature
            public static ConsoleEvent fine​(String message,
                                            Object... args)
            ```

        []{#info(java.lang.String)}

        -   #### info

            ``` methodSignature
            public static ConsoleEvent info​(String message)
            ```

        []{#info(java.lang.String,java.lang.Object...)}

        -   #### info

            ``` methodSignature
            public static ConsoleEvent info​(String message,
                                            Object... args)
            ```

        []{#warning(java.lang.String)}

        -   #### warning

            ``` methodSignature
            public static ConsoleEvent warning​(String message)
            ```

        []{#warning(java.lang.String,java.lang.Object...)}

        -   #### warning

            ``` methodSignature
            public static ConsoleEvent warning​(String message,
                                               Object... args)
            ```

        []{#severe(java.lang.String)}

        -   #### severe

            ``` methodSignature
            public static ConsoleEvent severe​(String message)
            ```

        []{#severe(java.lang.String,java.lang.Object...)}

        -   #### severe

            ``` methodSignature
            public static ConsoleEvent severe​(String message,
                                              Object... args)
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

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `AbstractBuckEvent`
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
