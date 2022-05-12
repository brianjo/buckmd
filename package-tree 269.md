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
# Hierarchy For Package com.facebook.buck.jvm.groovy {#hierarchy-for-package-com.facebook.buck.jvm.groovy .title}

[Package Hierarchies:]{.packageHierarchyLabel}

-   [All Packages](../../../../../overview-tree.html)
:::

::: contentContainer
::: {.section role="region"}
## Class Hierarchy {#class-hierarchy title="Class Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   com.facebook.buck.jvm.java.[[ConfiguredCompilerFactory]{.typeNameLink}](../java/ConfiguredCompilerFactory.html "class in com.facebook.buck.jvm.java")
        -   com.facebook.buck.jvm.groovy.[[GroovyConfiguredCompilerFactory]{.typeNameLink}](GroovyConfiguredCompilerFactory.html "class in com.facebook.buck.jvm.groovy")
    -   com.facebook.buck.jvm.groovy.[[GroovyBuckConfig]{.typeNameLink}](GroovyBuckConfig.html "class in com.facebook.buck.jvm.groovy")
    -   com.facebook.buck.jvm.groovy.[[Groovyc]{.typeNameLink}](Groovyc.html "class in com.facebook.buck.jvm.groovy")
        (implements
        com.facebook.buck.core.toolchain.tool.[Tool](../../core/toolchain/tool/Tool.html "interface in com.facebook.buck.core.toolchain.tool"))
    -   com.facebook.buck.jvm.groovy.[[GroovyDescriptionsProvider]{.typeNameLink}](GroovyDescriptionsProvider.html "class in com.facebook.buck.jvm.groovy")
        (implements
        com.facebook.buck.core.model.targetgraph.[DescriptionProvider](../../core/model/targetgraph/DescriptionProvider.html "interface in com.facebook.buck.core.model.targetgraph"))
    -   com.facebook.buck.jvm.groovy.[[GroovyLibraryDescription]{.typeNameLink}](GroovyLibraryDescription.html "class in com.facebook.buck.jvm.groovy")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>)
    -   com.facebook.buck.jvm.groovy.[[GroovyLibraryDescriptionArg]{.typeNameLink}](GroovyLibraryDescriptionArg.html "class in com.facebook.buck.jvm.groovy")
    -   com.facebook.buck.jvm.groovy.[[GroovyLibraryDescriptionArg.Builder]{.typeNameLink}](GroovyLibraryDescriptionArg.Builder.html "class in com.facebook.buck.jvm.groovy")
    -   com.facebook.buck.jvm.groovy.[[GroovyTestDescription]{.typeNameLink}](GroovyTestDescription.html "class in com.facebook.buck.jvm.groovy")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.description.attr.[ImplicitDepsInferringDescription](../../core/description/attr/ImplicitDepsInferringDescription.html "interface in com.facebook.buck.core.description.attr")\<T\>)
    -   com.facebook.buck.jvm.groovy.[[GroovyTestDescriptionArg]{.typeNameLink}](GroovyTestDescriptionArg.html "class in com.facebook.buck.jvm.groovy")
    -   com.facebook.buck.jvm.groovy.[[GroovyTestDescriptionArg.Builder]{.typeNameLink}](GroovyTestDescriptionArg.Builder.html "class in com.facebook.buck.jvm.groovy")
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
                    -   com.facebook.buck.jvm.groovy.[[GroovyLibraryDescription.CoreArg]{.typeNameLink}](GroovyLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.groovy")
-   com.facebook.buck.core.description.arg.[[HasDeclaredDeps]{.typeNameLink}](../../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.jvm.java.[[JavaLibraryDescription.CoreArg]{.typeNameLink}](../java/JavaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.java")
        (also extends
        com.facebook.buck.core.description.arg.[HasProvidedDeps](../../core/description/arg/HasProvidedDeps.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasSrcs](../../core/description/arg/HasSrcs.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasTests](../../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.jvm.java.[JvmLibraryArg](../java/JvmLibraryArg.html "interface in com.facebook.buck.jvm.java"))
        -   com.facebook.buck.jvm.groovy.[[GroovyLibraryDescription.CoreArg]{.typeNameLink}](GroovyLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.groovy")
-   com.facebook.buck.core.description.arg.[[HasProvidedDeps]{.typeNameLink}](../../core/description/arg/HasProvidedDeps.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.jvm.java.[[JavaLibraryDescription.CoreArg]{.typeNameLink}](../java/JavaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.java")
        (also extends
        com.facebook.buck.core.description.arg.[HasDeclaredDeps](../../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasSrcs](../../core/description/arg/HasSrcs.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasTests](../../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.jvm.java.[JvmLibraryArg](../java/JvmLibraryArg.html "interface in com.facebook.buck.jvm.java"))
        -   com.facebook.buck.jvm.groovy.[[GroovyLibraryDescription.CoreArg]{.typeNameLink}](GroovyLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.groovy")
-   com.facebook.buck.core.description.arg.[[HasSrcs]{.typeNameLink}](../../core/description/arg/HasSrcs.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.jvm.java.[[JavaLibraryDescription.CoreArg]{.typeNameLink}](../java/JavaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.java")
        (also extends
        com.facebook.buck.core.description.arg.[HasDeclaredDeps](../../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasProvidedDeps](../../core/description/arg/HasProvidedDeps.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasTests](../../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.jvm.java.[JvmLibraryArg](../java/JvmLibraryArg.html "interface in com.facebook.buck.jvm.java"))
        -   com.facebook.buck.jvm.groovy.[[GroovyLibraryDescription.CoreArg]{.typeNameLink}](GroovyLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.groovy")
-   com.facebook.buck.core.description.arg.[[HasTests]{.typeNameLink}](../../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg")
    -   com.facebook.buck.jvm.java.[[JavaLibraryDescription.CoreArg]{.typeNameLink}](../java/JavaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.java")
        (also extends
        com.facebook.buck.core.description.arg.[HasDeclaredDeps](../../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasProvidedDeps](../../core/description/arg/HasProvidedDeps.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.core.description.arg.[HasSrcs](../../core/description/arg/HasSrcs.html "interface in com.facebook.buck.core.description.arg"),
        com.facebook.buck.jvm.java.[JvmLibraryArg](../java/JvmLibraryArg.html "interface in com.facebook.buck.jvm.java"))
        -   com.facebook.buck.jvm.groovy.[[GroovyLibraryDescription.CoreArg]{.typeNameLink}](GroovyLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.groovy")
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
            -   com.facebook.buck.jvm.groovy.[[GroovyLibraryDescription.CoreArg]{.typeNameLink}](GroovyLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.groovy")
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
