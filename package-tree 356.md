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
-   Tree
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Hierarchy For Package com.facebook.buck.shell {#hierarchy-for-package-com.facebook.buck.shell .title}

[Package Hierarchies:]{.packageHierarchyLabel}

-   [All Packages](../../../../overview-tree.html)
:::

::: contentContainer
::: {.section role="region"}
## Class Hierarchy {#class-hierarchy title="Class Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   com.facebook.buck.core.rules.impl.[[AbstractBuildRule]{.typeNameLink}](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")
        (implements
        com.facebook.buck.core.rules.[BuildRule](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules"))
        -   com.facebook.buck.core.rules.impl.[[AbstractBuildRuleWithDeclaredAndExtraDeps]{.typeNameLink}](../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")
            (implements
            com.facebook.buck.core.rules.attr.[HasDeclaredAndExtraDeps](../core/rules/attr/HasDeclaredAndExtraDeps.html "interface in com.facebook.buck.core.rules.attr"))
            -   com.facebook.buck.core.rules.impl.[[NoopBuildRuleWithDeclaredAndExtraDeps]{.typeNameLink}](../core/rules/impl/NoopBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")
                -   com.facebook.buck.shell.[[ShTest]{.typeNameLink}](ShTest.html "class in com.facebook.buck.shell")
                    (implements
                    com.facebook.buck.core.rules.tool.[BinaryBuildRule](../core/rules/tool/BinaryBuildRule.html "interface in com.facebook.buck.core.rules.tool"),
                    com.facebook.buck.core.test.rule.[ExternalTestRunnerRule](../core/test/rule/ExternalTestRunnerRule.html "interface in com.facebook.buck.core.test.rule"),
                    com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"),
                    com.facebook.buck.core.test.rule.[TestRule](../core/test/rule/TestRule.html "interface in com.facebook.buck.core.test.rule"))
                -   com.facebook.buck.shell.[[TestSuite]{.typeNameLink}](TestSuite.html "class in com.facebook.buck.shell")
            -   com.facebook.buck.shell.[[ShBinary]{.typeNameLink}](ShBinary.html "class in com.facebook.buck.shell")
                (implements
                com.facebook.buck.core.rules.tool.[BinaryBuildRule](../core/rules/tool/BinaryBuildRule.html "interface in com.facebook.buck.core.rules.tool"),
                com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"))
        -   com.facebook.buck.shell.[[ExportFile]{.typeNameLink}](ExportFile.html "class in com.facebook.buck.shell")
            (implements
            com.facebook.buck.core.model.[HasOutputName](../core/model/HasOutputName.html "interface in com.facebook.buck.core.model"),
            com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"),
            com.facebook.buck.core.rules.attr.[SupportsInputBasedRuleKey](../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr"))
        -   com.facebook.buck.rules.modern.[[ModernBuildRule]{.typeNameLink}](../rules/modern/ModernBuildRule.html "class in com.facebook.buck.rules.modern")\<T\>
            (implements
            com.facebook.buck.core.rules.attr.[SupportsInputBasedRuleKey](../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr"))
            -   com.facebook.buck.shell.[[BaseGenrule]{.typeNameLink}](BaseGenrule.html "class in com.facebook.buck.shell")\<T\>
                (implements
                com.facebook.buck.core.rules.attr.[HasMultipleOutputs](../core/rules/attr/HasMultipleOutputs.html "interface in com.facebook.buck.core.rules.attr"),
                com.facebook.buck.core.model.[HasOutputName](../core/model/HasOutputName.html "interface in com.facebook.buck.core.model"))
                -   com.facebook.buck.shell.[[Genrule]{.typeNameLink}](Genrule.html "class in com.facebook.buck.shell")
                    (implements
                    com.facebook.buck.core.rules.attr.[HasMultipleOutputs](../core/rules/attr/HasMultipleOutputs.html "interface in com.facebook.buck.core.rules.attr"),
                    com.facebook.buck.core.model.[HasOutputName](../core/model/HasOutputName.html "interface in com.facebook.buck.core.model"))
                    -   com.facebook.buck.shell.[[GenruleBinary]{.typeNameLink}](GenruleBinary.html "class in com.facebook.buck.shell")
                        (implements
                        com.facebook.buck.core.rules.tool.[BinaryBuildRule](../core/rules/tool/BinaryBuildRule.html "interface in com.facebook.buck.core.rules.tool"))
        -   com.facebook.buck.core.rules.impl.[[NoopBuildRule]{.typeNameLink}](../core/rules/impl/NoopBuildRule.html "class in com.facebook.buck.core.rules.impl")
            (implements
            com.facebook.buck.core.rules.attr.[SupportsInputBasedRuleKey](../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr"))
            -   com.facebook.buck.shell.[[CommandAlias]{.typeNameLink}](CommandAlias.html "class in com.facebook.buck.shell")
                (implements
                com.facebook.buck.core.rules.tool.[BinaryBuildRule](../core/rules/tool/BinaryBuildRule.html "interface in com.facebook.buck.core.rules.tool"),
                com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"))
        -   com.facebook.buck.file.[[WriteFile]{.typeNameLink}](../file/WriteFile.html "class in com.facebook.buck.file")
            -   com.facebook.buck.shell.[[DefaultWorkerToolRule]{.typeNameLink}](DefaultWorkerToolRule.html "class in com.facebook.buck.shell")
                (implements
                com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"),
                com.facebook.buck.core.rules.attr.[InitializableFromDisk](../core/rules/attr/InitializableFromDisk.html "interface in com.facebook.buck.core.rules.attr")\<T\>,
                com.facebook.buck.shell.[ProvidesWorkerTool](ProvidesWorkerTool.html "interface in com.facebook.buck.shell"))
    -   com.facebook.buck.step.[[AbstractExecutionStep]{.typeNameLink}](../step/AbstractExecutionStep.html "class in com.facebook.buck.step")
        (implements
        com.facebook.buck.step.[Step](../step/Step.html "interface in com.facebook.buck.step"))
        -   com.facebook.buck.shell.[[SymlinkFilesIntoDirectoryStep]{.typeNameLink}](SymlinkFilesIntoDirectoryStep.html "class in com.facebook.buck.shell")
    -   com.facebook.buck.shell.[[AbstractGenruleDescription]{.typeNameLink}](AbstractGenruleDescription.html "class in com.facebook.buck.shell")\<T\>
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>)
        -   com.facebook.buck.shell.[[GenruleDescription]{.typeNameLink}](GenruleDescription.html "class in com.facebook.buck.shell")
            (implements
            com.facebook.buck.versions.[VersionRoot](../versions/VersionRoot.html "interface in com.facebook.buck.versions")\<A\>)
    -   com.facebook.buck.shell.[[AbstractGenruleStep.CommandString]{.typeNameLink}](AbstractGenruleStep.CommandString.html "class in com.facebook.buck.shell")
    -   com.facebook.buck.shell.[[CommandAliasDescription]{.typeNameLink}](CommandAliasDescription.html "class in com.facebook.buck.shell")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>)
    -   com.facebook.buck.shell.[[CommandAliasDescriptionArg]{.typeNameLink}](CommandAliasDescriptionArg.html "class in com.facebook.buck.shell")
    -   com.facebook.buck.shell.[[CommandAliasDescriptionArg.Builder]{.typeNameLink}](CommandAliasDescriptionArg.Builder.html "class in com.facebook.buck.shell")
    -   com.facebook.buck.shell.[[ExportFileDescription]{.typeNameLink}](ExportFileDescription.html "class in com.facebook.buck.shell")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.description.attr.[ImplicitInputsInferringDescription](../core/description/attr/ImplicitInputsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>)
    -   com.facebook.buck.shell.[[ExportFileDescriptionArg]{.typeNameLink}](ExportFileDescriptionArg.html "class in com.facebook.buck.shell")
    -   com.facebook.buck.shell.[[ExportFileDescriptionArg.Builder]{.typeNameLink}](ExportFileDescriptionArg.Builder.html "class in com.facebook.buck.shell")
    -   com.facebook.buck.shell.[[GenruleAndroidTools]{.typeNameLink}](GenruleAndroidTools.html "class in com.facebook.buck.shell")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"))
    -   com.facebook.buck.shell.[[GenruleBuildable]{.typeNameLink}](GenruleBuildable.html "class in com.facebook.buck.shell")
        (implements
        com.facebook.buck.rules.modern.[Buildable](../rules/modern/Buildable.html "interface in com.facebook.buck.rules.modern"))
    -   com.facebook.buck.shell.[[GenruleDescriptionArg]{.typeNameLink}](GenruleDescriptionArg.html "class in com.facebook.buck.shell")
    -   com.facebook.buck.shell.[[GenruleDescriptionArg.Builder]{.typeNameLink}](GenruleDescriptionArg.Builder.html "class in com.facebook.buck.shell")
    -   com.facebook.buck.shell.[[RunTestAndRecordResultStep]{.typeNameLink}](RunTestAndRecordResultStep.html "class in com.facebook.buck.shell")
        (implements
        com.facebook.buck.step.[Step](../step/Step.html "interface in com.facebook.buck.step"))
        -   com.facebook.buck.shell.[[RunShTestAndRecordResultStep]{.typeNameLink}](RunShTestAndRecordResultStep.html "class in com.facebook.buck.shell")
    -   com.facebook.buck.shell.[[ShBinaryDescription]{.typeNameLink}](ShBinaryDescription.html "class in com.facebook.buck.shell")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>)
    -   com.facebook.buck.shell.[[ShBinaryDescriptionArg]{.typeNameLink}](ShBinaryDescriptionArg.html "class in com.facebook.buck.shell")
    -   com.facebook.buck.shell.[[ShBinaryDescriptionArg.Builder]{.typeNameLink}](ShBinaryDescriptionArg.Builder.html "class in com.facebook.buck.shell")
    -   com.facebook.buck.shell.[[Shell]{.typeNameLink}](Shell.html "class in com.facebook.buck.shell")
    -   com.facebook.buck.shell.[[ShellDescriptionsProvider]{.typeNameLink}](ShellDescriptionsProvider.html "class in com.facebook.buck.shell")
        (implements
        com.facebook.buck.core.model.targetgraph.[DescriptionProvider](../core/model/targetgraph/DescriptionProvider.html "interface in com.facebook.buck.core.model.targetgraph"))
    -   com.facebook.buck.shell.[[ShellStep]{.typeNameLink}](ShellStep.html "class in com.facebook.buck.shell")
        (implements
        com.facebook.buck.step.[Step](../step/Step.html "interface in com.facebook.buck.step"))
        -   com.facebook.buck.shell.[[AbstractGenruleStep]{.typeNameLink}](AbstractGenruleStep.html "class in com.facebook.buck.shell")
        -   com.facebook.buck.shell.[[BashStep]{.typeNameLink}](BashStep.html "class in com.facebook.buck.shell")
        -   com.facebook.buck.shell.[[DefaultShellStep]{.typeNameLink}](DefaultShellStep.html "class in com.facebook.buck.shell")
    -   com.facebook.buck.shell.[[ShTestDescription]{.typeNameLink}](ShTestDescription.html "class in com.facebook.buck.shell")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>)
    -   com.facebook.buck.shell.[[ShTestDescriptionArg]{.typeNameLink}](ShTestDescriptionArg.html "class in com.facebook.buck.shell")
    -   com.facebook.buck.shell.[[ShTestDescriptionArg.Builder]{.typeNameLink}](ShTestDescriptionArg.Builder.html "class in com.facebook.buck.shell")
    -   com.facebook.buck.shell.[[TestSuiteDescription]{.typeNameLink}](TestSuiteDescription.html "class in com.facebook.buck.shell")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>)
    -   com.facebook.buck.shell.[[TestSuiteDescriptionArg]{.typeNameLink}](TestSuiteDescriptionArg.html "class in com.facebook.buck.shell")
    -   com.facebook.buck.shell.[[TestSuiteDescriptionArg.Builder]{.typeNameLink}](TestSuiteDescriptionArg.Builder.html "class in com.facebook.buck.shell")
    -   java.lang.[[Throwable]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Throwable.html?is-external=true "class or interface in java.lang"){.externalLink}
        (implements
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   java.lang.[[Exception]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Exception.html?is-external=true "class or interface in java.lang"){.externalLink}
            -   java.lang.[[RuntimeException]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/RuntimeException.html?is-external=true "class or interface in java.lang"){.externalLink}
                -   com.facebook.buck.core.exceptions.[[HumanReadableException]{.typeNameLink}](../core/exceptions/HumanReadableException.html "class in com.facebook.buck.core.exceptions")
                    (implements
                    com.facebook.buck.core.exceptions.[ExceptionWithHumanReadableMessage](../core/exceptions/ExceptionWithHumanReadableMessage.html "interface in com.facebook.buck.core.exceptions"))
                    -   com.facebook.buck.shell.[[CommandAlias.UnsupportedPlatformException]{.typeNameLink}](CommandAlias.UnsupportedPlatformException.html "class in com.facebook.buck.shell")
    -   com.facebook.buck.shell.[[WorkerShellStep]{.typeNameLink}](WorkerShellStep.html "class in com.facebook.buck.shell")
        (implements
        com.facebook.buck.step.[Step](../step/Step.html "interface in com.facebook.buck.step"))
    -   com.facebook.buck.shell.[[WorkerToolDescription]{.typeNameLink}](WorkerToolDescription.html "class in com.facebook.buck.shell")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>)
    -   com.facebook.buck.shell.[[WorkerToolDescriptionArg]{.typeNameLink}](WorkerToolDescriptionArg.html "class in com.facebook.buck.shell")
    -   com.facebook.buck.shell.[[WorkerToolDescriptionArg.Builder]{.typeNameLink}](WorkerToolDescriptionArg.Builder.html "class in com.facebook.buck.shell")
:::

::: {.section role="region"}
## Interface Hierarchy {#interface-hierarchy title="Interface Hierarchy"}

-   com.facebook.buck.core.rulekey.[[AddsToRuleKey]{.typeNameLink}](../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey")
    -   com.facebook.buck.shell.[[WorkerTool]{.typeNameLink}](WorkerTool.html "interface in com.facebook.buck.shell")
-   com.facebook.buck.core.description.arg.[[DataTransferObject]{.typeNameLink}](../core/description/arg/DataTransferObject.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.core.description.arg.[[ConstructorArg]{.typeNameLink}](../core/description/arg/ConstructorArg.html "interface in com.facebook.buck.core.description.arg")
        -   com.facebook.buck.core.description.arg.[[BuildRuleArg]{.typeNameLink}](../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")
            -   com.facebook.buck.shell.[[AbstractGenruleDescription.CommonArg]{.typeNameLink}](AbstractGenruleDescription.CommonArg.html "interface in com.facebook.buck.shell")
                (also extends
                com.facebook.buck.core.description.arg.[HasTests](../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg"))
-   com.facebook.buck.core.description.arg.[[HasTests]{.typeNameLink}](../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.shell.[[AbstractGenruleDescription.CommonArg]{.typeNameLink}](AbstractGenruleDescription.CommonArg.html "interface in com.facebook.buck.shell")
        (also extends
        com.facebook.buck.core.description.arg.[BuildRuleArg](../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg"))
-   com.facebook.buck.shell.[[ProvidesWorkerTool]{.typeNameLink}](ProvidesWorkerTool.html "interface in com.facebook.buck.shell")
:::

::: {.section role="region"}
## Enum Hierarchy {#enum-hierarchy title="Enum Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   java.lang.[[Enum]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<E\>
        (implements
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   com.facebook.buck.shell.[[ExportFileDescription.Mode]{.typeNameLink}](ExportFileDescription.Mode.html "enum in com.facebook.buck.shell")
        -   com.facebook.buck.shell.[[ExportFileDirectoryAction]{.typeNameLink}](ExportFileDirectoryAction.html "enum in com.facebook.buck.shell")
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
-   Tree
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

[]{#skip.navbar.bottom}
:::
