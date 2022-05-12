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
# Package com.facebook.buck.features.apple.projectV2 {#package-com.facebook.buck.features.apple.projectv2 .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [ProjectGenera                    | ::: block                         |
    | torOptions](ProjectGeneratorOptio | Options for how                   |
    | ns.html "interface in com.faceboo | [`ProjectGenerator`](ProjectGen   |
    | k.buck.features.apple.projectV2") | erator.html "class in com.faceboo |
    |                                   | k.buck.features.apple.projectV2") |
    |                                   | generates Xcode projects.         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [BuildConfiguration](BuildConfigu | ::: block                         |
    | ration.html "class in com.faceboo | Helper methods to process         |
    | k.buck.features.apple.projectV2") | xcconfig build configuration for  |
    |                                   | a target node.                    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CoreDataResource](CoreDataRe     | ::: block                         |
    | source.html "class in com.faceboo | Represents a core data resource   |
    | k.buck.features.apple.projectV2") | from disk.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | CoreDataResource.VersionInformati | Details the version information   |
    | on](CoreDataResource.VersionInfor | for a core data file.             |
    | mation.html "class in com.faceboo | :::                               |
    | k.buck.features.apple.projectV2") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Foc                              | ::: block                         |
    | usedTargetMatcher](FocusedTargetM | Matcher class that matches build  |
    | atcher.html "class in com.faceboo | targets against specific focused  |
    | k.buck.features.apple.projectV2") | target entries.                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NodeHelper](Node                 | ::: block                         |
    | Helper.html "class in com.faceboo | Helper class to derive            |
    | k.buck.features.apple.projectV2") | information about                 |
    |                                   | [`TargetNode`](../../.            |
    |                                   | ./core/model/targetgraph/TargetNo |
    |                                   | de.html "interface in com.faceboo |
    |                                   | k.buck.core.model.targetgraph")s. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ProjectFileWriter](ProjectFile   | ::: block                         |
    | Writer.html "class in com.faceboo | A class for writing files in      |
    | k.buck.features.apple.projectV2") | SourcePath or Path objects to a   |
    |                                   | PBXProject.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ProjectFile                      | ::: block                         |
    | Writer.Result](ProjectFileWriter. | Helper class for returning        |
    | Result.html "class in com.faceboo | metadata about a created          |
    | k.buck.features.apple.projectV2") | PBXFileReference Includes a       |
    |                                   | reference to the PBXFileReference |
    |                                   | and the Source Tree Path We       |
    |                                   | probably won\'t need this long    |
    |                                   | term as we kill off Xcode build   |
    |                                   | phases but for now, let\'s just   |
    |                                   | use this since it\'s named and    |
    |                                   | structured                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ProjectGeneration                | ::: block                         |
    | StateCache](ProjectGenerationStat | Cache of calculated values for    |
    | eCache.html "class in com.faceboo | targets during project            |
    | k.buck.features.apple.projectV2") | generation.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ProjectGenerator](ProjectGen     | ::: block                         |
    | erator.html "class in com.faceboo | Generates an Xcode project and    |
    | k.buck.features.apple.projectV2") | writes the output to disk.        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ProjectGe                        | ::: block                         |
    | nerator.Result](ProjectGenerator. | The output from generating an     |
    | Result.html "class in com.faceboo | Xcode project.                    |
    | k.buck.features.apple.projectV2") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ProjectGeneratorOptions.B        |                                   |
    | uilder](ProjectGeneratorOptions.B |                                   |
    | uilder.html "class in com.faceboo |                                   |
    | k.buck.features.apple.projectV2") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ProjectSource                    | ::: block                         |
    | PathResolver](ProjectSourcePathRe | Helper class to resolve           |
    | solver.html "class in com.faceboo | [`Sourc                           |
    | k.buck.features.apple.projectV2") | ePath`](../../../core/sourcepath/ |
    |                                   | SourcePath.html "interface in com |
    |                                   | .facebook.buck.core.sourcepath")s |
    |                                   | to the cell in which we generate  |
    |                                   | the Xcode project.                |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Swi                              | ::: block                         |
    | ftAttributeParser](SwiftAttribute | Parser that derives Swift         |
    | Parser.html "class in com.faceboo | specific attributes from a Target |
    | k.buck.features.apple.projectV2") | and returns `SwiftAttributes`.    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Utils]                           | ::: block                         |
    | (Utils.html "class in com.faceboo | Utility functions for project     |
    | k.buck.features.apple.projectV2") | generation.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [WorkspaceAndProject              |                                   |
    | Generator](WorkspaceAndProjectGen |                                   |
    | erator.html "class in com.faceboo |                                   |
    | k.buck.features.apple.projectV2") |                                   |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | WorkspaceAndProjectGenerator.Resu | The result of generating a        |
    | lt](WorkspaceAndProjectGenerator. | workspace project.                |
    | Result.html "class in com.faceboo | :::                               |
    | k.buck.features.apple.projectV2") |                                   |
    +-----------------------------------+-----------------------------------+
    | [XcconfigBaseC                    | ::: block                         |
    | onfiguration](XcconfigBaseConfigu | Metadata for Xcode to lay out and |
    | ration.html "class in com.faceboo | reference an Xcconfig file.       |
    | k.buck.features.apple.projectV2") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [XcodeNativeTarg                  | ::: block                         |
    | etGenerator](XcodeNativeTargetGen | Generates all the target          |
    | erator.html "class in com.faceboo | attributes                        |
    | k.buck.features.apple.projectV2") | `GeneratedTargetAttributes` to be |
    |                                   | written into a                    |
    |                                   | [`PBXNativeTarget`](../..         |
    |                                   | /../apple/xcode/xcodeproj/PBXNati |
    |                                   | veTarget.html "class in com.faceb |
    |                                   | ook.buck.apple.xcode.xcodeproj"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [XcodeNativeTargetGenerator.Re    | ::: block                         |
    | sult](XcodeNativeTargetGenerator. | The result of materializing the   |
    | Result.html "class in com.faceboo | build target.                     |
    | k.buck.features.apple.projectV2") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Xco                              | ::: block                         |
    | deProductMetadata](XcodeProductMe | Product metadata related to a     |
    | tadata.html "class in com.faceboo | product target for reference in   |
    | k.buck.features.apple.projectV2") | Xcode                             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [XCodeProjectC                    |                                   |
    | ommandHelper](XCodeProjectCommand |                                   |
    | Helper.html "class in com.faceboo |                                   |
    | k.buck.features.apple.projectV2") |                                   |
    +-----------------------------------+-----------------------------------+
    | [XCodeProjectCommandHelper.R      | ::: block                         |
    | esult](XCodeProjectCommandHelper. | A result with metadata about the  |
    | Result.html "class in com.faceboo | subcommand helper\'s output.      |
    | k.buck.features.apple.projectV2") | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   
      Enum                                                                                     Description
      ---------------------------------------------------------------------------------------- -------------
      [IDEForceKill](IDEForceKill.html "enum in com.facebook.buck.features.apple.projectV2")    

      : Enum Summary[ ]{.tabEnd}
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
