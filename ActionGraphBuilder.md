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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules](package-summary.html)
:::

## Interface ActionGraphBuilder {#interface-actiongraphbuilder .title title="Interface ActionGraphBuilder"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `BuildRuleResolver`, `SourcePathRuleFinder`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AbstractActionGraphBuilder`, `MultiThreadedActionGraphBuilder`,
        `RuleAnalysisCompatibleDelegatingActionGraphBuilder`

    ------------------------------------------------------------------------

        public interface ActionGraphBuilder
        extends BuildRuleResolver

    ::: block
    Provides methods to interact with the ActionGraph.
    :::
:::

::: summary
-   ::: {.section role="region"}
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
        | `com.google.common.ut | `requireRuleFuture    |                       |
        | il.concurrent.Listena | ​(BuildTarget target)` |                       |
        | bleFuture<BuildRule>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Deprecated
        Methods](javascript:show(32);)[ ]{.tabEnd}]{#t6 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.BuildRuleResolver}

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRuleResolver](BuildRuleResolver.html "interface in com.facebook.buck.core.rules")

            `getAllRules, getRule, getRuleOptional, getRuleOptionalWithType, getRuleWithType`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.SourcePathRuleFinder}

            ### Methods inherited from interface com.facebook.buck.core.rules.[SourcePathRuleFinder](SourcePathRuleFinder.html "interface in com.facebook.buck.core.rules")

            `filterBuildRuleInputs, filterBuildRuleInputs, filterBuildRuleInputs, filterBuildRuleInputs, getRule, getRule, getSourcePathResolver`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildRules()}

        -   #### getBuildRules

            ``` methodSignature
            Iterable<BuildRule> getBuildRules()
            ```

            [Returns:]{.returnLabel}
            :   an unmodifiable view of the rules in the index. Throws
                an exception if construction fails for any rule.

        []{#getSuccessfullyConstructedBuildRules()}

        -   #### getSuccessfullyConstructedBuildRules

            ``` methodSignature
            Iterable<BuildRule> getSuccessfullyConstructedBuildRules()
            ```

            [Returns:]{.returnLabel}
            :   an unmodifiable view of the successfully constructed
                (i.e. didn\'t throw an exception during construction)
                rules in the index. Does not throw an exception if
                construction failed for any rule.

        []{#computeIfAbsent(com.facebook.buck.core.model.BuildTarget,java.util.function.Function)}

        -   #### computeIfAbsent

            ``` methodSignature
            BuildRule computeIfAbsent​(BuildTarget target,
                                      java.util.function.Function<BuildTarget,​BuildRule> mappingFunction)
            ```

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

        []{#requireRule(com.facebook.buck.core.model.BuildTarget)}

        -   #### requireRule

            ``` methodSignature
            BuildRule requireRule​(BuildTarget target)
            ```

            ::: block
            Retrieve the `BuildRule` for the given `BuildTarget`. If no
            rules are associated with the target, compute it by
            transforming the `TargetNode` associated with this build
            target using the
            [`TargetNodeToBuildRuleTransformer`](transformer/TargetNodeToBuildRuleTransformer.html "interface in com.facebook.buck.core.rules.transformer")
            associated with this instance.
            :::

        []{#requireMetadata(com.facebook.buck.core.model.BuildTarget,java.lang.Class)}

        -   #### requireMetadata

            ``` methodSignature
            <T> Optional<T> requireMetadata​(BuildTarget target,
                                            Class<T> metadataClass)
            ```

            ::: block
            Retrieve a piece of metadata for a target. This metadata is
            computed via
            [`MetadataProvidingDescription.createMetadata(com.facebook.buck.core.model.BuildTarget, com.facebook.buck.core.rules.ActionGraphBuilder, com.facebook.buck.core.cell.CellPathResolver, T, java.util.Optional<com.google.common.collect.ImmutableMap<com.facebook.buck.core.model.BuildTarget, com.facebook.buck.versions.Version>>, java.lang.Class<U>)`](../description/metadata/MetadataProvidingDescription.html#createMetadata(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.cell.CellPathResolver,T,java.util.Optional,java.lang.Class)).
            :::

        []{#addToIndex(com.facebook.buck.core.rules.BuildRule)}
        []{#addToIndex(T)}

        -   #### addToIndex

            ``` methodSignature
            @Deprecated
            <T extends BuildRule> T addToIndex​(T buildRule)
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            ::: block
            Adds to the index a mapping from `buildRule`\'s target to
            itself and returns `  buildRule`.
            Please use `computeIfAbsent` instead
            :::

        []{#getParallelizer()}

        -   #### getParallelizer

            ``` methodSignature
            Parallelizer getParallelizer()
            ```

            ::: block
            Returns a parallelizer object that parallelizes if the
            current BuildRuleResolver supports parallelism.
            :::

        []{#invalidate()}

        -   #### invalidate

            ``` methodSignature
            void invalidate()
            ```

            ::: block
            Invalidates this object. All future calls will throw
            InvalidStateException.
            :::

        []{#requireAllRules(java.lang.Iterable)}

        -   #### requireAllRules

            ``` methodSignature
            com.google.common.collect.ImmutableSortedSet<BuildRule> requireAllRules​(Iterable<BuildTarget> buildTargets)
            ```

        []{#computeAllIfAbsent(com.google.common.collect.ImmutableMap)}

        -   #### computeAllIfAbsent

            ``` methodSignature
            com.google.common.collect.ImmutableSortedMap<BuildTarget,​BuildRule> computeAllIfAbsent​(com.google.common.collect.ImmutableMap<BuildTarget,​java.util.function.Function<BuildTarget,​BuildRule>> mappings)
            ```

        []{#requireRuleFuture(com.facebook.buck.core.model.BuildTarget)}

        -   #### requireRuleFuture

            ``` methodSignature
            com.google.common.util.concurrent.ListenableFuture<BuildRule> requireRuleFuture​(BuildTarget target)
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
