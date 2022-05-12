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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.analysis](package-summary.html)
:::

## Interface RuleAnalysisContext {#interface-ruleanalysiscontext .title title="Interface RuleAnalysisContext"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `DependencyOnlyRuleAnalysisContext`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `RuleAnalysisContextImpl`

    ------------------------------------------------------------------------

        public interface RuleAnalysisContext
        extends DependencyOnlyRuleAnalysisContext

    ::: block
    A context that will be supplied to a
    [`Description`](../../description/Description.html "interface in com.facebook.buck.core.description")\'s
    rule implementation so that the rule analysis can be performed. This
    context will be used to create the rule\'s `Provider`, and register
    corresponding Actions. Actions will be
    [`BuildRule`](../BuildRule.html "interface in com.facebook.buck.core.rules")s
    for now, but we will eventually migrate to some other representation
    of the set of
    [`Step`](../../../step/Step.html "interface in com.facebook.buck.step").
    The
    [`RuleAnalysisContext`](RuleAnalysisContext.html "interface in com.facebook.buck.core.rules.analysis")
    will be very similar to Bazel\'s
    `  com.google.devtools.build.lib.analysis.RuleContext`. {@see
    [RuleContext](https://github.com/bazelbuild/bazel/blob/master/src/main/java/com/google/devtools/build/lib/analysis/RuleContext.java)}

    This will contain information on the configurations of the current
    rule, information about it\'s transitive dependencies via
    `Provider`s and their corresponding `InfoInterface`s. It will also
    offer ways to register
    [`Step`](../../../step/Step.html "interface in com.facebook.buck.step")s.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `ActionRegistry`      | `actionRegistry()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuckEventBus`        | `getEventBus()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `resolve              | ::: block             |
        | oviderInfoCollection` | Dep​(BuildTarget dep)` | same as               |
        |                       |                       | [`resolveDeps(Ite     |
        |                       |                       | rable)`](#resolveDeps |
        |                       |                       | (java.lang.Iterable)) |
        |                       |                       | but for one dep       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Map<BuildTarget,​Pro  | `resolveDeps​(Iterabl  |                       |
        | viderInfoCollection>` | e<BuildTarget> deps)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Artifact`            | `resolv               | ::: block             |
        |                       | eSrc​(SourcePath src)` | same as               |
        |                       |                       | [`resolveSrcs(Ite     |
        |                       |                       | rable)`](#resolveSrcs |
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
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#resolveDeps(java.lang.Iterable)}

        -   #### resolveDeps

            ``` methodSignature
            Map<BuildTarget,​ProviderInfoCollection> resolveDeps​(Iterable<BuildTarget> deps)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolveDeps` in
                interface `DependencyOnlyRuleAnalysisContext`

            [Returns:]{.returnLabel}
            :   a map of the
                [`ProviderInfoCollection`](../providers/collect/ProviderInfoCollection.html "interface in com.facebook.buck.core.rules.providers.collect")
                of the providers propagated by each of the dependencies
                requested.

        []{#resolveDep(com.facebook.buck.core.model.BuildTarget)}

        -   #### resolveDep

            ``` methodSignature
            ProviderInfoCollection resolveDep​(BuildTarget dep)
            ```

            ::: block
            same as
            [`resolveDeps(Iterable)`](#resolveDeps(java.lang.Iterable))
            but for one dep
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolveDep` in
                interface `DependencyOnlyRuleAnalysisContext`

        []{#resolveSrcs(java.lang.Iterable)}

        -   #### resolveSrcs

            ``` methodSignature
            com.google.common.collect.ImmutableSortedSet<Artifact> resolveSrcs​(Iterable<SourcePath> srcs)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolveSrcs` in
                interface `DependencyOnlyRuleAnalysisContext`

            [Returns:]{.returnLabel}
            :   a list of the
                [`Artifact`](../../artifact/Artifact.html "interface in com.facebook.buck.core.artifact")
                of the sources of the providers propagated by each of
                the source paths requested.

        []{#resolveSrc(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### resolveSrc

            ``` methodSignature
            Artifact resolveSrc​(SourcePath src)
            ```

            ::: block
            same as
            [`resolveSrcs(Iterable)`](#resolveSrcs(java.lang.Iterable))
            but for one src
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolveSrc` in
                interface `DependencyOnlyRuleAnalysisContext`

        []{#actionRegistry()}

        -   #### actionRegistry

            ``` methodSignature
            ActionRegistry actionRegistry()
            ```

            [Returns:]{.returnLabel}
            :   the factory for creating
                [`Artifact`](../../artifact/Artifact.html "interface in com.facebook.buck.core.artifact")s
                and registering
                [`Action`](../actions/Action.html "interface in com.facebook.buck.core.rules.actions")s

        []{#getEventBus()}

        -   #### getEventBus

            ``` methodSignature
            BuckEventBus getEventBus()
            ```

            [Returns:]{.returnLabel}
            :   an
                [`BuckEventBus`](../../../event/BuckEventBus.html "interface in com.facebook.buck.event")
                for sending stats and printing
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
