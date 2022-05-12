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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Class JavaTestX {#class-javatestx .title title="Class JavaTestX"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps](../../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

        -   -   com.facebook.buck.jvm.java.JavaTestX

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `ExportDependencies`, `HasDeclaredAndExtraDeps`,
        `HasRuntimeDeps`, `HasSupplementaryOutputs`, `BuildRule`,
        `HasNameAndType`, `ExternalTestRunnerRule`, `TestRule`,
        `TestXRule`, `Comparable<BuildRule>`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `RobolectricTestX`

    ------------------------------------------------------------------------

        public class JavaTestX
        extends AbstractBuildRuleWithDeclaredAndExtraDeps
        implements TestXRule, HasRuntimeDeps, ExternalTestRunnerRule, ExportDependencies

    ::: block
    The new Java Test rule that uses the test protocol to run.
    It cannot be run via buck\'s internal runners
    :::
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

        ```{=html}
        <!-- -->
        ```
        -   []{#fields.inherited.from.class.com.facebook.buck.core.test.rule.TestXRule}

            ### Fields inherited from interface com.facebook.buck.core.test.rule.[TestXRule](../../core/test/rule/TestXRule.html "interface in com.facebook.buck.core.test.rule")

            `TEST_BINARY_OUTPUT`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                           Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `JavaTestX​(BuildTarget buildTarget,          ProjectFilesystem projectFilesystem,          BuildRuleParams params,          JavaBinary compiledTestsBinary,          JavaLibrary compiledTestsLibrary,          Set<String> labels,          Set<String> contacts,          CoercedTestRunnerSpec specs,          List<Arg> vmArg)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.                 | `getBu                |                       |
        | google.common.collect | ildSteps​(BuildContext |                       |
        | .ImmutableList<Step>` |  buildContext,        |                       |
        |                       |        BuildableConte |                       |
        |                       | xt buildableContext)` |                       |
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
        | `protected com.go     | `g                    |                       |
        | ogle.common.collect.I | etJvmArgs​(SourcePathR |                       |
        | mmutableList<String>` | esolverAdapter source |                       |
        |                       | PathResolverAdapter)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.g                | `getLabels()`         |                       |
        | oogle.common.collect. |                       |                       |
        | ImmutableSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getPathToT           |                       |
        |                       | estOutputDirectory()` |                       |
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
        | `SourcePath`          | `getSou               | ::: block             |
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

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.test.rule.TestXRule}

            ### Methods inherited from interface com.facebook.buck.core.test.rule.[TestXRule](../../core/test/rule/TestXRule.html "interface in com.facebook.buck.core.test.rule")

            `getExternalTestRunnerSpec, interpretTestResults, onPreTest, runTests, runTestSeparately, shouldNotBeCalled, supportsStreamingTests`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.jvm.java.JavaBinary,com.facebook.buck.jvm.core.JavaLibrary,java.util.Set,java.util.Set,com.facebook.buck.core.test.rule.CoercedTestRunnerSpec,java.util.List)}

        -   #### JavaTestX

                public JavaTestX​(BuildTarget buildTarget,
                                 ProjectFilesystem projectFilesystem,
                                 BuildRuleParams params,
                                 JavaBinary compiledTestsBinary,
                                 JavaLibrary compiledTestsLibrary,
                                 Set<String> labels,
                                 Set<String> contacts,
                                 CoercedTestRunnerSpec specs,
                                 List<Arg> vmArg)
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
            public com.google.common.collect.ImmutableList<Step> getBuildSteps​(BuildContext buildContext,
                                                                               BuildableContext buildableContext)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildSteps` in interface `BuildRule`

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

        []{#getSourcePathToOutput()}

        -   #### getSourcePathToOutput

            ``` methodSignature
            @Nullable
            public SourcePath getSourcePathToOutput()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in interface `BuildRule`

        []{#getRuntimeDeps(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### getRuntimeDeps

            ``` methodSignature
            public java.util.stream.Stream<BuildTarget> getRuntimeDeps​(BuildRuleResolver buildRuleResolver)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRuntimeDeps` in interface `HasRuntimeDeps`

        []{#getRuntimeClasspath(com.facebook.buck.core.build.context.BuildContext)}

        -   #### getRuntimeClasspath

            ``` methodSignature
            protected com.google.common.collect.ImmutableSet<Path> getRuntimeClasspath​(BuildContext buildContext)
            ```

            [Returns:]{.returnLabel}
            :   a set of paths to the files which must be passed as the
                classpath to the java process when this test is executed

        []{#getJvmArgs(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### getJvmArgs

            ``` methodSignature
            protected com.google.common.collect.ImmutableList<String> getJvmArgs​(SourcePathResolverAdapter sourcePathResolverAdapter)
            ```

            [Returns:]{.returnLabel}
            :   a list of JVM args that should be passed to JVM to run
                the command properly

        []{#getSpecs()}

        -   #### getSpecs

            ``` methodSignature
            public CoercedTestRunnerSpec getSpecs()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSpecs` in interface `TestXRule`

            [Returns:]{.returnLabel}
            :   the specs from the test protocol defined in BUCK files

        []{#getSourcePathToSupplementaryOutput(java.lang.String)}

        -   #### getSourcePathToSupplementaryOutput

            ``` methodSignature
            @Nullable
            public SourcePath getSourcePathToSupplementaryOutput​(String name)
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

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathToSupplementaryOutput` in
                interface `TestXRule`
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
