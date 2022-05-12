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
-   Nested \| 
-   Field \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Interface DefaultJavaLibraryRules.DefaultJavaLibraryConstructor {#interface-defaultjavalibraryrules.defaultjavalibraryconstructor .title title="Interface DefaultJavaLibraryRules.DefaultJavaLibraryConstructor"}
:::

::: contentContainer
::: description
-   

    Enclosing class:
    :   [DefaultJavaLibraryRules](DefaultJavaLibraryRules.html "class in com.facebook.buck.jvm.java")

    ------------------------------------------------------------------------

        public static interface DefaultJavaLibraryRules.DefaultJavaLibraryConstructor
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type      Method                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             Description
          ---------------------- ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `DefaultJavaLibrary`   `newInstance​(BuildTarget buildTarget,            ProjectFilesystem projectFilesystem,            JarBuildStepsFactory jarBuildStepsFactory,            SourcePathRuleFinder ruleFinder,            Optional<SourcePath> proguardConfig,            SortedSet<BuildRule> firstOrderPackageableDeps,            com.google.common.collect.ImmutableSortedSet<BuildRule> fullJarExportedDeps,            com.google.common.collect.ImmutableSortedSet<BuildRule> fullJarProvidedDeps,            com.google.common.collect.ImmutableSortedSet<BuildRule> fullJarExportedProvidedDeps,            com.google.common.collect.ImmutableSortedSet<BuildRule> runtimeDeps,            BuildTarget abiJar,            BuildTarget sourceOnlyAbiJar,            Optional<String> mavenCoords,            com.google.common.collect.ImmutableSortedSet<BuildTarget> tests,            boolean requiredForSourceOnlyAbi,            JavaBuckConfig.UnusedDependenciesAction unusedDependenciesAction,            Optional<UnusedDependenciesFinderFactory> unusedDependenciesFinderFactory,            CalculateSourceAbi previousRuleInPipeline,            boolean isDesugarEnabled,            boolean isInterfaceMethodsDesugarEnabled,            boolean neverMarkAsUnusedDependency)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#newInstance(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.jvm.java.JarBuildStepsFactory,com.facebook.buck.core.rules.SourcePathRuleFinder,java.util.Optional,java.util.SortedSet,com.google.common.collect.ImmutableSortedSet,com.google.common.collect.ImmutableSortedSet,com.google.common.collect.ImmutableSortedSet,com.google.common.collect.ImmutableSortedSet,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.model.BuildTarget,java.util.Optional,com.google.common.collect.ImmutableSortedSet,boolean,com.facebook.buck.jvm.java.JavaBuckConfig.UnusedDependenciesAction,java.util.Optional,com.facebook.buck.jvm.java.CalculateSourceAbi,boolean,boolean,boolean)}

        -   #### newInstance

            ``` methodSignature
            DefaultJavaLibrary newInstance​(BuildTarget buildTarget,
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
                                           CalculateSourceAbi previousRuleInPipeline,
                                           boolean isDesugarEnabled,
                                           boolean isInterfaceMethodsDesugarEnabled,
                                           boolean neverMarkAsUnusedDependency)
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
-   Nested \| 
-   Field \| 
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
