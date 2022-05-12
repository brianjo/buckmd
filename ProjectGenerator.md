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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.features.apple.project](package-summary.html)
:::

## Class ProjectGenerator {#class-projectgenerator .title title="Class ProjectGenerator"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.apple.project.ProjectGenerator

::: description
-   

    ------------------------------------------------------------------------

        public class ProjectGenerator
        extends Object

    ::: block
    Generator for xcode project and associated files from a set of
    xcode/ios rules.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `ProjectG             | ::: block             |
        |                       | enerator.FilterFlags` | Filter Flags for      |
        |                       |                       | subdividing           |
        |                       |                       | dependencies          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `ProjectGenerator​(XCodeDescriptions xcodeDescriptions,                 TargetGraph targetGraph,                 AppleDependenciesCache dependenciesCache,                 ProjectGenerationStateCache projGenerationStateCache,                 Set<BuildTarget> initialTargets,                 Cell cell,                 Path outputDirectory,                 String projectName,                 String buildFileName,                 com.facebook.buck.features.apple.project.ProjectGeneratorOptions options,                 RuleKeyConfiguration ruleKeyConfiguration,                 boolean isMainProject,                 Optional<BuildTarget> workspaceTarget,                 com.google.common.collect.ImmutableSet<BuildTarget> targetsInRequiredProjects,                 FocusedModuleTargetMatcher focusModules,                 CxxPlatform defaultCxxPlatform,                 com.google.common.collect.ImmutableSet<Flavor> appleCxxFlavors,                 java.util.function.Function<? super TargetNode<?>,​ActionGraphBuilder> actionGraphBuilderForNode,                 BuckEventBus buckEventBus,                 HalideBuckConfig halideBuckConfig,                 CxxBuckConfig cxxBuckConfig,                 AppleConfig appleConfig,                 SwiftBuckConfig swiftBuckConfig,                 Optional<com.google.common.collect.ImmutableMap<BuildTarget,​TargetNode<?>>> sharedLibraryToBundle)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static com           | `computeS             | ::: block             |
        | .google.common.collec | haredLibrariesToBundl | Generate a mapping    |
        | t.ImmutableMap<BuildT | es​(com.google.common. | from libraries to the |
        | arget,​TargetNode<?>>` | collect.ImmutableSet< | framework bundles     |
        |                       | TargetNode<?>> target | that include them.    |
        |                       | Nodes,                | :::                   |
        |                       |                  Targ |                       |
        |                       | etGraph targetGraph)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `c                    |                       |
        |                       | reateXcodeProjects()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.co | `getBuildTargetTo     |                       |
        | llect.ImmutableMap<Bu | GeneratedTargetMap()` |                       |
        | ildTarget,​PBXTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `get                  |                       |
        | common.collect.Immuta | FilesToCopyInXcode()` |                       |
        | bleList<CopyInXcode>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getGeneratedProject  |                       |
        | ogle.common.collect.I | ToGeneratedTargets()` |                       |
        | mmutableSetMultimap<P |                       |                       |
        | BXProject,​PBXTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getProjectPath()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getRe                |                       |
        | .common.collect.Immut | quiredBuildTargets()` |                       |
        | ableSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `getXcconfigPaths()`  |                       |
        | .google.common.collec |                       |                       |
        | t.ImmutableSet<Path>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `                     |                       |
        |                       | isProjectGenerated()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `parseAllPlatformHe   |                       |
        | static com.google.com | aders​(BuildTarget bui |                       |
        | mon.collect.Immutable | ldTarget,             |                       |
        | Map<Path,​SourcePath>` |             SourcePat |                       |
        |                       | hResolverAdapter sour |                       |
        |                       | cePathResolverAdapter |                       |
        |                       | ,                     |                       |
        |                       |     ProjectFilesystem |                       |
        |                       |  filesystem,          |                       |
        |                       |                com.go |                       |
        |                       | ogle.common.collect.I |                       |
        |                       | mmutableList<SourceSo |                       |
        |                       | rtedSet> platformHead |                       |
        |                       | ers,                  |                       |
        |                       |        boolean export |                       |
        |                       | ,                     |                       |
        |                       |     CxxLibraryDescrip |                       |
        |                       | tion.CommonArg args)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
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

        []{#<init>(com.facebook.buck.apple.XCodeDescriptions,com.facebook.buck.core.model.targetgraph.TargetGraph,com.facebook.buck.apple.AppleDependenciesCache,com.facebook.buck.features.apple.project.ProjectGenerationStateCache,java.util.Set,com.facebook.buck.core.cell.Cell,java.nio.file.Path,java.lang.String,java.lang.String,com.facebook.buck.features.apple.project.ProjectGeneratorOptions,com.facebook.buck.rules.keys.config.RuleKeyConfiguration,boolean,java.util.Optional,com.google.common.collect.ImmutableSet,com.facebook.buck.features.apple.project.FocusedModuleTargetMatcher,com.facebook.buck.cxx.toolchain.CxxPlatform,com.google.common.collect.ImmutableSet,java.util.function.Function,com.facebook.buck.event.BuckEventBus,com.facebook.buck.features.halide.HalideBuckConfig,com.facebook.buck.cxx.config.CxxBuckConfig,com.facebook.buck.apple.AppleConfig,com.facebook.buck.swift.SwiftBuckConfig,java.util.Optional)}

        -   #### ProjectGenerator

                public ProjectGenerator​(XCodeDescriptions xcodeDescriptions,
                                        TargetGraph targetGraph,
                                        AppleDependenciesCache dependenciesCache,
                                        ProjectGenerationStateCache projGenerationStateCache,
                                        Set<BuildTarget> initialTargets,
                                        Cell cell,
                                        Path outputDirectory,
                                        String projectName,
                                        String buildFileName,
                                        com.facebook.buck.features.apple.project.ProjectGeneratorOptions options,
                                        RuleKeyConfiguration ruleKeyConfiguration,
                                        boolean isMainProject,
                                        Optional<BuildTarget> workspaceTarget,
                                        com.google.common.collect.ImmutableSet<BuildTarget> targetsInRequiredProjects,
                                        FocusedModuleTargetMatcher focusModules,
                                        CxxPlatform defaultCxxPlatform,
                                        com.google.common.collect.ImmutableSet<Flavor> appleCxxFlavors,
                                        java.util.function.Function<? super TargetNode<?>,​ActionGraphBuilder> actionGraphBuilderForNode,
                                        BuckEventBus buckEventBus,
                                        HalideBuckConfig halideBuckConfig,
                                        CxxBuckConfig cxxBuckConfig,
                                        AppleConfig appleConfig,
                                        SwiftBuckConfig swiftBuckConfig,
                                        Optional<com.google.common.collect.ImmutableMap<BuildTarget,​TargetNode<?>>> sharedLibraryToBundle)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getProjectPath()}

        -   #### getProjectPath

            ``` methodSignature
            public Path getProjectPath()
            ```

        []{#getBuildTargetToGeneratedTargetMap()}

        -   #### getBuildTargetToGeneratedTargetMap

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<BuildTarget,​PBXTarget> getBuildTargetToGeneratedTargetMap()
            ```

        []{#getGeneratedProjectToGeneratedTargets()}

        -   #### getGeneratedProjectToGeneratedTargets

            ``` methodSignature
            public com.google.common.collect.ImmutableSetMultimap<PBXProject,​PBXTarget> getGeneratedProjectToGeneratedTargets()
            ```

            [Returns:]{.returnLabel}
            :   Map from the generated project to all contained targets.

        []{#getRequiredBuildTargets()}

        -   #### getRequiredBuildTargets

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<BuildTarget> getRequiredBuildTargets()
            ```

        []{#getXcconfigPaths()}

        -   #### getXcconfigPaths

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<Path> getXcconfigPaths()
            ```

        []{#getFilesToCopyInXcode()}

        -   #### getFilesToCopyInXcode

            ``` methodSignature
            public com.google.common.collect.ImmutableList<CopyInXcode> getFilesToCopyInXcode()
            ```

        []{#isProjectGenerated()}

        -   #### isProjectGenerated

            ``` methodSignature
            public boolean isProjectGenerated()
            ```

        []{#createXcodeProjects()}

        -   #### createXcodeProjects

            ``` methodSignature
            public void createXcodeProjects()
                                     throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#parseAllPlatformHeaders(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.facebook.buck.io.filesystem.ProjectFilesystem,com.google.common.collect.ImmutableList,boolean,com.facebook.buck.cxx.CxxLibraryDescription.CommonArg)}

        -   #### parseAllPlatformHeaders

            ``` methodSignature
            public static com.google.common.collect.ImmutableMap<Path,​SourcePath> parseAllPlatformHeaders​(BuildTarget buildTarget,
                                                                                                                SourcePathResolverAdapter sourcePathResolverAdapter,
                                                                                                                ProjectFilesystem filesystem,
                                                                                                                com.google.common.collect.ImmutableList<SourceSortedSet> platformHeaders,
                                                                                                                boolean export,
                                                                                                                CxxLibraryDescription.CommonArg args)
            ```

            [Returns:]{.returnLabel}
            :   a map of all exported platform headers without matching
                a specific platform.

        []{#computeSharedLibrariesToBundles(com.google.common.collect.ImmutableSet,com.facebook.buck.core.model.targetgraph.TargetGraph)}

        -   #### computeSharedLibrariesToBundles

            ``` methodSignature
            public static com.google.common.collect.ImmutableMap<BuildTarget,​TargetNode<?>> computeSharedLibrariesToBundles​(com.google.common.collect.ImmutableSet<TargetNode<?>> targetNodes,
                                                                                                                                  TargetGraph targetGraph)
                                                                                                                           throws HumanReadableException
            ```

            ::: block
            Generate a mapping from libraries to the framework bundles
            that include them.
            :::

            [Throws:]{.throwsLabel}
            :   `HumanReadableException`
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
