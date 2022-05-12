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
# Package com.facebook.buck.parser {#package-com.facebook.buck.parser .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [Bu                               | ::: block                         |
    | ildTargetParsePipeline](BuildTarg | Abstract node parsing pipeline.   |
    | etParsePipeline.html "interface i | :::                               |
    | n com.facebook.buck.parser")\<T\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [FileParsePipeline](              | ::: block                         |
    | FileParsePipeline.html "interface | Abstract node parsing pipeline.   |
    |  in com.facebook.buck.parser")\<T | :::                               |
    | extends                           |                                   |
    | [FileManifest](ap                 |                                   |
    | i/FileManifest.html "interface in |                                   |
    |  com.facebook.buck.parser.api")\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [FileParserFactory](              | ::: block                         |
    | FileParserFactory.html "interface | Factory for creating instances of |
    |  in com.facebook.buck.parser")\<T | [`FileParser`]                    |
    | extends                           | (api/FileParser.html "interface i |
    | [FileManifest](ap                 | n com.facebook.buck.parser.api"). |
    | i/FileManifest.html "interface in | :::                               |
    |  com.facebook.buck.parser.api")\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [PackageBoundaryChecker](Pa       | ::: block                         |
    | ckageBoundaryChecker.html "interf | Performs checks around accessing  |
    | ace in com.facebook.buck.parser") | files outside of a target\'s      |
    |                                   | package.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Parser](Parser.html "interf      | ::: block                         |
    | ace in com.facebook.buck.parser") | High-level build file parsing     |
    |                                   | machinery.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ParserTargetNodeF                | ::: block                         |
    | romAttrMapFactory](ParserTargetNo | Creates                           |
    | deFromAttrMapFactory.html "interf | [`TargetNode`]                    |
    | ace in com.facebook.buck.parser") | (../core/model/targetgraph/Target |
    |                                   | Node.html "interface in com.faceb |
    |                                   | ook.buck.core.model.targetgraph") |
    |                                   | instances from raw attribute map  |
    |                                   | returned by the parser.           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ParserTargetNo                   | ::: block                         |
    | deFromUnconfiguredTargetNodeFacto | Convert                           |
    | ry](ParserTargetNodeFromUnconfigu | [`Unconfigure                     |
    | redTargetNodeFactory.html "interf | dTargetNode`](../core/model/targe |
    | ace in com.facebook.buck.parser") | tgraph/raw/UnconfiguredTargetNode |
    |                                   | .html "interface in com.facebook. |
    |                                   | buck.core.model.targetgraph.raw") |
    |                                   | to                                |
    |                                   | [`TargetNode`]                    |
    |                                   | (../core/model/targetgraph/Target |
    |                                   | Node.html "interface in com.faceb |
    |                                   | ook.buck.core.model.targetgraph") |
    |                                   | for the parser.                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Project                          | ::: block                         |
    | BuildFileParserFactory](ProjectBu | Factory for creating instances of |
    | ildFileParserFactory.html "interf | {link ProjectBuildFileParser}.    |
    | ace in com.facebook.buck.parser") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [TargetNodeListener](Tar          | ::: block                         |
    | getNodeListener.html "interface i | Callback which is called when     |
    | n com.facebook.buck.parser")\<T\> | target node is created            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [TargetSpecResol                  | ::: block                         |
    | ver.FlavorEnhancer](TargetSpecRes | Allows to change flavors of some  |
    | olver.FlavorEnhancer.html "interf | targets while performing the      |
    | ace in com.facebook.buck.parser") | resolution.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [TargetSpecResolv                 | ::: block                         |
    | er.TargetNodeFilterForSpecResolve | Performs filtering of target      |
    | r](TargetSpecResolver.TargetNodeF | nodes using a given               |
    | ilterForSpecResolver.html "interf | [`TargetNodeSpec`](spec/          |
    | ace in com.facebook.buck.parser") | TargetNodeSpec.html "interface in |
    |                                   |  com.facebook.buck.parser.spec"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Unconfi                          | ::: block                         |
    | guredTargetNodeFactory](Unconfigu | Generic factory to create         |
    | redTargetNodeFactory.html "interf | [`Unconfigure                     |
    | ace in com.facebook.buck.parser") | dTargetNode`](../core/model/targe |
    |                                   | tgraph/raw/UnconfiguredTargetNode |
    |                                   | .html "interface in com.facebook. |
    |                                   | buck.core.model.targetgraph.raw") |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [Bui                              | ::: block                         |
    | ldFileRawNodeParsePipeline](Build | A pipeline that provides a        |
    | FileRawNodeParsePipeline.html "cl | [`BuildFileManifest`](a           |
    | ass in com.facebook.buck.parser") | pi/BuildFileManifest.html "class  |
    |                                   | in com.facebook.buck.parser.api") |
    |                                   | for a given build file.           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildTa                          | ::: block                         |
    | rgetRawNodeParsePipeline](BuildTa | A pipeline that provides access   |
    | rgetRawNodeParsePipeline.html "cl | to a raw node by its              |
    | ass in com.facebook.buck.parser") | [`BuildTarget`](../cor            |
    |                                   | e/model/BuildTarget.html "class i |
    |                                   | n com.facebook.buck.core.model"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuiltTargetVerif                 | ::: block                         |
    | ier](BuiltTargetVerifier.html "cl | Verifies that the                 |
    | ass in com.facebook.buck.parser") | [`BuildTarget`](../co             |
    |                                   | re/model/BuildTarget.html "class  |
    |                                   | in com.facebook.buck.core.model") |
    |                                   | is valid during parsing           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Concurren                        | ::: block                         |
    | tProjectBuildFileParser](Concurre | Add synchronization layer over    |
    | ntProjectBuildFileParser.html "cl | existing                          |
    | ass in com.facebook.buck.parser") | [`Pr                              |
    |                                   | ojectBuildFileParser`](api/Projec |
    |                                   | tBuildFileParser.html "interface  |
    |                                   | in com.facebook.buck.parser.api") |
    |                                   | by creating and maintaining a     |
    |                                   | pool of                           |
    |                                   | [`Proje                           |
    |                                   | ctBuildFileParser`](api/ProjectBu |
    |                                   | ildFileParser.html "interface in  |
    |                                   | com.facebook.buck.parser.api")\'s |
    |                                   | instances.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DaemonicParserSt                 | ::: block                         |
    | ate](DaemonicParserState.html "cl | Persistent parsing data, that can |
    | ass in com.facebook.buck.parser") | exist between invocations of the  |
    |                                   | [`Parser`](Parser.html "interfa   |
    |                                   | ce in com.facebook.buck.parser"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DefaultProjectBui                |                                   |
    | ldFileParserFactory](DefaultProje |                                   |
    | ctBuildFileParserFactory.html "cl |                                   |
    | ass in com.facebook.buck.parser") |                                   |
    +-----------------------------------+-----------------------------------+
    | [DefaultSelectableCo              | ::: block                         |
    | nfigurationContext](DefaultSelect | An implementation of              |
    | ableConfigurationContext.html "cl | [`SelectableConfigurationContext  |
    | ass in com.facebook.buck.parser") | `](../core/select/SelectableConfi |
    |                                   | gurationContext.html "interface i |
    |                                   | n com.facebook.buck.core.select") |
    |                                   | that is used in parser            |
    |                                   | implementation.                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DefaultUnconfigur                | ::: block                         |
    | edTargetNodeFactory](DefaultUncon | Creates                           |
    | figuredTargetNodeFactory.html "cl | [`Unconfigure                     |
    | ass in com.facebook.buck.parser") | dTargetNode`](../core/model/targe |
    |                                   | tgraph/raw/UnconfiguredTargetNode |
    |                                   | .html "interface in com.facebook. |
    |                                   | buck.core.model.targetgraph.raw") |
    |                                   | instances from raw data coming in |
    |                                   | form the                          |
    |                                   | [`Pro                             |
    |                                   | jectBuildFileParser`](api/Project |
    |                                   | BuildFileParser.html "interface i |
    |                                   | n com.facebook.buck.parser.api"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [GenericFileParsePipeline](Gen    | ::: block                         |
    | ericFileParsePipeline.html "class | A pipeline that provides cached   |
    |  in com.facebook.buck.parser")\<T | parsed results for a given file.  |
    | extends                           | :::                               |
    | [FileManifest](ap                 |                                   |
    | i/FileManifest.html "interface in |                                   |
    |  com.facebook.buck.parser.api")\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [H                                | ::: block                         |
    | ybridProjectBuildFileParser](Hybr | Hybrid project build file parser  |
    | idProjectBuildFileParser.html "cl | that uses Python DSL, Skylark or  |
    | ass in com.facebook.buck.parser") | any other                         |
    |                                   | [`Syntax`](api/Syntax.html "enum  |
    |                                   | in com.facebook.buck.parser.api") |
    |                                   | depending on which one is         |
    |                                   | requested for the individual      |
    |                                   | build file.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [I                                | ::: block                         |
    | nternalTargetAttributeNames](Inte | Contains names of attributes that |
    | rnalTargetAttributeNames.html "cl | are provided by Buck and cannot   |
    | ass in com.facebook.buck.parser") | be set by users.                  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [LabelCache](LabelCache.html "cl  | ::: block                         |
    | ass in com.facebook.buck.parser") | Create caches for `Label` objects |
    |                                   | in the Skylark Parser             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [MetaRules](MetaRules.html "cl    | ::: block                         |
    | ass in com.facebook.buck.parser") | Contains information about meta   |
    |                                   | rules (rules that are created by  |
    |                                   | Buck to pass internal information |
    |                                   | about parsing process)            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NoopPackageBoundaryChecker](No   |                                   |
    | opPackageBoundaryChecker.html "cl |                                   |
    | ass in com.facebook.buck.parser") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Packag                           | ::: block                         |
    | eFactory](PackageFactory.html "cl | Generic factory to create         |
    | ass in com.facebook.buck.parser") | [`Package`](..                    |
    |                                   | /core/model/targetgraph/impl/Pack |
    |                                   | age.html "class in com.facebook.b |
    |                                   | uck.core.model.targetgraph.impl") |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PackageFileParsePipeline](       | ::: block                         |
    | PackageFileParsePipeline.html "cl | A pipeline that provides a        |
    | ass in com.facebook.buck.parser") | [`PackageFileManifest`](api       |
    |                                   | /PackageFileManifest.html "class  |
    |                                   | in com.facebook.buck.parser.api") |
    |                                   | for a given package file.         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PackageFileParserFactory](       | ::: block                         |
    | PackageFileParserFactory.html "cl | Factory for creating instances of |
    | ass in com.facebook.buck.parser") | [`PackageFileParser`](api/Pa      |
    |                                   | ckageFileParser.html "interface i |
    |                                   | n com.facebook.buck.parser.api"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ParseEvent](ParseEvent.html "cl  | ::: block                         |
    | ass in com.facebook.buck.parser") | Base class for events about       |
    |                                   | parsing build files..             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ParseEvent.Finis                 |                                   |
    | hed](ParseEvent.Finished.html "cl |                                   |
    | ass in com.facebook.buck.parser") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ParseEvent.Sta                   |                                   |
    | rted](ParseEvent.Started.html "cl |                                   |
    | ass in com.facebook.buck.parser") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Pars                             | ::: block                         |
    | erFactory](ParserFactory.html "cl | Responsible for creating an       |
    | ass in com.facebook.buck.parser") | instance of                       |
    |                                   | [`Parser`](Parser.html "interfa   |
    |                                   | ce in com.facebook.buck.parser"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Parser                           |                                   |
    | Messages](ParserMessages.html "cl |                                   |
    | ass in com.facebook.buck.parser") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ParserP                          |                                   |
    | ythonInterpreterProvider](ParserP |                                   |
    | ythonInterpreterProvider.html "cl |                                   |
    | ass in com.facebook.buck.parser") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Parsin                           | ::: block                         |
    | gContext](ParsingContext.html "cl | Contains objects and information  |
    | ass in com.facebook.buck.parser") | that may be used during           |
    |                                   | processing a parsing request.     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ParsingContext.Builder           |                                   |
    | ](ParsingContext.Builder.html "cl |                                   |
    | ass in com.facebook.buck.parser") |                                   |
    +-----------------------------------+-----------------------------------+
    | [PerB                             |                                   |
    | uildState](PerBuildState.html "cl |                                   |
    | ass in com.facebook.buck.parser") |                                   |
    +-----------------------------------+-----------------------------------+
    | [PerBuildStateFacto               | ::: block                         |
    | ry](PerBuildStateFactory.html "cl | Can be used to create             |
    | ass in com.facebook.buck.parser") | [`PerBui                          |
    |                                   | ldState`](PerBuildState.html "cla |
    |                                   | ss in com.facebook.buck.parser"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PythonD                          | ::: block                         |
    | slProjectBuildFileParser](PythonD | Delegates to buck.py for parsing  |
    | slProjectBuildFileParser.html "cl | of buck build files.              |
    | ass in com.facebook.buck.parser") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [TargetSpecReso                   | ::: block                         |
    | lver](TargetSpecResolver.html "cl | Responsible for discovering all   |
    | ass in com.facebook.buck.parser") | the build targets that match a    |
    |                                   | set of                            |
    |                                   | [`TargetNodeSpec`](spec/          |
    |                                   | TargetNodeSpec.html "interface in |
    |                                   |  com.facebook.buck.parser.spec"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Throw                            | ::: block                         |
    | ingPackageBoundaryChecker](Throwi | [`PackageBoundaryChecker`](Pa     |
    | ngPackageBoundaryChecker.html "cl | ckageBoundaryChecker.html "interf |
    | ass in com.facebook.buck.parser") | ace in com.facebook.buck.parser") |
    |                                   | implementation that throws an     |
    |                                   | exception if any file in a set    |
    |                                   | does not belong to the same       |
    |                                   | package as provided build target  |
    |                                   | only if cell configuration allows |
    |                                   | that, otherwise noop.             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Uncon                            | ::: block                         |
    | figuredTargetNodePipeline](Unconf | Converts nodes in a raw form      |
    | iguredTargetNodePipeline.html "cl | (taken from build file parsers)   |
    | ass in com.facebook.buck.parser") | into                              |
    |                                   | [`Unconfigured                    |
    |                                   | TargetNode`](../core/model/target |
    |                                   | graph/raw/UnconfiguredTargetNode. |
    |                                   | html "interface in com.facebook.b |
    |                                   | uck.core.model.targetgraph.raw"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [UnconfiguredTargetNodeToTar      | ::: block                         |
    | getNodeFactory](UnconfiguredTarge | Creates                           |
    | tNodeToTargetNodeFactory.html "cl | [`TargetNode`]                    |
    | ass in com.facebook.buck.parser") | (../core/model/targetgraph/Target |
    |                                   | Node.html "interface in com.faceb |
    |                                   | ook.buck.core.model.targetgraph") |
    |                                   | from                              |
    |                                   | [`Unconfigured                    |
    |                                   | TargetNode`](../core/model/target |
    |                                   | graph/raw/UnconfiguredTargetNode. |
    |                                   | html "interface in com.facebook.b |
    |                                   | uck.core.model.targetgraph.raw"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Unconf                           | ::: block                         |
    | iguredTargetNodeToTargetNodeParse | Asynchronous loader/converter of  |
    | Pipeline](UnconfiguredTargetNodeT | raw target nodes to configured    |
    | oTargetNodeParsePipeline.html "cl | target nodes                      |
    | ass in com.facebook.buck.parser") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [U                                |                                   |
    | nflavoredBuildTargetFactory](Unfl |                                   |
    | avoredBuildTargetFactory.html "cl |                                   |
    | ass in com.facebook.buck.parser") |                                   |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   
      Enum                                                                               Description
      ---------------------------------------------------------------------------------- -------------
      [SpeculativeParsing](SpeculativeParsing.html "enum in com.facebook.buck.parser")    

      : Enum Summary[ ]{.tabEnd}

-   
      Exception                                                                                         Description
      ------------------------------------------------------------------------------------------------- -------------
      [UnexpectedFlavorException](UnexpectedFlavorException.html "class in com.facebook.buck.parser")    

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
