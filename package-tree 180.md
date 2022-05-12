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
# Hierarchy For Package com.facebook.buck.features.python {#hierarchy-for-package-com.facebook.buck.features.python .title}

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
            -   com.facebook.buck.core.rules.impl.[[NoopBuildRuleWithDeclaredAndExtraDeps]{.typeNameLink}](../../core/rules/impl/NoopBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")
                -   com.facebook.buck.features.python.[[CxxPythonExtension]{.typeNameLink}](CxxPythonExtension.html "class in com.facebook.buck.features.python")
                    (implements
                    com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"),
                    com.facebook.buck.features.python.[PythonPackagable](PythonPackagable.html "interface in com.facebook.buck.features.python"))
                -   com.facebook.buck.features.python.[[PythonLibrary]{.typeNameLink}](PythonLibrary.html "class in com.facebook.buck.features.python")
                    (implements
                    com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"),
                    com.facebook.buck.features.python.[PythonPackagable](PythonPackagable.html "interface in com.facebook.buck.features.python"))
            -   com.facebook.buck.features.python.[[PrebuiltPythonLibrary]{.typeNameLink}](PrebuiltPythonLibrary.html "class in com.facebook.buck.features.python")
                (implements
                com.facebook.buck.features.python.[PythonPackagable](PythonPackagable.html "interface in com.facebook.buck.features.python"))
            -   com.facebook.buck.features.python.[[PythonTest]{.typeNameLink}](PythonTest.html "class in com.facebook.buck.features.python")
                (implements
                com.facebook.buck.core.rules.tool.[BinaryBuildRule](../../core/rules/tool/BinaryBuildRule.html "interface in com.facebook.buck.core.rules.tool"),
                com.facebook.buck.core.test.rule.[ExternalTestRunnerRule](../../core/test/rule/ExternalTestRunnerRule.html "interface in com.facebook.buck.core.test.rule"),
                com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"),
                com.facebook.buck.core.test.rule.[TestRule](../../core/test/rule/TestRule.html "interface in com.facebook.buck.core.test.rule"))
            -   com.facebook.buck.features.python.[[PythonTestX]{.typeNameLink}](PythonTestX.html "class in com.facebook.buck.features.python")
                (implements
                com.facebook.buck.core.test.rule.[ExternalTestRunnerRule](../../core/test/rule/ExternalTestRunnerRule.html "interface in com.facebook.buck.core.test.rule"),
                com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"),
                com.facebook.buck.core.test.rule.[TestXRule](../../core/test/rule/TestXRule.html "interface in com.facebook.buck.core.test.rule"))
        -   com.facebook.buck.rules.modern.[[ModernBuildRule]{.typeNameLink}](../../rules/modern/ModernBuildRule.html "class in com.facebook.buck.rules.modern")\<T\>
            (implements
            com.facebook.buck.core.rules.attr.[SupportsInputBasedRuleKey](../../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr"))
            -   com.facebook.buck.features.python.[[PythonCompileRule]{.typeNameLink}](PythonCompileRule.html "class in com.facebook.buck.features.python")
        -   com.facebook.buck.core.rules.impl.[[NoopBuildRule]{.typeNameLink}](../../core/rules/impl/NoopBuildRule.html "class in com.facebook.buck.core.rules.impl")
            (implements
            com.facebook.buck.core.rules.attr.[SupportsInputBasedRuleKey](../../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr"))
            -   com.facebook.buck.features.python.[[PythonTestRunner]{.typeNameLink}](PythonTestRunner.html "class in com.facebook.buck.features.python")
        -   com.facebook.buck.features.python.[[PythonBinary]{.typeNameLink}](PythonBinary.html "class in com.facebook.buck.features.python")
            (implements
            com.facebook.buck.core.rules.tool.[BinaryBuildRule](../../core/rules/tool/BinaryBuildRule.html "interface in com.facebook.buck.core.rules.tool"),
            com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"))
            -   com.facebook.buck.features.python.[[PythonInPlaceBinary]{.typeNameLink}](PythonInPlaceBinary.html "class in com.facebook.buck.features.python")
                (implements
                com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"))
            -   com.facebook.buck.features.python.[[PythonPackagedBinary]{.typeNameLink}](PythonPackagedBinary.html "class in com.facebook.buck.features.python")
                (implements
                com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"))
        -   com.facebook.buck.core.rules.impl.[[SymlinkTree]{.typeNameLink}](../../core/rules/impl/SymlinkTree.html "class in com.facebook.buck.core.rules.impl")
            (implements
            com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"),
            com.facebook.buck.core.rules.attr.[SupportsInputBasedRuleKey](../../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr"))
            -   com.facebook.buck.features.python.[[PythonSymlinkTree]{.typeNameLink}](PythonSymlinkTree.html "class in com.facebook.buck.features.python")
    -   com.facebook.buck.features.python.[[CxxPythonExtensionDescription]{.typeNameLink}](CxxPythonExtensionDescription.html "class in com.facebook.buck.features.python")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.model.[Flavored](../../core/model/Flavored.html "interface in com.facebook.buck.core.model"),
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>,
        com.facebook.buck.versions.[VersionPropagator](../../versions/VersionPropagator.html "interface in com.facebook.buck.versions")\<A\>)
    -   com.facebook.buck.features.python.[[CxxPythonExtensionDescriptionArg]{.typeNameLink}](CxxPythonExtensionDescriptionArg.html "class in com.facebook.buck.features.python")
    -   com.facebook.buck.features.python.[[CxxPythonExtensionDescriptionArg.Builder]{.typeNameLink}](CxxPythonExtensionDescriptionArg.Builder.html "class in com.facebook.buck.features.python")
    -   com.facebook.buck.features.python.[[MovePythonWhlDataStep]{.typeNameLink}](MovePythonWhlDataStep.html "class in com.facebook.buck.features.python")
        (implements
        com.facebook.buck.step.[Step](../../step/Step.html "interface in com.facebook.buck.step"))
    -   org.pf4j.Plugin
        -   com.facebook.buck.features.python.[[PythonModuleAdapterPlugin]{.typeNameLink}](PythonModuleAdapterPlugin.html "class in com.facebook.buck.features.python")
    -   com.facebook.buck.features.python.[[PrebuiltPythonLibraryDescription]{.typeNameLink}](PrebuiltPythonLibraryDescription.html "class in com.facebook.buck.features.python")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.model.[Flavored](../../core/model/Flavored.html "interface in com.facebook.buck.core.model"))
    -   com.facebook.buck.features.python.[[PrebuiltPythonLibraryDescriptionArg]{.typeNameLink}](PrebuiltPythonLibraryDescriptionArg.html "class in com.facebook.buck.features.python")
    -   com.facebook.buck.features.python.[[PrebuiltPythonLibraryDescriptionArg.Builder]{.typeNameLink}](PrebuiltPythonLibraryDescriptionArg.Builder.html "class in com.facebook.buck.features.python")
    -   com.facebook.buck.features.python.[[PythonBinaryDescription]{.typeNameLink}](PythonBinaryDescription.html "class in com.facebook.buck.features.python")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>,
        com.facebook.buck.versions.[VersionRoot](../../versions/VersionRoot.html "interface in com.facebook.buck.versions")\<A\>)
    -   com.facebook.buck.features.python.[[PythonBinaryDescriptionArg]{.typeNameLink}](PythonBinaryDescriptionArg.html "class in com.facebook.buck.features.python")
    -   com.facebook.buck.features.python.[[PythonBinaryDescriptionArg.Builder]{.typeNameLink}](PythonBinaryDescriptionArg.Builder.html "class in com.facebook.buck.features.python")
    -   com.facebook.buck.features.python.[[PythonBuckConfig]{.typeNameLink}](PythonBuckConfig.html "class in com.facebook.buck.features.python")
    -   com.facebook.buck.features.python.[[PythonDescriptionsProvider]{.typeNameLink}](PythonDescriptionsProvider.html "class in com.facebook.buck.features.python")
        (implements
        com.facebook.buck.core.model.targetgraph.[DescriptionProvider](../../core/model/targetgraph/DescriptionProvider.html "interface in com.facebook.buck.core.model.targetgraph"))
    -   com.facebook.buck.features.python.[[PythonLibraryDescription]{.typeNameLink}](PythonLibraryDescription.html "class in com.facebook.buck.features.python")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.model.[Flavored](../../core/model/Flavored.html "interface in com.facebook.buck.core.model"),
        com.facebook.buck.core.description.metadata.[MetadataProvidingDescription](../../core/description/metadata/MetadataProvidingDescription.html "interface in com.facebook.buck.core.description.metadata")\<T\>,
        com.facebook.buck.versions.[VersionPropagator](../../versions/VersionPropagator.html "interface in com.facebook.buck.versions")\<A\>)
    -   com.facebook.buck.features.python.[[PythonLibraryDescriptionArg]{.typeNameLink}](PythonLibraryDescriptionArg.html "class in com.facebook.buck.features.python")
    -   com.facebook.buck.features.python.[[PythonLibraryDescriptionArg.Builder]{.typeNameLink}](PythonLibraryDescriptionArg.Builder.html "class in com.facebook.buck.features.python")
    -   com.facebook.buck.features.python.[[PythonMappedComponents]{.typeNameLink}](PythonMappedComponents.html "class in com.facebook.buck.features.python")
        (implements
        com.facebook.buck.features.python.[PythonComponents](PythonComponents.html "interface in com.facebook.buck.features.python"))
    -   com.facebook.buck.features.python.[[PythonMappedComponents.Resolved]{.typeNameLink}](PythonMappedComponents.Resolved.html "class in com.facebook.buck.features.python")
        (implements
        com.facebook.buck.features.python.[PythonComponents.Resolved](PythonComponents.Resolved.html "interface in com.facebook.buck.features.python"))
    -   com.facebook.buck.features.python.[[PythonModule]{.typeNameLink}](PythonModule.html "class in com.facebook.buck.features.python")
    -   com.facebook.buck.features.python.[[PythonPackageComponents]{.typeNameLink}](PythonPackageComponents.html "class in com.facebook.buck.features.python")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"))
    -   com.facebook.buck.features.python.[[PythonPackageComponents.Builder]{.typeNameLink}](PythonPackageComponents.Builder.html "class in com.facebook.buck.features.python")
    -   com.facebook.buck.features.python.[[PythonRunTestsStep]{.typeNameLink}](PythonRunTestsStep.html "class in com.facebook.buck.features.python")
        (implements
        com.facebook.buck.step.[Step](../../step/Step.html "interface in com.facebook.buck.step"))
    -   com.facebook.buck.features.python.[[PythonTestDescription]{.typeNameLink}](PythonTestDescription.html "class in com.facebook.buck.features.python")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>,
        com.facebook.buck.versions.[VersionRoot](../../versions/VersionRoot.html "interface in com.facebook.buck.versions")\<A\>)
    -   com.facebook.buck.features.python.[[PythonTestDescriptionArg]{.typeNameLink}](PythonTestDescriptionArg.html "class in com.facebook.buck.features.python")
    -   com.facebook.buck.features.python.[[PythonTestDescriptionArg.Builder]{.typeNameLink}](PythonTestDescriptionArg.Builder.html "class in com.facebook.buck.features.python")
    -   com.facebook.buck.features.python.[[PythonTestRunnerDescription]{.typeNameLink}](PythonTestRunnerDescription.html "class in com.facebook.buck.features.python")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>)
    -   com.facebook.buck.features.python.[[PythonTestRunnerDescriptionArg]{.typeNameLink}](PythonTestRunnerDescriptionArg.html "class in com.facebook.buck.features.python")
    -   com.facebook.buck.features.python.[[PythonTestRunnerDescriptionArg.Builder]{.typeNameLink}](PythonTestRunnerDescriptionArg.Builder.html "class in com.facebook.buck.features.python")
    -   com.facebook.buck.features.python.[[PythonUtil]{.typeNameLink}](PythonUtil.html "class in com.facebook.buck.features.python")
    -   com.facebook.buck.shell.[[ShellStep]{.typeNameLink}](../../shell/ShellStep.html "class in com.facebook.buck.shell")
        (implements
        com.facebook.buck.step.[Step](../../step/Step.html "interface in com.facebook.buck.step"))
        -   com.facebook.buck.features.python.[[PexStep]{.typeNameLink}](PexStep.html "class in com.facebook.buck.features.python")
:::

::: {.section role="region"}
## Interface Hierarchy {#interface-hierarchy title="Interface Hierarchy"}

-   com.facebook.buck.core.rulekey.[[AddsToRuleKey]{.typeNameLink}](../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey")
    -   com.facebook.buck.features.python.[[PythonComponents]{.typeNameLink}](PythonComponents.html "interface in com.facebook.buck.features.python")
-   com.facebook.buck.core.model.[[HasBuildTarget]{.typeNameLink}](../../core/model/HasBuildTarget.html "interface in com.facebook.buck.core.model")
    -   com.facebook.buck.features.python.[[PythonPackagable]{.typeNameLink}](PythonPackagable.html "interface in com.facebook.buck.features.python")
-   com.facebook.buck.features.python.[[PythonComponents.Resolved]{.typeNameLink}](PythonComponents.Resolved.html "interface in com.facebook.buck.features.python")
-   com.facebook.buck.features.python.[[PythonComponents.Resolved.ComponentConsumer]{.typeNameLink}](PythonComponents.Resolved.ComponentConsumer.html "interface in com.facebook.buck.features.python")
:::

::: {.section role="region"}
## Enum Hierarchy {#enum-hierarchy title="Enum Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   java.lang.[[Enum]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<E\>
        (implements
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   com.facebook.buck.features.python.[[CxxPythonExtensionDescription.Type]{.typeNameLink}](CxxPythonExtensionDescription.Type.html "enum in com.facebook.buck.features.python")
            (implements
            com.facebook.buck.core.model.[FlavorConvertible](../../core/model/FlavorConvertible.html "interface in com.facebook.buck.core.model"))
        -   com.facebook.buck.features.python.[[PythonBuckConfig.PackageStyle]{.typeNameLink}](PythonBuckConfig.PackageStyle.html "enum in com.facebook.buck.features.python")
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
