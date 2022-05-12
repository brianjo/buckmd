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

## Class WorkspaceAndProjectGenerator {#class-workspaceandprojectgenerator .title title="Class WorkspaceAndProjectGenerator"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.apple.projectV2.WorkspaceAndProjectGenerator

::: description
-   

    ------------------------------------------------------------------------

        public class WorkspaceAndProjectGenerator
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `WorkspaceAndPro      | ::: block             |
        |                       | jectGenerator.Result` | The result of         |
        |                       |                       | generating a          |
        |                       |                       | workspace project.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `WorkspaceAndProjectGenerator​(XCodeDescriptions xcodeDescriptions,                             Cell cell,                             TargetGraph projectGraph,                             XcodeWorkspaceConfigDescriptionArg workspaceArguments,                             BuildTarget workspaceBuildTarget,                             ProjectGeneratorOptions projectGeneratorOptions,                             FocusedTargetMatcher focusedTargetMatcher,                             boolean parallelizeBuild,                             CxxPlatform defaultCxxPlatform,                             com.google.common.collect.ImmutableSet<Flavor> appleCxxFlavors,                             String buildFileName,                             java.util.function.Function<TargetNode<?>,​ActionGraphBuilder> graphBuilderForNode,                             BuckEventBus buckEventBus,                             RuleKeyConfiguration ruleKeyConfiguration,                             HalideBuckConfig halideBuckConfig,                             CxxBuckConfig cxxBuckConfig,                             AppleConfig appleConfig,                             SwiftBuckConfig swiftBuckConfig,                             Optional<com.google.common.collect.ImmutableMap<BuildTarget,​TargetNode<?>>> sharedLibraryToBundle)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `WorkspaceAndPro      | `generateWorkspaceA   | ::: block             |
        | jectGenerator.Result` | ndDependentProjects​(c | Generates a workspace |
        |                       | om.google.common.util | and all projects      |
        |                       | .concurrent.Listening | :::                   |
        |                       | ExecutorService liste |                       |
        |                       | ningExecutorService)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getRe                |                       |
        | .common.collect.Immut | quiredBuildTargets()` |                       |
        | ableSet<BuildTarget>` |                       |                       |
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

        []{#<init>(com.facebook.buck.apple.XCodeDescriptions,com.facebook.buck.core.cell.Cell,com.facebook.buck.core.model.targetgraph.TargetGraph,com.facebook.buck.features.apple.common.XcodeWorkspaceConfigDescriptionArg,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.features.apple.projectV2.ProjectGeneratorOptions,com.facebook.buck.features.apple.projectV2.FocusedTargetMatcher,boolean,com.facebook.buck.cxx.toolchain.CxxPlatform,com.google.common.collect.ImmutableSet,java.lang.String,java.util.function.Function,com.facebook.buck.event.BuckEventBus,com.facebook.buck.rules.keys.config.RuleKeyConfiguration,com.facebook.buck.features.halide.HalideBuckConfig,com.facebook.buck.cxx.config.CxxBuckConfig,com.facebook.buck.apple.AppleConfig,com.facebook.buck.swift.SwiftBuckConfig,java.util.Optional)}

        -   #### WorkspaceAndProjectGenerator

                public WorkspaceAndProjectGenerator​(XCodeDescriptions xcodeDescriptions,
                                                    Cell cell,
                                                    TargetGraph projectGraph,
                                                    XcodeWorkspaceConfigDescriptionArg workspaceArguments,
                                                    BuildTarget workspaceBuildTarget,
                                                    ProjectGeneratorOptions projectGeneratorOptions,
                                                    FocusedTargetMatcher focusedTargetMatcher,
                                                    boolean parallelizeBuild,
                                                    CxxPlatform defaultCxxPlatform,
                                                    com.google.common.collect.ImmutableSet<Flavor> appleCxxFlavors,
                                                    String buildFileName,
                                                    java.util.function.Function<TargetNode<?>,​ActionGraphBuilder> graphBuilderForNode,
                                                    BuckEventBus buckEventBus,
                                                    RuleKeyConfiguration ruleKeyConfiguration,
                                                    HalideBuckConfig halideBuckConfig,
                                                    CxxBuckConfig cxxBuckConfig,
                                                    AppleConfig appleConfig,
                                                    SwiftBuckConfig swiftBuckConfig,
                                                    Optional<com.google.common.collect.ImmutableMap<BuildTarget,​TargetNode<?>>> sharedLibraryToBundle)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getRequiredBuildTargets()}

        -   #### getRequiredBuildTargets

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<BuildTarget> getRequiredBuildTargets()
            ```

        []{#generateWorkspaceAndDependentProjects(com.google.common.util.concurrent.ListeningExecutorService)}

        -   #### generateWorkspaceAndDependentProjects

            ``` methodSignature
            public WorkspaceAndProjectGenerator.Result generateWorkspaceAndDependentProjects​(com.google.common.util.concurrent.ListeningExecutorService listeningExecutorService)
                                                                                      throws IOException,
                                                                                             InterruptedException
            ```

            ::: block
            Generates a workspace and all projects
            :::

            [Returns:]{.returnLabel}
            :   A result indicating the output of the generation

            [Throws:]{.throwsLabel}
            :   `IOException`
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
