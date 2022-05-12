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
-   Nested \| 
-   Field \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.support.log](package-summary.html)
:::

## Class LogBuckConfig {#class-logbuckconfig .title title="Class LogBuckConfig"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.support.log.LogBuckConfig

::: description
-   

    All Implemented Interfaces:
    :   `ConfigView<BuckConfig>`

    ------------------------------------------------------------------------

        public abstract class LogBuckConfig
        extends Object
        implements ConfigView<BuckConfig>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor         Description
          ------------------- -------------
          `LogBuckConfig()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                  Method                                Description
          -------------------------------------------------- ------------------------------------- -------------
          `com.google.common.collect.ImmutableSet<String>`   `getBuildDetailsCommands()`            
          `Optional<String>`                                 `getBuildDetailsTemplate()`            
          `abstract BuckConfig`                              `getDelegate()`                        
          `boolean`                                          `isBuckConfigLocalWarningEnabled()`    
          `boolean`                                          `isJavaGCEventLoggingEnabled()`        
          `boolean`                                          `isJavaUtilsLoggingEnabled()`          
          `boolean`                                          `isLogBuildIdToConsoleEnabled()`       
          `boolean`                                          `isMachineReadableLoggerEnabled()`     
          `boolean`                                          `isProcessTrackerDeepEnabled()`        
          `boolean`                                          `isProcessTrackerEnabled()`            
          `boolean`                                          `isPublicAnnouncementsEnabled()`       
          `boolean`                                          `isRuleKeyLoggerEnabled()`             
          `static LogBuckConfig`                             `of​(BuckConfig delegate)`              

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### LogBuckConfig

                public LogBuckConfig()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getDelegate()}

        -   #### getDelegate

            ``` methodSignature
            public abstract BuckConfig getDelegate()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDelegate` in interface `ConfigView<BuckConfig>`

        []{#of(com.facebook.buck.core.config.BuckConfig)}

        -   #### of

            ``` methodSignature
            public static LogBuckConfig of​(BuckConfig delegate)
            ```

        []{#isPublicAnnouncementsEnabled()}

        -   #### isPublicAnnouncementsEnabled

            ``` methodSignature
            @Lazy
            public boolean isPublicAnnouncementsEnabled()
            ```

        []{#isProcessTrackerEnabled()}

        -   #### isProcessTrackerEnabled

            ``` methodSignature
            @Lazy
            public boolean isProcessTrackerEnabled()
            ```

        []{#isProcessTrackerDeepEnabled()}

        -   #### isProcessTrackerDeepEnabled

            ``` methodSignature
            @Lazy
            public boolean isProcessTrackerDeepEnabled()
            ```

        []{#isRuleKeyLoggerEnabled()}

        -   #### isRuleKeyLoggerEnabled

            ``` methodSignature
            @Lazy
            public boolean isRuleKeyLoggerEnabled()
            ```

        []{#isMachineReadableLoggerEnabled()}

        -   #### isMachineReadableLoggerEnabled

            ``` methodSignature
            @Lazy
            public boolean isMachineReadableLoggerEnabled()
            ```

        []{#isBuckConfigLocalWarningEnabled()}

        -   #### isBuckConfigLocalWarningEnabled

            ``` methodSignature
            @Lazy
            public boolean isBuckConfigLocalWarningEnabled()
            ```

        []{#isJavaUtilsLoggingEnabled()}

        -   #### isJavaUtilsLoggingEnabled

            ``` methodSignature
            @Lazy
            public boolean isJavaUtilsLoggingEnabled()
            ```

        []{#isJavaGCEventLoggingEnabled()}

        -   #### isJavaGCEventLoggingEnabled

            ``` methodSignature
            @Lazy
            public boolean isJavaGCEventLoggingEnabled()
            ```

        []{#isLogBuildIdToConsoleEnabled()}

        -   #### isLogBuildIdToConsoleEnabled

            ``` methodSignature
            public boolean isLogBuildIdToConsoleEnabled()
            ```

        []{#getBuildDetailsTemplate()}

        -   #### getBuildDetailsTemplate

            ``` methodSignature
            public Optional<String> getBuildDetailsTemplate()
            ```

        []{#getBuildDetailsCommands()}

        -   #### getBuildDetailsCommands

            ``` methodSignature
            @Lazy
            public com.google.common.collect.ImmutableSet<String> getBuildDetailsCommands()
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
-   Nested \| 
-   Field \| 
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
