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
# Hierarchy For Package com.facebook.buck.versions {#hierarchy-for-package-com.facebook.buck.versions .title}

[Package Hierarchies:]{.packageHierarchyLabel}

-   [All Packages](../../../../overview-tree.html)
:::

::: contentContainer
::: {.section role="region"}
## Class Hierarchy {#class-hierarchy title="Class Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   com.facebook.buck.event.[[AbstractBuckEvent]{.typeNameLink}](../event/AbstractBuckEvent.html "class in com.facebook.buck.event")
        (implements
        com.facebook.buck.event.[BuckEvent](../event/BuckEvent.html "interface in com.facebook.buck.event"))
        -   com.facebook.buck.versions.[[VersionedTargetGraphEvent]{.typeNameLink}](VersionedTargetGraphEvent.html "class in com.facebook.buck.versions")
            (implements
            com.facebook.buck.event.[LeafEvent](../event/LeafEvent.html "interface in com.facebook.buck.event"),
            com.facebook.buck.event.[WorkAdvanceEvent](../event/WorkAdvanceEvent.html "interface in com.facebook.buck.event"))
            -   com.facebook.buck.versions.[[VersionedTargetGraphEvent.Cache]{.typeNameLink}](VersionedTargetGraphEvent.Cache.html "class in com.facebook.buck.versions")
                (implements
                com.facebook.buck.event.[BuckEvent](../event/BuckEvent.html "interface in com.facebook.buck.event"))
                -   com.facebook.buck.versions.[[VersionedTargetGraphEvent.Cache.Hit]{.typeNameLink}](VersionedTargetGraphEvent.Cache.Hit.html "class in com.facebook.buck.versions")
                -   com.facebook.buck.versions.[[VersionedTargetGraphEvent.Cache.Miss]{.typeNameLink}](VersionedTargetGraphEvent.Cache.Miss.html "class in com.facebook.buck.versions")
            -   com.facebook.buck.versions.[[VersionedTargetGraphEvent.Finished]{.typeNameLink}](VersionedTargetGraphEvent.Finished.html "class in com.facebook.buck.versions")
            -   com.facebook.buck.versions.[[VersionedTargetGraphEvent.Started]{.typeNameLink}](VersionedTargetGraphEvent.Started.html "class in com.facebook.buck.versions")
            -   com.facebook.buck.versions.[[VersionedTargetGraphEvent.Timeout]{.typeNameLink}](VersionedTargetGraphEvent.Timeout.html "class in com.facebook.buck.versions")
    -   com.facebook.buck.versions.[[AbstractVersionedTargetGraphBuilder]{.typeNameLink}](AbstractVersionedTargetGraphBuilder.html "class in com.facebook.buck.versions")
        (implements
        com.facebook.buck.versions.[VersionedTargetGraphBuilder](VersionedTargetGraphBuilder.html "interface in com.facebook.buck.versions"))
        -   com.facebook.buck.versions.[[AsyncVersionedTargetGraphBuilder]{.typeNameLink}](AsyncVersionedTargetGraphBuilder.html "class in com.facebook.buck.versions")
    -   com.facebook.buck.core.util.graph.[[DirectedAcyclicGraph]{.typeNameLink}](../core/util/graph/DirectedAcyclicGraph.html "class in com.facebook.buck.core.util.graph")\<T\>
        (implements
        com.facebook.buck.core.util.graph.[TraversableGraph](../core/util/graph/TraversableGraph.html "interface in com.facebook.buck.core.util.graph")\<T\>)
        -   com.facebook.buck.core.model.targetgraph.[[TargetGraph]{.typeNameLink}](../core/model/targetgraph/TargetGraph.html "class in com.facebook.buck.core.model.targetgraph")
            -   com.facebook.buck.versions.[[VersionedTargetGraph]{.typeNameLink}](VersionedTargetGraph.html "class in com.facebook.buck.versions")
    -   com.facebook.buck.versions.[[ExactConstraint]{.typeNameLink}](ExactConstraint.html "class in com.facebook.buck.versions")
        (implements
        com.facebook.buck.versions.[Constraint](Constraint.html "interface in com.facebook.buck.versions"))
    -   com.facebook.buck.versions.ImmutableVersionUniverse.Builder
        -   com.facebook.buck.versions.[[VersionUniverse.Builder]{.typeNameLink}](VersionUniverse.Builder.html "class in com.facebook.buck.versions")
    -   com.facebook.buck.versions.[[InstrumentedVersionedTargetGraphCache]{.typeNameLink}](InstrumentedVersionedTargetGraphCache.html "class in com.facebook.buck.versions")
    -   com.facebook.buck.versions.[[QueryTargetTranslator]{.typeNameLink}](QueryTargetTranslator.html "class in com.facebook.buck.versions")
    -   com.facebook.buck.versions.[[TargetNodeTranslator]{.typeNameLink}](TargetNodeTranslator.html "class in com.facebook.buck.versions")
    -   java.lang.[[Throwable]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Throwable.html?is-external=true "class or interface in java.lang"){.externalLink}
        (implements
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   java.lang.[[Exception]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Exception.html?is-external=true "class or interface in java.lang"){.externalLink}
            -   com.facebook.buck.versions.[[VersionException]{.typeNameLink}](VersionException.html "class in com.facebook.buck.versions")
    -   com.facebook.buck.versions.[[VersionBuckConfig]{.typeNameLink}](VersionBuckConfig.html "class in com.facebook.buck.versions")
    -   com.facebook.buck.versions.[[VersionDescriptionsProvider]{.typeNameLink}](VersionDescriptionsProvider.html "class in com.facebook.buck.versions")
        (implements
        com.facebook.buck.core.model.targetgraph.[DescriptionProvider](../core/model/targetgraph/DescriptionProvider.html "interface in com.facebook.buck.core.model.targetgraph"))
    -   com.facebook.buck.versions.[[VersionedAliasDescription]{.typeNameLink}](VersionedAliasDescription.html "class in com.facebook.buck.versions")
        (implements
        com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>)
    -   com.facebook.buck.versions.[[VersionedAliasDescriptionArg]{.typeNameLink}](VersionedAliasDescriptionArg.html "class in com.facebook.buck.versions")
    -   com.facebook.buck.versions.[[VersionedAliasDescriptionArg.Builder]{.typeNameLink}](VersionedAliasDescriptionArg.Builder.html "class in com.facebook.buck.versions")
    -   com.facebook.buck.versions.[[VersionedTargetGraph.Builder]{.typeNameLink}](VersionedTargetGraph.Builder.html "class in com.facebook.buck.versions")
    -   com.facebook.buck.versions.[[VersionedTargetGraphCache]{.typeNameLink}](VersionedTargetGraphCache.html "class in com.facebook.buck.versions")
    -   com.facebook.buck.versions.[[VersionUniverse]{.typeNameLink}](VersionUniverse.html "class in com.facebook.buck.versions")
    -   com.facebook.buck.versions.[[VersionUniverseVersionSelector]{.typeNameLink}](VersionUniverseVersionSelector.html "class in com.facebook.buck.versions")
        (implements
        com.facebook.buck.versions.[VersionSelector](VersionSelector.html "interface in com.facebook.buck.versions"))
:::

::: {.section role="region"}
## Interface Hierarchy {#interface-hierarchy title="Interface Hierarchy"}

-   com.facebook.buck.core.description.[[BaseDescription]{.typeNameLink}](../core/description/BaseDescription.html "interface in com.facebook.buck.core.description")\<T\>
    -   com.facebook.buck.core.description.[[Description]{.typeNameLink}](../core/description/Description.html "interface in com.facebook.buck.core.description")\<T\>
        -   com.facebook.buck.core.rules.[[DescriptionWithTargetGraph]{.typeNameLink}](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")\<T\>
            -   com.facebook.buck.versions.[[VersionPropagator]{.typeNameLink}](VersionPropagator.html "interface in com.facebook.buck.versions")\<A\>
            -   com.facebook.buck.versions.[[VersionRoot]{.typeNameLink}](VersionRoot.html "interface in com.facebook.buck.versions")\<A\>
-   com.facebook.buck.versions.[[Constraint]{.typeNameLink}](Constraint.html "interface in com.facebook.buck.versions")
-   com.facebook.buck.versions.[[HasVersionUniverse]{.typeNameLink}](HasVersionUniverse.html "interface in com.facebook.buck.versions")
-   com.facebook.buck.versions.[[TargetTranslatable]{.typeNameLink}](TargetTranslatable.html "interface in com.facebook.buck.versions")\<T\>
-   com.facebook.buck.versions.[[Version]{.typeNameLink}](Version.html "interface in com.facebook.buck.versions")
-   com.facebook.buck.versions.[[VersionedTargetGraphBuilder]{.typeNameLink}](VersionedTargetGraphBuilder.html "interface in com.facebook.buck.versions")
-   com.facebook.buck.versions.[[VersionSelector]{.typeNameLink}](VersionSelector.html "interface in com.facebook.buck.versions")
:::

::: {.section role="region"}
## Enum Hierarchy {#enum-hierarchy title="Enum Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   java.lang.[[Enum]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<E\>
        (implements
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   com.facebook.buck.versions.[[VersionedTargetGraphCache.ResultType]{.typeNameLink}](VersionedTargetGraphCache.ResultType.html "enum in com.facebook.buck.versions")
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
