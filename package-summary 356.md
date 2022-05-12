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
# Package com.facebook.buck.features.project.intellij {#package-com.facebook.buck.features.project.intellij .title title="Package"}
:::

::: contentContainer
-   
      Interface                                                                                            Description
      ---------------------------------------------------------------------------------------------------- -------------
      [BuckBuildRunner](BuckBuildRunner.html "interface in com.facebook.buck.features.project.intellij")    

      : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [BaseIjModuleRule](BaseIjModuleRu | ::: block                         |
    | le.html "class in com.facebook.bu | Base class for IntelliJ module    |
    | ck.features.project.intellij")\<T | rules                             |
    | extends                           | :::                               |
    | [BuildRuleArg](../..              |                                   |
    | /../core/description/arg/BuildRul |                                   |
    | eArg.html "interface in com.faceb |                                   |
    | ook.buck.core.description.arg")\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [DefaultI                         |                                   |
    | jModuleFactory](DefaultIjModuleFa |                                   |
    | ctory.html "class in com.facebook |                                   |
    | .buck.features.project.intellij") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ExportedDepsClosur               | ::: block                         |
    | eResolver](ExportedDepsClosureRes | Calculates the transitive closure |
    | olver.html "class in com.facebook | of exported deps for every node   |
    | .buck.features.project.intellij") | in a                              |
    |                                   | [`TargetGraph`](../               |
    |                                   | ../../core/model/targetgraph/Targ |
    |                                   | etGraph.html "class in com.facebo |
    |                                   | ok.buck.core.model.targetgraph"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [IjAndroidHelper](IjAndroidH      |                                   |
    | elper.html "class in com.facebook |                                   |
    | .buck.features.project.intellij") |                                   |
    +-----------------------------------+-----------------------------------+
    | [IjBuckModule](IjBuckM            | ::: block                         |
    | odule.html "class in com.facebook | Module with project generator for |
    | .buck.features.project.intellij") | IntelliJ.                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [IjBuckModuleAd                   |                                   |
    | apterPlugin](IjBuckModuleAdapterP |                                   |
    | lugin.html "class in com.facebook |                                   |
    | .buck.features.project.intellij") |                                   |
    +-----------------------------------+-----------------------------------+
    | [IjDependen                       | ::: block                         |
    | cyListBuilder](IjDependencyListBu | Represents the dependencies of an |
    | ilder.html "class in com.facebook | `IjModule` in a form intended to  |
    | .buck.features.project.intellij") | be consumable by the              |
    |                                   | [`IjProjectWriter`](IjProjectWr   |
    |                                   | iter.html "class in com.facebook. |
    |                                   | buck.features.project.intellij"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [IjDepende                        | ::: block                         |
    | ncyListBuilder.DependencyEntry](I | The design of this classes API is |
    | jDependencyListBuilder.Dependency | tied to how the corresponding     |
    | Entry.html "class in com.facebook | StringTemplate template interacts |
    | .buck.features.project.intellij") | with it.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [IjKotlinHelper](IjKotlinH        | ::: block                         |
    | elper.html "class in com.facebook | Helper class related to Kotlin    |
    | .buck.features.project.intellij") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [IjModuleGraph](IjModule          | ::: block                         |
    | Graph.html "class in com.facebook | Represents a graph of IjModules   |
    | .buck.features.project.intellij") | and the dependencies between      |
    |                                   | them.                             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [IjMo                             |                                   |
    | duleGraphFactory](IjModuleGraphFa |                                   |
    | ctory.html "class in com.facebook |                                   |
    | .buck.features.project.intellij") |                                   |
    +-----------------------------------+-----------------------------------+
    | [IjProject](IjPr                  | ::: block                         |
    | oject.html "class in com.facebook | Top-level class for IntelliJ      |
    | .buck.features.project.intellij") | project generation.               |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Ij                               |                                   |
    | ProjectBuckConfig](IjProjectBuckC |                                   |
    | onfig.html "class in com.facebook |                                   |
    | .buck.features.project.intellij") |                                   |
    +-----------------------------------+-----------------------------------+
    | [IJProjectCleaner](IJProjectCl    | ::: block                         |
    | eaner.html "class in com.facebook | Cleans out any unwanted IntelliJ  |
    | .buck.features.project.intellij") | IDEA project files.               |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [IjProjec                         |                                   |
    | tCommandHelper](IjProjectCommandH |                                   |
    | elper.html "class in com.facebook |                                   |
    | .buck.features.project.intellij") |                                   |
    +-----------------------------------+-----------------------------------+
    | [IjProjectPaths](IjProject        |                                   |
    | Paths.html "class in com.facebook |                                   |
    | .buck.features.project.intellij") |                                   |
    +-----------------------------------+-----------------------------------+
    | [IjProjectSourcePat               | ::: block                         |
    | hResolver](IjProjectSourcePathRes | A SourcePathResolver              |
    | olver.html "class in com.facebook | implementation that uses only     |
    | .buck.features.project.intellij") | information found in the target   |
    |                                   | graph when converting a           |
    |                                   | BuildTargetSourcePath to an       |
    |                                   | outputPath.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Ij                               |                                   |
    | ProjectSubCommand](IjProjectSubCo |                                   |
    | mmand.html "class in com.facebook |                                   |
    | .buck.features.project.intellij") |                                   |
    +-----------------------------------+-----------------------------------+
    | [IjProjectSubCommand.Aggrega      |                                   |
    | tionModeOptionHandler](IjProjectS |                                   |
    | ubCommand.AggregationModeOptionHa |                                   |
    | ndler.html "class in com.facebook |                                   |
    | .buck.features.project.intellij") |                                   |
    +-----------------------------------+-----------------------------------+
    | [IjProjectTemplateDataP           | ::: block                         |
    | reparer](IjProjectTemplateDataPre | Does the converting of abstract   |
    | parer.html "class in com.facebook | data structures to a format       |
    | .buck.features.project.intellij") | immediately consumable by the     |
    |                                   | StringTemplate-based templates    |
    |                                   | employed by                       |
    |                                   | [`IjProjectWriter`](IjProjectWr   |
    |                                   | iter.html "class in com.facebook. |
    |                                   | buck.features.project.intellij"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [IjProjectWriter](IjProjectW      | ::: block                         |
    | riter.html "class in com.facebook | Writes the serialized             |
    | .buck.features.project.intellij") | representations of IntelliJ       |
    |                                   | project components to disk.       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [IjSource                         | ::: block                         |
    | RootSimplifier](IjSourceRootSimpl | Groups                            |
    | ifier.html "class in com.facebook | [`IjFolder`]                      |
    | .buck.features.project.intellij") | (model/folders/IjFolder.html "cla |
    |                                   | ss in com.facebook.buck.features. |
    |                                   | project.intellij.model.folders")s |
    |                                   | into sets which are of the same   |
    |                                   | type and belong to the same       |
    |                                   | package structure.                |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [IntellijModule                   | ::: block                         |
    | sListParser](IntellijModulesListP | Responsible for parsing an        |
    | arser.html "class in com.facebook | existing modules.xml file         |
    | .buck.features.project.intellij") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [IntelliJProjectSubCommandFac     |                                   |
    | tory](IntelliJProjectSubCommandFa |                                   |
    | ctory.html "class in com.facebook |                                   |
    | .buck.features.project.intellij") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JavaLangua                       |                                   |
    | geLevelHelper](JavaLanguageLevelH |                                   |
    | elper.html "class in com.facebook |                                   |
    | .buck.features.project.intellij") |                                   |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | ModuleBuildContext](ModuleBuildCo | Holds all of the mutable state    |
    | ntext.html "class in com.facebook | required during                   |
    | .buck.features.project.intellij") | [`IjModule`](model/IjModule.      |
    |                                   | html "class in com.facebook.buck. |
    |                                   | features.project.intellij.model") |
    |                                   | creation.                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Pregener                         |                                   |
    | atedCodeWriter](PregeneratedCodeW |                                   |
    | riter.html "class in com.facebook |                                   |
    | .buck.features.project.intellij") |                                   |
    +-----------------------------------+-----------------------------------+
    | [SupportedTargetTyp               |                                   |
    | eRegistry](SupportedTargetTypeReg |                                   |
    | istry.html "class in com.facebook |                                   |
    | .buck.features.project.intellij") |                                   |
    +-----------------------------------+-----------------------------------+
    | [TransitiveDepsClosureR           | ::: block                         |
    | esolver](TransitiveDepsClosureRes | Calculates the transitive closure |
    | olver.html "class in com.facebook | of exported deps for every node   |
    | .buck.features.project.intellij") | in a                              |
    |                                   | [`TargetGraph`](../               |
    |                                   | ../../core/model/targetgraph/Targ |
    |                                   | etGraph.html "class in com.facebo |
    |                                   | ok.buck.core.model.targetgraph"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Util]                            |                                   |
    | (Util.html "class in com.facebook |                                   |
    | .buck.features.project.intellij") |                                   |
    +-----------------------------------+-----------------------------------+
    | [WorkspaceUpdater](WorkspaceUp    | ::: block                         |
    | dater.html "class in com.facebook | Updates .idea/workspace.xml to    |
    | .buck.features.project.intellij") | avoid doing some operations by    |
    |                                   | IntelliJ.                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Enum                              | Description                       |
    +===================================+===================================+
    | [FolderTypeWit                    |                                   |
    | hPackageInfo](FolderTypeWithPacka |                                   |
    | geInfo.html "enum in com.facebook |                                   |
    | .buck.features.project.intellij") |                                   |
    +-----------------------------------+-----------------------------------+
    | [IjDependencyListBuild            | ::: block                         |
    | er.Scope](IjDependencyListBuilder | Set of scopes supported by        |
    | .Scope.html "enum in com.facebook | IntelliJ for the \"orderEntry\"   |
    | .buck.features.project.intellij") | element.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [IjDependencyListBuilder.SortO    |                                   |
    | rder](IjDependencyListBuilder.Sor |                                   |
    | tOrder.html "enum in com.facebook |                                   |
    | .buck.features.project.intellij") |                                   |
    +-----------------------------------+-----------------------------------+
    | [IjDependencyListBui              | ::: block                         |
    | lder.Type](IjDependencyListBuilde | Set of types supported by         |
    | r.Type.html "enum in com.facebook | IntelliJ for the \"orderEntry\"   |
    | .buck.features.project.intellij") | element.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

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
