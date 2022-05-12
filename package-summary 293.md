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
-   Package
-   Class
-   [Tree](package-tree.html)
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
# Package com.facebook.buck.versions {#package-com.facebook.buck.versions .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [Cons                             | ::: block                         |
    | traint](Constraint.html "interfac | Represents a version constraint   |
    | e in com.facebook.buck.versions") | applied to a dependency.          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HasVersionUniverse](             |                                   |
    | HasVersionUniverse.html "interfac |                                   |
    | e in com.facebook.buck.versions") |                                   |
    +-----------------------------------+-----------------------------------+
    | [TargetTranslatable](Targe        | ::: block                         |
    | tTranslatable.html "interface in  | Interface for objects which       |
    | com.facebook.buck.versions")\<T\> | defined how they should be        |
    |                                   | translated in constructor args    |
    |                                   | for versioning.                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Version](Version.html "interfac  |                                   |
    | e in com.facebook.buck.versions") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Versi                            | ::: block                         |
    | onedTargetGraphBuilder](Versioned | Takes a regular                   |
    | TargetGraphBuilder.html "interfac | [`TargetGraph                     |
    | e in com.facebook.buck.versions") | `](../core/model/targetgraph/Targ |
    |                                   | etGraph.html "class in com.facebo |
    |                                   | ok.buck.core.model.targetgraph"), |
    |                                   | resolves any versioned nodes, and |
    |                                   | returns a new graph with the      |
    |                                   | versioned nodes removed.          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [VersionPropagator](Ve            | ::: block                         |
    | rsionPropagator.html "interface i | A node constitutes the body of a  |
    | n com.facebook.buck.versions")\<A | version sub-graph.                |
    | extends                           | :::                               |
    | [BuildRuleArg]                    |                                   |
    | (../core/description/arg/BuildRul |                                   |
    | eArg.html "interface in com.faceb |                                   |
    | ook.buck.core.description.arg")\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [VersionRo                        | ::: block                         |
    | ot](VersionRoot.html "interface i | A node which is the root of a     |
    | n com.facebook.buck.versions")\<A | version sub-graph.                |
    | extends                           | :::                               |
    | [BuildRuleArg]                    |                                   |
    | (../core/description/arg/BuildRul |                                   |
    | eArg.html "interface in com.faceb |                                   |
    | ook.buck.core.description.arg")\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [VersionSelecto                   | ::: block                         |
    | r](VersionSelector.html "interfac | Interface for selecting versions  |
    | e in com.facebook.buck.versions") | for a versioned sub-graph         |
    |                                   | represented by a root node and    |
    |                                   | its version domain.               |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [AbstractVersioned                |                                   |
    | TargetGraphBuilder](AbstractVersi |                                   |
    | onedTargetGraphBuilder.html "clas |                                   |
    | s in com.facebook.buck.versions") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AsyncVersio                      | ::: block                         |
    | nedTargetGraphBuilder](AsyncVersi | Takes a regular                   |
    | onedTargetGraphBuilder.html "clas | [`TargetGraph                     |
    | s in com.facebook.buck.versions") | `](../core/model/targetgraph/Targ |
    |                                   | etGraph.html "class in com.facebo |
    |                                   | ok.buck.core.model.targetgraph"), |
    |                                   | resolves any versioned nodes, and |
    |                                   | returns a new graph with the      |
    |                                   | versioned nodes removed,          |
    |                                   | transforming it asynchronously    |
    |                                   | using                             |
    |                                   | [`GraphComputation`](../core/grap |
    |                                   | h/transformation/GraphComputation |
    |                                   | .html "interface in com.facebook. |
    |                                   | buck.core.graph.transformation"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ExactConst                       |                                   |
    | raint](ExactConstraint.html "clas |                                   |
    | s in com.facebook.buck.versions") |                                   |
    +-----------------------------------+-----------------------------------+
    | [InstrumentedVersioned            | ::: block                         |
    | TargetGraphCache](InstrumentedVer | Wrapper class around              |
    | sionedTargetGraphCache.html "clas | VersionedTargetGraphCache         |
    | s in com.facebook.buck.versions") | containing a command specific     |
    |                                   | stats tracker to track            |
    |                                   | performance of the cache          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [QueryTargetTranslator]           |                                   |
    | (QueryTargetTranslator.html "clas |                                   |
    | s in com.facebook.buck.versions") |                                   |
    +-----------------------------------+-----------------------------------+
    | [TargetNodeTranslator             | ::: block                         |
    | ](TargetNodeTranslator.html "clas | A helper class which uses         |
    | s in com.facebook.buck.versions") | reflection to translate           |
    |                                   | [`BuildTarget`](../cor            |
    |                                   | e/model/BuildTarget.html "class i |
    |                                   | n com.facebook.buck.core.model")s |
    |                                   | in                                |
    |                                   | [`TargetNode`](.                  |
    |                                   | ./core/model/targetgraph/TargetNo |
    |                                   | de.html "interface in com.faceboo |
    |                                   | k.buck.core.model.targetgraph")s. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [VersionBuckCon                   |                                   |
    | fig](VersionBuckConfig.html "clas |                                   |
    | s in com.facebook.buck.versions") |                                   |
    +-----------------------------------+-----------------------------------+
    | [V                                |                                   |
    | ersionDescriptionsProvider](Versi |                                   |
    | onDescriptionsProvider.html "clas |                                   |
    | s in com.facebook.buck.versions") |                                   |
    +-----------------------------------+-----------------------------------+
    | [VersionedAliasDescription](Ver   |                                   |
    | sionedAliasDescription.html "clas |                                   |
    | s in com.facebook.buck.versions") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Ver                              | ::: block                         |
    | sionedAliasDescriptionArg](Versio | Immutable implementation of       |
    | nedAliasDescriptionArg.html "clas | `VersionedAliasDescription.Abstr  |
    | s in com.facebook.buck.versions") | actVersionedAliasDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [VersionedAliasDescr              | ::: block                         |
    | iptionArg.Builder](VersionedAlias | Builds instances of type          |
    | DescriptionArg.Builder.html "clas | [`Versi                           |
    | s in com.facebook.buck.versions") | onedAliasDescriptionArg`](Version |
    |                                   | edAliasDescriptionArg.html "class |
    |                                   |  in com.facebook.buck.versions"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [VersionedTargetGraph             |                                   |
    | ](VersionedTargetGraph.html "clas |                                   |
    | s in com.facebook.buck.versions") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Ver                              |                                   |
    | sionedTargetGraph.Builder](Versio |                                   |
    | nedTargetGraph.Builder.html "clas |                                   |
    | s in com.facebook.buck.versions") |                                   |
    +-----------------------------------+-----------------------------------+
    | [VersionedTargetGraphCache](Ver   |                                   |
    | sionedTargetGraphCache.html "clas |                                   |
    | s in com.facebook.buck.versions") |                                   |
    +-----------------------------------+-----------------------------------+
    | [VersionedTargetGraphEvent](Ver   | ::: block                         |
    | sionedTargetGraphEvent.html "clas | Base class for events about       |
    | s in com.facebook.buck.versions") | building up the versioned target  |
    |                                   | graph.                            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Versioned                        |                                   |
    | TargetGraphEvent.Cache](Versioned |                                   |
    | TargetGraphEvent.Cache.html "clas |                                   |
    | s in com.facebook.buck.versions") |                                   |
    +-----------------------------------+-----------------------------------+
    | [VersionedTargetGr                |                                   |
    | aphEvent.Cache.Hit](VersionedTarg |                                   |
    | etGraphEvent.Cache.Hit.html "clas |                                   |
    | s in com.facebook.buck.versions") |                                   |
    +-----------------------------------+-----------------------------------+
    | [VersionedTargetGrap              |                                   |
    | hEvent.Cache.Miss](VersionedTarge |                                   |
    | tGraphEvent.Cache.Miss.html "clas |                                   |
    | s in com.facebook.buck.versions") |                                   |
    +-----------------------------------+-----------------------------------+
    | [VersionedTarget                  |                                   |
    | GraphEvent.Finished](VersionedTar |                                   |
    | getGraphEvent.Finished.html "clas |                                   |
    | s in com.facebook.buck.versions") |                                   |
    +-----------------------------------+-----------------------------------+
    | [VersionedTarg                    |                                   |
    | etGraphEvent.Started](VersionedTa |                                   |
    | rgetGraphEvent.Started.html "clas |                                   |
    | s in com.facebook.buck.versions") |                                   |
    +-----------------------------------+-----------------------------------+
    | [VersionedTarg                    |                                   |
    | etGraphEvent.Timeout](VersionedTa |                                   |
    | rgetGraphEvent.Timeout.html "clas |                                   |
    | s in com.facebook.buck.versions") |                                   |
    +-----------------------------------+-----------------------------------+
    | [VersionUni                       |                                   |
    | verse](VersionUniverse.html "clas |                                   |
    | s in com.facebook.buck.versions") |                                   |
    +-----------------------------------+-----------------------------------+
    | [VersionUniverse.Builder](V       |                                   |
    | ersionUniverse.Builder.html "clas |                                   |
    | s in com.facebook.buck.versions") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Version                          | ::: block                         |
    | UniverseVersionSelector](VersionU | A fast constraint resolver which  |
    | niverseVersionSelector.html "clas | selects versions using            |
    | s in com.facebook.buck.versions") | pre-defined version universes.    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Enum                              | Description                       |
    +===================================+===================================+
    | [VersionedTargetGra               | ::: block                         |
    | phCache.ResultType](VersionedTarg | The possible result types using   |
    | etGraphCache.ResultType.html "enu | the cache.                        |
    | m in com.facebook.buck.versions") | :::                               |
    +-----------------------------------+-----------------------------------+

    : Enum Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Exception                         | Description                       |
    +===================================+===================================+
    | [VersionExcep                     | ::: block                         |
    | tion](VersionException.html "clas | Error thrown when version         |
    | s in com.facebook.buck.versions") | selection fails.                  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Exception Summary[ ]{.tabEnd}
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../index.html)
-   Package
-   Class
-   [Tree](package-tree.html)
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
