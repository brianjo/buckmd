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
[Package]{.packageLabelInType} [com.facebook.buck.core.model.actiongraph.computation](package-summary.html)
:::

## Class ActionGraphProvider {#class-actiongraphprovider .title title="Class ActionGraphProvider"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.model.actiongraph.computation.ActionGraphProvider

::: description
-   

    ------------------------------------------------------------------------

        public class ActionGraphProvider
        extends Object

    ::: block
    Class that transforms
    [`TargetGraph`](../../targetgraph/TargetGraph.html "class in com.facebook.buck.core.model.targetgraph")
    to
    [`ActionGraph`](../ActionGraph.html "class in com.facebook.buck.core.model.actiongraph").
    It also holds a cache for the last ActionGraph it generated.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                           Description
          ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `ActionGraphProvider​(BuckEventBus eventBus,                    ActionGraphFactory actionGraphFactory,                    ActionGraphCache actionGraphCache,                    RuleKeyConfiguration ruleKeyConfiguration,                    boolean checkActionGraphs,                    boolean skipActionGraphCache,                    IncrementalActionGraphMode incrementalActionGraphMode)`    
          `ActionGraphProvider​(BuckEventBus eventBus,                    ActionGraphFactory actionGraphFactory,                    ActionGraphCache actionGraphCache,                    RuleKeyConfiguration ruleKeyConfiguration,                    BuckConfig buckConfig)`                                                                                                                                   

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `A                    | `getActionGra         | ::: block             |
        | ctionGraphAndBuilder` | ph​(TargetGraphCreatio | Create an             |
        |                       | nResult targetGraph)` | ActionGraph, using    |
        |                       |                       | options extracted     |
        |                       |                       | from a BuckConfig.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `getActionGraph​(Targ  | ::: block             |
        | ctionGraphAndBuilder` | etNodeToBuildRuleTran | It returns an         |
        |                       | sformer transformer,  | [`Ac                  |
        |                       |               TargetG | tionGraphAndBuilder`] |
        |                       | raphCreationResult ta | (../ActionGraphAndBui |
        |                       | rgetGraphCreationResu | lder.html "class in c |
        |                       | lt,               Opt | om.facebook.buck.core |
        |                       | ional<ThriftRuleKeyLo | .model.actiongraph"). |
        |                       | gger> ruleKeyLogger)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `getFreshActionGra    | ::: block             |
        | ctionGraphAndBuilder` | ph​(TargetGraphCreatio | \* It returns a new   |
        |                       | nResult targetGraph)` | [`A                   |
        |                       |                       | ctionGraphAndBuilder` |
        |                       |                       | ](../ActionGraphAndBu |
        |                       |                       | ilder.html "class in  |
        |                       |                       | com.facebook.buck.cor |
        |                       |                       | e.model.actiongraph") |
        |                       |                       | based on the          |
        |                       |                       | targetGraph without   |
        |                       |                       | checking the cache.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `getFreshActionGraph  | ::: block             |
        | ctionGraphAndBuilder` | ​(TargetNodeToBuildRul | It returns a new      |
        |                       | eTransformer transfor | [`A                   |
        |                       | mer,                  | ctionGraphAndBuilder` |
        |                       |    TargetGraphCreatio | ](../ActionGraphAndBu |
        |                       | nResult targetGraph)` | ilder.html "class in  |
        |                       |                       | com.facebook.buck.cor |
        |                       |                       | e.model.actiongraph") |
        |                       |                       | based on the          |
        |                       |                       | targetGraph without   |
        |                       |                       | checking the cache.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

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

        []{#<init>(com.facebook.buck.event.BuckEventBus,com.facebook.buck.core.model.actiongraph.computation.ActionGraphFactory,com.facebook.buck.core.model.actiongraph.computation.ActionGraphCache,com.facebook.buck.rules.keys.config.RuleKeyConfiguration,boolean,boolean,com.facebook.buck.core.model.actiongraph.computation.IncrementalActionGraphMode)}

        -   #### ActionGraphProvider

                public ActionGraphProvider​(BuckEventBus eventBus,
                                           ActionGraphFactory actionGraphFactory,
                                           ActionGraphCache actionGraphCache,
                                           RuleKeyConfiguration ruleKeyConfiguration,
                                           boolean checkActionGraphs,
                                           boolean skipActionGraphCache,
                                           IncrementalActionGraphMode incrementalActionGraphMode)

        []{#<init>(com.facebook.buck.event.BuckEventBus,com.facebook.buck.core.model.actiongraph.computation.ActionGraphFactory,com.facebook.buck.core.model.actiongraph.computation.ActionGraphCache,com.facebook.buck.rules.keys.config.RuleKeyConfiguration,com.facebook.buck.core.config.BuckConfig)}

        -   #### ActionGraphProvider

                public ActionGraphProvider​(BuckEventBus eventBus,
                                           ActionGraphFactory actionGraphFactory,
                                           ActionGraphCache actionGraphCache,
                                           RuleKeyConfiguration ruleKeyConfiguration,
                                           BuckConfig buckConfig)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getActionGraph(com.facebook.buck.core.model.targetgraph.TargetGraphCreationResult)}

        -   #### getActionGraph

            ``` methodSignature
            public ActionGraphAndBuilder getActionGraph​(TargetGraphCreationResult targetGraph)
            ```

            ::: block
            Create an ActionGraph, using options extracted from a
            BuckConfig.
            :::

        []{#getActionGraph(com.facebook.buck.core.rules.transformer.TargetNodeToBuildRuleTransformer,com.facebook.buck.core.model.targetgraph.TargetGraphCreationResult,java.util.Optional)}

        -   #### getActionGraph

            ``` methodSignature
            public ActionGraphAndBuilder getActionGraph​(TargetNodeToBuildRuleTransformer transformer,
                                                        TargetGraphCreationResult targetGraphCreationResult,
                                                        Optional<ThriftRuleKeyLogger> ruleKeyLogger)
            ```

            ::: block
            It returns an
            [`ActionGraphAndBuilder`](../ActionGraphAndBuilder.html "class in com.facebook.buck.core.model.actiongraph").
            If the `targetGraph` exists in the cache it returns a cached
            version of the
            [`ActionGraphAndBuilder`](../ActionGraphAndBuilder.html "class in com.facebook.buck.core.model.actiongraph"),
            else returns a new one and updates the cache.
            :::

            [Parameters:]{.paramLabel}
            :   `targetGraphCreationResult` - the target graph that the
                action graph will be based on.

            [Returns:]{.returnLabel}
            :   a
                [`ActionGraphAndBuilder`](../ActionGraphAndBuilder.html "class in com.facebook.buck.core.model.actiongraph")

        []{#getFreshActionGraph(com.facebook.buck.core.model.targetgraph.TargetGraphCreationResult)}

        -   #### getFreshActionGraph

            ``` methodSignature
            public ActionGraphAndBuilder getFreshActionGraph​(TargetGraphCreationResult targetGraph)
            ```

            ::: block
            \* It returns a new
            [`ActionGraphAndBuilder`](../ActionGraphAndBuilder.html "class in com.facebook.buck.core.model.actiongraph")
            based on the targetGraph without checking the cache. It uses
            a
            [`DefaultTargetNodeToBuildRuleTransformer`](../../../rules/transformer/impl/DefaultTargetNodeToBuildRuleTransformer.html "class in com.facebook.buck.core.rules.transformer.impl").
            :::

            [Parameters:]{.paramLabel}
            :   `targetGraph` - the target graph that the action graph
                will be based on.

            [Returns:]{.returnLabel}
            :   a
                [`ActionGraphAndBuilder`](../ActionGraphAndBuilder.html "class in com.facebook.buck.core.model.actiongraph")

        []{#getFreshActionGraph(com.facebook.buck.core.rules.transformer.TargetNodeToBuildRuleTransformer,com.facebook.buck.core.model.targetgraph.TargetGraphCreationResult)}

        -   #### getFreshActionGraph

            ``` methodSignature
            public ActionGraphAndBuilder getFreshActionGraph​(TargetNodeToBuildRuleTransformer transformer,
                                                             TargetGraphCreationResult targetGraph)
            ```

            ::: block
            It returns a new
            [`ActionGraphAndBuilder`](../ActionGraphAndBuilder.html "class in com.facebook.buck.core.model.actiongraph")
            based on the targetGraph without checking the cache. It uses
            a custom
            [`TargetNodeToBuildRuleTransformer`](../../../rules/transformer/TargetNodeToBuildRuleTransformer.html "interface in com.facebook.buck.core.rules.transformer").
            :::

            [Parameters:]{.paramLabel}
            :   `transformer` - Custom
                [`TargetNodeToBuildRuleTransformer`](../../../rules/transformer/TargetNodeToBuildRuleTransformer.html "interface in com.facebook.buck.core.rules.transformer")
                that the transformation will be based on.
            :   `targetGraph` - The target graph that the action graph
                will be based on.

            [Returns:]{.returnLabel}
            :   It returns a
                [`ActionGraphAndBuilder`](../ActionGraphAndBuilder.html "class in com.facebook.buck.core.model.actiongraph")
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
