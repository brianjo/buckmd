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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Class AndroidLibrary {#class-androidlibrary .title title="Class AndroidLibrary"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.rules.modern.ModernBuildRule](../rules/modern/ModernBuildRule.html "class in com.facebook.buck.rules.modern")\<T\>

        -   -   [com.facebook.buck.rules.modern.PipelinedModernBuildRule](../rules/modern/PipelinedModernBuildRule.html "class in com.facebook.buck.rules.modern")\<[JavacPipelineState](../jvm/java/JavacPipelineState.html "class in com.facebook.buck.jvm.java"),​com.facebook.buck.jvm.java.DefaultJavaLibraryBuildable\>

            -   -   [com.facebook.buck.jvm.java.DefaultJavaLibrary](../jvm/java/DefaultJavaLibrary.html "class in com.facebook.buck.jvm.java")

                -   -   com.facebook.buck.android.AndroidLibrary

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
    :   `AndroidPrebuiltAar`

    ------------------------------------------------------------------------

        public class AndroidLibrary
        extends DefaultJavaLibrary
        implements AndroidPackageable
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                      Description
          ------------------- -------------------------- -------------
          `static class `     `AndroidLibrary.Builder`    

          : Nested Classes[ ]{.tabEnd}

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
        | `static An            | `builder​(BuildTarg    |                       |
        | droidLibrary.Builder` | et buildTarget,       |                       |
        |                       |   ProjectFilesystem p |                       |
        |                       | rojectFilesystem,     |                       |
        |                       |     ToolchainProvider |                       |
        |                       |  toolchainProvider,   |                       |
        |                       |       BuildRuleParams |                       |
        |                       |  params,        Actio |                       |
        |                       | nGraphBuilder graphBu |                       |
        |                       | ilder,        JavaBuc |                       |
        |                       | kConfig javaBuckConfi |                       |
        |                       | g,        JavacFactor |                       |
        |                       | y javacFactory,       |                       |
        |                       |   JavacOptions javacO |                       |
        |                       | ptions,        Androi |                       |
        |                       | dLibraryDescription.C |                       |
        |                       | oreArg args,        C |                       |
        |                       | onfiguredCompilerFact |                       |
        |                       | ory compilerFactory)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getManifestFile()`   |                       |
        | Optional<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getType()`           |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.jvm.java.DefaultJavaLibrary}

            ### Methods inherited from class com.facebook.buck.jvm.java.[DefaultJavaLibrary](../jvm/java/DefaultJavaLibrary.html "class in com.facebook.buck.jvm.java")

            `getAbiInfo, getAbiJar, getBuildOutputInitializer, getClassHashesProvider, getClassNamesToHashes, getCompileTimeClasspathSourcePaths, getCoveredByDepFilePredicate, getDepsForTransitiveClasspathEntries, getExistenceOfInterestPredicate, getExportedDeps, getExportedProvidedDeps, getGeneratedAnnotationSourcePath, getImmediateClasspaths, getInputsAfterBuildingLocally, getJavaSrcs, getMavenCoords, getOutputClasspaths, getPipelineStateFactory, getPreviousRuleInPipeline, getRequiredForSourceOnlyAbi, getRequiredPackageables, getResources, getResourcesRoot, getRuntimeDeps, getSourceOnlyAbiJar, getSourcePathToOutput, getSources, getTests, getTransitiveClasspathDeps, getTransitiveClasspaths, hasAnnotationProcessing, initializeFromDisk, invalidateInitializeFromDiskState, isDesugarEnabled, isInterfaceMethodsDesugarEnabled, neverMarkAsUnusedDependency, rulesBuilder, setJavaClassHashesProvider, useDependencyFileRuleKeys, useRulePipelining`

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

            `compareTo, getBuildDeps, getBuildSteps, getBuildTarget, getFullyQualifiedName, getProjectFilesystem, hasBuildSteps, isCacheable, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString, updateBuildRuleResolver`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#builder(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.toolchain.ToolchainProvider,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.jvm.java.JavaBuckConfig,com.facebook.buck.jvm.java.JavacFactory,com.facebook.buck.jvm.java.JavacOptions,com.facebook.buck.android.AndroidLibraryDescription.CoreArg,com.facebook.buck.jvm.java.ConfiguredCompilerFactory)}

        -   #### builder

            ``` methodSignature
            public static AndroidLibrary.Builder builder​(BuildTarget buildTarget,
                                                         ProjectFilesystem projectFilesystem,
                                                         ToolchainProvider toolchainProvider,
                                                         BuildRuleParams params,
                                                         ActionGraphBuilder graphBuilder,
                                                         JavaBuckConfig javaBuckConfig,
                                                         JavacFactory javacFactory,
                                                         JavacOptions javacOptions,
                                                         AndroidLibraryDescription.CoreArg args,
                                                         ConfiguredCompilerFactory compilerFactory)
            ```

        []{#getManifestFile()}

        -   #### getManifestFile

            ``` methodSignature
            public Optional<SourcePath> getManifestFile()
            ```

        []{#getType()}

        -   #### getType

            ``` methodSignature
            public String getType()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getType` in interface `HasNameAndType`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getType` in class `AbstractBuildRule`

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
            :   `addToCollector` in class `DefaultJavaLibrary`

            [Parameters:]{.paramLabel}
            :   `collector` - The
                [`AndroidPackageableCollector`](packageable/AndroidPackageableCollector.html "class in com.facebook.buck.android.packageable")
                that will receive the content.
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
