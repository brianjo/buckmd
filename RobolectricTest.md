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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Class RobolectricTest {#class-robolectrictest .title title="Class RobolectricTest"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps](../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

        -   -   [com.facebook.buck.jvm.java.JavaTest](../jvm/java/JavaTest.html "class in com.facebook.buck.jvm.java")

            -   -   com.facebook.buck.android.RobolectricTest

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `ExportDependencies`, `HasDeclaredAndExtraDeps`,
        `HasPostBuildSteps`, `HasRuntimeDeps`, `BuildRule`,
        `HasNameAndType`, `ExternalTestRunnerRule`, `TestRule`,
        `HasClasspathEntries`, `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class RobolectricTest
        extends JavaTest
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.jvm.java.JavaTest}

            ### Nested classes/interfaces inherited from class com.facebook.buck.jvm.java.[JavaTest](../jvm/java/JavaTest.html "class in com.facebook.buck.jvm.java")

            `JavaTest.AdditionalClasspathEntriesProvider`

        ```{=html}
        <!-- -->
        ```
        -   []{#nested.classes.inherited.from.class.com.facebook.buck.core.test.rule.TestRule}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.core.test.rule.[TestRule](../core/test/rule/TestRule.html "interface in com.facebook.buck.core.test.rule")

            `TestRule.TestReportingCallback`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.jvm.java.JavaTest}

            ### Fields inherited from class com.facebook.buck.jvm.java.[JavaTest](../jvm/java/JavaTest.html "class in com.facebook.buck.jvm.java")

            `COMPILED_TESTS_LIBRARY_FLAVOR`

        ```{=html}
        <!-- -->
        ```
        -   []{#fields.inherited.from.class.com.facebook.buck.core.test.rule.TestRule}

            ### Fields inherited from interface com.facebook.buck.core.test.rule.[TestRule](../core/test/rule/TestRule.html "interface in com.facebook.buck.core.test.rule")

            `NOOP_REPORTING_CALLBACK`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   Description
          -------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `protected `   `RobolectricTest​(BuildTarget buildTarget,                ProjectFilesystem projectFilesystem,                BuildRuleParams buildRuleParams,                AndroidPlatformTarget androidPlatformTarget,                JavaLibrary compiledTestsLibrary,                Set<String> labels,                Set<String> contacts,                TestType testType,                String targetLevel,                List<Arg> vmArgs,                Map<String,​String> nativeLibsEnvironment,                Optional<DummyRDotJava> optionalDummyRDotJava,                Optional<UnitTestOptions> unitTestOptions,                Optional<Long> testRuleTimeoutMs,                Optional<Long> testCaseTimeoutMs,                com.google.common.collect.ImmutableMap<String,​Arg> env,                boolean runTestSeparately,                ForkMode forkMode,                Optional<Level> stdOutLogLevel,                Optional<Level> stdErrLogLevel,                Optional<SourcePath> unbundledResourcesRoot,                Optional<SourcePath> robolectricRuntimeDependency,                Optional<SourcePath> robolectricManifest,                boolean passDirectoriesInFile,                Tool javaRuntimeLauncher)`    

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
        | `protected com        | `getBo                |                       |
        | .google.common.collec | otClasspathEntries()` |                       |
        | t.ImmutableSet<Path>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `java.util.stream     | `getRuntime           |                       |
        | .Stream<BuildTarget>` | Deps​(BuildRuleResolve |                       |
        |                       | r buildRuleResolver)` |                       |
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

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.jvm.java.JavaTest}

            ### Methods inherited from class com.facebook.buck.jvm.java.[JavaTest](../jvm/java/JavaTest.html "class in com.facebook.buck.jvm.java")

            `forkMode, getBuildSteps, getCompiledTestsLibrary, getContacts, getExportedDeps, getExportedProvidedDeps, getExternalTestRunnerSpec, getImmediateClasspaths, getLabels, getOutputClasspaths, getPathToTestOutputDirectory, getPostBuildSteps, getRuntimeClasspath, getSourcePathToOutput, getTransitiveClasspathDeps, getTransitiveClasspaths, interpretTestResults, runTests, runTestSeparately, supportsStreamingTests`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRuleWithDeclaredAndExtraDeps](../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

            `deprecatedGetExtraDeps, getBuildDeps, getDeclaredDeps, getTargetGraphOnlyDeps`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRule}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

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

            ### Methods inherited from interface com.facebook.buck.core.build.action.[BuildEngineAction](../core/build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")

            `getDependencies, getSourcePathOutputs`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.BuildRule}

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRule](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")

            `compareTo, getBuildDeps, getBuildTarget, getFullyQualifiedName, getProjectFilesystem, hasBuildSteps, isCacheable, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.HasNameAndType}

            ### Methods inherited from interface com.facebook.buck.core.rules.[HasNameAndType](../core/rules/HasNameAndType.html "interface in com.facebook.buck.core.rules")

            `getType`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.android.toolchain.AndroidPlatformTarget,com.facebook.buck.jvm.core.JavaLibrary,java.util.Set,java.util.Set,com.facebook.buck.jvm.java.TestType,java.lang.String,java.util.List,java.util.Map,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional,com.google.common.collect.ImmutableMap,boolean,com.facebook.buck.jvm.java.ForkMode,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional,boolean,com.facebook.buck.core.toolchain.tool.Tool)}

        -   #### RobolectricTest

                protected RobolectricTest​(BuildTarget buildTarget,
                                          ProjectFilesystem projectFilesystem,
                                          BuildRuleParams buildRuleParams,
                                          AndroidPlatformTarget androidPlatformTarget,
                                          JavaLibrary compiledTestsLibrary,
                                          Set<String> labels,
                                          Set<String> contacts,
                                          TestType testType,
                                          String targetLevel,
                                          List<Arg> vmArgs,
                                          Map<String,​String> nativeLibsEnvironment,
                                          Optional<DummyRDotJava> optionalDummyRDotJava,
                                          Optional<UnitTestOptions> unitTestOptions,
                                          Optional<Long> testRuleTimeoutMs,
                                          Optional<Long> testCaseTimeoutMs,
                                          com.google.common.collect.ImmutableMap<String,​Arg> env,
                                          boolean runTestSeparately,
                                          ForkMode forkMode,
                                          Optional<Level> stdOutLogLevel,
                                          Optional<Level> stdErrLogLevel,
                                          Optional<SourcePath> unbundledResourcesRoot,
                                          Optional<SourcePath> robolectricRuntimeDependency,
                                          Optional<SourcePath> robolectricManifest,
                                          boolean passDirectoriesInFile,
                                          Tool javaRuntimeLauncher)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBootClasspathEntries()}

        -   #### getBootClasspathEntries

            ``` methodSignature
            protected com.google.common.collect.ImmutableSet<Path> getBootClasspathEntries()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `getBootClasspathEntries` in class `JavaTest`

        []{#addPreTestSteps(com.facebook.buck.core.build.context.BuildContext,com.google.common.collect.ImmutableList.Builder)}

        -   #### addPreTestSteps

            ``` methodSignature
            protected void addPreTestSteps​(BuildContext buildContext,
                                           com.google.common.collect.ImmutableList.Builder<Step> stepsBuilder)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `addPreTestSteps` in class `JavaTest`

        []{#onAmendVmArgs(com.google.common.collect.ImmutableList.Builder,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,java.util.Optional)}

        -   #### onAmendVmArgs

            ``` methodSignature
            protected void onAmendVmArgs​(com.google.common.collect.ImmutableList.Builder<String> vmArgsBuilder,
                                         SourcePathResolverAdapter pathResolver,
                                         Optional<TargetDevice> targetDevice)
            ```

            ::: block
            [Description copied from
            class: `JavaTest`]{.descfrmTypeLabel}
            :::

            ::: block
            Override this method if you need to amend vm args.
            Subclasses are required to call super.onAmendVmArgs(\...).
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `onAmendVmArgs` in class `JavaTest`

        []{#onPreTest(com.facebook.buck.core.build.context.BuildContext)}

        -   #### onPreTest

            ``` methodSignature
            public void onPreTest​(BuildContext buildContext)
                           throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `onPreTest` in interface `ExternalTestRunnerRule`

            [Overrides:]{.overrideSpecifyLabel}
            :   `onPreTest` in class `JavaTest`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getRuntimeDeps(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### getRuntimeDeps

            ``` methodSignature
            public java.util.stream.Stream<BuildTarget> getRuntimeDeps​(BuildRuleResolver buildRuleResolver)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRuntimeDeps` in interface `HasRuntimeDeps`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getRuntimeDeps` in class `JavaTest`
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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
