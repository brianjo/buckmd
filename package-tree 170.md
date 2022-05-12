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
# Hierarchy For Package com.facebook.buck.jvm.kotlin {#hierarchy-for-package-com.facebook.buck.jvm.kotlin .title}

[Package Hierarchies:]{.packageHierarchyLabel}

-   [All Packages](../../../../../overview-tree.html)
:::

::: contentContainer
::: {.section role="region"}
## Class Hierarchy {#class-hierarchy title="Class Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   com.facebook.buck.jvm.java.[[CompileToJarStepFactory]{.typeNameLink}](../java/CompileToJarStepFactory.html "class in com.facebook.buck.jvm.java")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"))
        -   com.facebook.buck.jvm.kotlin.[[KotlincToJarStepFactory]{.typeNameLink}](KotlincToJarStepFactory.html "class in com.facebook.buck.jvm.kotlin")
            (implements
            com.facebook.buck.core.rulekey.[AddsToRuleKey](../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"))
    -   com.facebook.buck.jvm.java.[[ConfiguredCompilerFactory]{.typeNameLink}](../java/ConfiguredCompilerFactory.html "class in com.facebook.buck.jvm.java")
        -   com.facebook.buck.jvm.kotlin.[[KotlinConfiguredCompilerFactory]{.typeNameLink}](KotlinConfiguredCompilerFactory.html "class in com.facebook.buck.jvm.kotlin")
    -   com.facebook.buck.jvm.kotlin.[[ExternalKotlinc]{.typeNameLink}](ExternalKotlinc.html "class in com.facebook.buck.jvm.kotlin")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"),
        com.facebook.buck.jvm.kotlin.[Kotlinc](Kotlinc.html "interface in com.facebook.buck.jvm.kotlin"))
    -   com.facebook.buck.jvm.kotlin.[[JarBackedReflectedKotlinc]{.typeNameLink}](JarBackedReflectedKotlinc.html "class in com.facebook.buck.jvm.kotlin")
        (implements
        com.facebook.buck.jvm.kotlin.[Kotlinc](Kotlinc.html "interface in com.facebook.buck.jvm.kotlin"))
    -   com.facebook.buck.jvm.kotlin.[[KotlinBuckConfig]{.typeNameLink}](KotlinBuckConfig.html "class in com.facebook.buck.jvm.kotlin")
        (implements
        com.facebook.buck.core.config.[ConfigView](../../core/config/ConfigView.html "interface in com.facebook.buck.core.config")\<T\>)
    -   com.facebook.buck.jvm.kotlin.[[KotlincStep]{.typeNameLink}](KotlincStep.html "class in com.facebook.buck.jvm.kotlin")
        (implements
        com.facebook.buck.step.[Step](../../step/Step.html "interface in com.facebook.buck.step"))
    -   com.facebook.buck.jvm.kotlin.[[KotlinDescriptionsProvider]{.typeNameLink}](KotlinDescriptionsProvider.html "class in com.facebook.buck.jvm.kotlin")
        (implements
        com.facebook.buck.core.model.targetgraph.[DescriptionProvider](../../core/model/targetgraph/DescriptionProvider.html "interface in com.facebook.buck.core.model.targetgraph"))
    -   com.facebook.buck.jvm.kotlin.[[KotlinLibraryDescription]{.typeNameLink}](KotlinLibraryDescription.html "class in com.facebook.buck.jvm.kotlin")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.model.[Flavored](../../core/model/Flavored.html "interface in com.facebook.buck.core.model"),
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>)
    -   com.facebook.buck.jvm.kotlin.[[KotlinLibraryDescriptionArg]{.typeNameLink}](KotlinLibraryDescriptionArg.html "class in com.facebook.buck.jvm.kotlin")
    -   com.facebook.buck.jvm.kotlin.[[KotlinLibraryDescriptionArg.Builder]{.typeNameLink}](KotlinLibraryDescriptionArg.Builder.html "class in com.facebook.buck.jvm.kotlin")
    -   com.facebook.buck.jvm.kotlin.[[KotlinTestDescription]{.typeNameLink}](KotlinTestDescription.html "class in com.facebook.buck.jvm.kotlin")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>)
    -   com.facebook.buck.jvm.kotlin.[[KotlinTestDescriptionArg]{.typeNameLink}](KotlinTestDescriptionArg.html "class in com.facebook.buck.jvm.kotlin")
    -   com.facebook.buck.jvm.kotlin.[[KotlinTestDescriptionArg.Builder]{.typeNameLink}](KotlinTestDescriptionArg.Builder.html "class in com.facebook.buck.jvm.kotlin")
