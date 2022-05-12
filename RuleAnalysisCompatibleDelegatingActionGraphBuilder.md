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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.resolver.impl](package-summary.html)
:::

## Class RuleAnalysisCompatibleDelegatingActionGraphBuilder {#class-ruleanalysiscompatibledelegatingactiongraphbuilder .title title="Class RuleAnalysisCompatibleDelegatingActionGraphBuilder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRuleResolver](../../impl/AbstractBuildRuleResolver.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.core.rules.resolver.impl.AbstractActionGraphBuilder](AbstractActionGraphBuilder.html "class in com.facebook.buck.core.rules.resolver.impl")

        -   -   com.facebook.buck.core.rules.resolver.impl.RuleAnalysisCompatibleDelegatingActionGraphBuilder

::: description
-   

    All Implemented Interfaces:
    :   `ActionGraphBuilder`, `RuleAnalysisGraph`, `BuildRuleResolver`,
        `SourcePathRuleFinder`

    ------------------------------------------------------------------------

        public class RuleAnalysisCompatibleDelegatingActionGraphBuilder
        extends AbstractActionGraphBuilder
        implements RuleAnalysisGraph

    ::: block
    An
    [`ActionGraphBuilder`](../../ActionGraphBuilder.html "interface in com.facebook.buck.core.rules")
    that manages both rule analysis computation and the legacy action
    graph construction.
    This builder delegates to the new
    [`RuleAnalysisGraph`](../../analysis/computation/RuleAnalysisGraph.html "interface in com.facebook.buck.core.rules.analysis.computation")
    and
    [`ActionGraphBuilder`](../../ActionGraphBuilder.html "interface in com.facebook.buck.core.rules")
    as appropriate depending on the rule that is requested.

    It satisfies the API of both computations to provide compatibility
    between them
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                     Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `RuleAnalysisCompatibleDelegatingActionGraphBuilder​(TargetNodeToBuildRuleTransformer buildRuleGenerator,                                                   java.util.function.Function<TargetNodeToBuildRuleTransformer,​ActionGraphBuilder> delegateBuilderConstructor,                                                   RuleAnalysisGraph delegateRuleAnalysisComputation)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `<T                   | `add                  | ::: block             |
        |  extends BuildRule>T` | ToIndex​(T buildRule)` | [Deprecate            |
        |                       |                       | d.]{.deprecatedLabel} |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `BuildRule`           | `computeIfAbsen       | ::: block             |
        |                       | t​(BuildTarget target, | Retrieve the          |
        |                       |                 java. | `BuildRule` for the   |
        |                       | util.function.Functio | given `BuildTarget`.  |
        |                       | n<BuildTarget,​BuildRu | :::                   |
        |                       | le> mappingFunction)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `RuleAnalysisResult`  | `get​(RuleAn           | ::: block             |
        |                       | alysisKey lookupKey)` | Finds the             |
        |                       |                       | [`RuleAnal            |
        |                       |                       | ysisResult`](../../an |
        |                       |                       | alysis/RuleAnalysisRe |
        |                       |                       | sult.html "interface  |
        |                       |                       | in com.facebook.buck. |
        |                       |                       | core.rules.analysis") |
        |                       |                       | of the given          |
        |                       |                       | [                     |
        |                       |                       | `RuleAnalysisKey`](.. |
        |                       |                       | /../analysis/RuleAnal |
        |                       |                       | ysisKey.html "class i |
        |                       |                       | n com.facebook.buck.c |
        |                       |                       | ore.rules.analysis"), |
        |                       |                       | starting computation  |
        |                       |                       | as necessary.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `getAll​(Set<RuleAnal  | ::: block             |
        | ommon.collect.Immutab | ysisKey> lookupKeys)` | same as               |
        | leMap<RuleAnalysisKey |                       | [`Rul                 |
        | ,​RuleAnalysisResult>` |                       | eAnalysisGraph.get(Ru |
        |                       |                       | leAnalysisKey)`](../. |
        |                       |                       | ./analysis/computatio |
        |                       |                       | n/RuleAnalysisGraph.h |
        |                       |                       | tml#get(com.facebook. |
        |                       |                       | buck.core.rules.analy |
        |                       |                       | sis.RuleAnalysisKey)) |
        |                       |                       | but for multiple      |
        |                       |                       | [                     |
        |                       |                       | `RuleAnalysisKey`](.. |
        |                       |                       | /../analysis/RuleAnal |
        |                       |                       | ysisKey.html "class i |
        |                       |                       | n com.facebook.buck.c |
        |                       |                       | ore.rules.analysis")s |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<BuildRule>` | `getBuildRules()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Parallelizer`        | `getParallelizer()`   | ::: block             |
        |                       |                       | Returns a             |
        |                       |                       | parallelizer object   |
        |                       |                       | that parallelizes if  |
        |                       |                       | the current           |
        |                       |                       | BuildRuleResolver     |
        |                       |                       | supports parallelism. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<BuildRule>` | `getRuleOptional​(Buil | ::: block             |
        |                       | dTarget buildTarget)` | Returns the           |
        |                       |                       | `BuildRule`           |
        |                       |                       | associated with the   |
        |                       |                       | given `BuildTarget`   |
        |                       |                       | if it is already      |
        |                       |                       | present.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<BuildRule>` | `getSuccessfullyCon   |                       |
        |                       | structedBuildRules()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `invalidate()`        | ::: block             |
        |                       |                       | Invalidates this      |
        |                       |                       | object.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `<T> Optional<T>`     | `requireMetad         | ::: block             |
        |                       | ata​(BuildTarget targe | Retrieve a piece of   |
        |                       | t,                Cla | metadata for a        |
        |                       | ss<T> metadataClass)` | target.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `BuildRule`           | `requireRule          | ::: block             |
        |                       | ​(BuildTarget target)` | Retrieve the          |
        |                       |                       | `BuildRule` for the   |
        |                       |                       | given `BuildTarget`.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.ut | `requireRuleFuture    |                       |
        | il.concurrent.Listena | ​(BuildTarget target)` |                       |
        | bleFuture<BuildRule>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4
        .tableTab}[[Deprecated
        Methods](javascript:show(32);)[ ]{.tabEnd}]{#t6 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.resolver.impl.AbstractActionGraphBuilder}

            ### Methods inherited from class com.facebook.buck.core.rules.resolver.impl.[AbstractActionGraphBuilder](AbstractActionGraphBuilder.html "class in com.facebook.buck.core.rules.resolver.impl")

            `checkRuleIsBuiltForCorrectTarget, computeAllIfAbsent, requireAllRules`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRuleResolver}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRuleResolver](../../impl/AbstractBuildRuleResolver.html "class in com.facebook.buck.core.rules.impl")

            `filterBuildRuleInputs, filterBuildRuleInputs, filterBuildRuleInputs, filterBuildRuleInputs, getAllRules, getRule, getRule, getRule, getRuleOptionalWithType, getRuleWithType, getSourcePathResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.BuildRuleResolver}

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRuleResolver](../../BuildRuleResolver.html "interface in com.facebook.buck.core.rules")

            `getAllRules, getRule, getRuleOptionalWithType, getRuleWithType`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.SourcePathRuleFinder}

            ### Methods inherited from interface com.facebook.buck.core.rules.[SourcePathRuleFinder](../../SourcePathRuleFinder.html "interface in com.facebook.buck.core.rules")

            `filterBuildRuleInputs, filterBuildRuleInputs, filterBuildRuleInputs, filterBuildRuleInputs, getRule, getRule, getSourcePathResolver`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.rules.transformer.TargetNodeToBuildRuleTransformer,java.util.function.Function,com.facebook.buck.core.rules.analysis.computation.RuleAnalysisGraph)}

        -   #### RuleAnalysisCompatibleDelegatingActionGraphBuilder

                public RuleAnalysisCompatibleDelegatingActionGraphBuilder​(TargetNodeToBuildRuleTransformer buildRuleGenerator,
                                                                          java.util.function.Function<TargetNodeToBuildRuleTransformer,​ActionGraphBuilder> delegateBuilderConstructor,
                                                                          RuleAnalysisGraph delegateRuleAnalysisComputation)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildRules()}

        -   #### getBuildRules

            ``` methodSignature
            public Iterable<BuildRule> getBuildRules()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildRules` in interface `ActionGraphBuilder`

            [Returns:]{.returnLabel}
            :   an unmodifiable view of the rules in the index. Throws
                an exception if construction fails for any rule.

        []{#getSuccessfullyConstructedBuildRules()}

        -   #### getSuccessfullyConstructedBuildRules

            ``` methodSignature
            public Iterable<BuildRule> getSuccessfullyConstructedBuildRules()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSuccessfullyConstructedBuildRules` in
                interface `ActionGraphBuilder`

            [Returns:]{.returnLabel}
            :   an unmodifiable view of the successfully constructed
                (i.e. didn\'t throw an exception during construction)
                rules in the index. Does not throw an exception if
                construction failed for any rule.

        []{#computeIfAbsent(com.facebook.buck.core.model.BuildTarget,java.util.function.Function)}

        -   #### computeIfAbsent

            ``` methodSignature
            public BuildRule computeIfAbsent​(BuildTarget target,
                                             java.util.function.Function<BuildTarget,​BuildRule> mappingFunction)
            ```

            ::: block
            [Description copied from
            interface: `ActionGraphBuilder`]{.descfrmTypeLabel}
            :::

            ::: block
            Retrieve the `BuildRule` for the given `BuildTarget`. If no
            rules are associated with the target, compute the rule using
            the given supplier and update the mapping.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `computeIfAbsent` in interface `ActionGraphBuilder`

            [Parameters:]{.paramLabel}
            :   `target` - target with which the BuildRule is
                associated.
            :   `mappingFunction` - function to compute the rule.

            [Returns:]{.returnLabel}
            :   the current value associated with the rule

        []{#requireRule(com.facebook.buck.core.model.BuildTarget)}

        -   #### requireRule

            ``` methodSignature
            public BuildRule requireRule​(BuildTarget target)
            ```

            ::: block
            [Description copied from
            interface: `ActionGraphBuilder`]{.descfrmTypeLabel}
            :::

            ::: block
            Retrieve the `BuildRule` for the given `BuildTarget`. If no
            rules are associated with the target, compute it by
            transforming the `TargetNode` associated with this build
            target using the
            [`TargetNodeToBuildRuleTransformer`](../../transformer/TargetNodeToBuildRuleTransformer.html "interface in com.facebook.buck.core.rules.transformer")
            associated with this instance.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `requireRule` in interface `ActionGraphBuilder`

        []{#requireRuleFuture(com.facebook.buck.core.model.BuildTarget)}

        -   #### requireRuleFuture

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<BuildRule> requireRuleFuture​(BuildTarget target)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `requireRuleFuture` in interface `ActionGraphBuilder`

            [Overrides:]{.overrideSpecifyLabel}
            :   `requireRuleFuture` in
                class `AbstractActionGraphBuilder`

        []{#requireMetadata(com.facebook.buck.core.model.BuildTarget,java.lang.Class)}

        -   #### requireMetadata

            ``` methodSignature
            public <T> Optional<T> requireMetadata​(BuildTarget target,
                                                   Class<T> metadataClass)
            ```

            ::: block
            [Description copied from
            interface: `ActionGraphBuilder`]{.descfrmTypeLabel}
            :::

            ::: block
            Retrieve a piece of metadata for a target. This metadata is
            computed via
            [`MetadataProvidingDescription.createMetadata(com.facebook.buck.core.model.BuildTarget, com.facebook.buck.core.rules.ActionGraphBuilder, com.facebook.buck.core.cell.CellPathResolver, T, java.util.Optional<com.google.common.collect.ImmutableMap<com.facebook.buck.core.model.BuildTarget, com.facebook.buck.versions.Version>>, java.lang.Class<U>)`](../../../description/metadata/MetadataProvidingDescription.html#createMetadata(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.cell.CellPathResolver,T,java.util.Optional,java.lang.Class)).
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `requireMetadata` in interface `ActionGraphBuilder`

        []{#addToIndex(com.facebook.buck.core.rules.BuildRule)}
        []{#addToIndex(T)}

        -   #### addToIndex

            ``` methodSignature
            @Deprecated
            public <T extends BuildRule> T addToIndex​(T buildRule)
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            ::: block
            [Description copied from
            interface: `ActionGraphBuilder`]{.descfrmTypeLabel}
            :::

            ::: block
            Adds to the index a mapping from `buildRule`\'s target to
            itself and returns `  buildRule`.
            Please use `computeIfAbsent` instead
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `addToIndex` in interface `ActionGraphBuilder`

        []{#getParallelizer()}

        -   #### getParallelizer

            ``` methodSignature
            public Parallelizer getParallelizer()
            ```

            ::: block
            [Description copied from
            interface: `ActionGraphBuilder`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns a parallelizer object that parallelizes if the
            current BuildRuleResolver supports parallelism.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getParallelizer` in interface `ActionGraphBuilder`

        []{#invalidate()}

        -   #### invalidate

            ``` methodSignature
            public void invalidate()
            ```

            ::: block
            [Description copied from
            interface: `ActionGraphBuilder`]{.descfrmTypeLabel}
            :::

            ::: block
            Invalidates this object. All future calls will throw
            InvalidStateException.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `invalidate` in interface `ActionGraphBuilder`

        []{#getRuleOptional(com.facebook.buck.core.model.BuildTarget)}

        -   #### getRuleOptional

            ``` methodSignature
            public Optional<BuildRule> getRuleOptional​(BuildTarget buildTarget)
            ```

            ::: block
            [Description copied from
            interface: `BuildRuleResolver`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the `BuildRule` associated with the given
            `BuildTarget` if it is already present.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRuleOptional` in interface `BuildRuleResolver`

        []{#get(com.facebook.buck.core.rules.analysis.RuleAnalysisKey)}

        -   #### get

            ``` methodSignature
            public RuleAnalysisResult get​(RuleAnalysisKey lookupKey)
            ```

            ::: block
            [Description copied from
            interface: `RuleAnalysisGraph`]{.descfrmTypeLabel}
            :::

            ::: block
            Finds the
            [`RuleAnalysisResult`](../../analysis/RuleAnalysisResult.html "interface in com.facebook.buck.core.rules.analysis")
            of the given
            [`RuleAnalysisKey`](../../analysis/RuleAnalysisKey.html "class in com.facebook.buck.core.rules.analysis"),
            starting computation as necessary. All dependencies required
            will also be transformed, and cached.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `get` in interface `RuleAnalysisGraph`

            [Parameters:]{.paramLabel}
            :   `lookupKey` - the
                [`RuleAnalysisKey`](../../analysis/RuleAnalysisKey.html "class in com.facebook.buck.core.rules.analysis")
                to find the result for

            [Returns:]{.returnLabel}
            :   the
                [`RuleAnalysisResult`](../../analysis/RuleAnalysisResult.html "interface in com.facebook.buck.core.rules.analysis")
                from analyzing the given
                [`RuleAnalysisKey`](../../analysis/RuleAnalysisKey.html "class in com.facebook.buck.core.rules.analysis")

        []{#getAll(java.util.Set)}

        -   #### getAll

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<RuleAnalysisKey,​RuleAnalysisResult> getAll​(Set<RuleAnalysisKey> lookupKeys)
            ```

            ::: block
            [Description copied from
            interface: `RuleAnalysisGraph`]{.descfrmTypeLabel}
            :::

            ::: block
            same as
            [`RuleAnalysisGraph.get(RuleAnalysisKey)`](../../analysis/computation/RuleAnalysisGraph.html#get(com.facebook.buck.core.rules.analysis.RuleAnalysisKey))
            but for multiple
            [`RuleAnalysisKey`](../../analysis/RuleAnalysisKey.html "class in com.facebook.buck.core.rules.analysis")s
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAll` in interface `RuleAnalysisGraph`
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
