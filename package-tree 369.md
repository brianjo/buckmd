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
# Hierarchy For Package com.facebook.buck.util.versioncontrol {#hierarchy-for-package-com.facebook.buck.util.versioncontrol .title}

[Package Hierarchies:]{.packageHierarchyLabel}

-   [All Packages](../../../../../overview-tree.html)
:::

::: contentContainer
::: {.section role="region"}
## Class Hierarchy {#class-hierarchy title="Class Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   com.facebook.buck.event.[[AbstractBuckEvent]{.typeNameLink}](../../event/AbstractBuckEvent.html "class in com.facebook.buck.event")
        (implements
        com.facebook.buck.event.[BuckEvent](../../event/BuckEvent.html "interface in com.facebook.buck.event"))
        -   com.facebook.buck.util.versioncontrol.[[FastVersionControlStatsEvent]{.typeNameLink}](FastVersionControlStatsEvent.html "class in com.facebook.buck.util.versioncontrol")
        -   com.facebook.buck.util.versioncontrol.[[VersionControlStatsEvent]{.typeNameLink}](VersionControlStatsEvent.html "class in com.facebook.buck.util.versioncontrol")
    -   com.facebook.buck.util.versioncontrol.[[DelegatingVersionControlCmdLineInterface]{.typeNameLink}](DelegatingVersionControlCmdLineInterface.html "class in com.facebook.buck.util.versioncontrol")
        (implements
        com.facebook.buck.util.versioncontrol.[VersionControlCmdLineInterface](VersionControlCmdLineInterface.html "interface in com.facebook.buck.util.versioncontrol"))
    -   com.facebook.buck.util.versioncontrol.[[HgCmdLineInterface]{.typeNameLink}](HgCmdLineInterface.html "class in com.facebook.buck.util.versioncontrol")
        (implements
        com.facebook.buck.util.versioncontrol.[VersionControlCmdLineInterface](VersionControlCmdLineInterface.html "interface in com.facebook.buck.util.versioncontrol"))
    -   com.facebook.buck.util.versioncontrol.ImmutableFullVersionControlStats.Builder
        -   com.facebook.buck.util.versioncontrol.[[FullVersionControlStats.Builder]{.typeNameLink}](FullVersionControlStats.Builder.html "class in com.facebook.buck.util.versioncontrol")
    -   com.facebook.buck.util.versioncontrol.[[NoOpCmdLineInterface]{.typeNameLink}](NoOpCmdLineInterface.html "class in com.facebook.buck.util.versioncontrol")
        (implements
        com.facebook.buck.util.versioncontrol.[VersionControlCmdLineInterface](VersionControlCmdLineInterface.html "interface in com.facebook.buck.util.versioncontrol"))
    -   java.lang.[[Throwable]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Throwable.html?is-external=true "class or interface in java.lang"){.externalLink}
        (implements
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   java.lang.[[Exception]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Exception.html?is-external=true "class or interface in java.lang"){.externalLink}
            -   com.facebook.buck.util.versioncontrol.[[VersionControlCommandFailedException]{.typeNameLink}](VersionControlCommandFailedException.html "class in com.facebook.buck.util.versioncontrol")
    -   com.facebook.buck.util.versioncontrol.[[VersionControlBuckConfig]{.typeNameLink}](VersionControlBuckConfig.html "class in com.facebook.buck.util.versioncontrol")
    -   com.facebook.buck.util.versioncontrol.[[VersionControlStatsGenerator]{.typeNameLink}](VersionControlStatsGenerator.html "class in com.facebook.buck.util.versioncontrol")
:::

::: {.section role="region"}
## Interface Hierarchy {#interface-hierarchy title="Interface Hierarchy"}

-   com.facebook.buck.util.versioncontrol.[[CommonFastVersionControlStats]{.typeNameLink}](CommonFastVersionControlStats.html "interface in com.facebook.buck.util.versioncontrol")
    -   com.facebook.buck.util.versioncontrol.[[CommonSlowVersionControlStats]{.typeNameLink}](CommonSlowVersionControlStats.html "interface in com.facebook.buck.util.versioncontrol")
        -   com.facebook.buck.util.versioncontrol.[[FullVersionControlStats]{.typeNameLink}](FullVersionControlStats.html "interface in com.facebook.buck.util.versioncontrol")
-   com.facebook.buck.util.versioncontrol.[[VersionControlCmdLineInterface]{.typeNameLink}](VersionControlCmdLineInterface.html "interface in com.facebook.buck.util.versioncontrol")
-   com.facebook.buck.util.versioncontrol.[[VersionControlSupplier]{.typeNameLink}](VersionControlSupplier.html "interface in com.facebook.buck.util.versioncontrol")\<T\>
:::

::: {.section role="region"}
## Enum Hierarchy {#enum-hierarchy title="Enum Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   java.lang.[[Enum]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<E\>
        (implements
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   com.facebook.buck.util.versioncontrol.[[VersionControlStatsGenerator.Mode]{.typeNameLink}](VersionControlStatsGenerator.Mode.html "enum in com.facebook.buck.util.versioncontrol")
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
