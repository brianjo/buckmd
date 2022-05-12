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
# Hierarchy For Package com.facebook.buck.core.artifact {#hierarchy-for-package-com.facebook.buck.core.artifact .title}

[Package Hierarchies:]{.packageHierarchyLabel}

-   [All Packages](../../../../../overview-tree.html)
:::

::: contentContainer
::: {.section role="region"}
## Class Hierarchy {#class-hierarchy title="Class Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   com.facebook.buck.core.artifact.[[ArtifactFilesystem]{.typeNameLink}](ArtifactFilesystem.html "class in com.facebook.buck.core.artifact")
    -   com.facebook.buck.core.artifact.[[BuildArtifactFactory]{.typeNameLink}](BuildArtifactFactory.html "class in com.facebook.buck.core.artifact")
    -   com.facebook.buck.core.artifact.[[BuildTargetSourcePathToArtifactConverter]{.typeNameLink}](BuildTargetSourcePathToArtifactConverter.html "class in com.facebook.buck.core.artifact")
    -   com.facebook.buck.core.artifact.[[OutputArtifact]{.typeNameLink}](OutputArtifact.html "class in com.facebook.buck.core.artifact")
        (implements
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"),
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        com.facebook.buck.core.starlark.rule.artifact.[SkylarkOutputArtifactApi](../starlark/rule/artifact/SkylarkOutputArtifactApi.html "interface in com.facebook.buck.core.starlark.rule.artifact"))
    -   com.facebook.buck.core.artifact.[[SourceArtifactImpl]{.typeNameLink}](SourceArtifactImpl.html "class in com.facebook.buck.core.artifact")
        (implements
        com.facebook.buck.core.artifact.[BoundArtifact](BoundArtifact.html "interface in com.facebook.buck.core.artifact"),
        com.facebook.buck.core.artifact.[SourceArtifact](SourceArtifact.html "interface in com.facebook.buck.core.artifact"))
    -   java.lang.[[Throwable]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Throwable.html?is-external=true "class or interface in java.lang"){.externalLink}
        (implements
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   java.lang.[[Exception]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Exception.html?is-external=true "class or interface in java.lang"){.externalLink}
            -   java.lang.[[RuntimeException]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/RuntimeException.html?is-external=true "class or interface in java.lang"){.externalLink}
                -   com.facebook.buck.core.exceptions.[[HumanReadableException]{.typeNameLink}](../exceptions/HumanReadableException.html "class in com.facebook.buck.core.exceptions")
                    (implements
                    com.facebook.buck.core.exceptions.[ExceptionWithHumanReadableMessage](../exceptions/ExceptionWithHumanReadableMessage.html "interface in com.facebook.buck.core.exceptions"))
                    -   com.facebook.buck.core.artifact.[[ArtifactDeclarationException]{.typeNameLink}](ArtifactDeclarationException.html "class in com.facebook.buck.core.artifact")
:::

::: {.section role="region"}
## Interface Hierarchy {#interface-hierarchy title="Interface Hierarchy"}

-   com.facebook.buck.core.rulekey.[[AddsToRuleKey]{.typeNameLink}](../rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey")
    -   com.facebook.buck.core.artifact.[[Artifact]{.typeNameLink}](Artifact.html "interface in com.facebook.buck.core.artifact")
        (also extends
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        com.facebook.buck.core.starlark.rule.artifact.[SkylarkArtifactApi](../starlark/rule/artifact/SkylarkArtifactApi.html "interface in com.facebook.buck.core.starlark.rule.artifact"))
        -   com.facebook.buck.core.artifact.[[BoundArtifact]{.typeNameLink}](BoundArtifact.html "interface in com.facebook.buck.core.artifact")
        -   com.facebook.buck.core.artifact.[[BuildArtifact]{.typeNameLink}](BuildArtifact.html "interface in com.facebook.buck.core.artifact")
        -   com.facebook.buck.core.artifact.[[SourceArtifact]{.typeNameLink}](SourceArtifact.html "interface in com.facebook.buck.core.artifact")
-   java.lang.[[Comparable]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>
    -   com.facebook.buck.core.artifact.[[Artifact]{.typeNameLink}](Artifact.html "interface in com.facebook.buck.core.artifact")
        (also extends
        com.facebook.buck.core.rulekey.[AddsToRuleKey](../rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"),
        com.facebook.buck.core.starlark.rule.artifact.[SkylarkArtifactApi](../starlark/rule/artifact/SkylarkArtifactApi.html "interface in com.facebook.buck.core.starlark.rule.artifact"))
        -   com.facebook.buck.core.artifact.[[BoundArtifact]{.typeNameLink}](BoundArtifact.html "interface in com.facebook.buck.core.artifact")
        -   com.facebook.buck.core.artifact.[[BuildArtifact]{.typeNameLink}](BuildArtifact.html "interface in com.facebook.buck.core.artifact")
        -   com.facebook.buck.core.artifact.[[SourceArtifact]{.typeNameLink}](SourceArtifact.html "interface in com.facebook.buck.core.artifact")
-   com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable
    -   com.google.devtools.build.lib.skylarkinterface.SkylarkValue
        -   com.facebook.buck.core.starlark.rule.artifact.[[SkylarkArtifactApi]{.typeNameLink}](../starlark/rule/artifact/SkylarkArtifactApi.html "interface in com.facebook.buck.core.starlark.rule.artifact")
            -   com.facebook.buck.core.artifact.[[Artifact]{.typeNameLink}](Artifact.html "interface in com.facebook.buck.core.artifact")
                (also extends
                com.facebook.buck.core.rulekey.[AddsToRuleKey](../rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey"),
                java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>)
                -   com.facebook.buck.core.artifact.[[BoundArtifact]{.typeNameLink}](BoundArtifact.html "interface in com.facebook.buck.core.artifact")
                -   com.facebook.buck.core.artifact.[[BuildArtifact]{.typeNameLink}](BuildArtifact.html "interface in com.facebook.buck.core.artifact")
                -   com.facebook.buck.core.artifact.[[SourceArtifact]{.typeNameLink}](SourceArtifact.html "interface in com.facebook.buck.core.artifact")
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
