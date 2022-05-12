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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   Tree
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
# Hierarchy For Package com.facebook.buck.core.model.targetgraph {#hierarchy-for-package-com.facebook.buck.core.model.targetgraph .title}

[Package Hierarchies:]{.packageHierarchyLabel}

-   [All Packages](../../../../../../overview-tree.html)
:::

::: contentContainer
::: {.section role="region"}
## Class Hierarchy {#class-hierarchy title="Class Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   com.facebook.buck.core.util.graph.[[DirectedAcyclicGraph]{.typeNameLink}](../../util/graph/DirectedAcyclicGraph.html "class in com.facebook.buck.core.util.graph")\<T\>
        (implements
        com.facebook.buck.core.util.graph.[TraversableGraph](../../util/graph/TraversableGraph.html "interface in com.facebook.buck.core.util.graph")\<T\>)
        -   com.facebook.buck.core.model.targetgraph.[[MergedTargetGraph]{.typeNameLink}](MergedTargetGraph.html "class in com.facebook.buck.core.model.targetgraph")
        -   com.facebook.buck.core.model.targetgraph.[[TargetGraph]{.typeNameLink}](TargetGraph.html "class in com.facebook.buck.core.model.targetgraph")
    -   com.facebook.buck.core.model.targetgraph.[[MergedTargetNode]{.typeNameLink}](MergedTargetNode.html "class in com.facebook.buck.core.model.targetgraph")
        (implements
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>)
    -   com.facebook.buck.core.model.targetgraph.[[TargetGraphCreationResult]{.typeNameLink}](TargetGraphCreationResult.html "class in com.facebook.buck.core.model.targetgraph")
    -   com.facebook.buck.core.model.targetgraph.[[TargetNodeMaybeIncompatible]{.typeNameLink}](TargetNodeMaybeIncompatible.html "class in com.facebook.buck.core.model.targetgraph")
    -   java.lang.[[Throwable]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Throwable.html?is-external=true "class or interface in java.lang"){.externalLink}
        (implements
        java.io.[Serializable](http://docs.oracle.com/javase/7/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"){.externalLink})
        -   java.lang.[[Exception]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Exception.html?is-external=true "class or interface in java.lang"){.externalLink}
            -   java.lang.[[RuntimeException]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/RuntimeException.html?is-external=true "class or interface in java.lang"){.externalLink}
                -   com.facebook.buck.core.model.targetgraph.[[NoSuchTargetException]{.typeNameLink}](NoSuchTargetException.html "class in com.facebook.buck.core.model.targetgraph")
                    (implements
                    com.facebook.buck.core.exceptions.[ExceptionWithHumanReadableMessage](../../exceptions/ExceptionWithHumanReadableMessage.html "interface in com.facebook.buck.core.exceptions"))
:::

::: {.section role="region"}
## Interface Hierarchy {#interface-hierarchy title="Interface Hierarchy"}

-   java.lang.[[Comparable]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>
    -   com.facebook.buck.core.model.targetgraph.[[TargetNode]{.typeNameLink}](TargetNode.html "interface in com.facebook.buck.core.model.targetgraph")\<T\>
        (also extends
        com.facebook.buck.core.graph.transformation.model.[ComputeResult](../../graph/transformation/model/ComputeResult.html "interface in com.facebook.buck.core.graph.transformation.model"),
        com.facebook.buck.core.exceptions.[DependencyStack.ProvidesElement](../../exceptions/DependencyStack.ProvidesElement.html "interface in com.facebook.buck.core.exceptions"),
        com.facebook.buck.core.model.[HasBuildTarget](../HasBuildTarget.html "interface in com.facebook.buck.core.model"),
        com.facebook.buck.rules.visibility.[ObeysVisibility](../../../rules/visibility/ObeysVisibility.html "interface in com.facebook.buck.rules.visibility"))
-   com.facebook.buck.core.graph.transformation.model.[[ComputeResult]{.typeNameLink}](../../graph/transformation/model/ComputeResult.html "interface in com.facebook.buck.core.graph.transformation.model")
    -   com.facebook.buck.core.model.targetgraph.[[TargetNode]{.typeNameLink}](TargetNode.html "interface in com.facebook.buck.core.model.targetgraph")\<T\>
        (also extends
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        com.facebook.buck.core.exceptions.[DependencyStack.ProvidesElement](../../exceptions/DependencyStack.ProvidesElement.html "interface in com.facebook.buck.core.exceptions"),
        com.facebook.buck.core.model.[HasBuildTarget](../HasBuildTarget.html "interface in com.facebook.buck.core.model"),
        com.facebook.buck.rules.visibility.[ObeysVisibility](../../../rules/visibility/ObeysVisibility.html "interface in com.facebook.buck.rules.visibility"))
-   com.facebook.buck.core.exceptions.[[DependencyStack.ProvidesElement]{.typeNameLink}](../../exceptions/DependencyStack.ProvidesElement.html "interface in com.facebook.buck.core.exceptions")
    -   com.facebook.buck.core.model.targetgraph.[[TargetNode]{.typeNameLink}](TargetNode.html "interface in com.facebook.buck.core.model.targetgraph")\<T\>
        (also extends
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        com.facebook.buck.core.graph.transformation.model.[ComputeResult](../../graph/transformation/model/ComputeResult.html "interface in com.facebook.buck.core.graph.transformation.model"),
        com.facebook.buck.core.model.[HasBuildTarget](../HasBuildTarget.html "interface in com.facebook.buck.core.model"),
        com.facebook.buck.rules.visibility.[ObeysVisibility](../../../rules/visibility/ObeysVisibility.html "interface in com.facebook.buck.rules.visibility"))
-   org.pf4j.ExtensionPoint
    -   com.facebook.buck.core.model.targetgraph.[[BuiltInProviderProvider]{.typeNameLink}](BuiltInProviderProvider.html "interface in com.facebook.buck.core.model.targetgraph")
    -   com.facebook.buck.core.model.targetgraph.[[DescriptionProvider]{.typeNameLink}](DescriptionProvider.html "interface in com.facebook.buck.core.model.targetgraph")
-   com.facebook.buck.core.model.[[HasBuildTarget]{.typeNameLink}](../HasBuildTarget.html "interface in com.facebook.buck.core.model")
    -   com.facebook.buck.core.model.targetgraph.[[TargetNode]{.typeNameLink}](TargetNode.html "interface in com.facebook.buck.core.model.targetgraph")\<T\>
        (also extends
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        com.facebook.buck.core.graph.transformation.model.[ComputeResult](../../graph/transformation/model/ComputeResult.html "interface in com.facebook.buck.core.graph.transformation.model"),
        com.facebook.buck.core.exceptions.[DependencyStack.ProvidesElement](../../exceptions/DependencyStack.ProvidesElement.html "interface in com.facebook.buck.core.exceptions"),
        com.facebook.buck.rules.visibility.[ObeysVisibility](../../../rules/visibility/ObeysVisibility.html "interface in com.facebook.buck.rules.visibility"))
-   com.facebook.buck.core.model.targetgraph.[[NodeCopier]{.typeNameLink}](NodeCopier.html "interface in com.facebook.buck.core.model.targetgraph")
-   com.facebook.buck.rules.visibility.[[ObeysVisibility]{.typeNameLink}](../../../rules/visibility/ObeysVisibility.html "interface in com.facebook.buck.rules.visibility")
    -   com.facebook.buck.core.model.targetgraph.[[TargetNode]{.typeNameLink}](TargetNode.html "interface in com.facebook.buck.core.model.targetgraph")\<T\>
        (also extends
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        com.facebook.buck.core.graph.transformation.model.[ComputeResult](../../graph/transformation/model/ComputeResult.html "interface in com.facebook.buck.core.graph.transformation.model"),
        com.facebook.buck.core.exceptions.[DependencyStack.ProvidesElement](../../exceptions/DependencyStack.ProvidesElement.html "interface in com.facebook.buck.core.exceptions"),
        com.facebook.buck.core.model.[HasBuildTarget](../HasBuildTarget.html "interface in com.facebook.buck.core.model"))
:::
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   Tree
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

[]{#skip.navbar.bottom}
:::
