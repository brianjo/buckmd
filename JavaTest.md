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
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Class JavaTest {#class-javatest .title title="Class JavaTest"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps](../../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

        -   -   com.facebook.buck.jvm.java.JavaTest

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `ExportDependencies`, `HasDeclaredAndExtraDeps`,
        `HasPostBuildSteps`, `HasRuntimeDeps`, `BuildRule`,
        `HasNameAndType`, `ExternalTestRunnerRule`, `TestRule`,
        `HasClasspathEntries`, `Comparable<BuildRule>`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `RobolectricTest`

    ------------------------------------------------------------------------

        public class JavaTest
        extends AbstractBuildRuleWithDeclaredAndExtraDeps
        implements TestRule, HasClasspathEntries, HasRuntimeDeps, HasPostBuildSteps, ExternalTestRunnerRule, ExportDependencies
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type     Class                                           Description
          --------------------- ----------------------------------------------- -------------
          `static interface `   `JavaTest.AdditionalClasspathEntriesProvider`    

          : Nested Classes[ ]{.tabEnd}

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.core.test.rule.TestRule}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.core.test.rule.[TestRule](../../core/test/rule/TestRule.html "interface in com.facebook.buck.core.test.rule")

            `TestRule.TestReportingCallback`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                             Description
          ------------------- --------------------------------- -------------
          `static Flavor`     `COMPILED_TESTS_LIBRARY_FLAVOR`    

          : Fields[ ]{.tabEnd}

        -   []{#fields.inherited.from.class.com.facebook.buck.core.test.rule.TestRule}

            ### Fields inherited from interface com.facebook.buck.core.test.rule.[TestRule](../../core/test/rule/TestRule.html "interface in com.facebook.buck.core.test.rule")

            `NOOP_REPORTING_CALLBACK`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `JavaTest​(BuildTarget buildTarget,         ProjectFilesystem projectFilesystem,         BuildRuleParams params,         JavaLibrary compiledTestsLibrary,         Optional<JavaTest.AdditionalClasspathEntriesProvider> additionalClasspathEntriesProvider,         Set<String> labels,         Set<String> contacts,         TestType testType,         String targetLevel,         Tool javaRuntimeLauncher,         List<Arg> vmArgs,         Map<String,​String> nativeLibsEnvironment,         Optional<Long> testRuleTimeoutMs,         Optional<Long> testCaseTimeoutMs,         com.google.common.collect.ImmutableMap<String,​Arg> env,         boolean runTestSeparately,         ForkMode forkMode,         Optional<Level> stdOutLogLevel,         Optional<Level> stdErrLogLevel,         Optional<SourcePath> unbundledResourcesRoot)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected void`      | `                     |                       |
        |                       | addPreTestSteps​(Build |                       |
        |                       | Context buildContext, |                       |
        |                       |                 com.g |                       |
        |                       | oogle.common.collect. |                       |
        |                       | ImmutableList.Builder |                       |
        |                       | <Step> stepsBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ForkMode`            | `forkMode()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected com        | `getBo                |                       |
        | .google.common.collec | otClasspathEntries()` |                       |
        | t.ImmutableSet<Path>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.                 | `                     |                       |
        | google.common.collect | getBuildSteps​(BuildCo |                       |
        | .ImmutableList<Step>` | ntext context,        |                       |
        |                       |        BuildableConte |                       |
        |                       | xt buildableContext)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `JavaLibrary`         | `getCo                | ::: block             |
        |                       | mpiledTestsLibrary()` | Returns the           |
        |                       |                       | underlying java       |
        |                       |                       | library containing    |
        |                       |                       | the compiled tests.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.g                | `getContacts()`       |                       |
        | oogle.common.collect. |                       |                       |
        | ImmutableSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getExportedDeps()`   |                       |
        | SortedSet<BuildRule>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getEx                |                       |
        | SortedSet<BuildRule>` | portedProvidedDeps()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ExternalTestSpec`    | `getExternalTestRunn  |                       |
        |                       | erSpec​(ExecutionConte |                       |
        |                       | xt executionContext,  |                       |
        |                       |                       |                       |
        |                       |     TestRunningOption |                       |
        |                       | s options,            |                       |
        |                       |                BuildC |                       |
        |                       | ontext buildContext)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getI                 | ::: block             |
        | e.common.collect.Immu | mmediateClasspaths()` | Returns the           |
        | tableSet<SourcePath>` |                       | classpaths for only   |
        |                       |                       | this rule, not its    |
        |                       |                       | deps.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.g                | `getLabels()`         |                       |
        | oogle.common.collect. |                       |                       |
        | ImmutableSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `g                    |                       |
        | e.common.collect.Immu | etOutputClasspaths()` |                       |
        | tableSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getPathToT           |                       |
        |                       | estOutputDirectory()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.                 | `get                  |                       |
        | google.common.collect | PostBuildSteps​(BuildC |                       |
        | .ImmutableList<Step>` | ontext buildContext)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected com        | `getRu                |                       |
        | .google.common.collec | ntimeClasspath​(BuildC |                       |
        | t.ImmutableSet<Path>` | ontext buildContext)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `java.util.stream     | `getRuntime           |                       |
        | .Stream<BuildTarget>` | Deps​(BuildRuleResolve |                       |
        |                       | r buildRuleResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `get                  |                       |
        |                       | SourcePathToOutput()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getTrans             |                       |
        | .common.collect.Immut | itiveClasspathDeps()` |                       |
        | ableSet<JavaLibrary>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getTr                |                       |
        | e.common.collect.Immu | ansitiveClasspaths()` |                       |
        | tableSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `C                    | `interpretT           |                       |
        | allable<TestResults>` | estResults​(ExecutionC |                       |
        |                       | ontext context,       |                       |
        |                       |                Source |                       |
        |                       | PathResolverAdapter p |                       |
        |                       | athResolver,          |                       |
        |                       |             boolean i |                       |
        |                       | sUsingTestSelectors)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected void`      | `onAmendVmArgs​(com.go | ::: block             |
        |                       | ogle.common.collect.I | Override this method  |
        |                       | mmutableList.Builder< | if you need to amend  |
        |                       | String> vmArgsBuilder | vm args.              |
        |                       | ,              Source | :::                   |
        |                       | PathResolverAdapter p |                       |
        |                       | athResolver,          |                       |
        |                       |      Optional<TargetD |                       |
        |                       | evice> targetDevice)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `onPreTest​(BuildC     |                       |
        |                       | ontext buildContext)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.                 | `runTests​(            | ::: block             |
        | google.common.collect | ExecutionContext exec | Runs the tests        |
        | .ImmutableList<Step>` | utionContext,         | specified by the      |
        |                       |  TestRunningOptions o | \"srcs\" of this      |
        |                       | ptions,         Build | class.                |
        |                       | Context buildContext, | :::                   |
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
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.HasNameAndType}

            ### Methods inherited from interface com.facebook.buck.core.rules.[HasNameAndType](../../core/rules/HasNameAndType.html "interface in com.facebook.buck.core.rules")

            `getType`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#COMPILED_TESTS_LIBRARY_FLAVOR}

        -   #### COMPILED_TESTS_LIBRARY_FLAVOR

                public static final Flavor COMPILED_TESTS_LIBRARY_FLAVOR
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.jvm.core.JavaLibrary,java.util.Optional,java.util.Set,java.util.Set,com.facebook.buck.jvm.java.TestType,java.lang.String,com.facebook.buck.core.toolchain.tool.Tool,java.util.List,java.util.Map,java.util.Optional,java.util.Optional,com.google.common.collect.ImmutableMap,boolean,com.facebook.buck.jvm.java.ForkMode,java.util.Optional,java.util.Optional,java.util.Optional)}

        -   #### JavaTest

                public JavaTest​(BuildTarget buildTarget,
                                ProjectFilesystem projectFilesystem,
                                BuildRuleParams params,
                                JavaLibrary compiledTestsLibrary,
                                Optional<JavaTest.AdditionalClasspathEntriesProvider> additionalClasspathEntriesProvider,
                                Set<String> labels,
                                Set<String> contacts,
                                TestType testType,
                                String targetLevel,
                                Tool javaRuntimeLauncher,
                                List<Arg> vmArgs,
                                Map<String,​String> nativeLibsEnvironment,
                                Optional<Long> testRuleTimeoutMs,
                                Optional<Long> testCaseTimeoutMs,
                                com.google.common.collect.ImmutableMap<String,​Arg> env,
                                boolean runTestSeparately,
                                ForkMode forkMode,
                                Optional<Level> stdOutLogLevel,
                                Optional<Level> stdErrLogLevel,
                                Optional<SourcePath> unbundledResourcesRoot)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

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

        []{#getBootClasspathEntries()}

        -   #### getBootClasspathEntries

            ``` methodSignature
            protected com.google.common.collect.ImmutableSet<Path> getBootClasspathEntries()
            ```

        []{#getCompiledTestsLibrary()}

        -   #### getCompiledTestsLibrary

            ``` methodSignature
            public JavaLibrary getCompiledTestsLibrary()
            ```

            ::: block
            Returns the underlying java library containing the compiled
            tests.
            :::

        []{#addPreTestSteps(com.facebook.buck.core.build.context.BuildContext,com.google.common.collect.ImmutableList.Builder)}

        -   #### addPreTestSteps

            ``` methodSignature
            protected void addPreTestSteps​(BuildContext buildContext,
                                           com.google.common.collect.ImmutableList.Builder<Step> stepsBuilder)
            ```

        []{#runTests(com.facebook.buck.core.build.execution.context.ExecutionContext,com.facebook.buck.test.TestRunningOptions,com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.test.rule.TestRule.TestReportingCallback)}

        -   #### runTests

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Step> runTests​(ExecutionContext executionContext,
                                                                          TestRunningOptions options,
                                                                          BuildContext buildContext,
                                                                          TestRule.TestReportingCallback testReportingCallback)
            ```

            ::: block
            Runs the tests specified by the \"srcs\" of this class. If
            this rule transitively depends on other `java_test()` rules,
            then they will be run separately.
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

        []{#onAmendVmArgs(com.google.common.collect.ImmutableList.Builder,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,java.util.Optional)}

        -   #### onAmendVmArgs

            ``` methodSignature
            protected void onAmendVmArgs​(com.google.common.collect.ImmutableList.Builder<String> vmArgsBuilder,
                                         SourcePathResolverAdapter pathResolver,
                                         Optional<TargetDevice> targetDevice)
            ```

            ::: block
            Override this method if you need to amend vm args.
            Subclasses are required to call super.onAmendVmArgs(\...).
            :::

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

        []{#interpretTestResults(com.facebook.buck.core.build.execution.context.ExecutionContext,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,boolean)}

        -   #### interpretTestResults

            ``` methodSignature
            public Callable<TestResults> interpretTestResults​(ExecutionContext context,
                                                              SourcePathResolverAdapter pathResolver,
                                                              boolean isUsingTestSelectors)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `interpretTestResults` in interface `TestRule`

        []{#getBuildSteps(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.build.buildable.context.BuildableContext)}

        -   #### getBuildSteps

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Step> getBuildSteps​(BuildContext context,
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

        []{#getTransitiveClasspaths()}

        -   #### getTransitiveClasspaths

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<SourcePath> getTransitiveClasspaths()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTransitiveClasspaths` in
                interface `HasClasspathEntries`

            [Returns:]{.returnLabel}
            :   Classpath entries for this rule and its dependencies.
                e.g. If the rule represents a java library, then these
                entries will be passed to `javac`\'s `-classpath` flag
                in order to build a jar associated with this rule.

        []{#getTransitiveClasspathDeps()}

        -   #### getTransitiveClasspathDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<JavaLibrary> getTransitiveClasspathDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTransitiveClasspathDeps` in
                interface `HasClasspathEntries`

            [Returns:]{.returnLabel}
            :   A set of rules contributing classpath entries for this
                rule and its dependencies.

        []{#getImmediateClasspaths()}

        -   #### getImmediateClasspaths

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<SourcePath> getImmediateClasspaths()
            ```

            ::: block
            [Description copied from
            interface: `HasClasspathEntries`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the classpaths for only this rule, not its deps.
            Used to generate the value of
            [`HasClasspathEntries.getTransitiveClasspaths()`](../core/HasClasspathEntries.html#getTransitiveClasspaths()).
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getImmediateClasspaths` in
                interface `HasClasspathEntries`

        []{#getOutputClasspaths()}

        -   #### getOutputClasspaths

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<SourcePath> getOutputClasspaths()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getOutputClasspaths` in interface `HasClasspathEntries`

            [Returns:]{.returnLabel}
            :   Classpath entries that this rule will contribute when it
                is used as a dependency. e.g. If the rule represents a
                java library, then these entries must be passed to
                `javac`\'s `-classpath` flag in order to compile rules
                that depend on this rule. This is a superset of
                `getImmediateClasspaths` which also contains the
                classpath entries of any exported deps.

        []{#getExportedDeps()}

        -   #### getExportedDeps

            ``` methodSignature
            public SortedSet<BuildRule> getExportedDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExportedDeps` in interface `ExportDependencies`

        []{#getExportedProvidedDeps()}

        -   #### getExportedProvidedDeps

            ``` methodSignature
            public SortedSet<BuildRule> getExportedProvidedDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExportedProvidedDeps` in
                interface `ExportDependencies`

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

        []{#forkMode()}

        -   #### forkMode

            ``` methodSignature
            public ForkMode forkMode()
            ```

        []{#getRuntimeDeps(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### getRuntimeDeps

            ``` methodSignature
            public java.util.stream.Stream<BuildTarget> getRuntimeDeps​(BuildRuleResolver buildRuleResolver)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRuntimeDeps` in interface `HasRuntimeDeps`

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
                                                              TestRunningOptions options,
                                                              BuildContext buildContext)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExternalTestRunnerSpec` in
                interface `ExternalTestRunnerRule`

        []{#onPreTest(com.facebook.buck.core.build.context.BuildContext)}

        -   #### onPreTest

            ``` methodSignature
            public void onPreTest​(BuildContext buildContext)
                           throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `onPreTest` in interface `ExternalTestRunnerRule`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getPostBuildSteps(com.facebook.buck.core.build.context.BuildContext)}

        -   #### getPostBuildSteps

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Step> getPostBuildSteps​(BuildContext buildContext)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPostBuildSteps` in interface `HasPostBuildSteps`

            [Returns:]{.returnLabel}
            :   a list of
                [`Step`](../../step/Step.html "interface in com.facebook.buck.step")s
                that run after the build regardless of whether this
                build rule actually ran or hit in the cache.

        []{#getRuntimeClasspath(com.facebook.buck.core.build.context.BuildContext)}

        -   #### getRuntimeClasspath

            ``` methodSignature
            protected com.google.common.collect.ImmutableSet<Path> getRuntimeClasspath​(BuildContext buildContext)
            ```

            [Returns:]{.returnLabel}
            :   a set of paths to the files which must be passed as the
                classpath to the java process when this test is executed
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
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
