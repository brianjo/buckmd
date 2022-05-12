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

## Class JarBuildStepsFactory {#class-jarbuildstepsfactory .title title="Class JarBuildStepsFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.JarBuildStepsFactory

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`, `RulePipelineStateFactory<JavacPipelineState>`

    ------------------------------------------------------------------------

        public class JarBuildStepsFactory
        extends Object
        implements AddsToRuleKey, RulePipelineStateFactory<JavacPipelineState>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `JarBuildStepsFactor  | ::: block             |
        |                       | y.JavaDependencyInfo` | Contains information  |
        |                       |                       | about a Java          |
        |                       |                       | classpath dependency. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `JarBuildStepsFactory​(BuildTarget libraryTarget,                     CompileToJarStepFactory configuredCompiler,                     com.google.common.collect.ImmutableSortedSet<SourcePath> srcs,                     com.google.common.collect.ImmutableSortedSet<SourcePath> resources,                     ResourcesParameters resourcesParameters,                     Optional<SourcePath> manifestFile,                     com.google.common.collect.ImmutableList<String> postprocessClassesCommands,                     boolean trackClassUsage,                     boolean trackJavacPhaseEvents,                     RemoveClassesPatternsMatcher classesToRemoveFromJar,                     AbiGenerationMode abiGenerationMode,                     AbiGenerationMode abiCompatibilityMode,                     com.google.common.collect.ImmutableList<JarBuildStepsFactory.JavaDependencyInfo> dependencyInfos,                     boolean isRequiredForSourceOnlyAbi)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected Opt        | `getAbiJarParameters​( |                       |
        | ional<JarParameters>` | BuildTarget target,   |                       |
        |                       |                   Bui |                       |
        |                       | ldContext context,    |                       |
        |                       |                  Proj |                       |
        |                       | ectFilesystem filesys |                       |
        |                       | tem,                  |                       |
        |                       |    CompilerParameters |                       |
        |                       |  compilerParameters)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.                 | `getBuildStepsForAb   |                       |
        | google.common.collect | iJar​(BuildContext con |                       |
        | .ImmutableList<Step>` | text,                 |                       |
        |                       |        ProjectFilesys |                       |
        |                       | tem filesystem,       |                       |
        |                       |                  Reco |                       |
        |                       | rdArtifactVerifier bu |                       |
        |                       | ildableContext,       |                       |
        |                       |                  Buil |                       |
        |                       | dTarget buildTarget)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.                 | `                     |                       |
        | google.common.collect | getBuildStepsForLibra |                       |
        | .ImmutableList<Step>` | ryJar​(BuildContext co |                       |
        |                       | ntext,                |                       |
        |                       |             ProjectFi |                       |
        |                       | lesystem filesystem,  |                       |
        |                       |                       |                       |
        |                       |      RecordArtifactVe |                       |
        |                       | rifier buildableConte |                       |
        |                       | xt,                   |                       |
        |                       |          BuildTarget  |                       |
        |                       | buildTarget,          |                       |
        |                       |                   Pat |                       |
        |                       | h pathToClassHashes)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protecte             | `getCompilerPara      |                       |
        | d CompilerParameters` | meters​(BuildContext c |                       |
        |                       | ontext,               |                       |
        |                       |         ProjectFilesy |                       |
        |                       | stem filesystem,      |                       |
        |                       |                  Buil |                       |
        |                       | dTarget buildTarget)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.comm      | `getCompileTimeCl     |                       |
        | on.collect.ImmutableS | asspathSourcePaths()` |                       |
        | ortedSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `java.util.function.P | `getCoveredByDepFileP | ::: block             |
        | redicate<SourcePath>` | redicate​(SourcePathRu | Returns a predicate   |
        |                       | leFinder ruleFinder)` | indicating whether a  |
        |                       |                       | SourcePath is covered |
        |                       |                       | by the depfile.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `java.util.function.P | `getExistenceO        |                       |
        | redicate<SourcePath>` | fInterestPredicate()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getInputsAfterBuil   |                       |
        | .common.collect.Immut | dingLocally​(BuildCont |                       |
        | ableList<SourcePath>` | ext context,          |                       |
        |                       |                       |                       |
        |                       | ProjectFilesystem fil |                       |
        |                       | esystem,              |                       |
        |                       |                  Sour |                       |
        |                       | cePathRuleFinder rule |                       |
        |                       | Finder,               |                       |
        |                       |                 CellP |                       |
        |                       | athResolver cellPathR |                       |
        |                       | esolver,              |                       |
        |                       |                  Buil |                       |
        |                       | dTarget buildTarget)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected Opt        | `getLibraryJarP       |                       |
        | ional<JarParameters>` | arameters​(BuildContex |                       |
        |                       | t context,            |                       |
        |                       |              ProjectF |                       |
        |                       | ilesystem filesystem, |                       |
        |                       |                       |                       |
        |                       |    CompilerParameters |                       |
        |                       |  compilerParameters)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.                 | `getPip               |                       |
        | google.common.collect | elinedBuildStepsForAb |                       |
        | .ImmutableList<Step>` | iJar​(BuildTarget buil |                       |
        |                       | dTarget,              |                       |
        |                       |                    Bu |                       |
        |                       | ildContext context,   |                       |
        |                       |                       |                       |
        |                       |          ProjectFiles |                       |
        |                       | ystem filesystem,     |                       |
        |                       |                       |                       |
        |                       |        RecordArtifact |                       |
        |                       | Verifier buildableCon |                       |
        |                       | text,                 |                       |
        |                       |                 Javac |                       |
        |                       | PipelineState state)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.                 | `getP                 |                       |
        | google.common.collect | ipelinedBuildStepsFor |                       |
        | .ImmutableList<Step>` | LibraryJar​(BuildConte |                       |
        |                       | xt context,           |                       |
        |                       |                       |                       |
        |                       |      ProjectFilesyste |                       |
        |                       | m filesystem,         |                       |
        |                       |                       |                       |
        |                       |        RecordArtifact |                       |
        |                       | Verifier buildableCon |                       |
        |                       | text,                 |                       |
        |                       |                     J |                       |
        |                       | avacPipelineState sta |                       |
        |                       | te,                   |                       |
        |                       |                   Pat |                       |
        |                       | h pathToClassHashes)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.comm      | `getResources()`      |                       |
        | on.collect.ImmutableS |                       |                       |
        | ortedSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected            | `getR                 |                       |
        |  ResourcesParameters` | esourcesParameters()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getResourcesRoot()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getSou               |                       |
        |                       | rcePathToGeneratedAnn |                       |
        |                       | otationPath​(BuildTarg |                       |
        |                       | et buildTarget,       |                       |
        |                       |                       |                       |
        |                       |             ProjectFi |                       |
        |                       | lesystem filesystem)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getSourcePathT       |                       |
        |                       | oOutput​(BuildTarget b |                       |
        |                       | uildTarget,           |                       |
        |                       |             ProjectFi |                       |
        |                       | lesystem filesystem)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.comm      | `getSources()`        |                       |
        | on.collect.ImmutableS |                       |                       |
        | ortedSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `hasAn                |                       |
        |                       | notationProcessing()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `JavacPipelineState`  | `newI                 |                       |
        |                       | nstance​(BuildContext  |                       |
        |                       | context,            P |                       |
        |                       | rojectFilesystem file |                       |
        |                       | system,            Bu |                       |
        |                       | ildTarget firstRule)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `producesJar()`       |                       |
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

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.jvm.java.CompileToJarStepFactory,com.google.common.collect.ImmutableSortedSet,com.google.common.collect.ImmutableSortedSet,com.facebook.buck.jvm.java.ResourcesParameters,java.util.Optional,com.google.common.collect.ImmutableList,boolean,boolean,com.facebook.buck.jvm.java.RemoveClassesPatternsMatcher,com.facebook.buck.jvm.java.abi.AbiGenerationMode,com.facebook.buck.jvm.java.abi.AbiGenerationMode,com.google.common.collect.ImmutableList,boolean)}

        -   #### JarBuildStepsFactory

                public JarBuildStepsFactory​(BuildTarget libraryTarget,
                                            CompileToJarStepFactory configuredCompiler,
                                            com.google.common.collect.ImmutableSortedSet<SourcePath> srcs,
                                            com.google.common.collect.ImmutableSortedSet<SourcePath> resources,
                                            ResourcesParameters resourcesParameters,
                                            Optional<SourcePath> manifestFile,
                                            com.google.common.collect.ImmutableList<String> postprocessClassesCommands,
                                            boolean trackClassUsage,
                                            boolean trackJavacPhaseEvents,
                                            RemoveClassesPatternsMatcher classesToRemoveFromJar,
                                            AbiGenerationMode abiGenerationMode,
                                            AbiGenerationMode abiCompatibilityMode,
                                            com.google.common.collect.ImmutableList<JarBuildStepsFactory.JavaDependencyInfo> dependencyInfos,
                                            boolean isRequiredForSourceOnlyAbi)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#producesJar()}

        -   #### producesJar

            ``` methodSignature
            public boolean producesJar()
            ```

        []{#getSources()}

        -   #### getSources

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<SourcePath> getSources()
            ```

        []{#getResources()}

        -   #### getResources

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<SourcePath> getResources()
            ```

        []{#getResourcesRoot()}

        -   #### getResourcesRoot

            ``` methodSignature
            public Optional<String> getResourcesRoot()
            ```

        []{#getSourcePathToOutput(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### getSourcePathToOutput

            ``` methodSignature
            @Nullable
            public SourcePath getSourcePathToOutput​(BuildTarget buildTarget,
                                                    ProjectFilesystem filesystem)
            ```

        []{#getSourcePathToGeneratedAnnotationPath(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### getSourcePathToGeneratedAnnotationPath

            ``` methodSignature
            @Nullable
            public SourcePath getSourcePathToGeneratedAnnotationPath​(BuildTarget buildTarget,
                                                                     ProjectFilesystem filesystem)
            ```

        []{#getCompileTimeClasspathSourcePaths()}

        -   #### getCompileTimeClasspathSourcePaths

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<SourcePath> getCompileTimeClasspathSourcePaths()
            ```

        []{#useDependencyFileRuleKeys()}

        -   #### useDependencyFileRuleKeys

            ``` methodSignature
            public boolean useDependencyFileRuleKeys()
            ```

        []{#getCoveredByDepFilePredicate(com.facebook.buck.core.rules.SourcePathRuleFinder)}

        -   #### getCoveredByDepFilePredicate

            ``` methodSignature
            public java.util.function.Predicate<SourcePath> getCoveredByDepFilePredicate​(SourcePathRuleFinder ruleFinder)
            ```

            ::: block
            Returns a predicate indicating whether a SourcePath is
            covered by the depfile.
            :::

        []{#getExistenceOfInterestPredicate()}

        -   #### getExistenceOfInterestPredicate

            ``` methodSignature
            public java.util.function.Predicate<SourcePath> getExistenceOfInterestPredicate()
            ```

        []{#useRulePipelining()}

        -   #### useRulePipelining

            ``` methodSignature
            public boolean useRulePipelining()
            ```

        []{#getBuildStepsForAbiJar(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.common.RecordArtifactVerifier,com.facebook.buck.core.model.BuildTarget)}

        -   #### getBuildStepsForAbiJar

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Step> getBuildStepsForAbiJar​(BuildContext context,
                                                                                        ProjectFilesystem filesystem,
                                                                                        RecordArtifactVerifier buildableContext,
                                                                                        BuildTarget buildTarget)
            ```

        []{#getPipelinedBuildStepsForAbiJar(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.common.RecordArtifactVerifier,com.facebook.buck.jvm.java.JavacPipelineState)}

        -   #### getPipelinedBuildStepsForAbiJar

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Step> getPipelinedBuildStepsForAbiJar​(BuildTarget buildTarget,
                                                                                                 BuildContext context,
                                                                                                 ProjectFilesystem filesystem,
                                                                                                 RecordArtifactVerifier buildableContext,
                                                                                                 JavacPipelineState state)
            ```

        []{#getBuildStepsForLibraryJar(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.common.RecordArtifactVerifier,com.facebook.buck.core.model.BuildTarget,java.nio.file.Path)}

        -   #### getBuildStepsForLibraryJar

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Step> getBuildStepsForLibraryJar​(BuildContext context,
                                                                                            ProjectFilesystem filesystem,
                                                                                            RecordArtifactVerifier buildableContext,
                                                                                            BuildTarget buildTarget,
                                                                                            Path pathToClassHashes)
            ```

        []{#getPipelinedBuildStepsForLibraryJar(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.common.RecordArtifactVerifier,com.facebook.buck.jvm.java.JavacPipelineState,java.nio.file.Path)}

        -   #### getPipelinedBuildStepsForLibraryJar

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Step> getPipelinedBuildStepsForLibraryJar​(BuildContext context,
                                                                                                     ProjectFilesystem filesystem,
                                                                                                     RecordArtifactVerifier buildableContext,
                                                                                                     JavacPipelineState state,
                                                                                                     Path pathToClassHashes)
            ```

        []{#getCompilerParameters(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget)}

        -   #### getCompilerParameters

            ``` methodSignature
            protected CompilerParameters getCompilerParameters​(BuildContext context,
                                                               ProjectFilesystem filesystem,
                                                               BuildTarget buildTarget)
            ```

        []{#getResourcesParameters()}

        -   #### getResourcesParameters

            ``` methodSignature
            protected ResourcesParameters getResourcesParameters()
            ```

        []{#getLibraryJarParameters(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.jvm.java.CompilerParameters)}

        -   #### getLibraryJarParameters

            ``` methodSignature
            protected Optional<JarParameters> getLibraryJarParameters​(BuildContext context,
                                                                      ProjectFilesystem filesystem,
                                                                      CompilerParameters compilerParameters)
            ```

        []{#getAbiJarParameters(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.jvm.java.CompilerParameters)}

        -   #### getAbiJarParameters

            ``` methodSignature
            protected Optional<JarParameters> getAbiJarParameters​(BuildTarget target,
                                                                  BuildContext context,
                                                                  ProjectFilesystem filesystem,
                                                                  CompilerParameters compilerParameters)
            ```

        []{#getInputsAfterBuildingLocally(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.SourcePathRuleFinder,com.facebook.buck.core.cell.CellPathResolver,com.facebook.buck.core.model.BuildTarget)}

        -   #### getInputsAfterBuildingLocally

            ``` methodSignature
            public com.google.common.collect.ImmutableList<SourcePath> getInputsAfterBuildingLocally​(BuildContext context,
                                                                                                     ProjectFilesystem filesystem,
                                                                                                     SourcePathRuleFinder ruleFinder,
                                                                                                     CellPathResolver cellPathResolver,
                                                                                                     BuildTarget buildTarget)
            ```

        []{#newInstance(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget)}

        -   #### newInstance

            ``` methodSignature
            public JavacPipelineState newInstance​(BuildContext context,
                                                  ProjectFilesystem filesystem,
                                                  BuildTarget firstRule)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `newInstance` in
                interface `RulePipelineStateFactory<JavacPipelineState>`

        []{#hasAnnotationProcessing()}

        -   #### hasAnnotationProcessing

            ``` methodSignature
            public boolean hasAnnotationProcessing()
            ```
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
