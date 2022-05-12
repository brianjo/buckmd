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
# Hierarchy For Package com.facebook.buck.jvm.scala {#hierarchy-for-package-com.facebook.buck.jvm.scala .title}

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
        -   com.facebook.buck.jvm.scala.[[ScalacToJarStepFactory]{.typeNameLink}](ScalacToJarStepFactory.html "class in com.facebook.buck.jvm.scala")
            (implements
            com.facebook.buck.core.rulekey.[AddsToRuleKey](../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"))
    -   com.facebook.buck.jvm.java.[[ConfiguredCompilerFactory]{.typeNameLink}](../java/ConfiguredCompilerFactory.html "class in com.facebook.buck.jvm.java")
        -   com.facebook.buck.jvm.scala.[[ScalaConfiguredCompilerFactory]{.typeNameLink}](ScalaConfiguredCompilerFactory.html "class in com.facebook.buck.jvm.scala")
    -   com.facebook.buck.jvm.scala.[[ScalaBuckConfig]{.typeNameLink}](ScalaBuckConfig.html "class in com.facebook.buck.jvm.scala")
    -   com.facebook.buck.jvm.scala.[[ScalaDescriptionsProvider]{.typeNameLink}](ScalaDescriptionsProvider.html "class in com.facebook.buck.jvm.scala")
        (implements
        com.facebook.buck.core.model.targetgraph.[DescriptionProvider](../../core/model/targetgraph/DescriptionProvider.html "interface in com.facebook.buck.core.model.targetgraph"))
    -   com.facebook.buck.jvm.scala.[[ScalaLibraryDescription]{.typeNameLink}](ScalaLibraryDescription.html "class in com.facebook.buck.jvm.scala")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.model.[Flavored](../../core/model/Flavored.html "interface in com.facebook.buck.core.model"),
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>)
    -   com.facebook.buck.jvm.scala.[[ScalaLibraryDescriptionArg]{.typeNameLink}](ScalaLibraryDescriptionArg.html "class in com.facebook.buck.jvm.scala")
    -   com.facebook.buck.jvm.scala.[[ScalaLibraryDescriptionArg.Builder]{.typeNameLink}](ScalaLibraryDescriptionArg.Builder.html "class in com.facebook.buck.jvm.scala")
    -   com.facebook.buck.jvm.scala.[[ScalaTestDescription]{.typeNameLink}](ScalaTestDescription.html "class in com.facebook.buck.jvm.scala")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>)
    -   com.facebook.buck.jvm.scala.[[ScalaTestDescriptionArg]{.typeNameLink}](ScalaTestDescriptionArg.html "class in com.facebook.buck.jvm.scala")
    -   com.facebook.buck.jvm.scala.[[ScalaTestDescriptionArg.Builder]{.typeNameLink}](ScalaTestDescriptionArg.Builder.html "class in com.facebook.buck.jvm.scala")
    -   com.facebook.buck.shell.[[ShellStep]{.typeNameLink}](../../shell/ShellStep.html "class in com.facebook.buck.shell")
        (implements
        com.facebook.buck.step.[Step](../../step/Step.html "interface in com.facebook.buck.step"))
        -   com.facebook.buck.jvm.scala.[[ScalacStep]{.typeNameLink}](ScalacStep.html "class in com.facebook.buck.jvm.scala")
:::

::: {.section role="region"}
## Interface Hierarchy {#interface-hierarchy title="Interface Hierarchy"}

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
                    -   com.facebook.buck.jvm.scala.[[ScalaLibraryDescription.CoreArg]{.typeNameLink}](ScalaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.scala")
-   com.facebook.buck.core.description.arg.[[HasDeclaredDeps]{.typeNameLink}](../../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.jvm.java.[[JavaLibraryDescription.CoreArg]{.typeNameLink}](../java/JavaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.java")
        (also extends
        com.facebook.buck.core.description.arg.[HasProvidedDeps](../../core/description/arg/HasProvidedDeps.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasSrcs](../../core/description/arg/HasSrcs.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasTests](../../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.jvm.java.[JvmLibraryArg](../java/JvmLibraryArg.html "interface in com.facebook.buck.jvm.java"))
        -   com.facebook.buck.jvm.scala.[[ScalaLibraryDescription.CoreArg]{.typeNameLink}](ScalaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.scala")
-   com.facebook.buck.core.description.arg.[[HasProvidedDeps]{.typeNameLink}](../../core/description/arg/HasProvidedDeps.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.jvm.java.[[JavaLibraryDescription.CoreArg]{.typeNameLink}](../java/JavaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.java")
        (also extends
        com.facebook.buck.core.description.arg.[HasDeclaredDeps](../../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasSrcs](../../core/description/arg/HasSrcs.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasTests](../../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.jvm.java.[JvmLibraryArg](../java/JvmLibraryArg.html "interface in com.facebook.buck.jvm.java"))
        -   com.facebook.buck.jvm.scala.[[ScalaLibraryDescription.CoreArg]{.typeNameLink}](ScalaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.scala")
-   com.facebook.buck.core.description.arg.[[HasSrcs]{.typeNameLink}](../../core/description/arg/HasSrcs.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.jvm.java.[[JavaLibraryDescription.CoreArg]{.typeNameLink}](../java/JavaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.java")
        (also extends
        com.facebook.buck.core.description.arg.[HasDeclaredDeps](../../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasProvidedDeps](../../core/description/arg/HasProvidedDeps.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasTests](../../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.jvm.java.[JvmLibraryArg](../java/JvmLibraryArg.html "interface in com.facebook.buck.jvm.java"))
        -   com.facebook.buck.jvm.scala.[[ScalaLibraryDescription.CoreArg]{.typeNameLink}](ScalaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.scala")
-   com.facebook.buck.core.description.arg.[[HasTests]{.typeNameLink}](../../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.jvm.java.[[JavaLibraryDescription.CoreArg]{.typeNameLink}](../java/JavaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.java")
        (also extends
        com.facebook.buck.core.description.arg.[HasDeclaredDeps](../../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasProvidedDeps](../../core/description/arg/HasProvidedDeps.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasSrcs](../../core/description/arg/HasSrcs.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.jvm.java.[JvmLibraryArg](../java/JvmLibraryArg.html "interface in com.facebook.buck.jvm.java"))
        -   com.facebook.buck.jvm.scala.[[ScalaLibraryDescription.CoreArg]{.typeNameLink}](ScalaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.scala")
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
            -   com.facebook.buck.jvm.scala.[[ScalaLibraryDescription.CoreArg]{.typeNameLink}](ScalaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.scala")
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
