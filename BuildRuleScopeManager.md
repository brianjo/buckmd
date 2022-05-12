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

-   [Overview](../../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../../index-all.html)
-   [Help](../../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.build.engine.cache.manager](package-summary.html)
:::

## Class BuildRuleScopeManager {#class-buildrulescopemanager .title title="Class BuildRuleScopeManager"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.build.engine.cache.manager.BuildRuleScopeManager

::: description
-   

    ------------------------------------------------------------------------

        public class BuildRuleScopeManager
        extends Object

    ::: block
    Handles BuildRule resumed/suspended/finished scopes. Only one scope
    can be active at a time. Scopes nested on the same thread are
    allowed.
    Once the rule has been marked as finished, any further scope() calls
    will fail.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `BuildRuleScopeManager​(RuleKeyFactories ruleKeyFactories,                      OnDiskBuildInfo onDiskBuildInfo,                      BuildRuleDurationTracker buildRuleDurationTracker,                      RuleKeyDiagnostics<RuleKey,​String> defaultRuleKeyDiagnostics,                      RuleKeyDiagnosticsMode ruleKeyDiagnosticsMode,                      BuildRule rule,                      RuleDepsCache ruleDeps,                      RuleKey defaultKey,                      BuckEventBus eventBus)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     Description
          ------------------- ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `void`              `finished​(BuildResult input,         Optional<Long> outputSize,         Optional<com.google.common.hash.HashCode> outputHash,         Optional<BuildRuleSuccessType> successType,         UploadToCacheResultType UploadToCacheResultType,         Optional<Pair<Long,​Long>> ruleKeyCacheCheckTimestamps,         Optional<Pair<Long,​Long>> inputRuleKeyCacheCheckTimestamps,         Optional<Pair<Long,​Long>> manifestRuleKeyCacheCheckTimestamps,         Optional<Pair<Long,​Long>> buildTimestamps)`    
          `Scope`             `scope()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   
          `void`              `setManifestFetchResult​(ManifestFetchResult manifestFetchResult)`                                                                                                                                                                                                                                                                                                                                                                                                                                           
          `void`              `setManifestStoreResult​(ManifestStoreResult manifestStoreResult)`                                                                                                                                                                                                                                                                                                                                                                                                                                           

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
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

        []{#<init>(com.facebook.buck.rules.keys.RuleKeyFactories,com.facebook.buck.core.build.engine.buildinfo.OnDiskBuildInfo,com.facebook.buck.core.build.stats.BuildRuleDurationTracker,com.facebook.buck.rules.keys.RuleKeyDiagnostics,com.facebook.buck.core.rulekey.RuleKeyDiagnosticsMode,com.facebook.buck.core.rules.BuildRule,com.facebook.buck.core.build.engine.RuleDepsCache,com.facebook.buck.core.rulekey.RuleKey,com.facebook.buck.event.BuckEventBus)}

        -   #### BuildRuleScopeManager

                public BuildRuleScopeManager​(RuleKeyFactories ruleKeyFactories,
                                             OnDiskBuildInfo onDiskBuildInfo,
                                             BuildRuleDurationTracker buildRuleDurationTracker,
                                             RuleKeyDiagnostics<RuleKey,​String> defaultRuleKeyDiagnostics,
                                             RuleKeyDiagnosticsMode ruleKeyDiagnosticsMode,
                                             BuildRule rule,
                                             RuleDepsCache ruleDeps,
                                             RuleKey defaultKey,
                                             BuckEventBus eventBus)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#scope()}

        -   #### scope

            ``` methodSignature
            public Scope scope()
            ```

        []{#finished(com.facebook.buck.core.build.engine.BuildResult,java.util.Optional,java.util.Optional,java.util.Optional,com.facebook.buck.core.build.engine.type.UploadToCacheResultType,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional)}

        -   #### finished

            ``` methodSignature
            public void finished​(BuildResult input,
                                 Optional<Long> outputSize,
                                 Optional<com.google.common.hash.HashCode> outputHash,
                                 Optional<BuildRuleSuccessType> successType,
                                 UploadToCacheResultType UploadToCacheResultType,
                                 Optional<Pair<Long,​Long>> ruleKeyCacheCheckTimestamps,
                                 Optional<Pair<Long,​Long>> inputRuleKeyCacheCheckTimestamps,
                                 Optional<Pair<Long,​Long>> manifestRuleKeyCacheCheckTimestamps,
                                 Optional<Pair<Long,​Long>> buildTimestamps)
            ```

        []{#setManifestStoreResult(com.facebook.buck.core.build.engine.manifest.ManifestStoreResult)}

        -   #### setManifestStoreResult

            ``` methodSignature
            public void setManifestStoreResult​(@Nullable
                                               ManifestStoreResult manifestStoreResult)
            ```

        []{#setManifestFetchResult(com.facebook.buck.core.build.engine.manifest.ManifestFetchResult)}

        -   #### setManifestFetchResult

            ``` methodSignature
            public void setManifestFetchResult​(@Nullable
                                               ManifestFetchResult manifestFetchResult)
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

-   [Overview](../../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../../index-all.html)
-   [Help](../../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../../allclasses.html)

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
