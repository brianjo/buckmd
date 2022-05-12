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
# Hierarchy For Package com.facebook.buck.features.d {#hierarchy-for-package-com.facebook.buck.features.d .title}

[Package Hierarchies:]{.packageHierarchyLabel}

-   [All Packages](../../../../../overview-tree.html)
:::

::: contentContainer
::: {.section role="region"}
## Class Hierarchy {#class-hierarchy title="Class Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   com.facebook.buck.core.rules.impl.[[AbstractBuildRule]{.typeNameLink}](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")
        (implements
        com.facebook.buck.core.rules.[BuildRule](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules"))
        -   com.facebook.buck.core.rules.impl.[[AbstractBuildRuleWithDeclaredAndExtraDeps]{.typeNameLink}](../../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")
            (implements
            com.facebook.buck.core.rules.attr.[HasDeclaredAndExtraDeps](../../core/rules/attr/HasDeclaredAndExtraDeps.html "interface in com.facebook.buck.core.rules.attr"))
            -   com.facebook.buck.features.d.[[DBinary]{.typeNameLink}](DBinary.html "class in com.facebook.buck.features.d")
                (implements
                com.facebook.buck.core.rules.tool.[BinaryBuildRule](../../core/rules/tool/BinaryBuildRule.html "interface in com.facebook.buck.core.rules.tool"),
                com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"))
            -   com.facebook.buck.features.d.[[DCompileBuildRule]{.typeNameLink}](DCompileBuildRule.html "class in com.facebook.buck.features.d")
            -   com.facebook.buck.features.d.[[DTest]{.typeNameLink}](DTest.html "class in com.facebook.buck.features.d")
                (implements
                com.facebook.buck.core.test.rule.[ExternalTestRunnerRule](../../core/test/rule/ExternalTestRunnerRule.html "interface in com.facebook.buck.core.test.rule"),
                com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"),
                com.facebook.buck.core.test.rule.[TestRule](../../core/test/rule/TestRule.html "interface in com.facebook.buck.core.test.rule"))
            -   com.facebook.buck.core.rules.impl.[[NoopBuildRuleWithDeclaredAndExtraDeps]{.typeNameLink}](../../core/rules/impl/NoopBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")
                -   com.facebook.buck.features.d.[[DLibrary]{.typeNameLink}](DLibrary.html "class in com.facebook.buck.features.d")
                    (implements
                    com.facebook.buck.cxx.toolchain.nativelink.[NativeLinkableGroup](../../cxx/toolchain/nativelink/NativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink"))
    -   com.facebook.buck.step.[[AbstractTestStep]{.typeNameLink}](../../step/AbstractTestStep.html "class in com.facebook.buck.step")
        (implements
        com.facebook.buck.step.[Step](../../step/Step.html "interface in com.facebook.buck.step"))
        -   com.facebook.buck.features.d.[[DTestStep]{.typeNameLink}](DTestStep.html "class in com.facebook.buck.features.d")
    -   com.facebook.buck.features.d.[[DBinaryDescription]{.typeNameLink}](DBinaryDescription.html "class in com.facebook.buck.features.d")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>,
        com.facebook.buck.versions.[VersionRoot](../../versions/VersionRoot.html "interface in com.facebook.buck.versions")\<A\>)
    -   com.facebook.buck.features.d.[[DBinaryDescriptionArg]{.typeNameLink}](DBinaryDescriptionArg.html "class in com.facebook.buck.features.d")
    -   com.facebook.buck.features.d.[[DBinaryDescriptionArg.Builder]{.typeNameLink}](DBinaryDescriptionArg.Builder.html "class in com.facebook.buck.features.d")
    -   com.facebook.buck.features.d.[[DBuckConfig]{.typeNameLink}](DBuckConfig.html "class in com.facebook.buck.features.d")
    -   com.facebook.buck.features.d.[[DDescriptionsProvider]{.typeNameLink}](DDescriptionsProvider.html "class in com.facebook.buck.features.d")
        (implements
        com.facebook.buck.core.model.targetgraph.[DescriptionProvider](../../core/model/targetgraph/DescriptionProvider.html "interface in com.facebook.buck.core.model.targetgraph"))
    -   com.facebook.buck.features.d.[[DLibraryDescription]{.typeNameLink}](DLibraryDescription.html "class in com.facebook.buck.features.d")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>,
        com.facebook.buck.versions.[VersionPropagator](../../versions/VersionPropagator.html "interface in com.facebook.buck.versions")\<A\>)
    -   com.facebook.buck.features.d.[[DLibraryDescriptionArg]{.typeNameLink}](DLibraryDescriptionArg.html "class in com.facebook.buck.features.d")
    -   com.facebook.buck.features.d.[[DLibraryDescriptionArg.Builder]{.typeNameLink}](DLibraryDescriptionArg.Builder.html "class in com.facebook.buck.features.d")
    -   com.facebook.buck.features.d.[[DModule]{.typeNameLink}](DModule.html "class in com.facebook.buck.features.d")
    -   com.facebook.buck.features.d.[[DTestDescription]{.typeNameLink}](DTestDescription.html "class in com.facebook.buck.features.d")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>,
        com.facebook.buck.versions.[VersionRoot](../../versions/VersionRoot.html "interface in com.facebook.buck.versions")\<A\>)
    -   com.facebook.buck.features.d.[[DTestDescriptionArg]{.typeNameLink}](DTestDescriptionArg.html "class in com.facebook.buck.features.d")
    -   com.facebook.buck.features.d.[[DTestDescriptionArg.Builder]{.typeNameLink}](DTestDescriptionArg.Builder.html "class in com.facebook.buck.features.d")
    -   org.pf4j.Plugin
        -   com.facebook.buck.features.d.[[DModuleAdapterPlugin]{.typeNameLink}](DModuleAdapterPlugin.html "class in com.facebook.buck.features.d")
    -   com.facebook.buck.shell.[[ShellStep]{.typeNameLink}](../../shell/ShellStep.html "class in com.facebook.buck.shell")
        (implements
        com.facebook.buck.step.[Step](../../step/Step.html "interface in com.facebook.buck.step"))
        -   com.facebook.buck.features.d.[[DCompileStep]{.typeNameLink}](DCompileStep.html "class in com.facebook.buck.features.d")
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
