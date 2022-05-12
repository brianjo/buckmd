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

## Class InstallEvent.Finished {#class-installevent.finished .title title="Class InstallEvent.Finished"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.event.AbstractBuckEvent](AbstractBuckEvent.html "class in com.facebook.buck.event")

    -   -   [com.facebook.buck.event.InstallEvent](InstallEvent.html "class in com.facebook.buck.event")

        -   -   com.facebook.buck.event.InstallEvent.Finished

::: description
-   

    All Implemented Interfaces:
    :   `BuckEvent`, `BuckEventExternalInterface`,
        `InstallFinishedEventExternalInterface`, `LeafEvent`,
        `WorkAdvanceEvent`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [InstallEvent](InstallEvent.html "class in com.facebook.buck.event")

    ------------------------------------------------------------------------

        public static class InstallEvent.Finished
        extends InstallEvent
        implements InstallFinishedEventExternalInterface
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.event.InstallEvent}

            ### Nested classes/interfaces inherited from class com.facebook.buck.event.[InstallEvent](InstallEvent.html "class in com.facebook.buck.event")

            `InstallEvent.Finished, InstallEvent.Started`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                   Description
          ------------------- ----------------------- -------------
          `static String`     `DEVICE_INFO_LOCALES`    

          : Fields[ ]{.tabEnd}

        -   []{#fields.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Fields inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `BUILD_FINISHED, BUILD_REPORT, BUILD_STARTED, BUILD_STATUS_EVENT, CACHE_RATE_STATS_UPDATE_EVENT, INDIVIDUAL_TEST_AWAITING_RESULTS, INSTALL_STARTED, PARSE_FINISHED, PARSE_STARTED, PROJECT_GENERATION_FINISHED, PROJECT_GENERATION_STARTED, TEST_RUN_STARTED`

        ```{=html}
        <!-- -->
        ```
        -   []{#fields.inherited.from.class.com.facebook.buck.event.external.events.InstallFinishedEventExternalInterface}

            ### Fields inherited from interface com.facebook.buck.event.external.events.[InstallFinishedEventExternalInterface](external/events/InstallFinishedEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `INSTALL_FINISHED`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                                                                                                                                                                            Description
          -------------- ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `protected `   `Finished​(InstallEvent.Started started,         boolean success,         Optional<Long> pid,         Optional<String> packageName,         com.google.common.collect.ImmutableMap<String,​String> installDeviceInfo)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `equals​(Object o)`    | ::: block             |
        |                       |                       | The default           |
        |                       |                       | implementation of     |
        |                       |                       | equals checks to see  |
        |                       |                       | if two events are     |
        |                       |                       | related, are on the   |
        |                       |                       | same thread, and are  |
        |                       |                       | the same concrete     |
        |                       |                       | class.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getEventName()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `ge                   |                       |
        | ommon.collect.Immutab | tInstallDeviceInfo()` |                       |
        | leMap<String,​String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getPackageName()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `getPid()`            |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isSuccess()`         |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.event.InstallEvent}

            ### Methods inherited from class com.facebook.buck.event.[InstallEvent](InstallEvent.html "class in com.facebook.buck.event")

            `finished, finished, getBuildTarget, getCategory, getValueString, started`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.event.AbstractBuckEvent}

            ### Methods inherited from class com.facebook.buck.event.[AbstractBuckEvent](AbstractBuckEvent.html "class in com.facebook.buck.event")

            `configure, getBuildId, getEventKey, getNanoTime, getThreadId, getThreadUserNanoTime, getTimestampMillis, isConfigured, isRelatedTo, toLogMessage, toString`

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
    -   []{#field.detail}

        ### Field Detail

        []{#DEVICE_INFO_LOCALES}

        -   #### DEVICE_INFO_LOCALES

                public static final String DEVICE_INFO_LOCALES

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.event.InstallEvent.Finished.DEVICE_INFO_LOCALES)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.event.InstallEvent.Started,boolean,java.util.Optional,java.util.Optional,com.google.common.collect.ImmutableMap)}

        -   #### Finished

                protected Finished​(InstallEvent.Started started,
                                   boolean success,
                                   Optional<Long> pid,
                                   Optional<String> packageName,
                                   com.google.common.collect.ImmutableMap<String,​String> installDeviceInfo)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#isSuccess()}

        -   #### isSuccess

            ``` methodSignature
            public boolean isSuccess()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isSuccess` in
                interface `InstallFinishedEventExternalInterface`

            [Returns:]{.returnLabel}
            :   the success status of the install action.

        []{#getPid()}

        -   #### getPid

            ``` methodSignature
            public long getPid()
            ```

        []{#getInstallDeviceInfo()}

        -   #### getInstallDeviceInfo

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​String> getInstallDeviceInfo()
            ```

        []{#getPackageName()}

        -   #### getPackageName

            ``` methodSignature
            public String getPackageName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPackageName` in
                interface `InstallFinishedEventExternalInterface`

            [Returns:]{.returnLabel}
            :   the package name of the installed application.

        []{#getEventName()}

        -   #### getEventName

            ``` methodSignature
            public String getEventName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getEventName` in interface `BuckEventExternalInterface`

            [Returns:]{.returnLabel}
            :   the type of the event.

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object o)
            ```

            ::: block
            [Description copied from
            class: `AbstractBuckEvent`]{.descfrmTypeLabel}
            :::

            ::: block
            The default implementation of equals checks to see if two
            events are related, are on the same thread, and are the same
            concrete class. Subclasses therefore can simply override
            isRelatedTo, and the equals method will work correctly.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `AbstractBuckEvent`

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `AbstractBuckEvent`
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
