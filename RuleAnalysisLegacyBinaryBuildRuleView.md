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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.tool](package-summary.html)
:::

## Class RuleAnalysisLegacyBinaryBuildRuleView {#class-ruleanalysislegacybinarybuildruleview .title title="Class RuleAnalysisLegacyBinaryBuildRuleView"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.core.rules.impl.RuleAnalysisLegacyBuildRuleView](../impl/RuleAnalysisLegacyBuildRuleView.html "class in com.facebook.buck.core.rules.impl")

        -   -   com.facebook.buck.core.rules.tool.RuleAnalysisLegacyBinaryBuildRuleView

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `HasMultipleOutputs`, `SupportsInputBasedRuleKey`, `BuildRule`,
        `HasNameAndType`, `BinaryBuildRule`, `Comparable<BuildRule>`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `RuleAnalysisLegacyTestBuildRuleView`

    ------------------------------------------------------------------------

        public class RuleAnalysisLegacyBinaryBuildRuleView
        extends RuleAnalysisLegacyBuildRuleView
        implements BinaryBuildRule

    ::: block
    As
    [`RuleAnalysisLegacyBuildRuleView`](../impl/RuleAnalysisLegacyBuildRuleView.html "class in com.facebook.buck.core.rules.impl"),
    but also implements
    [`BinaryBuildRule`](BinaryBuildRule.html "interface in com.facebook.buck.core.rules.tool")
    so that this rule can be executable (with `buck run`, in the legacy
    graph, etc)
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `RuleAn                           | ::: block                         |
        | alysisLegacyBinaryBuildRuleView​(S | Create an instance of             |
        | tring type,                       | [`RuleAnalysisLegacyBinaryBuild   |
        |                 BuildTarget build | RuleView`](RuleAnalysisLegacyBina |
        | Target,                           | ryBuildRuleView.html "class in co |
        |             Optional<Action> acti | m.facebook.buck.core.rules.tool") |
        | on,                               | :::                               |
        |         BuildRuleResolver ruleRes |                                   |
        | olver,                            |                                   |
        |            ProjectFilesystem proj |                                   |
        | ectFilesystem,                    |                                   |
        |                    ProviderInfoCo |                                   |
        | llection providerInfoCollection)` |                                   |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Tool`                | `getE                 | ::: block             |
        |                       | xecutableCommand​(Outp | Command to execute    |
        |                       | utLabel outputLabel)` | the output of this    |
        |                       |                       | rule.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.RuleAnalysisLegacyBuildRuleView}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[RuleAnalysisLegacyBuildRuleView](../impl/RuleAnalysisLegacyBuildRuleView.html "class in com.facebook.buck.core.rules.impl")

            `getBuildDeps, getBuildSteps, getOutputLabels, getProviderInfos, getSourcePathToOutput, getSourcePathToOutput, getType, isCacheable, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRule}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRule](../impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

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

            `compareTo, getBuildDeps, getBuildSteps, getBuildTarget, getFullyQualifiedName, getProjectFilesystem, hasBuildSteps, isCacheable, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.HasNameAndType}

            ### Methods inherited from interface com.facebook.buck.core.rules.[HasNameAndType](../HasNameAndType.html "interface in com.facebook.buck.core.rules")

            `getType`

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

        -   #### RuleAnalysisLegacyBinaryBuildRuleView

                public RuleAnalysisLegacyBinaryBuildRuleView​(String type,
                                                             BuildTarget buildTarget,
                                                             Optional<Action> action,
                                                             BuildRuleResolver ruleResolver,
                                                             ProjectFilesystem projectFilesystem,
                                                             ProviderInfoCollection providerInfoCollection)

            ::: block
            Create an instance of
            [`RuleAnalysisLegacyBinaryBuildRuleView`](RuleAnalysisLegacyBinaryBuildRuleView.html "class in com.facebook.buck.core.rules.tool")
            :::

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

            [Throws:]{.throwsLabel}
            :   `IllegalStateException` - if `providerInfoCollection`
                does not contain an instance of
                [`RunInfo`](../providers/lib/RunInfo.html "class in com.facebook.buck.core.rules.providers.lib")
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getExecutableCommand(com.facebook.buck.core.model.OutputLabel)}

        -   #### getExecutableCommand

            ``` methodSignature
            public Tool getExecutableCommand​(OutputLabel outputLabel)
            ```

            ::: block
            [Description copied from
            interface: `BinaryBuildRule`]{.descfrmTypeLabel}
            :::

            ::: block
            Command to execute the output of this rule.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExecutableCommand` in interface `BinaryBuildRule`

            [Parameters:]{.paramLabel}
            :   `outputLabel` - associated with the executable
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
