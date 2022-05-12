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
[Package]{.packageLabelInType} [com.facebook.buck.features.go](package-summary.html)
:::

## Class GoTest {#class-gotest .title title="Class GoTest"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps](../../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

        -   -   com.facebook.buck.features.go.GoTest

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `HasDeclaredAndExtraDeps`, `HasRuntimeDeps`, `BuildRule`,
        `HasNameAndType`, `BinaryBuildRule`, `ExternalTestRunnerRule`,
        `TestRule`, `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class GoTest
        extends AbstractBuildRuleWithDeclaredAndExtraDeps
        implements TestRule, HasRuntimeDeps, ExternalTestRunnerRule, BinaryBuildRule
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.core.test.rule.TestRule}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.core.test.rule.[TestRule](../../core/test/rule/TestRule.html "interface in com.facebook.buck.core.test.rule")

            `TestRule.TestReportingCallback`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.core.test.rule.TestRule}

            ### Fields inherited from interface com.facebook.buck.core.test.rule.[TestRule](../../core/test/rule/TestRule.html "interface in com.facebook.buck.core.test.rule")

            `NOOP_REPORTING_CALLBACK`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `GoTest​(BuildTarget buildTarget,       ProjectFilesystem projectFilesystem,       BuildRuleParams buildRuleParams,       GoBinary testMain,       com.google.common.collect.ImmutableSet<String> labels,       com.google.common.collect.ImmutableSet<String> contacts,       Optional<Long> testRuleTimeoutMs,       com.google.common.collect.ImmutableMap<String,​Arg> env,       boolean runTestsSeparately,       com.google.common.collect.ImmutableSortedSet<SourcePath> resources,       com.facebook.buck.features.go.GoTestCoverStep.Mode coverageMode)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.google.com       | `                     |                       |
        | mon.collect.Immutable | getBuildSteps​(BuildCo |                       |
        | List<? extends Step>` | ntext context,        |                       |
        |                       |        BuildableConte |                       |
        |                       | xt buildableContext)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.g                | `getContacts()`       |                       |
        | oogle.common.collect. |                       |                       |
        | ImmutableSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Tool`                | `getE                 | ::: block             |
        |                       | xecutableCommand​(Outp | Command to execute    |
        |                       | utLabel outputLabel)` | the output of this    |
        |                       |                       | rule.                 |
        |                       |                       | :::                   |
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
        | `protected Path`      | `get                  |                       |
        |                       | PathToTestExitCode()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getPathToT           |                       |
        |                       | estOutputDirectory()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected Path`      | `ge                   |                       |
        |                       | tPathToTestResults()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected Path`      | `getPathToTe          |                       |
        |                       | stWorkingDirectory()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `java.util.stream     | `getRuntime           |                       |
        | .Stream<BuildTarget>` | Deps​(BuildRuleResolve |                       |
        |                       | r buildRuleResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `get                  |                       |
        |                       | SourcePathToOutput()` |                       |
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

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRuleWithDeclaredAndExtraDeps](../../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

            `deprecatedGetExtraDeps, getBuildDeps, getDeclaredDeps, getTargetGraphOnlyDeps`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRule}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRule](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

            `equals, getBuildTarget, getDependencies, getProjectFilesystem, getSourcePathOutputs, getType, hasBuildSteps, hashCode, injectFields, isCacheable, toString, updateBuildRuleResolver`

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

            ### Methods inherited from interface com.facebook.buck.core.build.action.[BuildEngineAction](../../core/build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")

            `getDependencies, getSourcePathOutputs`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.BuildRule}

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRule](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")

            `compareTo, getBuildDeps, getBuildTarget, getFullyQualifiedName, getProjectFilesystem, hasBuildSteps, isCacheable, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.test.rule.ExternalTestRunnerRule}

            ### Methods inherited from interface com.facebook.buck.core.test.rule.[ExternalTestRunnerRule](../../core/test/rule/ExternalTestRunnerRule.html "interface in com.facebook.buck.core.test.rule")

            `onPreTest`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.HasNameAndType}

            ### Methods inherited from interface com.facebook.buck.core.rules.[HasNameAndType](../../core/rules/HasNameAndType.html "interface in com.facebook.buck.core.rules")

            `getType`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.features.go.GoBinary,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableSet,java.util.Optional,com.google.common.collect.ImmutableMap,boolean,com.google.common.collect.ImmutableSortedSet,com.facebook.buck.features.go.GoTestCoverStep.Mode)}

        -   #### GoTest

                public GoTest​(BuildTarget buildTarget,
                              ProjectFilesystem projectFilesystem,
                              BuildRuleParams buildRuleParams,
                              GoBinary testMain,
                              com.google.common.collect.ImmutableSet<String> labels,
                              com.google.common.collect.ImmutableSet<String> contacts,
                              Optional<Long> testRuleTimeoutMs,
                              com.google.common.collect.ImmutableMap<String,​Arg> env,
                              boolean runTestsSeparately,
                              com.google.common.collect.ImmutableSortedSet<SourcePath> resources,
                              com.facebook.buck.features.go.GoTestCoverStep.Mode coverageMode)
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
            [`BuildEngine.build(com.facebook.buck.core.build.engine.BuildEngineBuildContext,  ExecutionContext, BuildRule)`](../../core/build/engine/BuildEngine.html#build(com.facebook.buck.core.build.engine.BuildEngineBuildContext,com.facebook.buck.core.build.execution.context.ExecutionContext,com.facebook.buck.core.rules.BuildRule))
            having been run. This happens if the user has built \[and
            ran\] the test previously and then re-runs it using the
            `--debug` flag.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `runTests` in interface `TestRule`

            [Parameters:]{.paramLabel}
            :   `executionContext` - Provides context for creating
                [`Step`](../../step/Step.html "interface in com.facebook.buck.step")s.
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

        []{#getPathToTestResults()}

        -   #### getPathToTestResults

            ``` methodSignature
            protected Path getPathToTestResults()
            ```

        []{#getPathToTestWorkingDirectory()}

        -   #### getPathToTestWorkingDirectory

            ``` methodSignature
            protected Path getPathToTestWorkingDirectory()
            ```

        []{#getPathToTestExitCode()}

        -   #### getPathToTestExitCode

            ``` methodSignature
            protected Path getPathToTestExitCode()
            ```

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

        []{#getRuntimeDeps(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### getRuntimeDeps

            ``` methodSignature
            public java.util.stream.Stream<BuildTarget> getRuntimeDeps​(BuildRuleResolver buildRuleResolver)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRuntimeDeps` in interface `HasRuntimeDeps`

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
