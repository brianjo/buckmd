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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.build.event](package-summary.html)
:::

## Class BuildRuleEvent.Finished {#class-buildruleevent.finished .title title="Class BuildRuleEvent.Finished"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.event.AbstractBuckEvent](../../../event/AbstractBuckEvent.html "class in com.facebook.buck.event")

    -   -   [com.facebook.buck.core.build.event.BuildRuleEvent](BuildRuleEvent.html "class in com.facebook.buck.core.build.event")

        -   -   [com.facebook.buck.core.build.event.BuildRuleEvent.EndingBuildRuleEvent](BuildRuleEvent.EndingBuildRuleEvent.html "class in com.facebook.buck.core.build.event")

            -   -   com.facebook.buck.core.build.event.BuildRuleEvent.Finished

::: description
-   

    All Implemented Interfaces:
    :   `BuckEvent`, `BuckEventExternalInterface`, `WorkAdvanceEvent`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [BuildRuleEvent](BuildRuleEvent.html "class in com.facebook.buck.core.build.event")

    ------------------------------------------------------------------------

        public static class BuildRuleEvent.Finished
        extends BuildRuleEvent.EndingBuildRuleEvent

    ::: block
    Marks the end of processing a build rule.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.core.build.event.BuildRuleEvent}

            ### Nested classes/interfaces inherited from class com.facebook.buck.core.build.event.[BuildRuleEvent](BuildRuleEvent.html "class in com.facebook.buck.core.build.event")

            `BuildRuleEvent.BeginningBuildRuleEvent, BuildRuleEvent.EndingBuildRuleEvent, BuildRuleEvent.Finished, BuildRuleEvent.FinishedRuleKeyCalc, BuildRuleEvent.Resumed, BuildRuleEvent.Started, BuildRuleEvent.StartedRuleKeyCalc, BuildRuleEvent.Suspended, BuildRuleEvent.WillBuildLocally`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.core.build.event.BuildRuleEvent}

            ### Fields inherited from class com.facebook.buck.core.build.event.[BuildRuleEvent](BuildRuleEvent.html "class in com.facebook.buck.core.build.event")

            `duration`

        ```{=html}
        <!-- -->
        ```
        -   []{#fields.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Fields inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](../../../event/external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `BUILD_FINISHED, BUILD_REPORT, BUILD_STARTED, BUILD_STATUS_EVENT, CACHE_RATE_STATS_UPDATE_EVENT, INDIVIDUAL_TEST_AWAITING_RESULTS, INSTALL_STARTED, PARSE_FINISHED, PARSE_STARTED, PROJECT_GENERATION_FINISHED, PROJECT_GENERATION_STARTED, TEST_RUN_STARTED`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                             Method                                       Description
          --------------------------------------------- -------------------------------------------- -------------
          `Optional<Pair<Long,​Long>>`                   `getBuildTimestamps()`                        
          `CacheResult`                                 `getCacheResult()`                            
          `Optional<BuildRuleDiagnosticData>`           `getDiagnosticData()`                         
          `Optional<Pair<Long,​Long>>`                   `getInputRuleKeyCacheCheckTimestamps()`       
          `Optional<ManifestFetchResult>`               `getManifestFetchResult()`                    
          `Optional<Pair<Long,​Long>>`                   `getManifestRuleKeyCacheCheckTimestamps()`    
          `Optional<ManifestStoreResult>`               `getManifestStoreResult()`                    
          `Optional<BuildId>`                           `getOrigin()`                                 
          `Optional<com.google.common.hash.HashCode>`   `getOutputHash()`                             
          `Optional<Long>`                              `getOutputSize()`                             
          `String`                                      `getResultString()`                           
          `Optional<Pair<Long,​Long>>`                   `getRuleKeyCacheCheckTimestamps()`            
          `BuildRuleKeys`                               `getRuleKeys()`                               
          `BuildRuleStatus`                             `getStatus()`                                 
          `Optional<String>`                            `getStrategyResult()`                         
          `Optional<BuildRuleSuccessType>`              `getSuccessType()`                            
          `Optional<String>`                            `getSuccessTypeName()`                        
          `UploadToCacheResultType`                     `getUploadToCacheResultType()`                
          `boolean`                                     `isBuildRuleNoOp()`                           
          `String`                                      `toString()`                                  

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.build.event.BuildRuleEvent.EndingBuildRuleEvent}

            ### Methods inherited from class com.facebook.buck.core.build.event.[BuildRuleEvent.EndingBuildRuleEvent](BuildRuleEvent.EndingBuildRuleEvent.html "class in com.facebook.buck.core.build.event")

            `configure, getBeginningEvent, isRuleRunningAfterThisEvent`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.build.event.BuildRuleEvent}

            ### Methods inherited from class com.facebook.buck.core.build.event.[BuildRuleEvent](BuildRuleEvent.html "class in com.facebook.buck.core.build.event")

            `finished, getBuildRule, getDuration, getEventName, getValueString, resumed, ruleKeyCalculationFinished, ruleKeyCalculationScope, ruleKeyCalculationStarted, started, suspended, willBuildLocally`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.event.AbstractBuckEvent}

            ### Methods inherited from class com.facebook.buck.event.[AbstractBuckEvent](../../../event/AbstractBuckEvent.html "class in com.facebook.buck.event")

            `equals, getBuildId, getEventKey, getNanoTime, getThreadId, getThreadUserNanoTime, getTimestampMillis, hashCode, isConfigured, isRelatedTo, toLogMessage`

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

            ### Methods inherited from interface com.facebook.buck.event.[BuckEvent](../../../event/BuckEvent.html "interface in com.facebook.buck.event")

            `getBuildId, getEventKey, getNanoTime, getThreadId, getThreadUserNanoTime, isConfigured, isRelatedTo, toLogMessage`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Methods inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](../../../event/external/events/BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `getTimestampMillis, storeLastInstanceAndReplayForNewClients`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getStatus()}

        -   #### getStatus

            ``` methodSignature
            public BuildRuleStatus getStatus()
            ```

        []{#getCacheResult()}

        -   #### getCacheResult

            ``` methodSignature
            public CacheResult getCacheResult()
            ```

        []{#getOrigin()}

        -   #### getOrigin

            ``` methodSignature
            public Optional<BuildId> getOrigin()
            ```

        []{#getSuccessType()}

        -   #### getSuccessType

            ``` methodSignature
            public Optional<BuildRuleSuccessType> getSuccessType()
            ```

        []{#getSuccessTypeName()}

        -   #### getSuccessTypeName

            ``` methodSignature
            public Optional<String> getSuccessTypeName()
            ```

        []{#getUploadToCacheResultType()}

        -   #### getUploadToCacheResultType

            ``` methodSignature
            public UploadToCacheResultType getUploadToCacheResultType()
            ```

        []{#getRuleKeys()}

        -   #### getRuleKeys

            ``` methodSignature
            public BuildRuleKeys getRuleKeys()
            ```

        []{#getOutputHash()}

        -   #### getOutputHash

            ``` methodSignature
            public Optional<com.google.common.hash.HashCode> getOutputHash()
            ```

        []{#getOutputSize()}

        -   #### getOutputSize

            ``` methodSignature
            public Optional<Long> getOutputSize()
            ```

        []{#getDiagnosticData()}

        -   #### getDiagnosticData

            ``` methodSignature
            public Optional<BuildRuleDiagnosticData> getDiagnosticData()
            ```

        []{#getManifestFetchResult()}

        -   #### getManifestFetchResult

            ``` methodSignature
            public Optional<ManifestFetchResult> getManifestFetchResult()
            ```

        []{#getManifestStoreResult()}

        -   #### getManifestStoreResult

            ``` methodSignature
            public Optional<ManifestStoreResult> getManifestStoreResult()
            ```

        []{#getRuleKeyCacheCheckTimestamps()}

        -   #### getRuleKeyCacheCheckTimestamps

            ``` methodSignature
            public Optional<Pair<Long,​Long>> getRuleKeyCacheCheckTimestamps()
            ```

        []{#getInputRuleKeyCacheCheckTimestamps()}

        -   #### getInputRuleKeyCacheCheckTimestamps

            ``` methodSignature
            public Optional<Pair<Long,​Long>> getInputRuleKeyCacheCheckTimestamps()
            ```

        []{#getManifestRuleKeyCacheCheckTimestamps()}

        -   #### getManifestRuleKeyCacheCheckTimestamps

            ``` methodSignature
            public Optional<Pair<Long,​Long>> getManifestRuleKeyCacheCheckTimestamps()
            ```

        []{#getBuildTimestamps()}

        -   #### getBuildTimestamps

            ``` methodSignature
            public Optional<Pair<Long,​Long>> getBuildTimestamps()
            ```

        []{#getStrategyResult()}

        -   #### getStrategyResult

            ``` methodSignature
            public Optional<String> getStrategyResult()
            ```

        []{#isBuildRuleNoOp()}

        -   #### isBuildRuleNoOp

            ``` methodSignature
            public boolean isBuildRuleNoOp()
            ```

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `AbstractBuckEvent`

        []{#getResultString()}

        -   #### getResultString

            ``` methodSignature
            public String getResultString()
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
