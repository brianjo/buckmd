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
[Package]{.packageLabelInType} [com.facebook.buck.parser.events](package-summary.html)
:::

## Class ParseBuckFileEvent {#class-parsebuckfileevent .title title="Class ParseBuckFileEvent"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.event.AbstractBuckEvent](../../event/AbstractBuckEvent.html "class in com.facebook.buck.event")

    -   -   com.facebook.buck.parser.events.ParseBuckFileEvent

::: description
-   

    All Implemented Interfaces:
    :   `BuckEvent`, `BuckEventExternalInterface`, `WorkAdvanceEvent`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `ParseBuckFileEvent.Finished`, `ParseBuckFileEvent.Started`

    ------------------------------------------------------------------------

        public abstract class ParseBuckFileEvent
        extends AbstractBuckEvent
        implements WorkAdvanceEvent

    ::: block
    Base class for events about parsing build files
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `ParseBu              | ::: block             |
        |                       | ckFileEvent.Finished` | The event raised when |
        |                       |                       | build file parsing is |
        |                       |                       | finished              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `ParseBuck            | ::: block             |
        |                       | FileEvent.ParserKind` | The kind of parser    |
        |                       |                       | used to parse a       |
        |                       |                       | particular build      |
        |                       |                       | file.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `ParseB               | ::: block             |
        |                       | uckFileEvent.Started` | The event raised when |
        |                       |                       | build file parsing is |
        |                       |                       | started               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

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

          Modifier       Constructor                                                                                                                                  Description
          -------------- -------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `protected `   `ParseBuckFileEvent​(EventKey eventKey,                   Path buckFilePath,                   Class<? extends FileParser<?>> parserClass)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static ParseBu       | `finish               | ::: block             |
        | ckFileEvent.Finished` | ed​(ParseBuckFileEvent | Create an event when  |
        |                       | .Started started,     | parsing of build file |
        |                       |      int rulesCount,  | finishes              |
        |                       |         long processe | :::                   |
        |                       | dBytes,         Optio |                       |
        |                       | nal<String> profile)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getBuckFilePath()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Class<? ex           | `getParserClass()`    |                       |
        | tends FileParser<?>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getValueString()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static ParseB        | `started​(Path buckF   | ::: block             |
        | uckFileEvent.Started` | ilePath,        Parse | Create an event when  |
        |                       | BuckFileEvent.ParserK | parsing of build file |
        |                       | ind parser,        Cl | starts                |
        |                       | ass<? extends FilePar | :::                   |
        |                       | ser<?>> parserClass)` |                       |
        +-----------------------+-----------------------+-----------------------+

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

        []{#<init>(com.facebook.buck.event.EventKey,java.nio.file.Path,java.lang.Class)}

        -   #### ParseBuckFileEvent

                protected ParseBuckFileEvent​(EventKey eventKey,
                                             Path buckFilePath,
                                             Class<? extends FileParser<?>> parserClass)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuckFilePath()}

        -   #### getBuckFilePath

            ``` methodSignature
            public Path getBuckFilePath()
            ```

            [Returns:]{.returnLabel}
            :   Path to a build file being parsed

        []{#getParserClass()}

        -   #### getParserClass

            ``` methodSignature
            public Class<? extends FileParser<?>> getParserClass()
            ```

            [Returns:]{.returnLabel}
            :   Java class of parser implementation used to parse this
                build file

        []{#getValueString()}

        -   #### getValueString

            ``` methodSignature
            public String getValueString()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getValueString` in class `AbstractBuckEvent`

        []{#started(java.nio.file.Path,com.facebook.buck.parser.events.ParseBuckFileEvent.ParserKind,java.lang.Class)}

        -   #### started

            ``` methodSignature
            public static ParseBuckFileEvent.Started started​(Path buckFilePath,
                                                             ParseBuckFileEvent.ParserKind parser,
                                                             Class<? extends FileParser<?>> parserClass)
            ```

            ::: block
            Create an event when parsing of build file starts
            :::

            [Parameters:]{.paramLabel}
            :   `buckFilePath` - Path to a build file that is about to
                start parsing
            :   `parser` - Parser being used to parse this file
            :   `parserClass` - Java class of a parser implementation

        []{#finished(com.facebook.buck.parser.events.ParseBuckFileEvent.Started,int,long,java.util.Optional)}

        -   #### finished

            ``` methodSignature
            public static ParseBuckFileEvent.Finished finished​(ParseBuckFileEvent.Started started,
                                                               int rulesCount,
                                                               long processedBytes,
                                                               Optional<String> profile)
            ```

            ::: block
            Create an event when parsing of build file finishes
            :::

            [Parameters:]{.paramLabel}
            :   `started` - Event created when corresponding build file
                parsing was started
            :   `rulesCount` - Total number of rules parsed from this
                build file
            :   `processedBytes` - Total number of bytes read while
                parsing this build file, if applicable
            :   `profile` - This is the value of getProfile() from
                PythonDSL parser result. TODO(buck_team) Update
                description with real meaning
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