:::

::: {.section role="region"}
## Interface Hierarchy {#interface-hierarchy title="Interface Hierarchy"}

-   com.facebook.buck.core.rulekey.[[AddsToRuleKey]{.typeNameLink}](../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey")
    -   com.facebook.buck.core.toolchain.tool.[[Tool]{.typeNameLink}](../../core/toolchain/tool/Tool.html "interface in com.facebook.buck.core.toolchain.tool")
        -   com.facebook.buck.jvm.kotlin.[[Kotlinc]{.typeNameLink}](Kotlinc.html "interface in com.facebook.buck.jvm.kotlin")
-   com.facebook.buck.core.description.arg.[[DataTransferObject]{.typeNameLink}](../../core/description/arg/DataTransferObject.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.core.description.arg.[[ConstructorArg]{.typeNameLink}](../../core/description/arg/ConstructorArg.html "interface in com.facebook.buck.core.description.arg")
        -   com.facebook.buck.core.description.arg.[[BuildRuleArg]{.typeNameLink}](../../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")
            -   com.facebook.buck.jvm.java.[[JvmLibraryArg]{.typeNameLink}](../java/JvmLibraryArg.html "interface in com.facebook.buck.jvm.java")
                (also extends
                com.facebook.buck.jvm.java.[MaybeRequiredForSourceOnlyAbiArg](../java/MaybeRequiredForSourceOnlyAbiArg.html "interface in com.facebook.buck.jvm.java"))
                -   com.facebook.buck.jvm.java.[[JavaLibraryDescription.CoreArg]{.typeNameLink}](../java/JavaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.java")
                    (also extends
                    com.facebook.buck.core.description.arg.[HasDeclaredDeps](../../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg"),
                    com.facebook.buck.core.description.arg.[HasProvidedDeps](../../core/description/arg/HasProvidedDeps.html "interface in com.facebook.buck.core.description.arg"),
                    com.facebook.buck.core.description.arg.[HasSrcs](../../core/description/arg/HasSrcs.html "interface in com.facebook.buck.core.description.arg"),
                    com.facebook.buck.core.description.arg.[HasTests](../../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg"))
                    -   com.facebook.buck.jvm.kotlin.[[KotlinLibraryDescription.CoreArg]{.typeNameLink}](KotlinLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.kotlin")
-   com.facebook.buck.core.description.arg.[[HasDeclaredDeps]{.typeNameLink}](../../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.jvm.java.[[JavaLibraryDescription.CoreArg]{.typeNameLink}](../java/JavaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.java")
        (also extends
        com.facebook.buck.core.description.arg.[HasProvidedDeps](../../core/description/arg/HasProvidedDeps.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasSrcs](../../core/description/arg/HasSrcs.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasTests](../../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.jvm.java.[JvmLibraryArg](../java/JvmLibraryArg.html "interface in com.facebook.buck.jvm.java"))
        -   com.facebook.buck.jvm.kotlin.[[KotlinLibraryDescription.CoreArg]{.typeNameLink}](KotlinLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.kotlin")
-   com.facebook.buck.core.description.arg.[[HasProvidedDeps]{.typeNameLink}](../../core/description/arg/HasProvidedDeps.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.jvm.java.[[JavaLibraryDescription.CoreArg]{.typeNameLink}](../java/JavaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.java")
        (also extends
        com.facebook.buck.core.description.arg.[HasDeclaredDeps](../../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasSrcs](../../core/description/arg/HasSrcs.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasTests](../../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.jvm.java.[JvmLibraryArg](../java/JvmLibraryArg.html "interface in com.facebook.buck.jvm.java"))
        -   com.facebook.buck.jvm.kotlin.[[KotlinLibraryDescription.CoreArg]{.typeNameLink}](KotlinLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.kotlin")
-   com.facebook.buck.core.description.arg.[[HasSrcs]{.typeNameLink}](../../core/description/arg/HasSrcs.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.jvm.java.[[JavaLibraryDescription.CoreArg]{.typeNameLink}](../java/JavaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.java")
        (also extends
        com.facebook.buck.core.description.arg.[HasDeclaredDeps](../../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasProvidedDeps](../../core/description/arg/HasProvidedDeps.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasTests](../../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.jvm.java.[JvmLibraryArg](../java/JvmLibraryArg.html "interface in com.facebook.buck.jvm.java"))
        -   com.facebook.buck.jvm.kotlin.[[KotlinLibraryDescription.CoreArg]{.typeNameLink}](KotlinLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.kotlin")
-   com.facebook.buck.core.description.arg.[[HasTests]{.typeNameLink}](../../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.jvm.java.[[JavaLibraryDescription.CoreArg]{.typeNameLink}](../java/JavaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.java")
        (also extends
        com.facebook.buck.core.description.arg.[HasDeclaredDeps](../../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasProvidedDeps](../../core/description/arg/HasProvidedDeps.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasSrcs](../../core/description/arg/HasSrcs.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.jvm.java.[JvmLibraryArg](../java/JvmLibraryArg.html "interface in com.facebook.buck.jvm.java"))
        -   com.facebook.buck.jvm.kotlin.[[KotlinLibraryDescription.CoreArg]{.typeNameLink}](KotlinLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.kotlin")
-   com.facebook.buck.jvm.java.[[MaybeRequiredForSourceOnlyAbiArg]{.typeNameLink}](../java/MaybeRequiredForSourceOnlyAbiArg.html "interface in com.facebook.buck.jvm.java")
    -   com.facebook.buck.jvm.java.[[JvmLibraryArg]{.typeNameLink}](../java/JvmLibraryArg.html "interface in com.facebook.buck.jvm.java")
        (also extends
        com.facebook.buck.core.description.arg.[BuildRuleArg](../../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg"))
        -   com.facebook.buck.jvm.java.[[JavaLibraryDescription.CoreArg]{.typeNameLink}](../java/JavaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.java")
            (also extends
            com.facebook.buck.core.description.arg.[HasDeclaredDeps](../../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg"),
            com.facebook.buck.core.description.arg.[HasProvidedDeps](../../core/description/arg/HasProvidedDeps.html "interface in com.facebook.buck.core.description.arg"),
            com.facebook.buck.core.description.arg.[HasSrcs](../../core/description/arg/HasSrcs.html "interface in com.facebook.buck.core.description.arg"),
            com.facebook.buck.core.description.arg.[HasTests](../../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg"))
            -   com.facebook.buck.jvm.kotlin.[[KotlinLibraryDescription.CoreArg]{.typeNameLink}](KotlinLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.kotlin")
:::

::: {.section role="region"}
## Enum Hierarchy {#enum-hierarchy title="Enum Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   java.lang.[[Enum]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<E\>
        (implements
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   com.facebook.buck.jvm.kotlin.[[KotlinLibraryDescription.AnnotationProcessingTool]{.typeNameLink}](KotlinLibraryDescription.AnnotationProcessingTool.html "enum in com.facebook.buck.jvm.kotlin")
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
