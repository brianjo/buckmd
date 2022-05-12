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
-   Tree
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Hierarchy For Package com.facebook.buck.jvm.java {#hierarchy-for-package-com.facebook.buck.jvm.java .title}

[Package Hierarchies:]{.packageHierarchyLabel}

-   [All Packages](../../../../../overview-tree.html)
:::

::: contentContainer
::: {.section role="region"}
## Class Hierarchy {#class-hierarchy title="Class Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   com.facebook.buck.event.[[AbstractBuckEvent]{.typeNameLink}](../../event/AbstractBuckEvent.html "class in com.facebook.buck.event")
        (implements
        com.facebook.buck.event.[BuckEvent](../../event/BuckEvent.html "interface in com.facebook.buck.event"))
        -   com.facebook.buck.jvm.java.[[AnnotationProcessingEvent]{.typeNameLink}](AnnotationProcessingEvent.html "class in com.facebook.buck.jvm.java")
            (implements
            com.facebook.buck.event.[WorkAdvanceEvent](../../event/WorkAdvanceEvent.html "interface in com.facebook.buck.event"))
            -   com.facebook.buck.jvm.java.[[AnnotationProcessingEvent.Finished]{.typeNameLink}](AnnotationProcessingEvent.Finished.html "class in com.facebook.buck.jvm.java")
            -   com.facebook.buck.jvm.java.[[AnnotationProcessingEvent.Started]{.typeNameLink}](AnnotationProcessingEvent.Started.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.core.rules.impl.[[AbstractBuildRule]{.typeNameLink}](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")
        (implements
        com.facebook.buck.core.rules.[BuildRule](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules"))
        -   com.facebook.buck.core.rules.impl.[[AbstractBuildRuleWithDeclaredAndExtraDeps]{.typeNameLink}](../../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")
            (implements
            com.facebook.buck.core.rules.attr.[HasDeclaredAndExtraDeps](../../core/rules/attr/HasDeclaredAndExtraDeps.html "interface in com.facebook.buck.core.rules.attr"))
            -   com.facebook.buck.jvm.java.[[CompareAbis]{.typeNameLink}](CompareAbis.html "class in com.facebook.buck.jvm.java")
                (implements
                com.facebook.buck.jvm.core.[CalculateAbi](../core/CalculateAbi.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.core.rules.attr.[InitializableFromDisk](../../core/rules/attr/InitializableFromDisk.html "interface in com.facebook.buck.core.rules.attr")\<T\>,
                com.facebook.buck.core.rules.attr.[SupportsInputBasedRuleKey](../../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr"))
            -   com.facebook.buck.jvm.java.[[JarFattener]{.typeNameLink}](JarFattener.html "class in com.facebook.buck.jvm.java")
                (implements
                com.facebook.buck.core.rules.tool.[BinaryBuildRule](../../core/rules/tool/BinaryBuildRule.html "interface in com.facebook.buck.core.rules.tool"),
                com.facebook.buck.jvm.core.[HasClasspathEntries](../core/HasClasspathEntries.html "interface in com.facebook.buck.jvm.core"))
            -   com.facebook.buck.jvm.java.[[JavaBinary]{.typeNameLink}](JavaBinary.html "class in com.facebook.buck.jvm.java")
                (implements
                com.facebook.buck.core.rules.tool.[BinaryBuildRule](../../core/rules/tool/BinaryBuildRule.html "interface in com.facebook.buck.core.rules.tool"),
                com.facebook.buck.jvm.core.[HasClasspathDeps](../core/HasClasspathDeps.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasClasspathEntries](../core/HasClasspathEntries.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"))
            -   com.facebook.buck.jvm.java.[[Javadoc]{.typeNameLink}](Javadoc.html "class in com.facebook.buck.jvm.java")
                (implements
                com.facebook.buck.jvm.java.[MavenPublishable](MavenPublishable.html "interface in com.facebook.buck.jvm.java"))
            -   com.facebook.buck.jvm.java.[[JavaSourceJar]{.typeNameLink}](JavaSourceJar.html "class in com.facebook.buck.jvm.java")
                (implements
                com.facebook.buck.jvm.core.[HasMavenCoordinates](../core/HasMavenCoordinates.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasSources](../core/HasSources.html "interface in com.facebook.buck.jvm.core"))
                -   com.facebook.buck.jvm.java.[[MavenUberJar.SourceJar]{.typeNameLink}](MavenUberJar.SourceJar.html "class in com.facebook.buck.jvm.java")
                    (implements
                    com.facebook.buck.jvm.java.[MavenPublishable](MavenPublishable.html "interface in com.facebook.buck.jvm.java"))
            -   com.facebook.buck.jvm.java.[[JavaTest]{.typeNameLink}](JavaTest.html "class in com.facebook.buck.jvm.java")
                (implements
                com.facebook.buck.core.rules.attr.[ExportDependencies](../../core/rules/attr/ExportDependencies.html "interface in com.facebook.buck.core.rules.attr"),
                com.facebook.buck.core.test.rule.[ExternalTestRunnerRule](../../core/test/rule/ExternalTestRunnerRule.html "interface in com.facebook.buck.core.test.rule"),
                com.facebook.buck.jvm.core.[HasClasspathEntries](../core/HasClasspathEntries.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.core.rules.attr.[HasPostBuildSteps](../../core/rules/attr/HasPostBuildSteps.html "interface in com.facebook.buck.core.rules.attr"),
                com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"),
                com.facebook.buck.core.test.rule.[TestRule](../../core/test/rule/TestRule.html "interface in com.facebook.buck.core.test.rule"))
            -   com.facebook.buck.jvm.java.[[JavaTestX]{.typeNameLink}](JavaTestX.html "class in com.facebook.buck.jvm.java")
                (implements
                com.facebook.buck.core.rules.attr.[ExportDependencies](../../core/rules/attr/ExportDependencies.html "interface in com.facebook.buck.core.rules.attr"),
                com.facebook.buck.core.test.rule.[ExternalTestRunnerRule](../../core/test/rule/ExternalTestRunnerRule.html "interface in com.facebook.buck.core.test.rule"),
                com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"),
                com.facebook.buck.core.test.rule.[TestXRule](../../core/test/rule/TestXRule.html "interface in com.facebook.buck.core.test.rule"))
            -   com.facebook.buck.jvm.java.[[Keystore]{.typeNameLink}](Keystore.html "class in com.facebook.buck.jvm.java")
            -   com.facebook.buck.jvm.java.[[MavenUberJar]{.typeNameLink}](MavenUberJar.html "class in com.facebook.buck.jvm.java")
                (implements
                com.facebook.buck.jvm.java.[MavenPublishable](MavenPublishable.html "interface in com.facebook.buck.jvm.java"))
            -   com.facebook.buck.core.rules.impl.[[NoopBuildRuleWithDeclaredAndExtraDeps]{.typeNameLink}](../../core/rules/impl/NoopBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")
                -   com.facebook.buck.jvm.java.[[JavaAnnotationProcessor]{.typeNameLink}](JavaAnnotationProcessor.html "class in com.facebook.buck.jvm.java")
                -   com.facebook.buck.jvm.java.[[JavaTestRunner]{.typeNameLink}](JavaTestRunner.html "class in com.facebook.buck.jvm.java")
                -   com.facebook.buck.jvm.java.[[StandardJavacPlugin]{.typeNameLink}](StandardJavacPlugin.html "class in com.facebook.buck.jvm.java")
            -   com.facebook.buck.jvm.java.[[PrebuiltJar]{.typeNameLink}](PrebuiltJar.html "class in com.facebook.buck.jvm.java")
                (implements
                com.facebook.buck.android.packageable.[AndroidPackageable](../../android/packageable/AndroidPackageable.html "interface in com.facebook.buck.android.packageable"),
                com.facebook.buck.core.rules.attr.[ExportDependencies](../../core/rules/attr/ExportDependencies.html "interface in com.facebook.buck.core.rules.attr"),
                com.facebook.buck.core.rules.attr.[InitializableFromDisk](../../core/rules/attr/InitializableFromDisk.html "interface in com.facebook.buck.core.rules.attr")\<T\>,
                com.facebook.buck.jvm.core.[JavaLibrary](../core/JavaLibrary.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.java.[MaybeRequiredForSourceOnlyAbi](MaybeRequiredForSourceOnlyAbi.html "interface in com.facebook.buck.jvm.java"),
                com.facebook.buck.core.rules.attr.[SupportsInputBasedRuleKey](../../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr"))
        -   com.facebook.buck.rules.modern.[[ModernBuildRule]{.typeNameLink}](../../rules/modern/ModernBuildRule.html "class in com.facebook.buck.rules.modern")\<T\>
            (implements
            com.facebook.buck.core.rules.attr.[SupportsInputBasedRuleKey](../../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr"))
            -   com.facebook.buck.shell.[[BaseGenrule]{.typeNameLink}](../../shell/BaseGenrule.html "class in com.facebook.buck.shell")\<T\>
                (implements
                com.facebook.buck.core.rules.attr.[HasMultipleOutputs](../../core/rules/attr/HasMultipleOutputs.html "interface in com.facebook.buck.core.rules.attr"),
                com.facebook.buck.core.model.[HasOutputName](../../core/model/HasOutputName.html "interface in com.facebook.buck.core.model"))
                -   com.facebook.buck.jvm.java.[[JarGenrule]{.typeNameLink}](JarGenrule.html "class in com.facebook.buck.jvm.java")
                    (implements
                    com.facebook.buck.core.rules.tool.[BinaryBuildRule](../../core/rules/tool/BinaryBuildRule.html "interface in com.facebook.buck.core.rules.tool"))
            -   com.facebook.buck.jvm.java.[[CalculateClassAbi]{.typeNameLink}](CalculateClassAbi.html "class in com.facebook.buck.jvm.java")
                (implements
                com.facebook.buck.jvm.core.[CalculateAbi](../core/CalculateAbi.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.core.rules.attr.[InitializableFromDisk](../../core/rules/attr/InitializableFromDisk.html "interface in com.facebook.buck.core.rules.attr")\<T\>)
            -   com.facebook.buck.jvm.java.[[CalculateSourceAbiFromLibraryTarget]{.typeNameLink}](CalculateSourceAbiFromLibraryTarget.html "class in com.facebook.buck.jvm.java")
                (implements
                com.facebook.buck.jvm.core.[CalculateAbi](../core/CalculateAbi.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.core.rules.attr.[InitializableFromDisk](../../core/rules/attr/InitializableFromDisk.html "interface in com.facebook.buck.core.rules.attr")\<T\>)
            -   com.facebook.buck.rules.modern.[[PipelinedModernBuildRule]{.typeNameLink}](../../rules/modern/PipelinedModernBuildRule.html "class in com.facebook.buck.rules.modern")\<State,​T\>
                (implements
                com.facebook.buck.core.rules.pipeline.[SupportsPipelining](../../core/rules/pipeline/SupportsPipelining.html "interface in com.facebook.buck.core.rules.pipeline")\<T\>)
                -   com.facebook.buck.jvm.java.[[CalculateSourceAbi]{.typeNameLink}](CalculateSourceAbi.html "class in com.facebook.buck.jvm.java")
                    (implements
                    com.facebook.buck.jvm.core.[CalculateAbi](../core/CalculateAbi.html "interface in com.facebook.buck.jvm.core"),
                    com.facebook.buck.core.rules.attr.[InitializableFromDisk](../../core/rules/attr/InitializableFromDisk.html "interface in com.facebook.buck.core.rules.attr")\<T\>,
                    com.facebook.buck.core.rules.attr.[SupportsDependencyFileRuleKey](../../core/rules/attr/SupportsDependencyFileRuleKey.html "interface in com.facebook.buck.core.rules.attr"))
                -   com.facebook.buck.jvm.java.[[DefaultJavaLibrary]{.typeNameLink}](DefaultJavaLibrary.html "class in com.facebook.buck.jvm.java")
                    (implements
                    com.facebook.buck.android.packageable.[AndroidPackageable](../../android/packageable/AndroidPackageable.html "interface in com.facebook.buck.android.packageable"),
                    com.facebook.buck.core.rules.attr.[ExportDependencies](../../core/rules/attr/ExportDependencies.html "interface in com.facebook.buck.core.rules.attr"),
                    com.facebook.buck.core.rules.attr.[InitializableFromDisk](../../core/rules/attr/InitializableFromDisk.html "interface in com.facebook.buck.core.rules.attr")\<T\>,
                    com.facebook.buck.jvm.core.[JavaLibrary](../core/JavaLibrary.html "interface in com.facebook.buck.jvm.core"),
                    com.facebook.buck.jvm.java.[JavaLibraryWithTests](JavaLibraryWithTests.html "interface in com.facebook.buck.jvm.java"),
                    com.facebook.buck.jvm.java.[MaybeRequiredForSourceOnlyAbi](MaybeRequiredForSourceOnlyAbi.html "interface in com.facebook.buck.jvm.java"),
                    com.facebook.buck.core.rules.attr.[SupportsDependencyFileRuleKey](../../core/rules/attr/SupportsDependencyFileRuleKey.html "interface in com.facebook.buck.core.rules.attr"))
    -   com.facebook.buck.shell.[[AbstractGenruleDescription]{.typeNameLink}](../../shell/AbstractGenruleDescription.html "class in com.facebook.buck.shell")\<T\>
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>)
        -   com.facebook.buck.jvm.java.[[JarGenruleDescription]{.typeNameLink}](JarGenruleDescription.html "class in com.facebook.buck.jvm.java")
            (implements
            com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>)
    -   com.facebook.buck.jvm.java.[[AccumulateClassNamesStep]{.typeNameLink}](AccumulateClassNamesStep.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.step.[Step](../../step/Step.html "interface in com.facebook.buck.step"))
    -   com.facebook.buck.jvm.java.[[CalculateClassAbiStep]{.typeNameLink}](CalculateClassAbiStep.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.step.[Step](../../step/Step.html "interface in com.facebook.buck.step"))
    -   com.facebook.buck.jvm.java.[[CalculateSourceAbi.SourceAbiBuildable]{.typeNameLink}](CalculateSourceAbi.SourceAbiBuildable.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.rules.modern.[PipelinedBuildable](../../rules/modern/PipelinedBuildable.html "interface in com.facebook.buck.rules.modern")\<State\>)
    -   com.facebook.buck.jvm.java.[[ClasspathChecker]{.typeNameLink}](ClasspathChecker.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[CompilerOutputPaths]{.typeNameLink}](CompilerOutputPaths.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[CompilerParameters]{.typeNameLink}](CompilerParameters.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[CompileToJarStepFactory]{.typeNameLink}](CompileToJarStepFactory.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"))
        -   com.facebook.buck.jvm.java.[[JavacToJarStepFactory]{.typeNameLink}](JavacToJarStepFactory.html "class in com.facebook.buck.jvm.java")
            (implements
            com.facebook.buck.core.rulekey.[AddsToRuleKey](../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"))
    -   com.facebook.buck.jvm.java.[[ConfiguredCompilerFactory]{.typeNameLink}](ConfiguredCompilerFactory.html "class in com.facebook.buck.jvm.java")
        -   com.facebook.buck.jvm.java.[[JavaConfiguredCompilerFactory]{.typeNameLink}](JavaConfiguredCompilerFactory.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[ConstantJavacProvider]{.typeNameLink}](ConstantJavacProvider.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"),
        com.facebook.buck.jvm.java.[JavacProvider](JavacProvider.html "interface in com.facebook.buck.jvm.java"))
    -   com.facebook.buck.jvm.java.[[CopyResourcesStep]{.typeNameLink}](CopyResourcesStep.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.step.[Step](../../step/Step.html "interface in com.facebook.buck.step"))
    -   com.facebook.buck.jvm.java.[[DefaultClassUsageFileWriter]{.typeNameLink}](DefaultClassUsageFileWriter.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.jvm.java.[ClassUsageFileWriter](ClassUsageFileWriter.html "interface in com.facebook.buck.jvm.java"))
    -   com.facebook.buck.jvm.java.[[DefaultJavaClassHashesProvider]{.typeNameLink}](DefaultJavaClassHashesProvider.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.jvm.core.[JavaClassHashesProvider](../core/JavaClassHashesProvider.html "interface in com.facebook.buck.jvm.core"))
    -   com.facebook.buck.jvm.java.[[DefaultJavaLibraryRules]{.typeNameLink}](DefaultJavaLibraryRules.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[DefaultJavaPackageFinder]{.typeNameLink}](DefaultJavaPackageFinder.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.jvm.core.[JavaPackageFinder](../core/JavaPackageFinder.html "interface in com.facebook.buck.jvm.core"))
    -   com.facebook.buck.jvm.java.[[DiagnosticCleaner]{.typeNameLink}](DiagnosticCleaner.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[DiagnosticPrettyPrinter]{.typeNameLink}](DiagnosticPrettyPrinter.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[DiffAbisStep]{.typeNameLink}](DiffAbisStep.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.step.[Step](../../step/Step.html "interface in com.facebook.buck.step"))
    -   com.facebook.buck.jvm.java.[[ExternalJavac]{.typeNameLink}](ExternalJavac.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.jvm.java.[Javac](Javac.html "interface in com.facebook.buck.jvm.java"))
    -   com.facebook.buck.jvm.java.[[ExternalJavacProvider]{.typeNameLink}](ExternalJavacProvider.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.jvm.java.[JavacProvider](JavacProvider.html "interface in com.facebook.buck.jvm.java"))
    -   com.facebook.buck.jvm.java.[[ExtraClasspathProvider.EmptyExtraClasspathProvider]{.typeNameLink}](ExtraClasspathProvider.EmptyExtraClasspathProvider.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.jvm.java.[ExtraClasspathProvider](ExtraClasspathProvider.html "interface in com.facebook.buck.jvm.java"))
    -   com.facebook.buck.jvm.java.[[FatJar]{.typeNameLink}](FatJar.html "class in com.facebook.buck.jvm.java")
        (implements
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink})
    -   com.facebook.buck.jvm.java.[[FatJarMain]{.typeNameLink}](FatJarMain.html "class in com.facebook.buck.jvm.java")
    -   javax.tools.[[ForwardingJavaFileManager]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/javax/tools/ForwardingJavaFileManager.html?is-external=true "class or interface in javax.tools"){.externalLink}\<M\>
        (implements
        javax.tools.[JavaFileManager](http://docs.oracle.com/javase/7/docs/api/javax/tools/JavaFileManager.html?is-external=true "class or interface in javax.tools"){.externalLink})
        -   com.facebook.buck.jvm.java.[[ForwardingStandardJavaFileManager]{.typeNameLink}](ForwardingStandardJavaFileManager.html "class in com.facebook.buck.jvm.java")
            (implements
            javax.tools.[StandardJavaFileManager](http://docs.oracle.com/javase/7/docs/api/javax/tools/StandardJavaFileManager.html?is-external=true "class or interface in javax.tools"){.externalLink})
            -   com.facebook.buck.jvm.java.[[PluginLoaderJavaFileManager]{.typeNameLink}](PluginLoaderJavaFileManager.html "class in com.facebook.buck.jvm.java")
                (implements
                javax.tools.[StandardJavaFileManager](http://docs.oracle.com/javase/7/docs/api/javax/tools/StandardJavaFileManager.html?is-external=true "class or interface in javax.tools"){.externalLink})
        -   com.facebook.buck.jvm.java.[[JavaInMemoryFileManager]{.typeNameLink}](JavaInMemoryFileManager.html "class in com.facebook.buck.jvm.java")
            (implements
            javax.tools.[StandardJavaFileManager](http://docs.oracle.com/javase/7/docs/api/javax/tools/StandardJavaFileManager.html?is-external=true "class or interface in javax.tools"){.externalLink})
    -   com.facebook.buck.jvm.java.ImmutableCompilerParameters.Builder
        -   com.facebook.buck.jvm.java.[[CompilerParameters.Builder]{.typeNameLink}](CompilerParameters.Builder.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.ImmutableDefaultJavaLibraryRules.Builder
        -   com.facebook.buck.jvm.java.[[DefaultJavaLibraryRules.Builder]{.typeNameLink}](DefaultJavaLibraryRules.Builder.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.ImmutableJarParameters.Builder
        -   com.facebook.buck.jvm.java.[[JarParameters.Builder]{.typeNameLink}](JarParameters.Builder.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.ImmutableJavacLanguageLevelOptions.Builder
        -   com.facebook.buck.jvm.java.[[JavacLanguageLevelOptions.Builder]{.typeNameLink}](JavacLanguageLevelOptions.Builder.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.ImmutableJavacOptions.Builder
        -   com.facebook.buck.jvm.java.[[JavacOptions.Builder]{.typeNameLink}](JavacOptions.Builder.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.ImmutableJavacPluginParams.Builder
        -   com.facebook.buck.jvm.java.[[JavacPluginParams.Builder]{.typeNameLink}](JavacPluginParams.Builder.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.ImmutableJavacSpec.Builder
        -   com.facebook.buck.jvm.java.[[JavacSpec.Builder]{.typeNameLink}](JavacSpec.Builder.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.ImmutableJavaLibraryDeps.Builder
        -   com.facebook.buck.jvm.java.[[JavaLibraryDeps.Builder]{.typeNameLink}](JavaLibraryDeps.Builder.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[JacocoConstants]{.typeNameLink}](JacocoConstants.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[JarBackedJavacProvider]{.typeNameLink}](JarBackedJavacProvider.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"),
        com.facebook.buck.jvm.java.[JavacProvider](JavacProvider.html "interface in com.facebook.buck.jvm.java"))
    -   com.facebook.buck.jvm.java.[[JarBuildStepsFactory]{.typeNameLink}](JarBuildStepsFactory.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"),
        com.facebook.buck.core.rules.pipeline.[RulePipelineStateFactory](../../core/rules/pipeline/RulePipelineStateFactory.html "interface in com.facebook.buck.core.rules.pipeline")\<T\>)
    -   com.facebook.buck.jvm.java.[[JarBuildStepsFactory.JavaDependencyInfo]{.typeNameLink}](JarBuildStepsFactory.JavaDependencyInfo.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"))
    -   com.facebook.buck.jvm.java.[[JarDiffer]{.typeNameLink}](JarDiffer.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[JarDirectoryStep]{.typeNameLink}](JarDirectoryStep.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.step.[Step](../../step/Step.html "interface in com.facebook.buck.step"))
    -   com.facebook.buck.jvm.java.[[JarDumper]{.typeNameLink}](JarDumper.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[JarFileObject]{.typeNameLink}](JarFileObject.html "class in com.facebook.buck.jvm.java")
        (implements
        javax.tools.[JavaFileObject](http://docs.oracle.com/javase/7/docs/api/javax/tools/JavaFileObject.html?is-external=true "class or interface in javax.tools"){.externalLink})
        -   com.facebook.buck.jvm.java.[[JavaInMemoryFileObject]{.typeNameLink}](JavaInMemoryFileObject.html "class in com.facebook.buck.jvm.java")
        -   com.facebook.buck.jvm.java.[[JavaNoOpFileObject]{.typeNameLink}](JavaNoOpFileObject.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[JarGenruleDescriptionArg]{.typeNameLink}](JarGenruleDescriptionArg.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[JarGenruleDescriptionArg.Builder]{.typeNameLink}](JarGenruleDescriptionArg.Builder.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[JarParameters]{.typeNameLink}](JarParameters.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[JarShape.Summary]{.typeNameLink}](JarShape.Summary.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[JavaAnnotationProcessorDescription]{.typeNameLink}](JavaAnnotationProcessorDescription.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.versions.[VersionPropagator](../../versions/VersionPropagator.html "interface in com.facebook.buck.versions")\<A\>)
    -   com.facebook.buck.jvm.java.[[JavaAnnotationProcessorDescriptionArg]{.typeNameLink}](JavaAnnotationProcessorDescriptionArg.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[JavaAnnotationProcessorDescriptionArg.Builder]{.typeNameLink}](JavaAnnotationProcessorDescriptionArg.Builder.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[JavaBinaryDescription]{.typeNameLink}](JavaBinaryDescription.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>,
        com.facebook.buck.versions.[VersionRoot](../../versions/VersionRoot.html "interface in com.facebook.buck.versions")\<A\>)
    -   com.facebook.buck.jvm.java.[[JavaBinaryDescriptionArg]{.typeNameLink}](JavaBinaryDescriptionArg.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[JavaBinaryDescriptionArg.Builder]{.typeNameLink}](JavaBinaryDescriptionArg.Builder.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[JavaBuckConfig]{.typeNameLink}](JavaBuckConfig.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.core.config.[ConfigView](../../core/config/ConfigView.html "interface in com.facebook.buck.core.config")\<T\>)
    -   com.facebook.buck.jvm.java.[[JavacErrorParser]{.typeNameLink}](JavacErrorParser.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[JavacEventSinkScopedSimplePerfEvent]{.typeNameLink}](JavacEventSinkScopedSimplePerfEvent.html "class in com.facebook.buck.jvm.java")
        (implements
        java.lang.[AutoCloseable](http://docs.oracle.com/javase/7/docs/api/java/lang/AutoCloseable.html?is-external=true "class or interface in java.lang"){.externalLink})
    -   com.facebook.buck.jvm.java.[[JavacEventSinkToBuckEventBusBridge]{.typeNameLink}](JavacEventSinkToBuckEventBusBridge.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.jvm.java.[JavacEventSink](JavacEventSink.html "interface in com.facebook.buck.jvm.java"))
    -   com.facebook.buck.jvm.java.[[JavacFactory]{.typeNameLink}](JavacFactory.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[JavacLanguageLevelOptions]{.typeNameLink}](JavacLanguageLevelOptions.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"))
    -   com.facebook.buck.jvm.java.[[JavacOptions]{.typeNameLink}](JavacOptions.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"))
    -   com.facebook.buck.jvm.java.[[JavacOptionsFactory]{.typeNameLink}](JavacOptionsFactory.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[JavacPipelineState]{.typeNameLink}](JavacPipelineState.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.core.rules.pipeline.[RulePipelineState](../../core/rules/pipeline/RulePipelineState.html "interface in com.facebook.buck.core.rules.pipeline"))
    -   com.facebook.buck.jvm.java.[[JavacPluginJsr199Fields]{.typeNameLink}](JavacPluginJsr199Fields.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[JavacPluginParams]{.typeNameLink}](JavacPluginParams.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"))
    -   com.facebook.buck.jvm.java.[[JavacSpec]{.typeNameLink}](JavacSpec.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[JavacStep]{.typeNameLink}](JavacStep.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.step.[Step](../../step/Step.html "interface in com.facebook.buck.step"))
    -   com.facebook.buck.jvm.java.[[JavaDescriptionsProvider]{.typeNameLink}](JavaDescriptionsProvider.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.core.model.targetgraph.[DescriptionProvider](../../core/model/targetgraph/DescriptionProvider.html "interface in com.facebook.buck.core.model.targetgraph"))
    -   com.facebook.buck.jvm.java.[[JavaFileParser]{.typeNameLink}](JavaFileParser.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[JavaFileParser.JavaFileFeatures]{.typeNameLink}](JavaFileParser.JavaFileFeatures.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[JavaLibraryClasspathProvider]{.typeNameLink}](JavaLibraryClasspathProvider.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[JavaLibraryDeps]{.typeNameLink}](JavaLibraryDeps.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[JavaLibraryDescription]{.typeNameLink}](JavaLibraryDescription.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.model.[Flavored](../../core/model/Flavored.html "interface in com.facebook.buck.core.model"),
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>,
        com.facebook.buck.versions.[VersionPropagator](../../versions/VersionPropagator.html "interface in com.facebook.buck.versions")\<A\>)
    -   com.facebook.buck.jvm.java.[[JavaLibraryDescriptionArg]{.typeNameLink}](JavaLibraryDescriptionArg.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[JavaLibraryDescriptionArg.Builder]{.typeNameLink}](JavaLibraryDescriptionArg.Builder.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[JavaLibraryRules]{.typeNameLink}](JavaLibraryRules.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[JavaOptions]{.typeNameLink}](JavaOptions.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[JavaPaths]{.typeNameLink}](JavaPaths.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[JavaPluginDescription]{.typeNameLink}](JavaPluginDescription.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>)
    -   com.facebook.buck.jvm.java.[[JavaPluginDescriptionArg]{.typeNameLink}](JavaPluginDescriptionArg.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[JavaPluginDescriptionArg.Builder]{.typeNameLink}](JavaPluginDescriptionArg.Builder.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[JavaTestDescription]{.typeNameLink}](JavaTestDescription.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>,
        com.facebook.buck.versions.[VersionRoot](../../versions/VersionRoot.html "interface in com.facebook.buck.versions")\<A\>)
    -   com.facebook.buck.jvm.java.[[JavaTestDescription.CxxLibraryEnhancement]{.typeNameLink}](JavaTestDescription.CxxLibraryEnhancement.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[JavaTestDescriptionArg]{.typeNameLink}](JavaTestDescriptionArg.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[JavaTestDescriptionArg.Builder]{.typeNameLink}](JavaTestDescriptionArg.Builder.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[JavaTestRunnerDescription]{.typeNameLink}](JavaTestRunnerDescription.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>,
        com.facebook.buck.versions.[VersionPropagator](../../versions/VersionPropagator.html "interface in com.facebook.buck.versions")\<A\>)
    -   com.facebook.buck.jvm.java.[[JavaTestRunnerDescriptionArg]{.typeNameLink}](JavaTestRunnerDescriptionArg.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[JavaTestRunnerDescriptionArg.Builder]{.typeNameLink}](JavaTestRunnerDescriptionArg.Builder.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[Jsr199Javac]{.typeNameLink}](Jsr199Javac.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.jvm.java.[Javac](Javac.html "interface in com.facebook.buck.jvm.java"))
        -   com.facebook.buck.jvm.java.[[JarBackedJavac]{.typeNameLink}](JarBackedJavac.html "class in com.facebook.buck.jvm.java")
        -   com.facebook.buck.jvm.java.[[JdkProvidedInMemoryJavac]{.typeNameLink}](JdkProvidedInMemoryJavac.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[Jsr199TracingBridge]{.typeNameLink}](Jsr199TracingBridge.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.event.api.[BuckTracingInterface](../../event/api/BuckTracingInterface.html "interface in com.facebook.buck.event.api"))
    -   com.facebook.buck.jvm.java.[[KeystoreDescription]{.typeNameLink}](KeystoreDescription.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>)
    -   com.facebook.buck.jvm.java.[[KeystoreDescriptionArg]{.typeNameLink}](KeystoreDescriptionArg.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[KeystoreDescriptionArg.Builder]{.typeNameLink}](KeystoreDescriptionArg.Builder.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[LoggingJarBuilderObserver]{.typeNameLink}](LoggingJarBuilderObserver.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.util.zip.[JarBuilder.Observer](../../util/zip/JarBuilder.Observer.html "interface in com.facebook.buck.util.zip"))
    -   com.facebook.buck.jvm.java.[[PluginFactory]{.typeNameLink}](PluginFactory.html "class in com.facebook.buck.jvm.java")
        (implements
        java.lang.[AutoCloseable](http://docs.oracle.com/javase/7/docs/api/java/lang/AutoCloseable.html?is-external=true "class or interface in java.lang"){.externalLink})
    -   com.facebook.buck.jvm.java.[[PrebuiltJarDescription]{.typeNameLink}](PrebuiltJarDescription.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.versions.[VersionPropagator](../../versions/VersionPropagator.html "interface in com.facebook.buck.versions")\<A\>)
    -   com.facebook.buck.jvm.java.[[PrebuiltJarDescriptionArg]{.typeNameLink}](PrebuiltJarDescriptionArg.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[PrebuiltJarDescriptionArg.Builder]{.typeNameLink}](PrebuiltJarDescriptionArg.Builder.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[RemoveClassesPatternsMatcher]{.typeNameLink}](RemoveClassesPatternsMatcher.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"),
        java.util.function.Predicate\<T\>)
    -   com.facebook.buck.jvm.java.[[ResolvedJavacPluginProperties]{.typeNameLink}](ResolvedJavacPluginProperties.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"))
    -   com.facebook.buck.jvm.java.[[ResourcesParameters]{.typeNameLink}](ResourcesParameters.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"))
    -   com.facebook.buck.jvm.java.[[ResourcesRootPackageFinder]{.typeNameLink}](ResourcesRootPackageFinder.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.jvm.core.[JavaPackageFinder](../core/JavaPackageFinder.html "interface in com.facebook.buck.jvm.core"))
    -   com.facebook.buck.shell.[[ShellStep]{.typeNameLink}](../../shell/ShellStep.html "class in com.facebook.buck.shell")
        (implements
        com.facebook.buck.step.[Step](../../step/Step.html "interface in com.facebook.buck.step"))
        -   com.facebook.buck.jvm.java.[[GenerateCodeCoverageReportStep]{.typeNameLink}](GenerateCodeCoverageReportStep.html "class in com.facebook.buck.jvm.java")
        -   com.facebook.buck.jvm.java.[[JUnitStep]{.typeNameLink}](JUnitStep.html "class in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[UnusedDependenciesFinder]{.typeNameLink}](UnusedDependenciesFinder.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.step.[Step](../../step/Step.html "interface in com.facebook.buck.step"))
    -   com.facebook.buck.jvm.java.[[UnusedDependenciesFinderFactory]{.typeNameLink}](UnusedDependenciesFinderFactory.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"))
    -   com.facebook.buck.jvm.java.[[ZipArchiveDependencySupplier]{.typeNameLink}](ZipArchiveDependencySupplier.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.rules.keys.[ArchiveDependencySupplier](../../rules/keys/ArchiveDependencySupplier.html "interface in com.facebook.buck.rules.keys"))
:::

::: {.section role="region"}
## Interface Hierarchy {#interface-hierarchy title="Interface Hierarchy"}

-   com.facebook.buck.core.rulekey.[[AddsToRuleKey]{.typeNameLink}](../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey")
    -   com.facebook.buck.jvm.java.[[ExtraClasspathProvider]{.typeNameLink}](ExtraClasspathProvider.html "interface in com.facebook.buck.jvm.java")
    -   com.facebook.buck.core.toolchain.tool.[[Tool]{.typeNameLink}](../../core/toolchain/tool/Tool.html "interface in com.facebook.buck.core.toolchain.tool")
        -   com.facebook.buck.jvm.java.[[Javac]{.typeNameLink}](Javac.html "interface in com.facebook.buck.jvm.java")
-   com.facebook.buck.core.rulekey.[[AllowsNonAnnotatedFields]{.typeNameLink}](../../core/rulekey/AllowsNonAnnotatedFields.html "interface in com.facebook.buck.core.rulekey")
    -   com.facebook.buck.core.rules.[[BuildRule]{.typeNameLink}](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
        (also extends
        com.facebook.buck.core.build.action.[BuildEngineAction](../../core/build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action"),
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        com.facebook.buck.core.rules.[HasNameAndType](../../core/rules/HasNameAndType.html "interface in com.facebook.buck.core.rules"))
        -   com.facebook.buck.jvm.core.[[HasMavenCoordinates]{.typeNameLink}](../core/HasMavenCoordinates.html "interface in com.facebook.buck.jvm.core")
            -   com.facebook.buck.jvm.java.[[MavenPublishable]{.typeNameLink}](MavenPublishable.html "interface in com.facebook.buck.jvm.java")
        -   com.facebook.buck.jvm.java.[[MaybeRequiredForSourceOnlyAbi]{.typeNameLink}](MaybeRequiredForSourceOnlyAbi.html "interface in com.facebook.buck.jvm.java")
-   java.lang.[[AutoCloseable]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/AutoCloseable.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   com.facebook.buck.jvm.java.[[Javac.Invocation]{.typeNameLink}](Javac.Invocation.html "interface in com.facebook.buck.jvm.java")
-   com.facebook.buck.core.build.action.[[BuildEngineAction]{.typeNameLink}](../../core/build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")
    -   com.facebook.buck.core.rules.[[BuildRule]{.typeNameLink}](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
        (also extends
        com.facebook.buck.core.rulekey.[AllowsNonAnnotatedFields](../../core/rulekey/AllowsNonAnnotatedFields.html "interface in com.facebook.buck.core.rulekey"),
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        com.facebook.buck.core.rules.[HasNameAndType](../../core/rules/HasNameAndType.html "interface in com.facebook.buck.core.rules"))
        -   com.facebook.buck.jvm.core.[[HasMavenCoordinates]{.typeNameLink}](../core/HasMavenCoordinates.html "interface in com.facebook.buck.jvm.core")
            -   com.facebook.buck.jvm.java.[[MavenPublishable]{.typeNameLink}](MavenPublishable.html "interface in com.facebook.buck.jvm.java")
        -   com.facebook.buck.jvm.java.[[MaybeRequiredForSourceOnlyAbi]{.typeNameLink}](MaybeRequiredForSourceOnlyAbi.html "interface in com.facebook.buck.jvm.java")
-   com.facebook.buck.jvm.java.[[ClassUsageFileWriter]{.typeNameLink}](ClassUsageFileWriter.html "interface in com.facebook.buck.jvm.java")
-   java.lang.[[Comparable]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>
    -   com.facebook.buck.core.rules.[[BuildRule]{.typeNameLink}](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
        (also extends
        com.facebook.buck.core.rulekey.[AllowsNonAnnotatedFields](../../core/rulekey/AllowsNonAnnotatedFields.html "interface in com.facebook.buck.core.rulekey"),
        com.facebook.buck.core.build.action.[BuildEngineAction](../../core/build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action"),
        com.facebook.buck.core.rules.[HasNameAndType](../../core/rules/HasNameAndType.html "interface in com.facebook.buck.core.rules"))
        -   com.facebook.buck.jvm.core.[[HasMavenCoordinates]{.typeNameLink}](../core/HasMavenCoordinates.html "interface in com.facebook.buck.jvm.core")
            -   com.facebook.buck.jvm.java.[[MavenPublishable]{.typeNameLink}](MavenPublishable.html "interface in com.facebook.buck.jvm.java")
        -   com.facebook.buck.jvm.java.[[MaybeRequiredForSourceOnlyAbi]{.typeNameLink}](MaybeRequiredForSourceOnlyAbi.html "interface in com.facebook.buck.jvm.java")
-   com.facebook.buck.core.description.arg.[[DataTransferObject]{.typeNameLink}](../../core/description/arg/DataTransferObject.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.core.description.arg.[[ConstructorArg]{.typeNameLink}](../../core/description/arg/ConstructorArg.html "interface in com.facebook.buck.core.description.arg")
        -   com.facebook.buck.core.description.arg.[[BuildRuleArg]{.typeNameLink}](../../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")
            -   com.facebook.buck.jvm.java.[[JavacPluginArgs]{.typeNameLink}](JavacPluginArgs.html "interface in com.facebook.buck.jvm.java")
                (also extends
                com.facebook.buck.core.description.arg.[HasDeclaredDeps](../../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg"))
            -   com.facebook.buck.jvm.java.[[JvmLibraryArg]{.typeNameLink}](JvmLibraryArg.html "interface in com.facebook.buck.jvm.java")
                (also extends
                com.facebook.buck.jvm.java.[MaybeRequiredForSourceOnlyAbiArg](MaybeRequiredForSourceOnlyAbiArg.html "interface in com.facebook.buck.jvm.java"))
                -   com.facebook.buck.jvm.java.[[JavaLibraryDescription.CoreArg]{.typeNameLink}](JavaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.java")
                    (also extends
                    com.facebook.buck.core.description.arg.[HasDeclaredDeps](../../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg"),
                    com.facebook.buck.core.description.arg.[HasProvidedDeps](../../core/description/arg/HasProvidedDeps.html "interface in com.facebook.buck.core.description.arg"),
                    com.facebook.buck.core.description.arg.[HasSrcs](../../core/description/arg/HasSrcs.html "interface in com.facebook.buck.core.description.arg"),
                    com.facebook.buck.core.description.arg.[HasTests](../../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg"))
                    -   com.facebook.buck.jvm.java.[[JavaTestDescription.CoreArg]{.typeNameLink}](JavaTestDescription.CoreArg.html "interface in com.facebook.buck.jvm.java")
                        (also extends
                        com.facebook.buck.core.description.arg.[HasContacts](../../core/description/arg/HasContacts.html "interface in com.facebook.buck.core.description.arg"),
                        com.facebook.buck.core.description.arg.[HasTestTimeout](../../core/description/arg/HasTestTimeout.html "interface in com.facebook.buck.core.description.arg"))
-   com.facebook.buck.jvm.java.[[DefaultJavaLibraryRules.DefaultJavaLibraryConstructor]{.typeNameLink}](DefaultJavaLibraryRules.DefaultJavaLibraryConstructor.html "interface in com.facebook.buck.jvm.java")
-   com.facebook.buck.core.description.arg.[[HasContacts]{.typeNameLink}](../../core/description/arg/HasContacts.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.jvm.java.[[JavaTestDescription.CoreArg]{.typeNameLink}](JavaTestDescription.CoreArg.html "interface in com.facebook.buck.jvm.java")
        (also extends
        com.facebook.buck.core.description.arg.[HasTestTimeout](../../core/description/arg/HasTestTimeout.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.jvm.java.[JavaLibraryDescription.CoreArg](JavaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.java"))
-   com.facebook.buck.core.description.arg.[[HasDeclaredDeps]{.typeNameLink}](../../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.jvm.java.[[JavacPluginArgs]{.typeNameLink}](JavacPluginArgs.html "interface in com.facebook.buck.jvm.java")
        (also extends
        com.facebook.buck.core.description.arg.[BuildRuleArg](../../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg"))
    -   com.facebook.buck.jvm.java.[[JavaLibraryDescription.CoreArg]{.typeNameLink}](JavaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.java")
        (also extends
        com.facebook.buck.core.description.arg.[HasProvidedDeps](../../core/description/arg/HasProvidedDeps.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasSrcs](../../core/description/arg/HasSrcs.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasTests](../../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.jvm.java.[JvmLibraryArg](JvmLibraryArg.html "interface in com.facebook.buck.jvm.java"))
        -   com.facebook.buck.jvm.java.[[JavaTestDescription.CoreArg]{.typeNameLink}](JavaTestDescription.CoreArg.html "interface in com.facebook.buck.jvm.java")
            (also extends
            com.facebook.buck.core.description.arg.[HasContacts](../../core/description/arg/HasContacts.html "interface in com.facebook.buck.core.description.arg"),
            com.facebook.buck.core.description.arg.[HasTestTimeout](../../core/description/arg/HasTestTimeout.html "interface in com.facebook.buck.core.description.arg"))
-   com.facebook.buck.core.rules.[[HasNameAndType]{.typeNameLink}](../../core/rules/HasNameAndType.html "interface in com.facebook.buck.core.rules")
    -   com.facebook.buck.core.rules.[[BuildRule]{.typeNameLink}](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
        (also extends
        com.facebook.buck.core.rulekey.[AllowsNonAnnotatedFields](../../core/rulekey/AllowsNonAnnotatedFields.html "interface in com.facebook.buck.core.rulekey"),
        com.facebook.buck.core.build.action.[BuildEngineAction](../../core/build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action"),
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>)
        -   com.facebook.buck.jvm.core.[[HasMavenCoordinates]{.typeNameLink}](../core/HasMavenCoordinates.html "interface in com.facebook.buck.jvm.core")
            -   com.facebook.buck.jvm.java.[[MavenPublishable]{.typeNameLink}](MavenPublishable.html "interface in com.facebook.buck.jvm.java")
        -   com.facebook.buck.jvm.java.[[MaybeRequiredForSourceOnlyAbi]{.typeNameLink}](MaybeRequiredForSourceOnlyAbi.html "interface in com.facebook.buck.jvm.java")
-   com.facebook.buck.core.description.arg.[[HasProvidedDeps]{.typeNameLink}](../../core/description/arg/HasProvidedDeps.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.jvm.java.[[JavaLibraryDescription.CoreArg]{.typeNameLink}](JavaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.java")
        (also extends
        com.facebook.buck.core.description.arg.[HasDeclaredDeps](../../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasSrcs](../../core/description/arg/HasSrcs.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasTests](../../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.jvm.java.[JvmLibraryArg](JvmLibraryArg.html "interface in com.facebook.buck.jvm.java"))
        -   com.facebook.buck.jvm.java.[[JavaTestDescription.CoreArg]{.typeNameLink}](JavaTestDescription.CoreArg.html "interface in com.facebook.buck.jvm.java")
            (also extends
            com.facebook.buck.core.description.arg.[HasContacts](../../core/description/arg/HasContacts.html "interface in com.facebook.buck.core.description.arg"),
            com.facebook.buck.core.description.arg.[HasTestTimeout](../../core/description/arg/HasTestTimeout.html "interface in com.facebook.buck.core.description.arg"))
-   com.facebook.buck.core.description.arg.[[HasSrcs]{.typeNameLink}](../../core/description/arg/HasSrcs.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.jvm.java.[[JavaLibraryDescription.CoreArg]{.typeNameLink}](JavaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.java")
        (also extends
        com.facebook.buck.core.description.arg.[HasDeclaredDeps](../../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasProvidedDeps](../../core/description/arg/HasProvidedDeps.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasTests](../../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.jvm.java.[JvmLibraryArg](JvmLibraryArg.html "interface in com.facebook.buck.jvm.java"))
        -   com.facebook.buck.jvm.java.[[JavaTestDescription.CoreArg]{.typeNameLink}](JavaTestDescription.CoreArg.html "interface in com.facebook.buck.jvm.java")
            (also extends
            com.facebook.buck.core.description.arg.[HasContacts](../../core/description/arg/HasContacts.html "interface in com.facebook.buck.core.description.arg"),
            com.facebook.buck.core.description.arg.[HasTestTimeout](../../core/description/arg/HasTestTimeout.html "interface in com.facebook.buck.core.description.arg"))
-   com.facebook.buck.core.description.arg.[[HasTests]{.typeNameLink}](../../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.jvm.java.[[JavaLibraryDescription.CoreArg]{.typeNameLink}](JavaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.java")
        (also extends
        com.facebook.buck.core.description.arg.[HasDeclaredDeps](../../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasProvidedDeps](../../core/description/arg/HasProvidedDeps.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasSrcs](../../core/description/arg/HasSrcs.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.jvm.java.[JvmLibraryArg](JvmLibraryArg.html "interface in com.facebook.buck.jvm.java"))
        -   com.facebook.buck.jvm.java.[[JavaTestDescription.CoreArg]{.typeNameLink}](JavaTestDescription.CoreArg.html "interface in com.facebook.buck.jvm.java")
            (also extends
            com.facebook.buck.core.description.arg.[HasContacts](../../core/description/arg/HasContacts.html "interface in com.facebook.buck.core.description.arg"),
            com.facebook.buck.core.description.arg.[HasTestTimeout](../../core/description/arg/HasTestTimeout.html "interface in com.facebook.buck.core.description.arg"))
-   com.facebook.buck.core.description.arg.[[HasTestTimeout]{.typeNameLink}](../../core/description/arg/HasTestTimeout.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.jvm.java.[[JavaTestDescription.CoreArg]{.typeNameLink}](JavaTestDescription.CoreArg.html "interface in com.facebook.buck.jvm.java")
        (also extends
        com.facebook.buck.core.description.arg.[HasContacts](../../core/description/arg/HasContacts.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.jvm.java.[JavaLibraryDescription.CoreArg](JavaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.java"))
-   com.facebook.buck.jvm.java.[[JavacEventSink]{.typeNameLink}](JavacEventSink.html "interface in com.facebook.buck.jvm.java")
-   com.facebook.buck.jvm.java.[[JavacExecutionContext]{.typeNameLink}](JavacExecutionContext.html "interface in com.facebook.buck.jvm.java")
-   com.facebook.buck.jvm.java.[[JavacProvider]{.typeNameLink}](JavacProvider.html "interface in com.facebook.buck.jvm.java")
-   com.facebook.buck.jvm.java.[[JavaLibraryWithTests]{.typeNameLink}](JavaLibraryWithTests.html "interface in com.facebook.buck.jvm.java")
-   com.facebook.buck.jvm.java.[[JavaTest.AdditionalClasspathEntriesProvider]{.typeNameLink}](JavaTest.AdditionalClasspathEntriesProvider.html "interface in com.facebook.buck.jvm.java")
-   com.facebook.buck.jvm.java.[[MaybeRequiredForSourceOnlyAbiArg]{.typeNameLink}](MaybeRequiredForSourceOnlyAbiArg.html "interface in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[JvmLibraryArg]{.typeNameLink}](JvmLibraryArg.html "interface in com.facebook.buck.jvm.java")
        (also extends
        com.facebook.buck.core.description.arg.[BuildRuleArg](../../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg"))
        -   com.facebook.buck.jvm.java.[[JavaLibraryDescription.CoreArg]{.typeNameLink}](JavaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.java")
            (also extends
            com.facebook.buck.core.description.arg.[HasDeclaredDeps](../../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg"),
            com.facebook.buck.core.description.arg.[HasProvidedDeps](../../core/description/arg/HasProvidedDeps.html "interface in com.facebook.buck.core.description.arg"),
            com.facebook.buck.core.description.arg.[HasSrcs](../../core/description/arg/HasSrcs.html "interface in com.facebook.buck.core.description.arg"),
            com.facebook.buck.core.description.arg.[HasTests](../../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg"))
            -   com.facebook.buck.jvm.java.[[JavaTestDescription.CoreArg]{.typeNameLink}](JavaTestDescription.CoreArg.html "interface in com.facebook.buck.jvm.java")
                (also extends
                com.facebook.buck.core.description.arg.[HasContacts](../../core/description/arg/HasContacts.html "interface in com.facebook.buck.core.description.arg"),
                com.facebook.buck.core.description.arg.[HasTestTimeout](../../core/description/arg/HasTestTimeout.html "interface in com.facebook.buck.core.description.arg"))
-   com.facebook.buck.jvm.java.[[OptionsConsumer]{.typeNameLink}](OptionsConsumer.html "interface in com.facebook.buck.jvm.java")
-   com.facebook.buck.jvm.java.[[StandardJavaFileManagerFactory]{.typeNameLink}](StandardJavaFileManagerFactory.html "interface in com.facebook.buck.jvm.java")
:::

::: {.section role="region"}
## Annotation Type Hierarchy {#annotation-type-hierarchy title="Annotation Type Hierarchy"}

-   com.facebook.buck.jvm.java.[[BuildsAnnotationProcessor]{.typeNameLink}](BuildsAnnotationProcessor.html "annotation in com.facebook.buck.jvm.java")
    (implements
    java.lang.annotation.[Annotation](http://docs.oracle.com/javase/7/docs/api/java/lang/annotation/Annotation.html?is-external=true "class or interface in java.lang.annotation"){.externalLink})
:::

::: {.section role="region"}
## Enum Hierarchy {#enum-hierarchy title="Enum Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   java.lang.[[Enum]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<E\>
        (implements
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   com.facebook.buck.jvm.java.[[AnnotationProcessingEvent.Operation]{.typeNameLink}](AnnotationProcessingEvent.Operation.html "enum in com.facebook.buck.jvm.java")
        -   com.facebook.buck.jvm.java.[[BuiltInJavac]{.typeNameLink}](BuiltInJavac.html "enum in com.facebook.buck.jvm.java")
        -   com.facebook.buck.jvm.java.[[CompileAgainstLibraryType]{.typeNameLink}](CompileAgainstLibraryType.html "enum in com.facebook.buck.jvm.java")
        -   com.facebook.buck.jvm.java.[[ForkMode]{.typeNameLink}](ForkMode.html "enum in com.facebook.buck.jvm.java")
        -   com.facebook.buck.jvm.java.[[JarShape]{.typeNameLink}](JarShape.html "enum in com.facebook.buck.jvm.java")
        -   com.facebook.buck.jvm.java.[[JavaBuckConfig.DuplicatesLogLevel]{.typeNameLink}](JavaBuckConfig.DuplicatesLogLevel.html "enum in com.facebook.buck.jvm.java")
        -   com.facebook.buck.jvm.java.[[JavaBuckConfig.SourceAbiVerificationMode]{.typeNameLink}](JavaBuckConfig.SourceAbiVerificationMode.html "enum in com.facebook.buck.jvm.java")
        -   com.facebook.buck.jvm.java.[[JavaBuckConfig.UnusedDependenciesAction]{.typeNameLink}](JavaBuckConfig.UnusedDependenciesAction.html "enum in com.facebook.buck.jvm.java")
        -   com.facebook.buck.jvm.java.[[JavaBuckConfig.UnusedDependenciesConfig]{.typeNameLink}](JavaBuckConfig.UnusedDependenciesConfig.html "enum in com.facebook.buck.jvm.java")
        -   com.facebook.buck.jvm.java.[[Javac.Source]{.typeNameLink}](Javac.Source.html "enum in com.facebook.buck.jvm.java")
        -   com.facebook.buck.jvm.java.[[JavacOptions.SpoolMode]{.typeNameLink}](JavacOptions.SpoolMode.html "enum in com.facebook.buck.jvm.java")
        -   com.facebook.buck.jvm.java.[[TestType]{.typeNameLink}](TestType.html "enum in com.facebook.buck.jvm.java")
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
-   Tree
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

[]{#skip.navbar.bottom}
:::
