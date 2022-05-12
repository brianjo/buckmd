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
[Package]{.packageLabelInType} [com.facebook.buck.rules.keys](package-summary.html)
:::

## Interface TrackableRuleKeyCache\<V\> {#interface-trackablerulekeycachev .title title="Interface TrackableRuleKeyCache"}
:::

::: contentContainer
::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `V` -

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `DefaultRuleKeyCache`

    ------------------------------------------------------------------------

        public interface TrackableRuleKeyCache<V>

    ::: block
    RuleKeyCache that can be tracked with `CacheStatsTracker`
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                   Method                                                                                                                                                                  Description
          ------------------------------------------------------------------- ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `V`                                                                 `get​(BuildEngineAction action,    CacheStatsTracker statsTracker)`                                                                                                       
          `V`                                                                 `get​(BuildEngineAction rule,    java.util.function.Function<? super BuildEngineAction,​RuleKeyResult<V>> create,    CacheStatsTracker statsTracker)`                      
          `V`                                                                 `get​(AddsToRuleKey appendable,    java.util.function.Function<? super AddsToRuleKey,​RuleKeyResult<V>> create,    CacheStatsTracker statsTracker)`                        
          `com.google.common.collect.ImmutableList<Map.Entry<BuildRule,​V>>`   `getCachedBuildRules()`                                                                                                                                                  
          `void`                                                              `invalidateAll​(CacheStatsTracker statsTracker)`                                                                                                                          
          `void`                                                              `invalidateAllExceptFilesystems​(com.google.common.collect.ImmutableSet<ProjectFilesystem> filesystems,                               CacheStatsTracker statsTracker)`    
          `void`                                                              `invalidateFilesystem​(ProjectFilesystem filesystem,                     CacheStatsTracker statsTracker)`                                                                 
          `void`                                                              `invalidateInputs​(Iterable<com.facebook.buck.rules.keys.RuleKeyInput> inputs,                 CacheStatsTracker statsTracker)`                                           

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#get(com.facebook.buck.core.build.action.BuildEngineAction,com.facebook.buck.util.cache.CacheStatsTracker)}

        -   #### get

            ``` methodSignature
            @Nullable
            V get​(BuildEngineAction action,
                  CacheStatsTracker statsTracker)
            ```

        []{#get(com.facebook.buck.core.build.action.BuildEngineAction,java.util.function.Function,com.facebook.buck.util.cache.CacheStatsTracker)}

        -   #### get

            ``` methodSignature
            V get​(BuildEngineAction rule,
                  java.util.function.Function<? super BuildEngineAction,​RuleKeyResult<V>> create,
                  CacheStatsTracker statsTracker)
            ```

        []{#get(com.facebook.buck.core.rulekey.AddsToRuleKey,java.util.function.Function,com.facebook.buck.util.cache.CacheStatsTracker)}

        -   #### get

            ``` methodSignature
            V get​(AddsToRuleKey appendable,
                  java.util.function.Function<? super AddsToRuleKey,​RuleKeyResult<V>> create,
                  CacheStatsTracker statsTracker)
            ```

        []{#invalidateInputs(java.lang.Iterable,com.facebook.buck.util.cache.CacheStatsTracker)}

        -   #### invalidateInputs

            ``` methodSignature
            void invalidateInputs​(Iterable<com.facebook.buck.rules.keys.RuleKeyInput> inputs,
                                  CacheStatsTracker statsTracker)
            ```

        []{#invalidateAllExceptFilesystems(com.google.common.collect.ImmutableSet,com.facebook.buck.util.cache.CacheStatsTracker)}

        -   #### invalidateAllExceptFilesystems

            ``` methodSignature
            void invalidateAllExceptFilesystems​(com.google.common.collect.ImmutableSet<ProjectFilesystem> filesystems,
                                                CacheStatsTracker statsTracker)
            ```

        []{#invalidateFilesystem(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.util.cache.CacheStatsTracker)}

        -   #### invalidateFilesystem

            ``` methodSignature
            void invalidateFilesystem​(ProjectFilesystem filesystem,
                                      CacheStatsTracker statsTracker)
            ```

        []{#invalidateAll(com.facebook.buck.util.cache.CacheStatsTracker)}

        -   #### invalidateAll

            ``` methodSignature
            void invalidateAll​(CacheStatsTracker statsTracker)
            ```

        []{#getCachedBuildRules()}

        -   #### getCachedBuildRules

            ``` methodSignature
            com.google.common.collect.ImmutableList<Map.Entry<BuildRule,​V>> getCachedBuildRules()
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
