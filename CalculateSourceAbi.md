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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Class CalculateSourceAbi {#class-calculatesourceabi .title title="Class CalculateSourceAbi"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.rules.modern.ModernBuildRule](../../rules/modern/ModernBuildRule.html "class in com.facebook.buck.rules.modern")\<T\>

        -   -   [com.facebook.buck.rules.modern.PipelinedModernBuildRule](../../rules/modern/PipelinedModernBuildRule.html "class in com.facebook.buck.rules.modern")\<[JavacPipelineState](JavacPipelineState.html "class in com.facebook.buck.jvm.java"),​[CalculateSourceAbi.SourceAbiBuildable](CalculateSourceAbi.SourceAbiBuildable.html "class in com.facebook.buck.jvm.java")\>

            -   -   com.facebook.buck.jvm.java.CalculateSourceAbi

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `InitializableFromDisk<Object>`,
        `SupportsDependencyFileRuleKey`, `SupportsInputBasedRuleKey`,
        `BuildRule`, `HasNameAndType`,
        `SupportsPipelining<JavacPipelineState>`, `CalculateAbi`,
        `HasJavaAbi`, `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class CalculateSourceAbi
        extends PipelinedModernBuildRule<JavacPipelineState,​CalculateSourceAbi.SourceAbiBuildable>
        implements CalculateAbi, InitializableFromDisk<Object>, SupportsDependencyFileRuleKey

    ::: block
    Source Abi calculation. Derives the abi from the source files
    (possibly with access to dependencies).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `CalculateSourceAb    | ::: block             |
        |                       | i.SourceAbiBuildable` | Buildable             |
        |                       |                       | implementation.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                            Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `CalculateSourceAbi​(BuildTarget buildTarget,                   ProjectFilesystem projectFilesystem,                   JarBuildStepsFactory jarBuildStepsFactory,                   SourcePathRuleFinder ruleFinder)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `JavaAbiInfo`         | `getAbiInfo()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildOutpu           | `getBuil              |                       |
        | tInitializer<Object>` | dOutputInitializer()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `java.util.function.P | `getCov               | ::: block             |
        | redicate<SourcePath>` | eredByDepFilePredicat | Returns a predicate   |
        |                       | e​(SourcePathResolverA | that can tell whether |
        |                       | dapter pathResolver)` | a given path is       |
        |                       |                       | covered by dep-file   |
        |                       |                       | or not.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `java.util.function.P | `getExiste            | ::: block             |
        | redicate<SourcePath>` | nceOfInterestPredicat | Returns a predicate   |
        |                       | e​(SourcePathResolverA | that can tell whether |
        |                       | dapter pathResolver)` | the existence of a    |
        |                       |                       | given path may be of  |
        |                       |                       | interest to compiler. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getInputsAf          | ::: block             |
        | .common.collect.Immut | terBuildingLocally​(Bu | Returns a list of     |
        | ableList<SourcePath>` | ildContext context,   | source paths that     |
        |                       |                       | were actually used    |
        |                       |        CellPathResolv | for the rule.         |
        |                       | er cellPathResolver)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Rul                  | `getPi                |                       |
        | ePipelineStateFactory | pelineStateFactory()` |                       |
        | <JavacPipelineState>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SupportsPipelining   | `getPrev              |                       |
        | <JavacPipelineState>` | iousRuleInPipeline()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `get                  |                       |
        |                       | SourcePathToOutput()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getType()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Object`              | `initializeFromDis    |                       |
        |                       | k​(SourcePathResolverA |                       |
        |                       | dapter pathResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `invalidateIniti      |                       |
        |                       | alizeFromDiskState()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `useDepe              |                       |
        |                       | ndencyFileRuleKeys()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `useRulePipelining()` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.rules.modern.PipelinedModernBuildRule}

            ### Methods inherited from class com.facebook.buck.rules.modern.[PipelinedModernBuildRule](../../rules/modern/PipelinedModernBuildRule.html "class in com.facebook.buck.rules.modern")

            `getPipelinedBuildSteps`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.rules.modern.ModernBuildRule}

            ### Methods inherited from class com.facebook.buck.rules.modern.[ModernBuildRule](../../rules/modern/ModernBuildRule.html "class in com.facebook.buck.rules.modern")

            `compareTo, getBuildable, getBuildCellPathFactory, getBuildDeps, getBuildSteps, getOutputPathResolver, getSetupStepsForBuildable, getSourcePath, getSourcePaths, injectFieldsIfNecessary, inputBasedRuleKeyIsEnabled, recordOutputs, recordOutputs, recordOutputs, stepsForBuildable, stepsForBuildable, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRule}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRule](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

            `equals, getBuildTarget, getDependencies, getProjectFilesystem, getSourcePathOutputs, hasBuildSteps, hashCode, injectFields, isCacheable, toString`

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

            `compareTo, getBuildDeps, getBuildSteps, getBuildTarget, getFullyQualifiedName, getProjectFilesystem, hasBuildSteps, isCacheable, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.jvm.core.CalculateAbi}

            ### Methods inherited from interface com.facebook.buck.jvm.core.[CalculateAbi](../core/CalculateAbi.html "interface in com.facebook.buck.jvm.core")

            `getAbiJar`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.jvm.core.HasJavaAbi}

            ### Methods inherited from interface com.facebook.buck.jvm.core.[HasJavaAbi](../core/HasJavaAbi.html "interface in com.facebook.buck.jvm.core")

            `getSourceOnlyAbiJar`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.jvm.java.JarBuildStepsFactory,com.facebook.buck.core.rules.SourcePathRuleFinder)}

        -   #### CalculateSourceAbi

                public CalculateSourceAbi​(BuildTarget buildTarget,
                                          ProjectFilesystem projectFilesystem,
                                          JarBuildStepsFactory jarBuildStepsFactory,
                                          SourcePathRuleFinder ruleFinder)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getSourcePathToOutput()}

        -   #### getSourcePathToOutput

            ``` methodSignature
            public SourcePath getSourcePathToOutput()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in interface `BuildRule`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in
                class `ModernBuildRule<CalculateSourceAbi.SourceAbiBuildable>`

        []{#getAbiInfo()}

        -   #### getAbiInfo

            ``` methodSignature
            public JavaAbiInfo getAbiInfo()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAbiInfo` in interface `HasJavaAbi`

        []{#getType()}

        -   #### getType

            ``` methodSignature
            public String getType()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getType` in interface `HasNameAndType`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getType` in class `AbstractBuildRule`

        []{#invalidateInitializeFromDiskState()}

        -   #### invalidateInitializeFromDiskState

            ``` methodSignature
            public void invalidateInitializeFromDiskState()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `invalidateInitializeFromDiskState` in
                interface `InitializableFromDisk<Object>`

        []{#initializeFromDisk(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### initializeFromDisk

            ``` methodSignature
            public Object initializeFromDisk​(SourcePathResolverAdapter pathResolver)
                                      throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `initializeFromDisk` in
                interface `InitializableFromDisk<Object>`

            [Returns:]{.returnLabel}
            :   an object that has the in-memory data structures that
                need to be populated as a result of executing this
                object\'s steps.

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getBuildOutputInitializer()}

        -   #### getBuildOutputInitializer

            ``` methodSignature
            public BuildOutputInitializer<Object> getBuildOutputInitializer()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildOutputInitializer` in
                interface `InitializableFromDisk<Object>`

        []{#useRulePipelining()}

        -   #### useRulePipelining

            ``` methodSignature
            public boolean useRulePipelining()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `useRulePipelining` in
                interface `SupportsPipelining<JavacPipelineState>`

        []{#getPreviousRuleInPipeline()}

        -   #### getPreviousRuleInPipeline

            ``` methodSignature
            @Nullable
            public SupportsPipelining<JavacPipelineState> getPreviousRuleInPipeline()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPreviousRuleInPipeline` in
                interface `SupportsPipelining<JavacPipelineState>`

        []{#getPipelineStateFactory()}

        -   #### getPipelineStateFactory

            ``` methodSignature
            public RulePipelineStateFactory<JavacPipelineState> getPipelineStateFactory()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPipelineStateFactory` in
                interface `SupportsPipelining<JavacPipelineState>`

        []{#useDependencyFileRuleKeys()}

        -   #### useDependencyFileRuleKeys

            ``` methodSignature
            public boolean useDependencyFileRuleKeys()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `useDependencyFileRuleKeys` in
                interface `SupportsDependencyFileRuleKey`

        []{#getCoveredByDepFilePredicate(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### getCoveredByDepFilePredicate

            ``` methodSignature
            public java.util.function.Predicate<SourcePath> getCoveredByDepFilePredicate​(SourcePathResolverAdapter pathResolver)
            ```

            ::: block
            [Description copied from
            interface: `SupportsDependencyFileRuleKey`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns a predicate that can tell whether a given path is
            covered by dep-file or not. Note that being covered by
            dep-file doesn\'t necessarily mean being present in the
            dep-file. A covered path will only be present if actually
            used and that\'s the core idea of dep-file keys.
            I.e. this predicate should return true only for source paths
            that \*may\* be returned from
            [`SupportsDependencyFileRuleKey.getInputsAfterBuildingLocally(BuildContext, CellPathResolver)`](../../core/rules/attr/SupportsDependencyFileRuleKey.html#getInputsAfterBuildingLocally(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.cell.CellPathResolver)).
            This information is used by the rule key builder to infer
            that inputs \*not\* in this list should be included
            unconditionally in the rule key. Inputs that \*are\* in this
            list should be included in the rule key if and only if they
            are actually being used for the rule. I.e. if they are
            present in the dep-file listed by
            [`SupportsDependencyFileRuleKey.getInputsAfterBuildingLocally(BuildContext, CellPathResolver)`](../../core/rules/attr/SupportsDependencyFileRuleKey.html#getInputsAfterBuildingLocally(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.cell.CellPathResolver)).
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCoveredByDepFilePredicate` in
                interface `SupportsDependencyFileRuleKey`

        []{#getExistenceOfInterestPredicate(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### getExistenceOfInterestPredicate

            ``` methodSignature
            public java.util.function.Predicate<SourcePath> getExistenceOfInterestPredicate​(SourcePathResolverAdapter pathResolver)
            ```

            ::: block
            [Description copied from
            interface: `SupportsDependencyFileRuleKey`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns a predicate that can tell whether the existence of a
            given path may be of interest to compiler. If this predicate
            returns true, the path should be included in the rule key.
            Note that we only care about the existence here. The actual
            content of the file is not relevant.
            The main purpose of this predicate is to support scenarios
            where compiler decides whether to use a file or not solely
            based on its path. Of course, if compiler decides to use the
            file, it should list it in the dep-file in which case both
            the path and the content will be included in the rule key.
            However, relying only on presence in the dep-file for such
            paths is not sufficient. The problem occurs when a new such
            file just gets added, in which case it won\'t be present in
            the dep-file produced in the previous build, and yet if we
            run a local build now the compiler may decide to use it. For
            that reason rule key needs to reflect existence of all such
            files and change when a such a file gets added or removed.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExistenceOfInterestPredicate` in
                interface `SupportsDependencyFileRuleKey`

        []{#getInputsAfterBuildingLocally(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.cell.CellPathResolver)}

        -   #### getInputsAfterBuildingLocally

            ``` methodSignature
            public com.google.common.collect.ImmutableList<SourcePath> getInputsAfterBuildingLocally​(BuildContext context,
                                                                                                     CellPathResolver cellPathResolver)
            ```

            ::: block
            [Description copied from
            interface: `SupportsDependencyFileRuleKey`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns a list of source paths that were actually used for
            the rule. This list comes from the dep-file produced by
            compiler.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getInputsAfterBuildingLocally` in
                interface `SupportsDependencyFileRuleKey`
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
