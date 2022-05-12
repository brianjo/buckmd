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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.impl](package-summary.html)
:::

## Class RuleAnalysisLegacyBuildRuleView {#class-ruleanalysislegacybuildruleview .title title="Class RuleAnalysisLegacyBuildRuleView"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   com.facebook.buck.core.rules.impl.RuleAnalysisLegacyBuildRuleView

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `HasMultipleOutputs`, `SupportsInputBasedRuleKey`, `BuildRule`,
        `HasNameAndType`, `Comparable<BuildRule>`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `RuleAnalysisLegacyBinaryBuildRuleView`

    ------------------------------------------------------------------------

        public class RuleAnalysisLegacyBuildRuleView
        extends AbstractBuildRule
        implements SupportsInputBasedRuleKey, HasMultipleOutputs

    ::: block
    This represents the
    [`RuleAnalysisResult`](../analysis/RuleAnalysisResult.html "interface in com.facebook.buck.core.rules.analysis")
    in the modern action framework as a legacy
    [`BuildRule`](../BuildRule.html "interface in com.facebook.buck.core.rules")
    so that existing architecture can use them.
    TODO(bobyf): figure out how to propagate provider info from here
    TODO(bobyf): make this a
    [`ModernBuildRule`](../../../rules/modern/ModernBuildRule.html "class in com.facebook.buck.rules.modern")
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                       Description
          --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `RuleAnalysisLegacyBuildRuleView​(String type,                                BuildTarget buildTarget,                                Optional<Action> action,                                BuildRuleResolver ruleResolver,                                ProjectFilesystem projectFilesystem,                                ProviderInfoCollection providerInfoCollection)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `                     | `getBuildDeps()`      |                       |
        | SortedSet<BuildRule>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.com       | `                     |                       |
        | mon.collect.Immutable | getBuildSteps​(BuildCo |                       |
        | List<? extends Step>` | ntext context,        |                       |
        |                       |        BuildableConte |                       |
        |                       | xt buildableContext)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getOutputLabels()`   | ::: block             |
        | .common.collect.Immut |                       | returns a set of      |
        | ableSet<OutputLabel>` |                       | [                     |
        |                       |                       | `OutputLabel`](../../ |
        |                       |                       | model/OutputLabel.htm |
        |                       |                       | l "class in com.faceb |
        |                       |                       | ook.buck.core.model") |
        |                       |                       | instances associated  |
        |                       |                       | with this build rule. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `getProviderInfos()`  |                       |
        | oviderInfoCollection` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `get                  |                       |
        |                       | SourcePathToOutput()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.comm      | `getSo                | ::: block             |
        | on.collect.ImmutableS | urcePathToOutput​(Outp | Returns               |
        | ortedSet<SourcePath>` | utLabel outputLabel)` | [`SourcePath`         |
        |                       |                       | ](../../sourcepath/So |
        |                       |                       | urcePath.html "interf |
        |                       |                       | ace in com.facebook.b |
        |                       |                       | uck.core.sourcepath") |
        |                       |                       | instances to the      |
        |                       |                       | outputs associated    |
        |                       |                       | with the given output |
        |                       |                       | label, or `null` if   |
        |                       |                       | the output label does |
        |                       |                       | not exist.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getType()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isCacheable()`       | ::: block             |
        |                       |                       | Whether this          |
        |                       |                       | [`BuildRule`]         |
        |                       |                       | (../BuildRule.html "i |
        |                       |                       | nterface in com.faceb |
        |                       |                       | ook.buck.core.rules") |
        |                       |                       | can be cached.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `updateBuildRul       | ::: block             |
        |                       | eResolver​(BuildRuleRe | Updates the           |
        |                       | solver ruleResolver)` | BuildRuleResolver and |
        |                       |                       | associated objects    |
        |                       |                       | for this build rule.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRule}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRule](AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

            `equals, getBuildTarget, getDependencies, getProjectFilesystem, getSourcePathOutputs, hasBuildSteps, hashCode, injectFields, toString`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.build.action.BuildEngineAction}

            ### Methods inherited from interface com.facebook.buck.core.build.action.[BuildEngineAction](../../build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")

            `getDependencies, getSourcePathOutputs`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.BuildRule}

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRule](../BuildRule.html "interface in com.facebook.buck.core.rules")

            `compareTo, getBuildTarget, getFullyQualifiedName, getProjectFilesystem, hasBuildSteps, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.attr.SupportsInputBasedRuleKey}

            ### Methods inherited from interface com.facebook.buck.core.rules.attr.[SupportsInputBasedRuleKey](../attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr")

            `inputBasedRuleKeyIsEnabled`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.lang.String,com.facebook.buck.core.model.BuildTarget,java.util.Optional,com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.providers.collect.ProviderInfoCollection)}

        -   #### RuleAnalysisLegacyBuildRuleView

                public RuleAnalysisLegacyBuildRuleView​(String type,
                                                       BuildTarget buildTarget,
                                                       Optional<Action> action,
                                                       BuildRuleResolver ruleResolver,
                                                       ProjectFilesystem projectFilesystem,
                                                       ProviderInfoCollection providerInfoCollection)

            [Parameters:]{.paramLabel}
            :   `type` - the type of this
                [`BuildRule`](../BuildRule.html "interface in com.facebook.buck.core.rules")
            :   `buildTarget` - the
                [`BuildTarget`](../../model/BuildTarget.html "class in com.facebook.buck.core.model")
                of this analysis rule
            :   `action` - the action of the result for which we want to
                provide the
                [`BuildRule`](../BuildRule.html "interface in com.facebook.buck.core.rules")
                view
            :   `ruleResolver` - the current
                [`BuildRuleResolver`](../BuildRuleResolver.html "interface in com.facebook.buck.core.rules")
                to query dependent rules
            :   `projectFilesystem` - the filesystem
            :   `providerInfoCollection` - the providers returned by
                this build target
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getType()}

        -   #### getType

            ``` methodSignature
            public String getType()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getType` in interface `HasNameAndType`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getType` in class `AbstractBuildRule`

        []{#getBuildDeps()}

        -   #### getBuildDeps

            ``` methodSignature
            public SortedSet<BuildRule> getBuildDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildDeps` in interface `BuildRule`

            [Returns:]{.returnLabel}

            :   the set of rules that must be built before this rule.
                Normally, this matches the value of the `deps` argument
                for this build rule in the build file in which it was
                defined.

                However, there are special cases where other arguments
                pull in implicit dependencies (e.g., the `keystore`
                argument in `android_binary`). In these cases, the
                implicit dependencies are also included in the set
                returned by this method. The value of the original
                `deps` argument, as defined in the build file, must be
                accessed via a custom getter provided by the build rule.

        []{#getBuildSteps(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.build.buildable.context.BuildableContext)}

        -   #### getBuildSteps

            ``` methodSignature
            public com.google.common.collect.ImmutableList<? extends Step> getBuildSteps​(BuildContext context,
                                                                                         BuildableContext buildableContext)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildSteps` in interface `BuildRule`

        []{#getSourcePathToOutput()}

        -   #### getSourcePathToOutput

            ``` methodSignature
            @Nullable
            public SourcePath getSourcePathToOutput()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in interface `BuildRule`

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in
                interface `HasMultipleOutputs`

        []{#getSourcePathToOutput(com.facebook.buck.core.model.OutputLabel)}

        -   #### getSourcePathToOutput

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<SourcePath> getSourcePathToOutput​(OutputLabel outputLabel)
            ```

            ::: block
            [Description copied from
            interface: `HasMultipleOutputs`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns
            [`SourcePath`](../../sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
            instances to the outputs associated with the given output
            label, or `null` if the output label does not exist. If the
            default output label is given, returns the default outputs
            associated with the rule.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in
                interface `HasMultipleOutputs`

        []{#getOutputLabels()}

        -   #### getOutputLabels

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<OutputLabel> getOutputLabels()
            ```

            ::: block
            [Description copied from
            interface: `HasMultipleOutputs`]{.descfrmTypeLabel}
            :::

            ::: block
            returns a set of
            [`OutputLabel`](../../model/OutputLabel.html "class in com.facebook.buck.core.model")
            instances associated with this build rule.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getOutputLabels` in interface `HasMultipleOutputs`

        []{#isCacheable()}

        -   #### isCacheable

            ``` methodSignature
            public boolean isCacheable()
            ```

            ::: block
            [Description copied from
            interface: `BuildRule`]{.descfrmTypeLabel}
            :::

            ::: block
            Whether this
            [`BuildRule`](../BuildRule.html "interface in com.facebook.buck.core.rules")
            can be cached.
            Uncached build rules are never written out to cache, never
            read from cache, and does not count in cache statistics.
            This rule is useful for artifacts which cannot be easily
            normalized.

            Uncached rules are not always rebuilt, however, as long as
            the existing on-disk representation is up to date. This
            means that these rules can take advantage of
            [`SupportsInputBasedRuleKey`](../attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr")
            to prevent rebuilding.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `isCacheable` in interface `BuildEngineAction`

            [Specified by:]{.overrideSpecifyLabel}
            :   `isCacheable` in interface `BuildRule`

            [Overrides:]{.overrideSpecifyLabel}
            :   `isCacheable` in class `AbstractBuildRule`

        []{#updateBuildRuleResolver(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### updateBuildRuleResolver

            ``` methodSignature
            public void updateBuildRuleResolver​(BuildRuleResolver ruleResolver)
            ```

            ::: block
            [Description copied from
            interface: `BuildRule`]{.descfrmTypeLabel}
            :::

            ::: block
            Updates the BuildRuleResolver and associated objects for
            this build rule.
            Build rules sometimes hold field references to build rule
            resolvers. If this build rule is to be cached, it must
            update its BuildRuleResolver when a new action graph is
            constructed to avoid leaking the entire action graph it was
            originally associated with.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `updateBuildRuleResolver` in interface `BuildRule`

            [Overrides:]{.overrideSpecifyLabel}
            :   `updateBuildRuleResolver` in class `AbstractBuildRule`

        []{#getProviderInfos()}

        -   #### getProviderInfos

            ``` methodSignature
            public ProviderInfoCollection getProviderInfos()
            ```

            [Returns:]{.returnLabel}
            :   the
                [`ProviderInfoCollection`](../providers/collect/ProviderInfoCollection.html "interface in com.facebook.buck.core.rules.providers.collect")
                returned from rule analysis
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
