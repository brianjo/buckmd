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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.analysis.context](package-summary.html)
:::

## Interface DependencyOnlyRuleAnalysisContext {#interface-dependencyonlyruleanalysiscontext .title title="Interface DependencyOnlyRuleAnalysisContext"}
:::

::: contentContainer
::: description
-   

    All Known Subinterfaces:
    :   `RuleAnalysisContext`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `RuleAnalysisContextImpl`

    ------------------------------------------------------------------------

        public interface DependencyOnlyRuleAnalysisContext

    ::: block
    Reduced context from
    [`RuleAnalysisContext`](../RuleAnalysisContext.html "interface in com.facebook.buck.core.rules.analysis")
    that only resolves deps and sources. This primarily exists to get
    around a circular dependency in some places that we want to use
    providers (namely in toolchains, where
    [`ActionRegistry`](../../actions/ActionRegistry.html "interface in com.facebook.buck.core.rules.actions")
    causes a circular dependency)
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
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

            [Returns:]{.returnLabel}
            :   a map of the
                [`ProviderInfoCollection`](../../providers/collect/ProviderInfoCollection.html "interface in com.facebook.buck.core.rules.providers.collect")
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

        []{#resolveSrcs(java.lang.Iterable)}

        -   #### resolveSrcs

            ``` methodSignature
            com.google.common.collect.ImmutableSortedSet<Artifact> resolveSrcs​(Iterable<SourcePath> srcs)
            ```

            [Returns:]{.returnLabel}
            :   a list of the
                [`Artifact`](../../../artifact/Artifact.html "interface in com.facebook.buck.core.artifact")
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
