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
-   Package
-   Class
-   [Tree](package-tree.html)
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
# Package com.facebook.buck.core.model {#package-com.facebook.buck.core.model .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [BuildFileTre                     | ::: block                         |
    | e](BuildFileTree.html "interface  | Interface to allow looking up     |
    | in com.facebook.buck.core.model") | parents and children of build     |
    |                                   | files.                            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Flavor](Flavor.html "interface   |                                   |
    | in com.facebook.buck.core.model") |                                   |
    +-----------------------------------+-----------------------------------+
    | [FlavorConvertible](F             | ::: block                         |
    | lavorConvertible.html "interface  | Values that has a canonical       |
    | in com.facebook.buck.core.model") | mapping to flavors.               |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Fl                               | ::: block                         |
    | avored](Flavored.html "interface  | When applied to a                 |
    | in com.facebook.buck.core.model") | [`DescriptionWith                 |
    |                                   | TargetGraph`](../rules/Descriptio |
    |                                   | nWithTargetGraph.html "interface  |
    |                                   | in com.facebook.buck.core.rules") |
    |                                   | this indicates that it supports   |
    |                                   | flavours.                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HasBuildTarget                   | ::: block                         |
    | ](HasBuildTarget.html "interface  | Some object that has a build      |
    | in com.facebook.buck.core.model") | target.                           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HasDefaultFlavors](H             | ::: block                         |
    | asDefaultFlavors.html "interface  | A constructor arg of rules which  |
    | in com.facebook.buck.core.model") | have default flavors.             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HasOutputNam                     | ::: block                         |
    | e](HasOutputName.html "interface  | Interface for                     |
    | in com.facebook.buck.core.model") | [`BuildRule`](..                  |
    |                                   | /rules/BuildRule.html "interface  |
    |                                   | in com.facebook.buck.core.rules") |
    |                                   | instances which generate sources  |
    |                                   | with logical \"names\" (e.g.      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [QueryTar                         | ::: block                         |
    | get](QueryTarget.html "interface  | Currently, this is a marker       |
    | in com.facebook.buck.core.model") | interface, but given the actual   |
    |                                   | implementations of this           |
    |                                   | interface, it would be more       |
    |                                   | accurate to represent it as an    |
    |                                   | algebraic data type:              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [TargetConfi                      | ::: block                         |
    | gurationSerializer](TargetConfigu | Allows to convert                 |
    | rationSerializer.html "interface  | [`TargetConfiguration`]           |
    | in com.facebook.buck.core.model") | (TargetConfiguration.html "class  |
    |                                   | in com.facebook.buck.core.model") |
    |                                   | to and from a string.             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [TargetConfigu                    | ::: block                         |
    | rationTransformer](TargetConfigur | Interface that allows             |
    | ationTransformer.html "interface  | transforming target               |
    | in com.facebook.buck.core.model") | configurations.                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [BaseName](BaseName.html "class   | ::: block                         |
    | in com.facebook.buck.core.model") | `//foo/bar` part of               |
    |                                   | `cell//foo/bar:baz`.              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildId](BuildId.html "class     | ::: block                         |
    | in com.facebook.buck.core.model") | A strongly typed representation   |
    |                                   | of a build id.                    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildId.BuildIdSerializer](Build |                                   |
    | Id.BuildIdSerializer.html "class  |                                   |
    | in com.facebook.buck.core.model") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Buil                             |                                   |
    | dTarget](BuildTarget.html "class  |                                   |
    | in com.facebook.buck.core.model") |                                   |
    +-----------------------------------+-----------------------------------+
    | [BuildTargetWithOutputs](Bu       | ::: block                         |
    | ildTargetWithOutputs.html "class  | Wrapper for a build target and    |
    | in com.facebook.buck.core.model") | its output label.                 |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CellRelativePa                   | ::: block                         |
    | th](CellRelativePath.html "class  | A pair of                         |
    | in com.facebook.buck.core.model") | [`C                               |
    |                                   | anonicalCellName`](../cell/name/C |
    |                                   | anonicalCellName.html "class in c |
    |                                   | om.facebook.buck.core.cell.name") |
    |                                   | and                               |
    |                                   | [`ForwardRelativePath`](../pat    |
    |                                   | h/ForwardRelativePath.html "class |
    |                                   |  in com.facebook.buck.core.path") |
    |                                   | relative the the cell.            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ConfigurationBuildTargets](Confi | ::: block                         |
    | gurationBuildTargets.html "class  | Encapsulates logic to convert     |
    | in com.facebook.buck.core.model") | [`UnconfiguredBuildTarget`](Unc   |
    |                                   | onfiguredBuildTarget.html "class  |
    |                                   | in com.facebook.buck.core.model") |
    |                                   | that represents a configuration   |
    |                                   | target to an instance of          |
    |                                   | [`BuildT                          |
    |                                   | arget`](BuildTarget.html "class i |
    |                                   | n com.facebook.buck.core.model"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ConfigurationForConfi            | ::: block                         |
    | gurationTargets](ConfigurationFor | Special configuration that is     |
    | ConfigurationTargets.html "class  | used together with                |
    | in com.facebook.buck.core.model") | [`UnconfiguredBuildTarget`](Unc   |
    |                                   | onfiguredBuildTarget.html "class  |
    |                                   | in com.facebook.buck.core.model") |
    |                                   | that represent configuration      |
    |                                   | targets in order to form          |
    |                                   | [`BuildT                          |
    |                                   | arget`](BuildTarget.html "class i |
    |                                   | n com.facebook.buck.core.model"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ErrorTargetConfiguration](Erro   | ::: block                         |
    | rTargetConfiguration.html "class  | Stub configuration which can be   |
    | in com.facebook.buck.core.model") | used when configuration is not    |
    |                                   | actually needed.                  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [FlavorDomai                      | ::: block                         |
    | n](FlavorDomain.html "class in co | Provides a named flavor           |
    | m.facebook.buck.core.model")\<T\> | abstraction on top of boolean     |
    |                                   | flavors.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | FlavorSet](FlavorSet.html "class  | Set of                            |
    | in com.facebook.buck.core.model") | [`F                               |
    |                                   | lavor`](Flavor.html "interface in |
    |                                   |  com.facebook.buck.core.model")s. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [InternalFl                       | ::: block                         |
    | avor](InternalFlavor.html "class  | A                                 |
    | in com.facebook.buck.core.model") | [                                 |
    |                                   | `Flavor`](Flavor.html "interface  |
    |                                   | in com.facebook.buck.core.model") |
    |                                   | passing information between       |
    |                                   | targets, which is irrelevant to   |
    |                                   | the end user.                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Outp                             | ::: block                         |
    | utLabel](OutputLabel.html "class  | Type-safe wrapper for a target    |
    | in com.facebook.buck.core.model") | output label.                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [OutputLabel.Internals](O         | ::: block                         |
    | utputLabel.Internals.html "class  | Provides access to internal       |
    | in com.facebook.buck.core.model") | implementation details of         |
    |                                   | OutputLabels.                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RuleB                            | ::: block                         |
    | asedTargetConfiguration](RuleBase | Platform target implementation of |
    | dTargetConfiguration.html "class  | [`TargetConfiguration`](          |
    | in com.facebook.buck.core.model") | TargetConfiguration.html "class i |
    |                                   | n com.facebook.buck.core.model"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RuleType](RuleType.html "class   |                                   |
    | in com.facebook.buck.core.model") |                                   |
    +-----------------------------------+-----------------------------------+
    | [TargetConfiguration]             | ::: block                         |
    | (TargetConfiguration.html "class  | Contains configuration            |
    | in com.facebook.buck.core.model") | information attached to a         |
    |                                   | configured build target.          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [UnconfiguredBuildTarget](Unc     | ::: block                         |
    | onfiguredBuildTarget.html "class  | Data object that holds properties |
    | in com.facebook.buck.core.model") | to uniquely identify a build      |
    |                                   | target with flavors               |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [UnconfiguredBuild                | ::: block                         |
    | TargetWithOutputs](UnconfiguredBu | Wrapper for an unconfigured build |
    | ildTargetWithOutputs.html "class  | target and its output label.      |
    | in com.facebook.buck.core.model") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Unconfigure                      | ::: block                         |
    | dTargetConfiguration](Unconfigure | Configuration that resolves to    |
    | dTargetConfiguration.html "class  | unconfigured platform, which      |
    | in com.facebook.buck.core.model") | results in error on any           |
    |                                   | operations with platforms (like   |
    |                                   | `compatible_with` or `select()`   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [UnflavoredBuildTarget](U         | ::: block                         |
    | nflavoredBuildTarget.html "class  | A build target in the form of     |
    | in com.facebook.buck.core.model") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Us                               | ::: block                         |
    | erFlavor](UserFlavor.html "class  | A                                 |
    | in com.facebook.buck.core.model") | [                                 |
    |                                   | `Flavor`](Flavor.html "interface  |
    |                                   | in com.facebook.buck.core.model") |
    |                                   | visible to the user, with which   |
    |                                   | they can modify output of a       |
    |                                   | target.                           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Enum                              | Description                       |
    +===================================+===================================+
    | [RuleTyp                          | ::: block                         |
    | e.Kind](RuleType.Kind.html "enum  | The kind of a rule type.          |
    | in com.facebook.buck.core.model") | :::                               |
    +-----------------------------------+-----------------------------------+

    : Enum Summary[ ]{.tabEnd}

-   
      Exception                                                                                     Description
      --------------------------------------------------------------------------------------------- -------------
      [FlavorDomainException](FlavorDomainException.html "class in com.facebook.buck.core.model")    

      : Exception Summary[ ]{.tabEnd}
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../../index.html)
-   Package
-   Class
-   [Tree](package-tree.html)
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
