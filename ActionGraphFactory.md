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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.model.actiongraph.computation](package-summary.html)
:::

## Class ActionGraphFactory {#class-actiongraphfactory .title title="Class ActionGraphFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.model.actiongraph.computation.ActionGraphFactory

::: description
-   

    ------------------------------------------------------------------------

        public class ActionGraphFactory
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type             Method                                                                                                                                                                                                                                                                                                                                                    Description
          ----------------------------- --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `static ActionGraphFactory`   `create​(BuckEventBus eventBus,       CellProvider cellProvider,       com.google.common.collect.ImmutableMap<ExecutorPool,​com.google.common.util.concurrent.ListeningExecutorService> executorSupplier,       CloseableMemoizedSupplier<DepsAwareExecutor<? super ComputeResult,​?>> depsAwareExecutor,       BuckConfig buckConfig)`                       
          `ActionGraphAndBuilder`       `createActionGraph​(TargetNodeToBuildRuleTransformer transformer,                  TargetGraph targetGraph,                  IncrementalActionGraphMode incrementalActionGraphMode,                  com.facebook.buck.core.model.actiongraph.computation.ActionGraphFactory.ActionGraphCreationLifecycleListener actionGraphCreationLifecycleListener)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
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
    -   []{#method.detail}

        ### Method Detail

        []{#create(com.facebook.buck.event.BuckEventBus,com.facebook.buck.core.cell.CellProvider,com.google.common.collect.ImmutableMap,com.facebook.buck.util.CloseableMemoizedSupplier,com.facebook.buck.core.config.BuckConfig)}

        -   #### create

            ``` methodSignature
            public static ActionGraphFactory create​(BuckEventBus eventBus,
                                                    CellProvider cellProvider,
                                                    com.google.common.collect.ImmutableMap<ExecutorPool,​com.google.common.util.concurrent.ListeningExecutorService> executorSupplier,
                                                    CloseableMemoizedSupplier<DepsAwareExecutor<? super ComputeResult,​?>> depsAwareExecutor,
                                                    BuckConfig buckConfig)
            ```

        []{#createActionGraph(com.facebook.buck.core.rules.transformer.TargetNodeToBuildRuleTransformer,com.facebook.buck.core.model.targetgraph.TargetGraph,com.facebook.buck.core.model.actiongraph.computation.IncrementalActionGraphMode,com.facebook.buck.core.model.actiongraph.computation.ActionGraphFactory.ActionGraphCreationLifecycleListener)}

        -   #### createActionGraph

            ``` methodSignature
            public ActionGraphAndBuilder createActionGraph​(TargetNodeToBuildRuleTransformer transformer,
                                                           TargetGraph targetGraph,
                                                           IncrementalActionGraphMode incrementalActionGraphMode,
                                                           com.facebook.buck.core.model.actiongraph.computation.ActionGraphFactory.ActionGraphCreationLifecycleListener actionGraphCreationLifecycleListener)
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
