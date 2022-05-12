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

## Class ArtifactCompressionEvent {#class-artifactcompressionevent .title title="Class ArtifactCompressionEvent"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.event.AbstractBuckEvent](AbstractBuckEvent.html "class in com.facebook.buck.event")

    -   -   com.facebook.buck.event.ArtifactCompressionEvent

::: description
-   

    All Implemented Interfaces:
    :   `BuckEvent`, `BuckEventExternalInterface`, `LeafEvent`,
        `WorkAdvanceEvent`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `ArtifactCompressionEvent.Finished`,
        `ArtifactCompressionEvent.Started`

    ------------------------------------------------------------------------

        public abstract class ArtifactCompressionEvent
        extends AbstractBuckEvent
        implements LeafEvent, WorkAdvanceEvent

    ::: block
    Event for artifact compression / decompression
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `ArtifactCompr        | ::: block             |
        |                       | essionEvent.Finished` | Event for when a      |
        |                       |                       | artifact finishes     |
        |                       |                       | comp                  |
        |                       |                       | ression/decompression |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `ArtifactCompre       |                       |
        |                       | ssionEvent.Operation` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `ArtifactComp         | ::: block             |
        |                       | ressionEvent.Started` | Event for when a      |
        |                       |                       | artifact starts       |
        |                       |                       | comp                  |
        |                       |                       | ression/decompression |
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

          Modifier       Constructor                                                                                                                                                                                                                                          Description
          -------------- ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `protected `   `ArtifactCompressionEvent​(EventKey eventKey,                         ArtifactCompressionEvent.Operation operation,                         com.google.common.collect.ImmutableSet<RuleKey> ruleKeys,                         HasNameAndType rule)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static ArtifactCompr | `finish               | ::: block             |
        | essionEvent.Finished` | ed​(ArtifactCompressio | Create a new Finished |
        |                       | nEvent.Started starte | event for             |
        |                       | d,         long fullS | corresponding Started |
        |                       | ize,         long com | event                 |
        |                       | pressedSize,          | :::                   |
        |                       | HasNameAndType rule)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getCategory()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ArtifactCompre       | `getOperation()`      |                       |
        | ssionEvent.Operation` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getRuleKeys()`       |                       |
        | ogle.common.collect.I |                       |                       |
        | mmutableSet<RuleKey>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getValueString()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static ArtifactComp  | `                     | ::: block             |
        | ressionEvent.Started` | started​(ArtifactCompr | Create a new Started  |
        |                       | essionEvent.Operation | event for the         |
        |                       |  operation,        co | operation and set of  |
        |                       | m.google.common.colle | RuleKeys              |
        |                       | ct.ImmutableSet<RuleK | :::                   |
        |                       | ey> ruleKeys,         |                       |
        |                       | HasNameAndType rule)` |                       |
        +-----------------------+-----------------------+-----------------------+

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

        []{#<init>(com.facebook.buck.event.EventKey,com.facebook.buck.event.ArtifactCompressionEvent.Operation,com.google.common.collect.ImmutableSet,com.facebook.buck.core.rules.HasNameAndType)}

        -   #### ArtifactCompressionEvent

                protected ArtifactCompressionEvent​(EventKey eventKey,
                                                   ArtifactCompressionEvent.Operation operation,
                                                   com.google.common.collect.ImmutableSet<RuleKey> ruleKeys,
                                                   HasNameAndType rule)
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

        []{#getValueString()}

        -   #### getValueString

            ``` methodSignature
            public String getValueString()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getValueString` in class `AbstractBuckEvent`

        []{#getRuleKeys()}

        -   #### getRuleKeys

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<RuleKey> getRuleKeys()
            ```

        []{#getOperation()}

        -   #### getOperation

            ``` methodSignature
            public ArtifactCompressionEvent.Operation getOperation()
            ```

        []{#started(com.facebook.buck.event.ArtifactCompressionEvent.Operation,com.google.common.collect.ImmutableSet,com.facebook.buck.core.rules.HasNameAndType)}

        -   #### started

            ``` methodSignature
            public static ArtifactCompressionEvent.Started started​(ArtifactCompressionEvent.Operation operation,
                                                                   com.google.common.collect.ImmutableSet<RuleKey> ruleKeys,
                                                                   HasNameAndType rule)
            ```

            ::: block
            Create a new Started event for the operation and set of
            RuleKeys
            :::

        []{#finished(com.facebook.buck.event.ArtifactCompressionEvent.Started,long,long,com.facebook.buck.core.rules.HasNameAndType)}

        -   #### finished

            ``` methodSignature
            public static ArtifactCompressionEvent.Finished finished​(ArtifactCompressionEvent.Started started,
                                                                     long fullSize,
                                                                     long compressedSize,
                                                                     HasNameAndType rule)
            ```

            ::: block
            Create a new Finished event for corresponding Started event
            :::
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
