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
# Hierarchy For Package com.facebook.buck.file {#hierarchy-for-package-com.facebook.buck.file .title}

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
            -   com.facebook.buck.file.[[HttpArchive]{.typeNameLink}](HttpArchive.html "class in com.facebook.buck.file")
            -   com.facebook.buck.file.[[HttpFile]{.typeNameLink}](HttpFile.html "class in com.facebook.buck.file")
                -   com.facebook.buck.file.[[HttpFileBinary]{.typeNameLink}](HttpFileBinary.html "class in com.facebook.buck.file")
                    (implements
                    com.facebook.buck.core.rules.tool.[BinaryBuildRule](../core/rules/tool/BinaryBuildRule.html "interface in com.facebook.buck.core.rules.tool"))
            -   com.facebook.buck.file.[[RemoteFile]{.typeNameLink}](RemoteFile.html "class in com.facebook.buck.file")
                -   com.facebook.buck.file.[[RemoteFileBinary]{.typeNameLink}](RemoteFileBinary.html "class in com.facebook.buck.file")
                    (implements
                    com.facebook.buck.core.rules.tool.[BinaryBuildRule](../core/rules/tool/BinaryBuildRule.html "interface in com.facebook.buck.core.rules.tool"))
        -   com.facebook.buck.file.[[WriteFile]{.typeNameLink}](WriteFile.html "class in com.facebook.buck.file")
    -   com.facebook.buck.file.[[DownloadStep]{.typeNameLink}](DownloadStep.html "class in com.facebook.buck.file")
        (implements
        com.facebook.buck.step.[Step](../step/Step.html "interface in com.facebook.buck.step"))
    -   com.facebook.buck.file.[[FileDescriptionsProvider]{.typeNameLink}](FileDescriptionsProvider.html "class in com.facebook.buck.file")
        (implements
        com.facebook.buck.core.model.targetgraph.[DescriptionProvider](../core/model/targetgraph/DescriptionProvider.html "interface in com.facebook.buck.core.model.targetgraph"))
    -   com.facebook.buck.file.[[FileHash]{.typeNameLink}](FileHash.html "class in com.facebook.buck.file")
    -   com.facebook.buck.file.[[HttpArchiveDescription]{.typeNameLink}](HttpArchiveDescription.html "class in com.facebook.buck.file")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.rules.[LegacyProviderCompatibleDescription](../core/rules/LegacyProviderCompatibleDescription.html "interface in com.facebook.buck.core.rules")\<T\>)
    -   com.facebook.buck.file.[[HttpArchiveDescriptionArg]{.typeNameLink}](HttpArchiveDescriptionArg.html "class in com.facebook.buck.file")
    -   com.facebook.buck.file.[[HttpArchiveDescriptionArg.Builder]{.typeNameLink}](HttpArchiveDescriptionArg.Builder.html "class in com.facebook.buck.file")
    -   com.facebook.buck.file.[[HttpFileDescription]{.typeNameLink}](HttpFileDescription.html "class in com.facebook.buck.file")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>,
        com.facebook.buck.core.rules.[LegacyProviderCompatibleDescription](../core/rules/LegacyProviderCompatibleDescription.html "interface in com.facebook.buck.core.rules")\<T\>)
    -   com.facebook.buck.file.[[HttpFileDescriptionArg]{.typeNameLink}](HttpFileDescriptionArg.html "class in com.facebook.buck.file")
    -   com.facebook.buck.file.[[HttpFileDescriptionArg.Builder]{.typeNameLink}](HttpFileDescriptionArg.Builder.html "class in com.facebook.buck.file")
    -   com.facebook.buck.file.[[RemoteFileDescription]{.typeNameLink}](RemoteFileDescription.html "class in com.facebook.buck.file")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>)
    -   com.facebook.buck.file.[[RemoteFileDescriptionArg]{.typeNameLink}](RemoteFileDescriptionArg.html "class in com.facebook.buck.file")
    -   com.facebook.buck.file.[[RemoteFileDescriptionArg.Builder]{.typeNameLink}](RemoteFileDescriptionArg.Builder.html "class in com.facebook.buck.file")
:::

::: {.section role="region"}
## Enum Hierarchy {#enum-hierarchy title="Enum Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   java.lang.[[Enum]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<E\>
        (implements
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   com.facebook.buck.file.[[RemoteFile.Type]{.typeNameLink}](RemoteFile.Type.html "enum in com.facebook.buck.file")
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
