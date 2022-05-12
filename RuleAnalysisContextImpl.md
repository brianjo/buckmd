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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.analysis.impl](package-summary.html)
:::

## Class RuleAnalysisContextImpl {#class-ruleanalysiscontextimpl .title title="Class RuleAnalysisContextImpl"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rules.analysis.impl.RuleAnalysisContextImpl

::: description
-   

    All Implemented Interfaces:
    :   `ActionAnalysisDataRegistry`,
        `DependencyOnlyRuleAnalysisContext`, `RuleAnalysisContext`

    ------------------------------------------------------------------------

        public class RuleAnalysisContextImpl
        extends Object
        implements RuleAnalysisContext, ActionAnalysisDataRegistry

    ::: block
    Implementation of
    [`RuleAnalysisContext`](../RuleAnalysisContext.html "interface in com.facebook.buck.core.rules.analysis").
    This context is created per rule analysis.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                             Description
          ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `RuleAnalysisContextImpl​(BuildTarget buildTarget,                        com.google.common.collect.ImmutableMap<BuildTarget,​ProviderInfoCollection> depProviders,                        ProjectFilesystem filesystem,                        BuckEventBus eventBus)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `ActionRegistry`      | `actionRegistry()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuckEventBus`        | `getEventBus()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Map<                 | `getRe                | ::: block             |
        | ActionAnalysisData.ID | gisteredActionData()` | Verifies that the     |
        | ,​ActionAnalysisData>` |                       | [`ActionRegistry`](.. |
        |                       |                       | /../actions/ActionReg |
        |                       |                       | istry.html "interface |
        |                       |                       |  in com.facebook.buck |
        |                       |                       | .core.rules.actions") |
        |                       |                       | has been finalized    |
        |                       |                       | where all             |
        |                       |                       | [`Artifac             |
        |                       |                       | t`](../../../artifact |
        |                       |                       | /Artifact.html "inter |
        |                       |                       | face in com.facebook. |
        |                       |                       | buck.core.artifact")s |
        |                       |                       | are bound, and then   |
        |                       |                       | returns all the       |
        |                       |                       | [`ActionAnal          |
        |                       |                       | ysisData`](../action/ |
        |                       |                       | ActionAnalysisData.ht |
        |                       |                       | ml "interface in com. |
        |                       |                       | facebook.buck.core.ru |
        |                       |                       | les.analysis.action") |
        |                       |                       | registered.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `registerActi         |                       |
        |                       | on​(ActionAnalysisData |                       |
        |                       |  actionAnalysisData)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `resolve              | ::: block             |
        | oviderInfoCollection` | Dep​(BuildTarget dep)` | same as               |
        |                       |                       | [                     |
        |                       |                       | `RuleAnalysisContext. |
        |                       |                       | resolveDeps(Iterable) |
        |                       |                       | `](../RuleAnalysisCon |
        |                       |                       | text.html#resolveDeps |
        |                       |                       | (java.lang.Iterable)) |
        |                       |                       | but for one dep       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Map<BuildTarget,​Pro  | `resolveDeps​(Iterabl  |                       |
        | viderInfoCollection>` | e<BuildTarget> deps)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Artifact`            | `resolv               | ::: block             |
        |                       | eSrc​(SourcePath src)` | same as               |
        |                       |                       | [                     |
        |                       |                       | `RuleAnalysisContext. |
        |                       |                       | resolveSrcs(Iterable) |
        |                       |                       | `](../RuleAnalysisCon |
        |                       |                       | text.html#resolveSrcs |
        |                       |                       | (java.lang.Iterable)) |
        |                       |                       | but for one src       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.co        | `resolveSrcs​(Iterab   |                       |
        | mmon.collect.Immutabl | le<SourcePath> srcs)` |                       |
        | eSortedSet<Artifact>` |                       |                       |
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

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.google.common.collect.ImmutableMap,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.event.BuckEventBus)}

        -   #### RuleAnalysisContextImpl

                public RuleAnalysisContextImpl​(BuildTarget buildTarget,
                                               com.google.common.collect.ImmutableMap<BuildTarget,​ProviderInfoCollection> depProviders,
                                               ProjectFilesystem filesystem,
                                               BuckEventBus eventBus)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#resolveDeps(java.lang.Iterable)}

        -   #### resolveDeps

            ``` methodSignature
            public Map<BuildTarget,​ProviderInfoCollection> resolveDeps​(Iterable<BuildTarget> deps)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolveDeps` in
                interface `DependencyOnlyRuleAnalysisContext`

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolveDeps` in interface `RuleAnalysisContext`

            [Returns:]{.returnLabel}
            :   a map of the
                [`ProviderInfoCollection`](../../providers/collect/ProviderInfoCollection.html "interface in com.facebook.buck.core.rules.providers.collect")
                of the providers propagated by each of the dependencies
                requested.

        []{#resolveDep(com.facebook.buck.core.model.BuildTarget)}

        -   #### resolveDep

            ``` methodSignature
            public ProviderInfoCollection resolveDep​(BuildTarget dep)
            ```

            ::: block
            [Description copied from
            interface: `RuleAnalysisContext`]{.descfrmTypeLabel}
            :::

            ::: block
            same as
            [`RuleAnalysisContext.resolveDeps(Iterable)`](../RuleAnalysisContext.html#resolveDeps(java.lang.Iterable))
            but for one dep
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolveDep` in
                interface `DependencyOnlyRuleAnalysisContext`

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolveDep` in interface `RuleAnalysisContext`

        []{#resolveSrcs(java.lang.Iterable)}

        -   #### resolveSrcs

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<Artifact> resolveSrcs​(Iterable<SourcePath> srcs)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolveSrcs` in
                interface `DependencyOnlyRuleAnalysisContext`

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolveSrcs` in interface `RuleAnalysisContext`

            [Returns:]{.returnLabel}
            :   a list of the
                [`Artifact`](../../../artifact/Artifact.html "interface in com.facebook.buck.core.artifact")
                of the sources of the providers propagated by each of
                the source paths requested.

        []{#resolveSrc(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### resolveSrc

            ``` methodSignature
            public Artifact resolveSrc​(SourcePath src)
            ```

            ::: block
            [Description copied from
            interface: `RuleAnalysisContext`]{.descfrmTypeLabel}
            :::

            ::: block
            same as
            [`RuleAnalysisContext.resolveSrcs(Iterable)`](../RuleAnalysisContext.html#resolveSrcs(java.lang.Iterable))
            but for one src
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolveSrc` in
                interface `DependencyOnlyRuleAnalysisContext`

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolveSrc` in interface `RuleAnalysisContext`

        []{#actionRegistry()}

        -   #### actionRegistry

            ``` methodSignature
            public ActionRegistry actionRegistry()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `actionRegistry` in interface `RuleAnalysisContext`

            [Returns:]{.returnLabel}
            :   the factory for creating
                [`Artifact`](../../../artifact/Artifact.html "interface in com.facebook.buck.core.artifact")s
                and registering
                [`Action`](../../actions/Action.html "interface in com.facebook.buck.core.rules.actions")s

        []{#getEventBus()}

        -   #### getEventBus

            ``` methodSignature
            public BuckEventBus getEventBus()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getEventBus` in interface `RuleAnalysisContext`

            [Returns:]{.returnLabel}
            :   an
                [`BuckEventBus`](../../../../event/BuckEventBus.html "interface in com.facebook.buck.event")
                for sending stats and printing

        []{#registerAction(com.facebook.buck.core.rules.analysis.action.ActionAnalysisData)}

        -   #### registerAction

            ``` methodSignature
            public void registerAction​(ActionAnalysisData actionAnalysisData)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `registerAction` in
                interface `ActionAnalysisDataRegistry`

        []{#getRegisteredActionData()}

        -   #### getRegisteredActionData

            ``` methodSignature
            public Map<ActionAnalysisData.ID,​ActionAnalysisData> getRegisteredActionData()
            ```

            ::: block
            Verifies that the
            [`ActionRegistry`](../../actions/ActionRegistry.html "interface in com.facebook.buck.core.rules.actions")
            has been finalized where all
            [`Artifact`](../../../artifact/Artifact.html "interface in com.facebook.buck.core.artifact")s
            are bound, and then returns all the
            [`ActionAnalysisData`](../action/ActionAnalysisData.html "interface in com.facebook.buck.core.rules.analysis.action")
            registered.
            :::
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
