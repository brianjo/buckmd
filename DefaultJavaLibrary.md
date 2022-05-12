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

## Class DefaultJavaLibrary {#class-defaultjavalibrary .title title="Class DefaultJavaLibrary"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.rules.modern.ModernBuildRule](../../rules/modern/ModernBuildRule.html "class in com.facebook.buck.rules.modern")\<T\>

        -   -   [com.facebook.buck.rules.modern.PipelinedModernBuildRule](../../rules/modern/PipelinedModernBuildRule.html "class in com.facebook.buck.rules.modern")\<[JavacPipelineState](JavacPipelineState.html "class in com.facebook.buck.jvm.java"),​com.facebook.buck.jvm.java.DefaultJavaLibraryBuildable\>

            -   -   com.facebook.buck.jvm.java.DefaultJavaLibrary

::: description
-   

    All Implemented Interfaces:
    :   `AndroidPackageable`, `BuildEngineAction`,
        `AllowsNonAnnotatedFields`, `ExportDependencies`,
        `HasRuntimeDeps`, `InitializableFromDisk<JavaLibrary.Data>`,
        `SupportsDependencyFileRuleKey`, `SupportsInputBasedRuleKey`,
        `BuildRule`, `HasNameAndType`,
        `SupportsPipelining<JavacPipelineState>`, `HasClasspathDeps`,
        `HasClasspathEntries`, `HasDesugarSupport`, `HasJavaAbi`,
        `HasJavaClassHashes`, `HasMavenCoordinates`, `HasSources`,
        `JavaLibrary`, `JavaLibraryWithTests`,
        `MaybeRequiredForSourceOnlyAbi`, `Comparable<BuildRule>`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `AndroidLibrary`

    ------------------------------------------------------------------------

        public class DefaultJavaLibrary
        extends PipelinedModernBuildRule<JavacPipelineState,​com.facebook.buck.jvm.java.DefaultJavaLibraryBuildable>
        implements JavaLibrary, ExportDependencies, InitializableFromDisk<JavaLibrary.Data>, AndroidPackageable, MaybeRequiredForSourceOnlyAbi, SupportsDependencyFileRuleKey, JavaLibraryWithTests

    ::: block
    Suppose this were a rule defined in `src/com/facebook/feed/BUCK`:
         java_library(
           name = 'feed',
           srcs = [
             'FeedStoryRenderer.java',
           ],
           deps = [
             '//src/com/facebook/feed/model:model',
             '//third-party/java/guava:guava',
           ],
         )
         

    Then this would compile `FeedStoryRenderer.java` against Guava and
    the classes generated from the `//src/com/facebook/feed/model:model`
    rule.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.jvm.core.JavaLibrary}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.jvm.core.[JavaLibrary](../core/JavaLibrary.html "interface in com.facebook.buck.jvm.core")

            `JavaLibrary.Data`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.jvm.core.JavaLibrary}

            ### Fields inherited from interface com.facebook.buck.jvm.core.[JavaLibrary](../core/JavaLibrary.html "interface in com.facebook.buck.jvm.core")

            `GWT_MODULE_FLAVOR, MAVEN_JAR, SRC_JAR`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              Description
          -------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `protected `   `DefaultJavaLibrary​(BuildTarget buildTarget,                   ProjectFilesystem projectFilesystem,                   JarBuildStepsFactory jarBuildStepsFactory,                   SourcePathRuleFinder ruleFinder,                   Optional<SourcePath> proguardConfig,                   SortedSet<BuildRule> firstOrderPackageableDeps,                   com.google.common.collect.ImmutableSortedSet<BuildRule> fullJarExportedDeps,                   com.google.common.collect.ImmutableSortedSet<BuildRule> fullJarProvidedDeps,                   com.google.common.collect.ImmutableSortedSet<BuildRule> fullJarExportedProvidedDeps,                   com.google.common.collect.ImmutableSortedSet<BuildRule> runtimeDeps,                   BuildTarget abiJar,                   BuildTarget sourceOnlyAbiJar,                   Optional<String> mavenCoords,                   com.google.common.collect.ImmutableSortedSet<BuildTarget> tests,                   boolean requiredForSourceOnlyAbi,                   JavaBuckConfig.UnusedDependenciesAction unusedDependenciesAction,                   Optional<UnusedDependenciesFinderFactory> unusedDependenciesFinderFactory,                   CalculateSourceAbi sourceAbi,                   boolean isDesugarEnabled,                   boolean isInterfaceMethodsDesugarEnabled,                   boolean neverMarkAsUnusedDependency)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `addToCollect         | ::: block             |
        |                       | or​(AndroidPackageable | Add concrete          |
        |                       | Collector collector)` | resources to the      |
        |                       |                       | given collector.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaAbiInfo`         | `getAbiInfo()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `O                    | `getAbiJar()`         |                       |
        | ptional<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildOutputInitializ | `getBuil              |                       |
        | er<JavaLibrary.Data>` | dOutputInitializer()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Jav                  | `getC                 |                       |
        | aClassHashesProvider` | lassHashesProvider()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `c                    | `get                  |                       |
        | om.google.common.coll | ClassNamesToHashes()` |                       |
        | ect.ImmutableSortedMa |                       |                       |
        | p<String,​com.google.c |                       |                       |
        | ommon.hash.HashCode>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.comm      | `getCompileTimeCl     |                       |
        | on.collect.ImmutableS | asspathSourcePaths()` |                       |
        | ortedSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `java.util.function.P | `getCov               | ::: block             |
        | redicate<SourcePath>` | eredByDepFilePredicat | Returns a predicate   |
        |                       | e​(SourcePathResolverA | that can tell whether |
        |                       | dapter pathResolver)` | a given path is       |
        |                       |                       | covered by dep-file   |
        |                       |                       | or not.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Set<BuildRule>`      | `getDepsForTransiti   |                       |
        |                       | veClasspathEntries()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `java.util.function.P | `getExiste            | ::: block             |
        | redicate<SourcePath>` | nceOfInterestPredicat | Returns a predicate   |
        |                       | e​(SourcePathResolverA | that can tell whether |
        |                       | dapter pathResolver)` | the existence of a    |
        |                       |                       | given path may be of  |
        |                       |                       | interest to compiler. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getExportedDeps()`   |                       |
        | SortedSet<BuildRule>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getEx                |                       |
        | SortedSet<BuildRule>` | portedProvidedDeps()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getGeneratedAn       |                       |
        | Optional<SourcePath>` | notationSourcePath()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getI                 | ::: block             |
        | e.common.collect.Immu | mmediateClasspaths()` | Returns the           |
        | tableSet<SourcePath>` |                       | classpaths for only   |
        |                       |                       | this rule, not its    |
        |                       |                       | deps.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getInputsAf          | ::: block             |
        | .common.collect.Immut | terBuildingLocally​(Bu | Returns a list of     |
        | ableList<SourcePath>` | ildContext context,   | source paths that     |
        |                       |                       | were actually used    |
        |                       |        CellPathResolv | for the rule.         |
        |                       | er cellPathResolver)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.comm      | `getJavaSrcs()`       |                       |
        | on.collect.ImmutableS |                       |                       |
        | ortedSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getMavenCoords()`    | ::: block             |
        |                       |                       | Used to identify this |
        |                       |                       | library within a      |
        |                       |                       | maven repository      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `g                    |                       |
        | e.common.collect.Immu | etOutputClasspaths()` |                       |
        | tableSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Rul                  | `getPi                |                       |
        | ePipelineStateFactory | pelineStateFactory()` |                       |
        | <JavacPipelineState>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SupportsPipelining   | `getPrev              |                       |
        | <JavacPipelineState>` | iousRuleInPipeline()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getRequir            |                       |
        |                       | edForSourceOnlyAbi()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable             | `getRequiredPac       | ::: block             |
        | <AndroidPackageable>` | kageables​(BuildRuleRe | Get the set of        |
        |                       | solver ruleResolver)` | packagables that need |
        |                       |                       | to be included in any |
        |                       |                       | package that includes |
        |                       |                       | this object.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.comm      | `getResources()`      |                       |
        | on.collect.ImmutableS |                       |                       |
        | ortedSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getResourcesRoot()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `java.util.stream     | `getRuntime           |                       |
        | .Stream<BuildTarget>` | Deps​(BuildRuleResolve |                       |
        |                       | r buildRuleResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `O                    | `g                    |                       |
        | ptional<BuildTarget>` | etSourceOnlyAbiJar()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `get                  |                       |
        |                       | SourcePathToOutput()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.comm      | `getSources()`        |                       |
        | on.collect.ImmutableS |                       |                       |
        | ortedSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getTests()`          |                       |
        | n.collect.ImmutableSo |                       |                       |
        | rtedSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getTrans             |                       |
        | .common.collect.Immut | itiveClasspathDeps()` |                       |
        | ableSet<JavaLibrary>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getTr                |                       |
        | e.common.collect.Immu | ansitiveClasspaths()` |                       |
        | tableSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `hasAn                |                       |
        |                       | notationProcessing()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `JavaLibrary.Data`    | `initializeFromDis    | ::: block             |
        |                       | k​(SourcePathResolverA | Instructs this rule   |
        |                       | dapter pathResolver)` | to report the ABI it  |
        |                       |                       | has on disk as its    |
        |                       |                       | current ABI.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `invalidateIniti      |                       |
        |                       | alizeFromDiskState()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isDesugarEnabled()`  | ::: block             |
        |                       |                       | Desugar support for   |
        |                       |                       | java 8 features       |
        |                       |                       | withing single class  |
        |                       |                       | file.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isInterfaceMet       | ::: block             |
        |                       | hodsDesugarEnabled()` | Desugar support for   |
        |                       |                       | interface default and |
        |                       |                       | static methods.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `neverMark            |                       |
        |                       | AsUnusedDependency()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static DefaultJava   | `rulesBu              |                       |
        | LibraryRules.Builder` | ilder​(BuildTarget bui |                       |
        |                       | ldTarget,             |                       |
        |                       |  ProjectFilesystem pr |                       |
        |                       | ojectFilesystem,      |                       |
        |                       |         ToolchainProv |                       |
        |                       | ider toolchainProvide |                       |
        |                       | r,             BuildR |                       |
        |                       | uleParams params,     |                       |
        |                       |          ActionGraphB |                       |
        |                       | uilder graphBuilder,  |                       |
        |                       |             Configure |                       |
        |                       | dCompilerFactory comp |                       |
        |                       | ilerFactory,          |                       |
        |                       |     JavaBuckConfig ja |                       |
        |                       | vaBuckConfig,         |                       |
        |                       |      JavaLibraryDescr |                       |
        |                       | iption.CoreArg args)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `setJavaClassH        |                       |
        |                       | ashesProvider​(JavaCla |                       |
        |                       | ssHashesProvider java |                       |
        |                       | ClassHashesProvider)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `useDepe              |                       |
        |                       | ndencyFileRuleKeys()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `useRulePipelining()` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
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

            `equals, getBuildTarget, getDependencies, getProjectFilesystem, getSourcePathOutputs, getType, hasBuildSteps, hashCode, injectFields, isCacheable, toString`

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
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.HasNameAndType}

            ### Methods inherited from interface com.facebook.buck.core.rules.[HasNameAndType](../../core/rules/HasNameAndType.html "interface in com.facebook.buck.core.rules")

            `getType`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.jvm.java.JarBuildStepsFactory,com.facebook.buck.core.rules.SourcePathRuleFinder,java.util.Optional,java.util.SortedSet,com.google.common.collect.ImmutableSortedSet,com.google.common.collect.ImmutableSortedSet,com.google.common.collect.ImmutableSortedSet,com.google.common.collect.ImmutableSortedSet,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.model.BuildTarget,java.util.Optional,com.google.common.collect.ImmutableSortedSet,boolean,com.facebook.buck.jvm.java.JavaBuckConfig.UnusedDependenciesAction,java.util.Optional,com.facebook.buck.jvm.java.CalculateSourceAbi,boolean,boolean,boolean)}

        -   #### DefaultJavaLibrary

                protected DefaultJavaLibrary​(BuildTarget buildTarget,
                                             ProjectFilesystem projectFilesystem,
                                             JarBuildStepsFactory jarBuildStepsFactory,
                                             SourcePathRuleFinder ruleFinder,
                                             Optional<SourcePath> proguardConfig,
                                             SortedSet<BuildRule> firstOrderPackageableDeps,
                                             com.google.common.collect.ImmutableSortedSet<BuildRule> fullJarExportedDeps,
                                             com.google.common.collect.ImmutableSortedSet<BuildRule> fullJarProvidedDeps,
                                             com.google.common.collect.ImmutableSortedSet<BuildRule> fullJarExportedProvidedDeps,
                                             com.google.common.collect.ImmutableSortedSet<BuildRule> runtimeDeps,
                                             @Nullable
                                             BuildTarget abiJar,
                                             @Nullable
                                             BuildTarget sourceOnlyAbiJar,
                                             Optional<String> mavenCoords,
                                             com.google.common.collect.ImmutableSortedSet<BuildTarget> tests,
                                             boolean requiredForSourceOnlyAbi,
                                             JavaBuckConfig.UnusedDependenciesAction unusedDependenciesAction,
                                             Optional<UnusedDependenciesFinderFactory> unusedDependenciesFinderFactory,
                                             @Nullable
                                             CalculateSourceAbi sourceAbi,
                                             boolean isDesugarEnabled,
                                             boolean isInterfaceMethodsDesugarEnabled,
                                             boolean neverMarkAsUnusedDependency)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#rulesBuilder(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.toolchain.ToolchainProvider,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.jvm.java.ConfiguredCompilerFactory,com.facebook.buck.jvm.java.JavaBuckConfig,com.facebook.buck.jvm.java.JavaLibraryDescription.CoreArg)}

        -   #### rulesBuilder

            ``` methodSignature
            public static DefaultJavaLibraryRules.Builder rulesBuilder​(BuildTarget buildTarget,
                                                                       ProjectFilesystem projectFilesystem,
                                                                       ToolchainProvider toolchainProvider,
                                                                       BuildRuleParams params,
                                                                       ActionGraphBuilder graphBuilder,
                                                                       ConfiguredCompilerFactory compilerFactory,
                                                                       @Nullable
                                                                       JavaBuckConfig javaBuckConfig,
                                                                       @Nullable
                                                                       JavaLibraryDescription.CoreArg args)
            ```

        []{#getTests()}

        -   #### getTests

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildTarget> getTests()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTests` in interface `JavaLibraryWithTests`

            [Returns:]{.returnLabel}
            :   A list of tests of this target.

        []{#isDesugarEnabled()}

        -   #### isDesugarEnabled

            ``` methodSignature
            public boolean isDesugarEnabled()
            ```

            ::: block
            [Description copied from
            interface: `HasDesugarSupport`]{.descfrmTypeLabel}
            :::

            ::: block
            Desugar support for java 8 features withing single class
            file.
            Such as Lambda expressions, Method references, Repeating
            annotations
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `isDesugarEnabled` in interface `HasDesugarSupport`

        []{#isInterfaceMethodsDesugarEnabled()}

        -   #### isInterfaceMethodsDesugarEnabled

            ``` methodSignature
            public boolean isInterfaceMethodsDesugarEnabled()
            ```

            ::: block
            [Description copied from
            interface: `HasDesugarSupport`]{.descfrmTypeLabel}
            :::

            ::: block
            Desugar support for interface default and static methods.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `isInterfaceMethodsDesugarEnabled` in
                interface `HasDesugarSupport`

        []{#getRequiredForSourceOnlyAbi()}

        -   #### getRequiredForSourceOnlyAbi

            ``` methodSignature
            public boolean getRequiredForSourceOnlyAbi()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRequiredForSourceOnlyAbi` in
                interface `MaybeRequiredForSourceOnlyAbi`

        []{#getJavaSrcs()}

        -   #### getJavaSrcs

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<SourcePath> getJavaSrcs()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getJavaSrcs` in interface `JavaLibrary`

        []{#getSources()}

        -   #### getSources

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<SourcePath> getSources()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSources` in interface `HasSources`

        []{#getResources()}

        -   #### getResources

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<SourcePath> getResources()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getResources` in interface `JavaLibrary`

        []{#getResourcesRoot()}

        -   #### getResourcesRoot

            ``` methodSignature
            public Optional<String> getResourcesRoot()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getResourcesRoot` in interface `JavaLibrary`

        []{#hasAnnotationProcessing()}

        -   #### hasAnnotationProcessing

            ``` methodSignature
            public boolean hasAnnotationProcessing()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `hasAnnotationProcessing` in interface `JavaLibrary`

        []{#getDepsForTransitiveClasspathEntries()}

        -   #### getDepsForTransitiveClasspathEntries

            ``` methodSignature
            public Set<BuildRule> getDepsForTransitiveClasspathEntries()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDepsForTransitiveClasspathEntries` in
                interface `HasClasspathDeps`

            [Returns:]{.returnLabel}
            :   all direct dependencies which may contribute to the
                classpath of this rule

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

        []{#getCompileTimeClasspathSourcePaths()}

        -   #### getCompileTimeClasspathSourcePaths

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<SourcePath> getCompileTimeClasspathSourcePaths()
            ```

        []{#getGeneratedAnnotationSourcePath()}

        -   #### getGeneratedAnnotationSourcePath

            ``` methodSignature
            public Optional<SourcePath> getGeneratedAnnotationSourcePath()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getGeneratedAnnotationSourcePath` in
                interface `JavaLibrary`

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

        []{#invalidateInitializeFromDiskState()}

        -   #### invalidateInitializeFromDiskState

            ``` methodSignature
            public void invalidateInitializeFromDiskState()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `invalidateInitializeFromDiskState` in
                interface `InitializableFromDisk<JavaLibrary.Data>`

        []{#initializeFromDisk(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### initializeFromDisk

            ``` methodSignature
            public JavaLibrary.Data initializeFromDisk​(SourcePathResolverAdapter pathResolver)
                                                throws IOException
            ```

            ::: block
            Instructs this rule to report the ABI it has on disk as its
            current ABI.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `initializeFromDisk` in
                interface `InitializableFromDisk<JavaLibrary.Data>`

            [Parameters:]{.paramLabel}
            :   `pathResolver` -

            [Returns:]{.returnLabel}
            :   an object that has the in-memory data structures that
                need to be populated as a result of executing this
                object\'s steps.

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getBuildOutputInitializer()}

        -   #### getBuildOutputInitializer

            ``` methodSignature
            public BuildOutputInitializer<JavaLibrary.Data> getBuildOutputInitializer()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildOutputInitializer` in
                interface `InitializableFromDisk<JavaLibrary.Data>`

        []{#getAbiJar()}

        -   #### getAbiJar

            ``` methodSignature
            public final Optional<BuildTarget> getAbiJar()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAbiJar` in interface `HasJavaAbi`

            [Returns:]{.returnLabel}
            :   the
                [`SourcePath`](../../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
                representing the ABI Jar for this rule.

        []{#getSourceOnlyAbiJar()}

        -   #### getSourceOnlyAbiJar

            ``` methodSignature
            public Optional<BuildTarget> getSourceOnlyAbiJar()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourceOnlyAbiJar` in interface `HasJavaAbi`

        []{#getAbiInfo()}

        -   #### getAbiInfo

            ``` methodSignature
            public JavaAbiInfo getAbiInfo()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAbiInfo` in interface `HasJavaAbi`

        []{#getClassNamesToHashes()}

        -   #### getClassNamesToHashes

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedMap<String,​com.google.common.hash.HashCode> getClassNamesToHashes()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getClassNamesToHashes` in
                interface `HasJavaClassHashes`

            [Returns:]{.returnLabel}
            :   a (possibly empty) map of names of `.class` files in the
                output of this rule to SHA-1 hashes of their contents.

        []{#getSourcePathToOutput()}

        -   #### getSourcePathToOutput

            ``` methodSignature
            @Nullable
            public SourcePath getSourcePathToOutput()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in interface `BuildRule`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in
                class `ModernBuildRule<com.facebook.buck.jvm.java.DefaultJavaLibraryBuildable>`

        []{#getRequiredPackageables(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### getRequiredPackageables

            ``` methodSignature
            public Iterable<AndroidPackageable> getRequiredPackageables​(BuildRuleResolver ruleResolver)
            ```

            ::: block
            [Description copied from
            interface: `AndroidPackageable`]{.descfrmTypeLabel}
            :::

            ::: block
            Get the set of packagables that need to be included in any
            package that includes this object.
            For example, an android_library will need all of its Java
            deps (except provided_deps), its resource deps, and its
            native library deps (even though it doesn\'t need the native
            library as a build-time dependency). An android_resource
            might need an android_library that declares a custom view
            that it references, as well as other android_resource rules
            that it references directly.

            TODO(natthu): Once build rules and buildables are merged,
            replace this method with another interface that lets an
            [`AndroidPackageable`](../../android/packageable/AndroidPackageable.html "interface in com.facebook.buck.android.packageable")
            override the default set which is all deps of the type
            [`AndroidPackageable`](../../android/packageable/AndroidPackageable.html "interface in com.facebook.buck.android.packageable").
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRequiredPackageables` in
                interface `AndroidPackageable`

            [Returns:]{.returnLabel}
            :   All
                [`AndroidPackageable`](../../android/packageable/AndroidPackageable.html "interface in com.facebook.buck.android.packageable")s
                that must be included along with this one.

        []{#getRuntimeDeps(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### getRuntimeDeps

            ``` methodSignature
            public java.util.stream.Stream<BuildTarget> getRuntimeDeps​(BuildRuleResolver buildRuleResolver)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRuntimeDeps` in interface `HasRuntimeDeps`

        []{#getMavenCoords()}

        -   #### getMavenCoords

            ``` methodSignature
            public Optional<String> getMavenCoords()
            ```

            ::: block
            [Description copied from
            interface: `HasMavenCoordinates`]{.descfrmTypeLabel}
            :::

            ::: block
            Used to identify this library within a maven repository
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getMavenCoords` in interface `HasMavenCoordinates`

        []{#addToCollector(com.facebook.buck.android.packageable.AndroidPackageableCollector)}

        -   #### addToCollector

            ``` methodSignature
            public void addToCollector​(AndroidPackageableCollector collector)
            ```

            ::: block
            [Description copied from
            interface: `AndroidPackageable`]{.descfrmTypeLabel}
            :::

            ::: block
            Add concrete resources to the given collector.
            Implementations should call methods on the collector specify
            what concrete content must be included in an Android package
            that includes this object. For example, an android_library
            will add Java classes, an ndk_library will add native
            libraries, and android_resource will add resource
            directories.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `addToCollector` in interface `AndroidPackageable`

            [Parameters:]{.paramLabel}
            :   `collector` - The
                [`AndroidPackageableCollector`](../../android/packageable/AndroidPackageableCollector.html "class in com.facebook.buck.android.packageable")
                that will receive the content.

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

        []{#useRulePipelining()}

        -   #### useRulePipelining

            ``` methodSignature
            public boolean useRulePipelining()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `useRulePipelining` in
                interface `SupportsPipelining<JavacPipelineState>`

        []{#getPipelineStateFactory()}

        -   #### getPipelineStateFactory

            ``` methodSignature
            public RulePipelineStateFactory<JavacPipelineState> getPipelineStateFactory()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPipelineStateFactory` in
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

        []{#getClassHashesProvider()}

        -   #### getClassHashesProvider

            ``` methodSignature
            public JavaClassHashesProvider getClassHashesProvider()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getClassHashesProvider` in
                interface `HasJavaClassHashes`

        []{#setJavaClassHashesProvider(com.facebook.buck.jvm.core.JavaClassHashesProvider)}

        -   #### setJavaClassHashesProvider

            ``` methodSignature
            public void setJavaClassHashesProvider​(JavaClassHashesProvider javaClassHashesProvider)
            ```

        []{#neverMarkAsUnusedDependency()}

        -   #### neverMarkAsUnusedDependency

            ``` methodSignature
            public boolean neverMarkAsUnusedDependency()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `neverMarkAsUnusedDependency` in interface `JavaLibrary`
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
