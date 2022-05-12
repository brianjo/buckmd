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
[Package]{.packageLabelInType} [com.facebook.buck.cli](package-summary.html)
:::

## Interface MainRunner.ParserAndCaches {#interface-mainrunner.parserandcaches .title title="Interface MainRunner.ParserAndCaches"}
:::

::: contentContainer
::: description
-   

    Enclosing class:
    :   [MainRunner](MainRunner.html "class in com.facebook.buck.cli")

    ------------------------------------------------------------------------

        public static interface MainRunner.ParserAndCaches

    ::: block
    Struct for the multiple values returned by
    [`MainRunner.getParserAndCaches(java.util.Optional<com.facebook.nailgun.NGContext>, com.facebook.buck.io.watchman.WatchmanWatcher.FreshInstanceAction, com.facebook.buck.io.filesystem.ProjectFilesystem, com.facebook.buck.core.config.BuckConfig, com.facebook.buck.io.watchman.Watchman, com.facebook.buck.core.rules.knowntypes.provider.KnownRuleTypesProvider, com.facebook.buck.core.cell.Cell, com.facebook.buck.support.state.BuckGlobalState, com.facebook.buck.event.BuckEventBus, com.google.common.collect.ImmutableMap<com.facebook.buck.util.concurrent.ExecutorPool, com.google.common.util.concurrent.ListeningExecutorService>, com.facebook.buck.rules.keys.config.RuleKeyConfiguration, com.facebook.buck.util.CloseableMemoizedSupplier<com.facebook.buck.core.graph.transformation.executor.DepsAwareExecutor<? super com.facebook.buck.core.graph.transformation.model.ComputeResult, ?>>, com.facebook.buck.io.ExecutableFinder, com.facebook.buck.core.parser.buildtargetparser.UnconfiguredBuildTargetViewFactory, com.facebook.buck.core.model.TargetConfiguration, com.facebook.buck.parser.TargetSpecResolver)`](MainRunner.html#getParserAndCaches(java.util.Optional,com.facebook.buck.io.watchman.WatchmanWatcher.FreshInstanceAction,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.config.BuckConfig,com.facebook.buck.io.watchman.Watchman,com.facebook.buck.core.rules.knowntypes.provider.KnownRuleTypesProvider,com.facebook.buck.core.cell.Cell,com.facebook.buck.support.state.BuckGlobalState,com.facebook.buck.event.BuckEventBus,com.google.common.collect.ImmutableMap,com.facebook.buck.rules.keys.config.RuleKeyConfiguration,com.facebook.buck.util.CloseableMemoizedSupplier,com.facebook.buck.io.ExecutableFinder,com.facebook.buck.core.parser.buildtargetparser.UnconfiguredBuildTargetViewFactory,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.parser.TargetSpecResolver)).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                           Method                                      Description
          ------------------------------------------- ------------------------------------------- -------------
          `ActionGraphProvider`                       `getActionGraphProvider()`                   
          `Optional<RuleKeyCacheRecycler<RuleKey>>`   `getDefaultRuleKeyFactoryCacheRecycler()`    
          `Parser`                                    `getParser()`                                
          `TypeCoercerFactory`                        `getTypeCoercerFactory()`                    
          `InstrumentedVersionedTargetGraphCache`     `getVersionedTargetGraphCache()`             

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

        []{#getParser()}

        -   #### getParser

            ``` methodSignature
            Parser getParser()
            ```

        []{#getTypeCoercerFactory()}

        -   #### getTypeCoercerFactory

            ``` methodSignature
            TypeCoercerFactory getTypeCoercerFactory()
            ```

        []{#getVersionedTargetGraphCache()}

        -   #### getVersionedTargetGraphCache

            ``` methodSignature
            InstrumentedVersionedTargetGraphCache getVersionedTargetGraphCache()
            ```

        []{#getActionGraphProvider()}

        -   #### getActionGraphProvider

            ``` methodSignature
            ActionGraphProvider getActionGraphProvider()
            ```

        []{#getDefaultRuleKeyFactoryCacheRecycler()}

        -   #### getDefaultRuleKeyFactoryCacheRecycler

            ``` methodSignature
            Optional<RuleKeyCacheRecycler<RuleKey>> getDefaultRuleKeyFactoryCacheRecycler()
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
