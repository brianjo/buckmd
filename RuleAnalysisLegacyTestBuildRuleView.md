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
-   [Nested](#nested.class.summary) \| 
-   [Field](#field.summary) \| 
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

## Class RuleAnalysisLegacyTestBuildRuleView {#class-ruleanalysislegacytestbuildruleview .title title="Class RuleAnalysisLegacyTestBuildRuleView"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.core.rules.impl.RuleAnalysisLegacyBuildRuleView](../impl/RuleAnalysisLegacyBuildRuleView.html "class in com.facebook.buck.core.rules.impl")

        -   -   [com.facebook.buck.core.rules.tool.RuleAnalysisLegacyBinaryBuildRuleView](RuleAnalysisLegacyBinaryBuildRuleView.html "class in com.facebook.buck.core.rules.tool")

            -   -   com.facebook.buck.core.rules.tool.RuleAnalysisLegacyTestBuildRuleView

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `HasMultipleOutputs`, `SupportsInputBasedRuleKey`, `BuildRule`,
        `HasNameAndType`, `BinaryBuildRule`, `ExternalTestRunnerRule`,
        `TestRule`, `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class RuleAnalysisLegacyTestBuildRuleView
        extends RuleAnalysisLegacyBinaryBuildRuleView
        implements TestRule, ExternalTestRunnerRule

    ::: block
    As
    [`RuleAnalysisLegacyBuildRuleView`](../impl/RuleAnalysisLegacyBuildRuleView.html "class in com.facebook.buck.core.rules.impl"),
    but also implements
    [`TestRule`](../../test/rule/TestRule.html "interface in com.facebook.buck.core.test.rule")
    so that this rule can be run by `buck test`
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.core.test.rule.TestRule}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.core.test.rule.[TestRule](../../test/rule/TestRule.html "interface in com.facebook.buck.core.test.rule")

            `TestRule.TestReportingCallback`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.core.test.rule.TestRule}

            ### Fields inherited from interface com.facebook.buck.core.test.rule.[TestRule](../../test/rule/TestRule.html "interface in com.facebook.buck.core.test.rule")

            `NOOP_REPORTING_CALLBACK`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `RuleAnalysisLegacyTestBuild      | ::: block                         |
        | RuleView​(String type,             | Create an instance of             |
        |                         BuildTarg | [`RuleAnalysisLegacyTestBui       |
        | et buildTarget,                   | ldRuleView`](RuleAnalysisLegacyTe |
        |                   Optional<Action | stBuildRuleView.html "class in co |
        | > action,                         | m.facebook.buck.core.rules.tool") |
        |             BuildRuleResolver rul | :::                               |
        | eResolver,                        |                                   |
        |              ProjectFilesystem pr |                                   |
        | ojectFilesystem,                  |                                   |
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
        | `com.g                | `getContacts()`       |                       |
        | oogle.common.collect. |                       |                       |
        | ImmutableSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ExternalTestSpec`    | `getExtern            |                       |
        |                       | alTestRunnerSpec​(Exec |                       |
        |                       | utionContext executio |                       |
        |                       | nContext,             |                       |
        |                       |               TestRun |                       |
        |                       | ningOptions testRunni |                       |
        |                       | ngOptions,            |                       |
        |                       |                BuildC |                       |
        |                       | ontext buildContext)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.g                | `getLabels()`         |                       |
        | oogle.common.collect. |                       |                       |
        | ImmutableSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getPathToT           |                       |
        |                       | estOutputDirectory()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `C                    | `interpretTestResult  |                       |
        | allable<TestResults>` | s​(ExecutionContext ex |                       |
        |                       | ecutionContext,       |                       |
        |                       |                Source |                       |
        |                       | PathResolverAdapter p |                       |
        |                       | athResolver,          |                       |
        |                       |             boolean i |                       |
        |                       | sUsingTestSelectors)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.                 | `runTests​(            | ::: block             |
        | google.common.collect | ExecutionContext exec | Returns the commands  |
        | .ImmutableList<Step>` | utionContext,         | required to run the   |
        |                       |  TestRunningOptions o | tests.                |
        |                       | ptions,         Build | :::                   |
        |                       | Context buildContext, |                       |
        |                       |          TestRule.Tes |                       |
        |                       | tReportingCallback te |                       |
        |                       | stReportingCallback)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `runTestSeparately()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `supp                 |                       |
        |                       | ortsStreamingTests()` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.tool.RuleAnalysisLegacyBinaryBuildRuleView}

            ### Methods inherited from class com.facebook.buck.core.rules.tool.[RuleAnalysisLegacyBinaryBuildRuleView](RuleAnalysisLegacyBinaryBuildRuleView.html "class in com.facebook.buck.core.rules.tool")

            `getExecutableCommand`

        ```{=html}
        <!-- -->
        ```
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
        -   []{#methods.inherited.from.class.com.facebook.buck.core.test.rule.ExternalTestRunnerRule}

            ### Methods inherited from interface com.facebook.buck.core.test.rule.[ExternalTestRunnerRule](../../test/rule/ExternalTestRunnerRule.html "interface in com.facebook.buck.core.test.rule")

            `onPreTest`

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

        -   #### RuleAnalysisLegacyTestBuildRuleView

                public RuleAnalysisLegacyTestBuildRuleView​(String type,
                                                           BuildTarget buildTarget,
                                                           Optional<Action> action,
                                                           BuildRuleResolver ruleResolver,
                                                           ProjectFilesystem projectFilesystem,
                                                           ProviderInfoCollection providerInfoCollection)

            ::: block
            Create an instance of
            [`RuleAnalysisLegacyTestBuildRuleView`](RuleAnalysisLegacyTestBuildRuleView.html "class in com.facebook.buck.core.rules.tool")
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
                does not contain an instance of both
                [`RunInfo`](../providers/lib/RunInfo.html "class in com.facebook.buck.core.rules.providers.lib")
                and
                [`TestInfo`](../providers/lib/TestInfo.html "class in com.facebook.buck.core.rules.providers.lib")
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#runTests(com.facebook.buck.core.build.execution.context.ExecutionContext,com.facebook.buck.test.TestRunningOptions,com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.test.rule.TestRule.TestReportingCallback)}

        -   #### runTests

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Step> runTests​(ExecutionContext executionContext,
                                                                          TestRunningOptions options,
                                                                          BuildContext buildContext,
                                                                          TestRule.TestReportingCallback testReportingCallback)
            ```

            ::: block
            [Description copied from
            interface: `TestRule`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the commands required to run the tests.
            **Note:** This method may be run without
            [`BuildEngine.build(com.facebook.buck.core.build.engine.BuildEngineBuildContext,  ExecutionContext, BuildRule)`](../../build/engine/BuildEngine.html#build(com.facebook.buck.core.build.engine.BuildEngineBuildContext,com.facebook.buck.core.build.execution.context.ExecutionContext,com.facebook.buck.core.rules.BuildRule))
            having been run. This happens if the user has built \[and
            ran\] the test previously and then re-runs it using the
            `--debug` flag.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `runTests` in interface `TestRule`

            [Parameters:]{.paramLabel}
            :   `executionContext` - Provides context for creating
                [`Step`](../../../step/Step.html "interface in com.facebook.buck.step")s.
            :   `options` - The runtime testing options.
            :   `buildContext` - A SourcePathResolverAdapter from the
                build.

            [Returns:]{.returnLabel}
            :   the commands required to run the tests

        []{#interpretTestResults(com.facebook.buck.core.build.execution.context.ExecutionContext,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,boolean)}

        -   #### interpretTestResults

            ``` methodSignature
            public Callable<TestResults> interpretTestResults​(ExecutionContext executionContext,
                                                              SourcePathResolverAdapter pathResolver,
                                                              boolean isUsingTestSelectors)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `interpretTestResults` in interface `TestRule`

        []{#getLabels()}

        -   #### getLabels

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<String> getLabels()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLabels` in interface `TestRule`

            [Returns:]{.returnLabel}
            :   The set of labels for this build rule.

        []{#getContacts()}

        -   #### getContacts

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<String> getContacts()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getContacts` in interface `TestRule`

            [Returns:]{.returnLabel}
            :   The set of email addresses to act as contact points for
                this test.

        []{#getPathToTestOutputDirectory()}

        -   #### getPathToTestOutputDirectory

            ``` methodSignature
            public Path getPathToTestOutputDirectory()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPathToTestOutputDirectory` in interface `TestRule`

            [Returns:]{.returnLabel}
            :   The relative path to the output directory of the test
                rule.

        []{#runTestSeparately()}

        -   #### runTestSeparately

            ``` methodSignature
            public boolean runTestSeparately()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `runTestSeparately` in interface `TestRule`

            [Returns:]{.returnLabel}
            :   true if the test should run by itself when no other
                tests are run, false otherwise.

        []{#supportsStreamingTests()}

        -   #### supportsStreamingTests

            ``` methodSignature
            public boolean supportsStreamingTests()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `supportsStreamingTests` in interface `TestRule`

            [Returns:]{.returnLabel}
            :   true if calling `runTests()` on this rule invokes the
                callbacks in `      testReportingCallback` as the tests
                run, false otherwise.

        []{#getExternalTestRunnerSpec(com.facebook.buck.core.build.execution.context.ExecutionContext,com.facebook.buck.test.TestRunningOptions,com.facebook.buck.core.build.context.BuildContext)}

        -   #### getExternalTestRunnerSpec

            ``` methodSignature
            public ExternalTestSpec getExternalTestRunnerSpec​(ExecutionContext executionContext,
                                                              TestRunningOptions testRunningOptions,
                                                              BuildContext buildContext)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExternalTestRunnerSpec` in
                interface `ExternalTestRunnerRule`
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
-   [Nested](#nested.class.summary) \| 
-   [Field](#field.summary) \| 
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
