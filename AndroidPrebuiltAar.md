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

## Class AndroidPrebuiltAar {#class-androidprebuiltaar .title title="Class AndroidPrebuiltAar"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.rules.modern.ModernBuildRule](../rules/modern/ModernBuildRule.html "class in com.facebook.buck.rules.modern")\<T\>

        -   -   [com.facebook.buck.rules.modern.PipelinedModernBuildRule](../rules/modern/PipelinedModernBuildRule.html "class in com.facebook.buck.rules.modern")\<[JavacPipelineState](../jvm/java/JavacPipelineState.html "class in com.facebook.buck.jvm.java"),​com.facebook.buck.jvm.java.DefaultJavaLibraryBuildable\>

            -   -   [com.facebook.buck.jvm.java.DefaultJavaLibrary](../jvm/java/DefaultJavaLibrary.html "class in com.facebook.buck.jvm.java")

                -   -   [com.facebook.buck.android.AndroidLibrary](AndroidLibrary.html "class in com.facebook.buck.android")

                    -   -   com.facebook.buck.android.AndroidPrebuiltAar

::: description
-   

    All Implemented Interfaces:
    :   `HasAndroidResourceDeps`, `AndroidPackageable`,
        `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `ExportDependencies`, `HasRuntimeDeps`,
        `InitializableFromDisk<JavaLibrary.Data>`,
        `SupportsDependencyFileRuleKey`, `SupportsInputBasedRuleKey`,
        `BuildRule`, `HasNameAndType`,
        `SupportsPipelining<JavacPipelineState>`, `HasClasspathDeps`,
        `HasClasspathEntries`, `HasDesugarSupport`, `HasJavaAbi`,
        `HasJavaClassHashes`, `HasMavenCoordinates`, `HasSources`,
        `JavaLibrary`, `JavaLibraryWithTests`,
        `MaybeRequiredForSourceOnlyAbi`, `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class AndroidPrebuiltAar
        extends AndroidLibrary
        implements HasAndroidResourceDeps, HasRuntimeDeps
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.android.AndroidLibrary}

            ### Nested classes/interfaces inherited from class com.facebook.buck.android.[AndroidLibrary](AndroidLibrary.html "class in com.facebook.buck.android")

            `AndroidLibrary.Builder`

        ```{=html}
        <!-- -->
        ```
        -   []{#nested.classes.inherited.from.class.com.facebook.buck.jvm.core.JavaLibrary}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.jvm.core.[JavaLibrary](../jvm/core/JavaLibrary.html "interface in com.facebook.buck.jvm.core")

            `JavaLibrary.Data`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.jvm.core.JavaLibrary}

            ### Fields inherited from interface com.facebook.buck.jvm.core.[JavaLibrary](../jvm/core/JavaLibrary.html "interface in com.facebook.buck.jvm.core")

            `GWT_MODULE_FLAVOR, MAVEN_JAR, SRC_JAR`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `AndroidPrebuiltAar​(BuildTarget androidLibraryBuildTarget,                   ProjectFilesystem projectFilesystem,                   BuildRuleParams androidLibraryParams,                   SourcePathRuleFinder ruleFinder,                   SourcePath proguardConfig,                   SourcePath nativeLibsDirectory,                   PrebuiltJar prebuiltJar,                   UnzipAar unzipAar,                   CompileToJarStepFactory configuredCompiler,                   Iterable<PrebuiltJar> exportedDeps,                   boolean requiredForSourceAbi,                   Optional<String> mavenCoords,                   boolean useSystemLibraryLoader)`    

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
        | `SourcePath`          | `getAssets()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getBinaryJar()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getPathToR           |                       |
        |                       | DotJavaPackageFile()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getPat               |                       |
        |                       | hToTextSymbolsFile()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltJar`         | `getPrebuiltJar()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `                     |                       |
        |                       | getRDotJavaPackage()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getRes()`            |                       |
        +-----------------------+-----------------------+-----------------------+
        | `java.util.stream     | `getRuntime           |                       |
        | .Stream<BuildTarget>` | Deps​(BuildRuleResolve |                       |
        |                       | r buildRuleResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `useDepe              |                       |
        |                       | ndencyFileRuleKeys()` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.android.AndroidLibrary}

            ### Methods inherited from class com.facebook.buck.android.[AndroidLibrary](AndroidLibrary.html "class in com.facebook.buck.android")

            `builder, getManifestFile, getType`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.jvm.java.DefaultJavaLibrary}

            ### Methods inherited from class com.facebook.buck.jvm.java.[DefaultJavaLibrary](../jvm/java/DefaultJavaLibrary.html "class in com.facebook.buck.jvm.java")

            `getAbiInfo, getAbiJar, getBuildOutputInitializer, getClassHashesProvider, getClassNamesToHashes, getCompileTimeClasspathSourcePaths, getCoveredByDepFilePredicate, getDepsForTransitiveClasspathEntries, getExistenceOfInterestPredicate, getExportedDeps, getExportedProvidedDeps, getGeneratedAnnotationSourcePath, getImmediateClasspaths, getInputsAfterBuildingLocally, getJavaSrcs, getMavenCoords, getOutputClasspaths, getPipelineStateFactory, getPreviousRuleInPipeline, getRequiredForSourceOnlyAbi, getRequiredPackageables, getResources, getResourcesRoot, getSourceOnlyAbiJar, getSourcePathToOutput, getSources, getTests, getTransitiveClasspathDeps, getTransitiveClasspaths, hasAnnotationProcessing, initializeFromDisk, invalidateInitializeFromDiskState, isDesugarEnabled, isInterfaceMethodsDesugarEnabled, neverMarkAsUnusedDependency, rulesBuilder, setJavaClassHashesProvider, useRulePipelining`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.rules.modern.PipelinedModernBuildRule}

            ### Methods inherited from class com.facebook.buck.rules.modern.[PipelinedModernBuildRule](../rules/modern/PipelinedModernBuildRule.html "class in com.facebook.buck.rules.modern")

            `getPipelinedBuildSteps`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.rules.modern.ModernBuildRule}

            ### Methods inherited from class com.facebook.buck.rules.modern.[ModernBuildRule](../rules/modern/ModernBuildRule.html "class in com.facebook.buck.rules.modern")

            `compareTo, getBuildable, getBuildCellPathFactory, getBuildDeps, getBuildSteps, getOutputPathResolver, getSetupStepsForBuildable, getSourcePath, getSourcePaths, injectFieldsIfNecessary, inputBasedRuleKeyIsEnabled, recordOutputs, recordOutputs, recordOutputs, stepsForBuildable, stepsForBuildable, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRule}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

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
        -   []{#methods.inherited.from.class.com.facebook.buck.android.packageable.AndroidPackageable}

            ### Methods inherited from interface com.facebook.buck.android.packageable.[AndroidPackageable](packageable/AndroidPackageable.html "interface in com.facebook.buck.android.packageable")

            `getRequiredPackageables`

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

            `compareTo, getBuildDeps, getBuildSteps, getBuildTarget, getFullyQualifiedName, getProjectFilesystem, getSourcePathToOutput, hasBuildSteps, isCacheable, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.android.HasAndroidResourceDeps}

            ### Methods inherited from interface com.facebook.buck.android.[HasAndroidResourceDeps](HasAndroidResourceDeps.html "interface in com.facebook.buck.android")

            `getBuildTarget`

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

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.rules.SourcePathRuleFinder,com.facebook.buck.core.sourcepath.SourcePath,com.facebook.buck.core.sourcepath.SourcePath,com.facebook.buck.jvm.java.PrebuiltJar,com.facebook.buck.android.UnzipAar,com.facebook.buck.jvm.java.CompileToJarStepFactory,java.lang.Iterable,boolean,java.util.Optional,boolean)}

        -   #### AndroidPrebuiltAar

                public AndroidPrebuiltAar​(BuildTarget androidLibraryBuildTarget,
                                          ProjectFilesystem projectFilesystem,
                                          BuildRuleParams androidLibraryParams,
                                          SourcePathRuleFinder ruleFinder,
                                          SourcePath proguardConfig,
                                          SourcePath nativeLibsDirectory,
                                          PrebuiltJar prebuiltJar,
                                          UnzipAar unzipAar,
                                          CompileToJarStepFactory configuredCompiler,
                                          Iterable<PrebuiltJar> exportedDeps,
                                          boolean requiredForSourceAbi,
                                          Optional<String> mavenCoords,
                                          boolean useSystemLibraryLoader)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getRDotJavaPackage()}

        -   #### getRDotJavaPackage

            ``` methodSignature
            public String getRDotJavaPackage()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRDotJavaPackage` in
                interface `HasAndroidResourceDeps`

            [Returns:]{.returnLabel}
            :   the package name in which to generate the R.java
                representing these resources.

        []{#useDependencyFileRuleKeys()}

        -   #### useDependencyFileRuleKeys

            ``` methodSignature
            public boolean useDependencyFileRuleKeys()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `useDependencyFileRuleKeys` in
                interface `SupportsDependencyFileRuleKey`

            [Overrides:]{.overrideSpecifyLabel}
            :   `useDependencyFileRuleKeys` in
                class `DefaultJavaLibrary`

        []{#getPathToTextSymbolsFile()}

        -   #### getPathToTextSymbolsFile

            ``` methodSignature
            public SourcePath getPathToTextSymbolsFile()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPathToTextSymbolsFile` in
                interface `HasAndroidResourceDeps`

            [Returns:]{.returnLabel}
            :   path to a temporary directory for storing text symbols.

        []{#getPathToRDotJavaPackageFile()}

        -   #### getPathToRDotJavaPackageFile

            ``` methodSignature
            public SourcePath getPathToRDotJavaPackageFile()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPathToRDotJavaPackageFile` in
                interface `HasAndroidResourceDeps`

            [Returns:]{.returnLabel}
            :   path to a file containing the package name for R.java.

        []{#getRes()}

        -   #### getRes

            ``` methodSignature
            public SourcePath getRes()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRes` in interface `HasAndroidResourceDeps`

            [Returns:]{.returnLabel}
            :   path to a directory containing Android resources.

        []{#getAssets()}

        -   #### getAssets

            ``` methodSignature
            public SourcePath getAssets()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAssets` in interface `HasAndroidResourceDeps`

            [Returns:]{.returnLabel}
            :   path to a directory containing Android assets.

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

            [Overrides:]{.overrideSpecifyLabel}
            :   `addToCollector` in class `AndroidLibrary`

            [Parameters:]{.paramLabel}
            :   `collector` - The
                [`AndroidPackageableCollector`](packageable/AndroidPackageableCollector.html "class in com.facebook.buck.android.packageable")
                that will receive the content.

        []{#getPrebuiltJar()}

        -   #### getPrebuiltJar

            ``` methodSignature
            public PrebuiltJar getPrebuiltJar()
            ```

        []{#getBinaryJar()}

        -   #### getBinaryJar

            ``` methodSignature
            public SourcePath getBinaryJar()
            ```

        []{#getRuntimeDeps(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### getRuntimeDeps

            ``` methodSignature
            public java.util.stream.Stream<BuildTarget> getRuntimeDeps​(BuildRuleResolver buildRuleResolver)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRuntimeDeps` in interface `HasRuntimeDeps`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getRuntimeDeps` in class `DefaultJavaLibrary`
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
