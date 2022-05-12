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

## Class MultiThreadedActionGraphBuilder {#class-multithreadedactiongraphbuilder .title title="Class MultiThreadedActionGraphBuilder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRuleResolver](../../impl/AbstractBuildRuleResolver.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.core.rules.resolver.impl.AbstractActionGraphBuilder](AbstractActionGraphBuilder.html "class in com.facebook.buck.core.rules.resolver.impl")

        -   -   com.facebook.buck.core.rules.resolver.impl.MultiThreadedActionGraphBuilder

::: description
-   

    All Implemented Interfaces:
    :   `ActionGraphBuilder`, `BuildRuleResolver`,
        `SourcePathRuleFinder`

    ------------------------------------------------------------------------

        public class MultiThreadedActionGraphBuilder
        extends AbstractActionGraphBuilder

    ::: block
    Implementation of BuildRuleResolver that supports build rules being
    created in parallel.
    In order to prevent race-conditions and duplicate work, this
    implementation imposes additional semantics for concurrent access:

    -   Rules are stored in futures.
    -   Accessing incomplete rules from the current thread behaves as if
        the rule does not exist. Accessing incomplete rules from other
        threads waits for the rule future to complete.

    The implementation parallelizes work via the parallelizer and when
    it receives a call for multiple things at the same time via
    requireAllRules or computeAllIfAbsent. For all of these cases, it
    basically creates a list of Tasks, schedules them, tries to finish
    them on the current thread and then waiting for them. When a Task is
    scheduled, we submit a job to the executor service to complete that
    task.
    This means that a task that is doing work will only recursively
    process tasks that it has directly asked for (i.e. stack traces will
    look nice). In the case where work is done by another thread, stack
    traces will be captured on that thread and then re-thrown from the
    thread that requested the work.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                        Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `MultiThreadedActionGraphBuilder​(com.google.common.util.concurrent.ListeningExecutorService executor,                                TargetGraph targetGraph,                                ConfigurationRuleRegistry configurationRuleRegistry,                                TargetNodeToBuildRuleTransformer buildRuleGenerator,                                CellProvider cellProvider)`    

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
        | `com.g                | `comput               |                       |
        | oogle.common.collect. | eAllIfAbsent​(com.goog |                       |
        | ImmutableSortedMap<Bu | le.common.collect.Imm |                       |
        | ildTarget,​BuildRule>` | utableMap<BuildTarget |                       |
        |                       | ,​java.util.function.F |                       |
        |                       | unction<BuildTarget,​B |                       |
        |                       | uildRule>> mappings)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildRule`           | `computeIfAbsen       | ::: block             |
        |                       | t​(BuildTarget target, | Retrieve the          |
        |                       |                 java. | `BuildRule` for the   |
        |                       | util.function.Functio | given `BuildTarget`.  |
        |                       | n<BuildTarget,​BuildRu | :::                   |
        |                       | le> mappingFunction)` |                       |
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
        | `com.google.com       | `requireAll           |                       |
        | mon.collect.Immutable | Rules​(Iterable<BuildT |                       |
        | SortedSet<BuildRule>` | arget> buildTargets)` |                       |
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
        | `com.google.common.ut | `requireRuleFuture    | ::: block             |
        | il.concurrent.Listena | ​(BuildTarget target)` | Requires the rule     |
        | bleFuture<BuildRule>` |                       | asynchronously.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4
        .tableTab}[[Deprecated
        Methods](javascript:show(32);)[ ]{.tabEnd}]{#t6 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.resolver.impl.AbstractActionGraphBuilder}

            ### Methods inherited from class com.facebook.buck.core.rules.resolver.impl.[AbstractActionGraphBuilder](AbstractActionGraphBuilder.html "class in com.facebook.buck.core.rules.resolver.impl")

            `checkRuleIsBuiltForCorrectTarget`

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

        []{#<init>(com.google.common.util.concurrent.ListeningExecutorService,com.facebook.buck.core.model.targetgraph.TargetGraph,com.facebook.buck.core.rules.config.registry.ConfigurationRuleRegistry,com.facebook.buck.core.rules.transformer.TargetNodeToBuildRuleTransformer,com.facebook.buck.core.cell.CellProvider)}

        -   #### MultiThreadedActionGraphBuilder

                public MultiThreadedActionGraphBuilder​(com.google.common.util.concurrent.ListeningExecutorService executor,
                                                       TargetGraph targetGraph,
                                                       ConfigurationRuleRegistry configurationRuleRegistry,
                                                       TargetNodeToBuildRuleTransformer buildRuleGenerator,
                                                       CellProvider cellProvider)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildRules()}

        -   #### getBuildRules

            ``` methodSignature
            public Iterable<BuildRule> getBuildRules()
            ```

            [Returns:]{.returnLabel}
            :   an unmodifiable view of the rules in the index. Throws
                an exception if construction fails for any rule.

        []{#getSuccessfullyConstructedBuildRules()}

        -   #### getSuccessfullyConstructedBuildRules

            ``` methodSignature
            public Iterable<BuildRule> getSuccessfullyConstructedBuildRules()
            ```

            [Returns:]{.returnLabel}
            :   an unmodifiable view of the successfully constructed
                (i.e. didn\'t throw an exception during construction)
                rules in the index. Does not throw an exception if
                construction failed for any rule.

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

            [Parameters:]{.paramLabel}
            :   `target` - target with which the BuildRule is
                associated.
            :   `mappingFunction` - function to compute the rule.

            [Returns:]{.returnLabel}
            :   the current value associated with the rule

        []{#requireAllRules(java.lang.Iterable)}

        -   #### requireAllRules

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildRule> requireAllRules​(Iterable<BuildTarget> buildTargets)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `requireAllRules` in interface `ActionGraphBuilder`

            [Overrides:]{.overrideSpecifyLabel}
            :   `requireAllRules` in class `AbstractActionGraphBuilder`

        []{#computeAllIfAbsent(com.google.common.collect.ImmutableMap)}

        -   #### computeAllIfAbsent

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedMap<BuildTarget,​BuildRule> computeAllIfAbsent​(com.google.common.collect.ImmutableMap<BuildTarget,​java.util.function.Function<BuildTarget,​BuildRule>> mappings)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `computeAllIfAbsent` in interface `ActionGraphBuilder`

            [Overrides:]{.overrideSpecifyLabel}
            :   `computeAllIfAbsent` in
                class `AbstractActionGraphBuilder`

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

        []{#requireRuleFuture(com.facebook.buck.core.model.BuildTarget)}

        -   #### requireRuleFuture

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<BuildRule> requireRuleFuture​(BuildTarget target)
            ```

            ::: block
            Requires the rule asynchronously. This isn\'t part of the
            ActionGraphBuilder interface and so is only used in places
            where we know we have a multithreaded one.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `requireRuleFuture` in interface `ActionGraphBuilder`

            [Overrides:]{.overrideSpecifyLabel}
            :   `requireRuleFuture` in
                class `AbstractActionGraphBuilder`

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
            Please use `computeIfAbsent` instead
            :::

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
