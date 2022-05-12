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
[Package]{.packageLabelInType} [com.facebook.buck.features.apple.projectV2](package-summary.html)
:::

## Class ProjectGenerator {#class-projectgenerator .title title="Class ProjectGenerator"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.apple.projectV2.ProjectGenerator

::: description
-   

    ------------------------------------------------------------------------

        public class ProjectGenerator
        extends Object

    ::: block
    Generates an Xcode project and writes the output to disk.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `Pro                  | ::: block             |
        |                       | jectGenerator.Result` | The output from       |
        |                       |                       | generating an Xcode   |
        |                       |                       | project.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           Description
          --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `ProjectGenerator​(XCodeDescriptions xcodeDescriptions,                 TargetGraph targetGraph,                 AppleDependenciesCache dependenciesCache,                 ProjectGenerationStateCache projGenerationStateCache,                 Set<BuildTarget> projectTargets,                 Cell cell,                 String buildFileName,                 ProjectGeneratorOptions options,                 RuleKeyConfiguration ruleKeyConfiguration,                 BuildTarget workspaceTarget,                 com.google.common.collect.ImmutableSet<BuildTarget> targetsInRequiredProjects,                 CxxPlatform defaultCxxPlatform,                 com.google.common.collect.ImmutableSet<Flavor> appleCxxFlavors,                 java.util.function.Function<? super TargetNode<?>,​ActionGraphBuilder> actionGraphBuilderForNode,                 BuckEventBus buckEventBus,                 HalideBuckConfig halideBuckConfig,                 CxxBuckConfig cxxBuckConfig,                 AppleConfig appleConfig,                 SwiftBuckConfig swiftBuckConfig,                 Optional<com.google.common.collect.ImmutableMap<BuildTarget,​TargetNode<?>>> sharedLibraryToBundle)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Pro                  | `create               | ::: block             |
        | jectGenerator.Result` | XcodeProject​(com.face | Creates an xcode      |
        |                       | book.buck.features.ap | project.              |
        |                       | ple.projectV2.XcodePr | :::                   |
        |                       | ojectWriteOptions xco |                       |
        |                       | deProjectWriteOptions |                       |
        |                       | ,                   c |                       |
        |                       | om.google.common.util |                       |
        |                       | .concurrent.Listening |                       |
        |                       | ExecutorService liste |                       |
        |                       | ningExecutorService)` |                       |
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

        []{#<init>(com.facebook.buck.apple.XCodeDescriptions,com.facebook.buck.core.model.targetgraph.TargetGraph,com.facebook.buck.apple.AppleDependenciesCache,com.facebook.buck.features.apple.projectV2.ProjectGenerationStateCache,java.util.Set,com.facebook.buck.core.cell.Cell,java.lang.String,com.facebook.buck.features.apple.projectV2.ProjectGeneratorOptions,com.facebook.buck.rules.keys.config.RuleKeyConfiguration,com.facebook.buck.core.model.BuildTarget,com.google.common.collect.ImmutableSet,com.facebook.buck.cxx.toolchain.CxxPlatform,com.google.common.collect.ImmutableSet,java.util.function.Function,com.facebook.buck.event.BuckEventBus,com.facebook.buck.features.halide.HalideBuckConfig,com.facebook.buck.cxx.config.CxxBuckConfig,com.facebook.buck.apple.AppleConfig,com.facebook.buck.swift.SwiftBuckConfig,java.util.Optional)}

        -   #### ProjectGenerator

                public ProjectGenerator​(XCodeDescriptions xcodeDescriptions,
                                        TargetGraph targetGraph,
                                        AppleDependenciesCache dependenciesCache,
                                        ProjectGenerationStateCache projGenerationStateCache,
                                        Set<BuildTarget> projectTargets,
                                        Cell cell,
                                        String buildFileName,
                                        ProjectGeneratorOptions options,
                                        RuleKeyConfiguration ruleKeyConfiguration,
                                        BuildTarget workspaceTarget,
                                        com.google.common.collect.ImmutableSet<BuildTarget> targetsInRequiredProjects,
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

        []{#createXcodeProject(com.facebook.buck.features.apple.projectV2.XcodeProjectWriteOptions,com.google.common.util.concurrent.ListeningExecutorService)}

        -   #### createXcodeProject

            ``` methodSignature
            public ProjectGenerator.Result createXcodeProject​(com.facebook.buck.features.apple.projectV2.XcodeProjectWriteOptions xcodeProjectWriteOptions,
                                                              com.google.common.util.concurrent.ListeningExecutorService listeningExecutorService)
                                                       throws IOException,
                                                              InterruptedException
            ```

            ::: block
            Creates an xcode project.
            :::

            [Returns:]{.returnLabel}
            :   A result containing the data about that project.

            [Throws:]{.throwsLabel}
            :   `IOException` - An IO exception occurred while trying to
                write to disk.
            :   `InterruptedException`
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
