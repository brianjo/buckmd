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
-   Package
-   Class
-   [Tree](package-tree.html)
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
# Package com.facebook.buck.core.model.targetgraph {#package-com.facebook.buck.core.model.targetgraph .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [BuiltInProv                      | ::: block                         |
    | iderProvider](BuiltInProviderProv | An `ExtensionPoint` that provides |
    | ider.html "interface in com.faceb | all                               |
    | ook.buck.core.model.targetgraph") | [`BuiltInProvider`](../..         |
    |                                   | /rules/providers/impl/BuiltInProv |
    |                                   | ider.html "class in com.facebook. |
    |                                   | buck.core.rules.providers.impl")s |
    |                                   | that should be made available to  |
    |                                   | users by this module              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Des                              | ::: block                         |
    | criptionProvider](DescriptionProv | An `ExtensionPoint` which         |
    | ider.html "interface in com.faceb | provides a way to register an     |
    | ook.buck.core.model.targetgraph") | arbitrary set of                  |
    |                                   | [`De                              |
    |                                   | scription`](../../description/Des |
    |                                   | cription.html "interface in com.f |
    |                                   | acebook.buck.core.description")s. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NodeCopier](NodeCo               | ::: block                         |
    | pier.html "interface in com.faceb | Provides method for copying       |
    | ook.buck.core.model.targetgraph") | TargetNodes.                      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [TargetNode](TargetNod            | ::: block                         |
    | e.html "interface in com.facebook | A                                 |
    | .buck.core.model.targetgraph")\<T | [`TargetNode`](Target             |
    | extends                           | Node.html "interface in com.faceb |
    | [ConstructorArg]                  | ook.buck.core.model.targetgraph") |
    | (../../description/arg/Constructo | represents a node in the target   |
    | rArg.html "interface in com.faceb | graph which is created by the     |
    | ook.buck.core.description.arg")\> | [`Parser`](..                     |
    |                                   | /../../parser/Parser.html "interf |
    |                                   | ace in com.facebook.buck.parser") |
    |                                   | as a result of parsing BUCK files |
    |                                   | in a project.                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [MergedTargetGraph](MergedTar     | ::: block                         |
    | getGraph.html "class in com.faceb | Target graph version where node   |
    | ook.buck.core.model.targetgraph") | is a set of all nodes with the    |
    |                                   | same                              |
    |                                   | [`UnflavoredBuildTarget`](../Un   |
    |                                   | flavoredBuildTarget.html "class i |
    |                                   | n com.facebook.buck.core.model"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [MergedTargetNode](MergedTa       | ::: block                         |
    | rgetNode.html "class in com.faceb | A set of target nodes with the    |
    | ook.buck.core.model.targetgraph") | same unconfigured build target.   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [TargetGraph](Tar                 | ::: block                         |
    | getGraph.html "class in com.faceb | Represents the graph of           |
    | ook.buck.core.model.targetgraph") | [`TargetNode`](TargetN            |
    |                                   | ode.html "interface in com.facebo |
    |                                   | ok.buck.core.model.targetgraph")s |
    |                                   | constructed by parsing the build  |
    |                                   | files.                            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [TargetGraph                      | ::: block                         |
    | CreationResult](TargetGraphCreati | Contains information produced as  |
    | onResult.html "class in com.faceb | a result of the phase of target   |
    | ook.buck.core.model.targetgraph") | graph creation.                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [TargetNodeMaybe                  | ::: block                         |
    | Incompatible](TargetNodeMaybeInco | This may have a TargetNode or     |
    | mpatible.html "class in com.faceb | some diagnostic information, in   |
    | ook.buck.core.model.targetgraph") | case the target was found         |
    |                                   | incompatible.                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   
      Exception                                                                                                 Description
      --------------------------------------------------------------------------------------------------------- -------------
      [NoSuchTargetException](NoSuchTargetException.html "class in com.facebook.buck.core.model.targetgraph")    

      : Exception Summary[ ]{.tabEnd}
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../../../index.html)
-   Package
-   Class
-   [Tree](package-tree.html)
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
