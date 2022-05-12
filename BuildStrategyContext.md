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
[Package]{.packageLabelInType} [com.facebook.buck.core.build.engine](package-summary.html)
:::

## Interface BuildStrategyContext {#interface-buildstrategycontext .title title="Interface BuildStrategyContext"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `DelegatingBuildStrategyContext`

    ------------------------------------------------------------------------

        public interface BuildStrategyContext

    ::: block
    Used for running a BuildExecutor within the context of the build
    engine such that the engine\'s internal state/tracking is updated as
    expected. Provides ability to decide at runtime whether to use
    custom BuildExecutor or just the default.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                             Method                                                                                                    Description
          ----------------------------------------------------------------------------- --------------------------------------------------------------------------------------------------------- -------------
          `Scope`                                                                       `buildRuleScope()`                                                                                         
          `BuildResult`                                                                 `createBuildResult​(BuildRuleSuccessType successType,                  Optional<String> strategyResult)`    
          `BuildResult`                                                                 `createCancelledResult​(Throwable throwable)`                                                               
          `BuildableContext`                                                            `getBuildableContext()`                                                                                    
          `BuildContext`                                                                `getBuildRuleBuildContext()`                                                                               
          `ExecutionContext`                                                            `getExecutionContext()`                                                                                    
          `com.google.common.util.concurrent.ListeningExecutorService`                  `getExecutorService()`                                                                                     
          `com.google.common.util.concurrent.ListenableFuture<Optional<BuildResult>>`   `runWithDefaultBehavior()`                                                                                 

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

        []{#runWithDefaultBehavior()}

        -   #### runWithDefaultBehavior

            ``` methodSignature
            com.google.common.util.concurrent.ListenableFuture<Optional<BuildResult>> runWithDefaultBehavior()
            ```

        []{#getExecutorService()}

        -   #### getExecutorService

            ``` methodSignature
            com.google.common.util.concurrent.ListeningExecutorService getExecutorService()
            ```

        []{#createBuildResult(com.facebook.buck.core.build.engine.BuildRuleSuccessType,java.util.Optional)}

        -   #### createBuildResult

            ``` methodSignature
            BuildResult createBuildResult​(BuildRuleSuccessType successType,
                                          Optional<String> strategyResult)
            ```

        []{#createCancelledResult(java.lang.Throwable)}

        -   #### createCancelledResult

            ``` methodSignature
            BuildResult createCancelledResult​(Throwable throwable)
            ```

        []{#getExecutionContext()}

        -   #### getExecutionContext

            ``` methodSignature
            ExecutionContext getExecutionContext()
            ```

        []{#buildRuleScope()}

        -   #### buildRuleScope

            ``` methodSignature
            Scope buildRuleScope()
            ```

        []{#getBuildRuleBuildContext()}

        -   #### getBuildRuleBuildContext

            ``` methodSignature
            BuildContext getBuildRuleBuildContext()
            ```

        []{#getBuildableContext()}

        -   #### getBuildableContext

            ``` methodSignature
            BuildableContext getBuildableContext()
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
