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
[Package]{.packageLabelInType} [com.facebook.buck.apple](package-summary.html)
:::

## Class AppleTestX {#class-appletestx .title title="Class AppleTestX"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps](../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

        -   -   com.facebook.buck.apple.AppleTestX

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `HasDeclaredAndExtraDeps`, `HasRuntimeDeps`,
        `HasSupplementaryOutputs`, `BuildRule`, `HasNameAndType`,
        `ExternalTestRunnerRule`, `TestRule`, `TestXRule`,
        `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class AppleTestX
        extends AbstractBuildRuleWithDeclaredAndExtraDeps
        implements TestXRule, HasRuntimeDeps

    ::: block
    Represents an apple_test rule that implements the test protocol
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.core.test.rule.TestRule}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.core.test.rule.[TestRule](../core/test/rule/TestRule.html "interface in com.facebook.buck.core.test.rule")

            `TestRule.TestReportingCallback`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.core.test.rule.TestRule}

            ### Fields inherited from interface com.facebook.buck.core.test.rule.[TestRule](../core/test/rule/TestRule.html "interface in com.facebook.buck.core.test.rule")

            `NOOP_REPORTING_CALLBACK`

        ```{=html}
        <!-- -->
        ```
        -   []{#fields.inherited.from.class.com.facebook.buck.core.test.rule.TestXRule}

            ### Fields inherited from interface com.facebook.buck.core.test.rule.[TestXRule](../core/test/rule/TestXRule.html "interface in com.facebook.buck.core.test.rule")

            `TEST_BINARY_OUTPUT`
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
        | `com.g                | `getLabels()`         |                       |
        | oogle.common.collect. |                       |                       |
        | ImmutableSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getPathToT           |                       |
        |                       | estOutputDirectory()` |                       |
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
        | `boolean`             | `isCacheable()`       | ::: block             |
        |                       |                       | not cacheable because |
        |                       |                       | our build steps       |
        |                       |                       | writes out a bunch of |
        |                       |                       | apple configurations  |
        |                       |                       | for the test specific |
        |                       |                       | to the run time.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRuleWithDeclaredAndExtraDeps](../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

            `deprecatedGetExtraDeps, getBuildDeps, getDeclaredDeps, getTargetGraphOnlyDeps`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRule}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

            `equals, getBuildTarget, getDependencies, getProjectFilesystem, getSourcePathOutputs, getType, hasBuildSteps, hashCode, injectFields, toString, updateBuildRuleResolver`

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

            `compareTo, getBuildDeps, getBuildTarget, getFullyQualifiedName, getProjectFilesystem, hasBuildSteps, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.HasNameAndType}

            ### Methods inherited from interface com.facebook.buck.core.rules.[HasNameAndType](../core/rules/HasNameAndType.html "interface in com.facebook.buck.core.rules")

            `getType`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.test.rule.TestXRule}

            ### Methods inherited from interface com.facebook.buck.core.test.rule.[TestXRule](../core/test/rule/TestXRule.html "interface in com.facebook.buck.core.test.rule")

            `getExternalTestRunnerSpec, interpretTestResults, onPreTest, runTests, runTestSeparately, shouldNotBeCalled, supportsStreamingTests`
    :::
:::

::: details
-   ::: {.section role="region"}
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

        []{#getSpecs()}

        -   #### getSpecs

            ``` methodSignature
            public CoercedTestRunnerSpec getSpecs()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSpecs` in interface `TestXRule`

            [Returns:]{.returnLabel}
            :   the specs from the test protocol defined in BUCK files

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

        []{#getRuntimeDeps(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### getRuntimeDeps

            ``` methodSignature
            public java.util.stream.Stream<BuildTarget> getRuntimeDeps​(BuildRuleResolver buildRuleResolver)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRuntimeDeps` in interface `HasRuntimeDeps`

        []{#getBuildSteps(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.build.buildable.context.BuildableContext)}

        -   #### getBuildSteps

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Step> getBuildSteps​(BuildContext buildContext,
                                                                               BuildableContext buildableContext)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildSteps` in interface `BuildRule`

        []{#getSourcePathToOutput()}

        -   #### getSourcePathToOutput

            ``` methodSignature
            public SourcePath getSourcePathToOutput()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in interface `BuildRule`

        []{#isCacheable()}

        -   #### isCacheable

            ``` methodSignature
            public boolean isCacheable()
            ```

            ::: block
            not cacheable because our build steps writes out a bunch of
            apple configurations for the test specific to the run time.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `isCacheable` in interface `BuildEngineAction`

            [Specified by:]{.overrideSpecifyLabel}
            :   `isCacheable` in interface `BuildRule`

            [Overrides:]{.overrideSpecifyLabel}
            :   `isCacheable` in class `AbstractBuildRule`

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
