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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.test.rule](package-summary.html)
:::

## Interface TestXRule {#interface-testxrule .title title="Interface TestXRule"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AllowsNonAnnotatedFields`, `BuildEngineAction`, `BuildRule`,
        `Comparable<BuildRule>`, `ExternalTestRunnerRule`,
        `HasNameAndType`, `HasSupplementaryOutputs`, `TestRule`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AppleTestX`, `GoTestX`, `JavaTestX`, `PythonTestX`,
        `RobolectricTestX`

    ------------------------------------------------------------------------

        public interface TestXRule
        extends TestRule, ExternalTestRunnerRule, HasSupplementaryOutputs

    ::: block
    Marks a rule as implementing the test protocol
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.core.test.rule.TestRule}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.core.test.rule.[TestRule](TestRule.html "interface in com.facebook.buck.core.test.rule")

            `TestRule.TestReportingCallback`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `static String`       | `TEST_BINARY_OUTPUT`  | ::: block             |
        |                       |                       | The named output for  |
        |                       |                       | test rules that maps  |
        |                       |                       | to the location of    |
        |                       |                       | where Buck            |
        |                       |                       | materializes the      |
        |                       |                       | final test binary.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}

        -   []{#fields.inherited.from.class.com.facebook.buck.core.test.rule.TestRule}

            ### Fields inherited from interface com.facebook.buck.core.test.rule.[TestRule](TestRule.html "interface in com.facebook.buck.core.test.rule")

            `NOOP_REPORTING_CALLBACK`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `defa                 | `getExtern            | ::: block             |
        | ult ExternalTestSpec` | alTestRunnerSpec​(Exec | This shouldn\'t be    |
        |                       | utionContext executio | overriden as the      |
        |                       | nContext,             | default               |
        |                       |               TestRun | implementation is     |
        |                       | ningOptions testRunni | sufficient.           |
        |                       | ngOptions,            | :::                   |
        |                       |                BuildC |                       |
        |                       | ontext buildContext)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default SourcePath`  | `getSou               | ::: block             |
        |                       | rcePathToSupplementar | Returns a SourcePath  |
        |                       | yOutput​(String name)` | to a named            |
        |                       |                       | supplementary output, |
        |                       |                       | or null if it does    |
        |                       |                       | not exist.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `C                    | `getSpecs()`          |                       |
        | oercedTestRunnerSpec` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default C            | `interpretTestResult  | ::: block             |
        | allable<TestResults>` | s​(ExecutionContext ex | [Deprecate            |
        |                       | ecutionContext,       | d.]{.deprecatedLabel} |
        |                       |                Source | :::                   |
        |                       | PathResolverAdapter p |                       |
        |                       | athResolver,          |                       |
        |                       |             boolean i |                       |
        |                       | sUsingTestSelectors)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default void`        | `onPreTest​(BuildC     | ::: block             |
        |                       | ontext buildContext)` | [Deprecate            |
        |                       |                       | d.]{.deprecatedLabel} |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default com.         | `runTests​(            | ::: block             |
        | google.common.collect | ExecutionContext exec | [Deprecate            |
        | .ImmutableList<Step>` | utionContext,         | d.]{.deprecatedLabel} |
        |                       |  TestRunningOptions o | :::                   |
        |                       | ptions,         Build |                       |
        |                       | Context buildContext, |                       |
        |                       |          TestRule.Tes |                       |
        |                       | tReportingCallback te |                       |
        |                       | stReportingCallback)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `runTestSeparately()` | ::: block             |
        |                       |                       | [Deprecate            |
        |                       |                       | d.]{.deprecatedLabel} |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default I            | `shouldNotBeCalled()` |                       |
        | llegalStateException` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `supp                 | ::: block             |
        |                       | ortsStreamingTests()` | [Deprecate            |
        |                       |                       | d.]{.deprecatedLabel} |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5
        .tableTab}[[Deprecated
        Methods](javascript:show(32);)[ ]{.tabEnd}]{#t6 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.build.action.BuildEngineAction}

            ### Methods inherited from interface com.facebook.buck.core.build.action.[BuildEngineAction](../../build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")

            `getDependencies, getSourcePathOutputs`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.BuildRule}

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRule](../../rules/BuildRule.html "interface in com.facebook.buck.core.rules")

            `compareTo, getBuildDeps, getBuildSteps, getBuildTarget, getFullyQualifiedName, getProjectFilesystem, getSourcePathToOutput, hasBuildSteps, isCacheable, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.HasNameAndType}

            ### Methods inherited from interface com.facebook.buck.core.rules.[HasNameAndType](../../rules/HasNameAndType.html "interface in com.facebook.buck.core.rules")

            `getType`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.test.rule.TestRule}

            ### Methods inherited from interface com.facebook.buck.core.test.rule.[TestRule](TestRule.html "interface in com.facebook.buck.core.test.rule")

            `getContacts, getLabels, getPathToTestOutputDirectory`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#TEST_BINARY_OUTPUT}

        -   #### TEST_BINARY_OUTPUT

                static final String TEST_BINARY_OUTPUT

            ::: block
            The named output for test rules that maps to the location of
            where Buck materializes the final test binary.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.core.test.rule.TestXRule.TEST_BINARY_OUTPUT)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#shouldNotBeCalled()}

        -   #### shouldNotBeCalled

            ``` methodSignature
            default IllegalStateException shouldNotBeCalled()
            ```

        []{#getSpecs()}

        -   #### getSpecs

            ``` methodSignature
            CoercedTestRunnerSpec getSpecs()
            ```

            [Returns:]{.returnLabel}
            :   the specs from the test protocol defined in BUCK files

        []{#runTests(com.facebook.buck.core.build.execution.context.ExecutionContext,com.facebook.buck.test.TestRunningOptions,com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.test.rule.TestRule.TestReportingCallback)}

        -   #### runTests

            ``` methodSignature
            @Deprecated
            default com.google.common.collect.ImmutableList<Step> runTests​(ExecutionContext executionContext,
                                                                           TestRunningOptions options,
                                                                           BuildContext buildContext,
                                                                           TestRule.TestReportingCallback testReportingCallback)
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            ::: block
            tests are no longer ran by Buck, so test protocol rules
            should not have this.
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
            @Deprecated
            default Callable<TestResults> interpretTestResults​(ExecutionContext executionContext,
                                                               SourcePathResolverAdapter pathResolver,
                                                               boolean isUsingTestSelectors)
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            ::: block
            tests are no longer ran by Buck, and hence we don\'t need to
            interpret the test results
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `interpretTestResults` in interface `TestRule`

        []{#runTestSeparately()}

        -   #### runTestSeparately

            ``` methodSignature
            @Deprecated
            default boolean runTestSeparately()
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            ::: block
            tests are not ran by Buck. This attribute should be on the
            test specs for the test runner to interpret
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `runTestSeparately` in interface `TestRule`

            [Returns:]{.returnLabel}
            :   true if the test should run by itself when no other
                tests are run, false otherwise.

        []{#supportsStreamingTests()}

        -   #### supportsStreamingTests

            ``` methodSignature
            @Deprecated
            default boolean supportsStreamingTests()
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            ::: block
            tests are not ran by Buck. This attribute should be on the
            test specs for the test runner to interpret
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `supportsStreamingTests` in interface `TestRule`

            [Returns:]{.returnLabel}
            :   true if calling `runTests()` on this rule invokes the
                callbacks in `      testReportingCallback` as the tests
                run, false otherwise.

        []{#getExternalTestRunnerSpec(com.facebook.buck.core.build.execution.context.ExecutionContext,com.facebook.buck.test.TestRunningOptions,com.facebook.buck.core.build.context.BuildContext)}

        -   #### getExternalTestRunnerSpec

            ``` methodSignature
            default ExternalTestSpec getExternalTestRunnerSpec​(ExecutionContext executionContext,
                                                               TestRunningOptions testRunningOptions,
                                                               BuildContext buildContext)
            ```

            ::: block
            This shouldn\'t be overriden as the default implementation
            is sufficient. Unfortunately it\'s not trivial to convert
            this to an Abstract class and make this final because rules
            also extend a variety of AbstractBuildRule classes and
            multiple inheritance is not available in Java.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExternalTestRunnerSpec` in
                interface `ExternalTestRunnerRule`

            [Returns:]{.returnLabel}
            :   the test protocol specs.

        []{#onPreTest(com.facebook.buck.core.build.context.BuildContext)}

        -   #### onPreTest

            ``` methodSignature
            @Deprecated
            default void onPreTest​(BuildContext buildContext)
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            ::: block
            since Buck doesn\'t actually run the test, pre test steps
            make no sense.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `onPreTest` in interface `ExternalTestRunnerRule`

        []{#getSourcePathToSupplementaryOutput(java.lang.String)}

        -   #### getSourcePathToSupplementaryOutput

            ``` methodSignature
            @Nullable
            default SourcePath getSourcePathToSupplementaryOutput​(String name)
            ```

            ::: block
            [Description copied from
            interface: `HasSupplementaryOutputs`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns a SourcePath to a named supplementary output, or
            null if it does not exist.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathToSupplementaryOutput` in
                interface `HasSupplementaryOutputs`
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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
