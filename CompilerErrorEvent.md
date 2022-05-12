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

## Class CompilerErrorEvent {#class-compilererrorevent .title title="Class CompilerErrorEvent"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.event.AbstractBuckEvent](AbstractBuckEvent.html "class in com.facebook.buck.event")

    -   -   com.facebook.buck.event.CompilerErrorEvent

::: description
-   

    All Implemented Interfaces:
    :   `BuckEvent`, `BuckEventExternalInterface`,
        `CompilerErrorEventExternalInterface`

    ------------------------------------------------------------------------

        public class CompilerErrorEvent
        extends AbstractBuckEvent
        implements CompilerErrorEventExternalInterface
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                               Description
          ------------------- ----------------------------------- -------------
          `static class `     `CompilerErrorEvent.CompilerType`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Fields inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `BUILD_FINISHED, BUILD_REPORT, BUILD_STARTED, BUILD_STATUS_EVENT, CACHE_RATE_STATS_UPDATE_EVENT, INDIVIDUAL_TEST_AWAITING_RESULTS, INSTALL_STARTED, PARSE_FINISHED, PARSE_STARTED, PROJECT_GENERATION_FINISHED, PROJECT_GENERATION_STARTED, TEST_RUN_STARTED`

        ```{=html}
        <!-- -->
        ```
        -   []{#fields.inherited.from.class.com.facebook.buck.event.external.events.CompilerErrorEventExternalInterface}

            ### Fields inherited from interface com.facebook.buck.event.external.events.[CompilerErrorEventExternalInterface](external/events/CompilerErrorEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `COMPILER_ERROR_EVENT`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                  Method                                                                                                                                                                   Description
          -------------------------------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `static CompilerErrorEvent`                        `create​(BuildTarget target,       String error,       CompilerErrorEvent.CompilerType compilerType,       com.google.common.collect.ImmutableSet<String> suggestions)`    
          `CompilerErrorEvent.CompilerType`                  `getCompilerType()`                                                                                                                                                       
          `String`                                           `getError()`                                                                                                                                                              
          `String`                                           `getEventName()`                                                                                                                                                          
          `com.google.common.collect.ImmutableSet<String>`   `getSuggestions()`                                                                                                                                                        
          `String`                                           `getTarget()`                                                                                                                                                             
          `protected String`                                 `getValueString()`                                                                                                                                                        

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

            `getTimestampMillis, storeLastInstanceAndReplayForNewClients`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#create(com.facebook.buck.core.model.BuildTarget,java.lang.String,com.facebook.buck.event.CompilerErrorEvent.CompilerType,com.google.common.collect.ImmutableSet)}

        -   #### create

            ``` methodSignature
            public static CompilerErrorEvent create​(BuildTarget target,
                                                    String error,
                                                    CompilerErrorEvent.CompilerType compilerType,
                                                    com.google.common.collect.ImmutableSet<String> suggestions)
            ```

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

        []{#getError()}

        -   #### getError

            ``` methodSignature
            public String getError()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getError` in
                interface `CompilerErrorEventExternalInterface`

            [Returns:]{.returnLabel}
            :   the stacktrace of the error that occurred.

        []{#getTarget()}

        -   #### getTarget

            ``` methodSignature
            public String getTarget()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTarget` in
                interface `CompilerErrorEventExternalInterface`

            [Returns:]{.returnLabel}
            :   the target on which the error occurred.

        []{#getCompilerType()}

        -   #### getCompilerType

            ``` methodSignature
            public CompilerErrorEvent.CompilerType getCompilerType()
            ```

        []{#getSuggestions()}

        -   #### getSuggestions

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<String> getSuggestions()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSuggestions` in
                interface `CompilerErrorEventExternalInterface`

            [Returns:]{.returnLabel}
            :   suggestions on how to fix the error.
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
