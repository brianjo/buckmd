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
# Package com.facebook.buck.cxx {#package-com.facebook.buck.cxx .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [AbstractCxxLibraryGroup](        | ::: block                         |
    | AbstractCxxLibraryGroup.html "int | Base class for CxxLibrary-like    |
    | erface in com.facebook.buck.cxx") | things.                           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxBin                           |                                   |
    | aryDescription.CommonArg](CxxBina |                                   |
    | ryDescription.CommonArg.html "int |                                   |
    | erface in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CxxConstructo                    |                                   |
    | rArg](CxxConstructorArg.html "int |                                   |
    | erface in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | CxxIntermediateBuildProduct](CxxI | Interface marker for a type that  |
    | ntermediateBuildProduct.html "int | emits intermediate products in a  |
    | erface in com.facebook.buck.cxx") | cxx build                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxLibra                         |                                   |
    | ryDescription.CommonArg](CxxLibra |                                   |
    | ryDescription.CommonArg.html "int |                                   |
    | erface in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | CxxLibraryDescription.TransitiveC | This is a hack to allow fine      |
    | xxPreprocessorInputFunction](CxxL | grained control over how the      |
    | ibraryDescription.TransitiveCxxPr | transitive                        |
    | eprocessorInputFunction.html "int | `  CxxPreprocessorInput`s are     |
    | erface in com.facebook.buck.cxx") | found.                            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxL                             | ::: block                         |
    | ibraryDescriptionDelegate](CxxLib | Defines a plugin interface for    |
    | raryDescriptionDelegate.html "int | [`CxxLibraryDescript              |
    | erface in com.facebook.buck.cxx") | ion`](CxxLibraryDescription.html  |
    |                                   | "class in com.facebook.buck.cxx") |
    |                                   | so that its behavior can be       |
    |                                   | extended.                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxLibrar                        | ::: block                         |
    | yDescriptionDelegate.ConfiguredDe | The delegate for a specific       |
    | legate](CxxLibraryDescriptionDele | target and platform.              |
    | gate.ConfiguredDelegate.html "int | :::                               |
    | erface in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CxxPreprocessor                  | ::: block                         |
    | Dep](CxxPreprocessorDep.html "int | An interface that represents a    |
    | erface in com.facebook.buck.cxx") | [`BuildRule`](../core             |
    |                                   | /rules/BuildRule.html "interface  |
    |                                   | in com.facebook.buck.core.rules") |
    |                                   | which can contribute components   |
    |                                   | (e.g.                             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HasAppleDebugSymbolDeps](        | ::: block                         |
    | HasAppleDebugSymbolDeps.html "int | Returns all archives and object   |
    | erface in com.facebook.buck.cxx") | files, or other instances of      |
    |                                   | HasAppleDebugSymbolDeps.          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [LinkableCxxConstructorArg](Li    |                                   |
    | nkableCxxConstructorArg.html "int |                                   |
    | erface in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [LinkOutputPostprocessor](        | ::: block                         |
    | LinkOutputPostprocessor.html "int | Pluggable postprocessor for the   |
    | erface in com.facebook.buck.cxx") | output of a                       |
    |                                   | [`CxxLink`](CxxLink.html "        |
    |                                   | class in com.facebook.buck.cxx"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NativeT                          | ::: block                         |
    | estable](NativeTestable.html "int | Interface marking a rule as       |
    | erface in com.facebook.buck.cxx") | having tests.                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Omnibus.OmnibusLibrary]          |                                   |
    | (Omnibus.OmnibusLibrary.html "int |                                   |
    | erface in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Omnibus.OmnibusRo                |                                   |
    | ot](Omnibus.OmnibusRoot.html "int |                                   |
    | erface in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [UntrackedHeaderReporter](        | ::: block                         |
    | UntrackedHeaderReporter.html "int | Produces the error message when   |
    | erface in com.facebook.buck.cxx") | an untracked header is detected.  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [Archive](Archive.html            | ::: block                         |
    | "class in com.facebook.buck.cxx") | A                                 |
    |                                   | [`BuildRule`](../core             |
    |                                   | /rules/BuildRule.html "interface  |
    |                                   | in com.facebook.buck.core.rules") |
    |                                   | which builds an \"ar\" archive    |
    |                                   | from input files represented as   |
    |                                   | [                                 |
    |                                   | `SourcePath`](../core/sourcepath/ |
    |                                   | SourcePath.html "interface in com |
    |                                   | .facebook.buck.core.sourcepath"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxBinary](CxxBinary.html        |                                   |
    | "class in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CxxBinaryDescri                  |                                   |
    | ption](CxxBinaryDescription.html  |                                   |
    | "class in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CxxBinaryDescriptionA            | ::: block                         |
    | rg](CxxBinaryDescriptionArg.html  | Immutable implementation of       |
    | "class in com.facebook.buck.cxx") | `CxxBinaryDescription.            |
    |                                   | AbstractCxxBinaryDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxB                             | ::: block                         |
    | inaryDescriptionArg.Builder](CxxB | Builds instances of type          |
    | inaryDescriptionArg.Builder.html  | [`CxxBinaryDescriptionArg         |
    | "class in com.facebook.buck.cxx") | `](CxxBinaryDescriptionArg.html " |
    |                                   | class in com.facebook.buck.cxx"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxBina                          |                                   |
    | ryFactory](CxxBinaryFactory.html  |                                   |
    | "class in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CxxBinary                        |                                   |
    | Flavored](CxxBinaryFlavored.html  |                                   |
    | "class in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CxxBinaryImplicitFlavor          |                                   |
    | s](CxxBinaryImplicitFlavors.html  |                                   |
    | "class in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CxxBinaryMetadataFactor          |                                   |
    | y](CxxBinaryMetadataFactory.html  |                                   |
    | "class in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CxxCompilationDatab              |                                   |
    | ase](CxxCompilationDatabase.html  |                                   |
    | "class in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CxxCompilationDatabaseEntry](    |                                   |
    | CxxCompilationDatabaseEntry.html  |                                   |
    | "class in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CxxDeps](CxxDeps.html            | ::: block                         |
    | "class in com.facebook.buck.cxx") | The group of                      |
    |                                   | [`BuildTarget`](../cor            |
    |                                   | e/model/BuildTarget.html "class i |
    |                                   | n com.facebook.buck.core.model")s |
    |                                   | from C/C++ constructor args which |
    |                                   | comprise a C/C++ descriptions     |
    |                                   | logical C/C++ deps used to find   |
    |                                   | dependency                        |
    |                                   | [`NativeLinkableGroup`](toolch    |
    |                                   | ain/nativelink/NativeLinkableGrou |
    |                                   | p.html "interface in com.facebook |
    |                                   | .buck.cxx.toolchain.nativelink")s |
    |                                   | or                                |
    |                                   | [`CxxPreprocessorDep              |
    |                                   | `](CxxPreprocessorDep.html "inter |
    |                                   | face in com.facebook.buck.cxx")s. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxDe                            |                                   |
    | ps.Builder](CxxDeps.Builder.html  |                                   |
    | "class in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CxxDescriptionEnhan              |                                   |
    | cer](CxxDescriptionEnhancer.html  |                                   |
    | "class in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CxxDescriptionsProvid            |                                   |
    | er](CxxDescriptionsProvider.html  |                                   |
    | "class in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CxxFlags](CxxFlags.html          |                                   |
    | "class in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CxxFlags.Trans                   | ::: block                         |
    | lateMacrosArgsFunction](CxxFlags. | Function for translating cxx flag |
    | TranslateMacrosArgsFunction.html  | macros in list of Arg.            |
    | "class in com.facebook.buck.cxx") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxFla                           | ::: block                         |
    | gs.TranslateMacrosFunction](CxxFl | Function for translating cxx flag |
    | ags.TranslateMacrosFunction.html  | macros.                           |
    | "class in com.facebook.buck.cxx") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxGenrule](CxxGenrule.html      | ::: block                         |
    | "class in com.facebook.buck.cxx") | Genrule with C++ aware macros.    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxGenruleDescrip                |                                   |
    | tion](CxxGenruleDescription.html  |                                   |
    | "class in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CxxGenruleDescriptionAr          | ::: block                         |
    | g](CxxGenruleDescriptionArg.html  | Immutable implementation of       |
    | "class in com.facebook.buck.cxx") | `CxxGenruleDescription.A          |
    |                                   | bstractCxxGenruleDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxGen                           | ::: block                         |
    | ruleDescriptionArg.Builder](CxxGe | Builds instances of type          |
    | nruleDescriptionArg.Builder.html  | [`CxxGenruleDescriptionArg`       |
    | "class in com.facebook.buck.cxx") | ](CxxGenruleDescriptionArg.html " |
    |                                   | class in com.facebook.buck.cxx"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxHeaders](CxxHeaders.html      | ::: block                         |
    | "class in com.facebook.buck.cxx") | Encapsulates headers from a       |
    |                                   | single root location.             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [C                                | ::: block                         |
    | xxHeadersDir](CxxHeadersDir.html  | Wraps a header directory to add   |
    | "class in com.facebook.buck.cxx") | to the preprocessors search path. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxInfe                          | ::: block                         |
    | rEnhancer](CxxInferEnhancer.html  | Handles infer flavors for         |
    | "class in com.facebook.buck.cxx") | [`CxxLib                          |
    |                                   | raryGroup`](CxxLibraryGroup.html  |
    |                                   | "class in com.facebook.buck.cxx") |
    |                                   | and                               |
    |                                   | [`CxxBinary`](CxxBinary.html "    |
    |                                   | class in com.facebook.buck.cxx"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxLibraryDescrip                |                                   |
    | tion](CxxLibraryDescription.html  |                                   |
    | "class in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CxxLibraryDescriptionAr          | ::: block                         |
    | g](CxxLibraryDescriptionArg.html  | Immutable implementation of       |
    | "class in com.facebook.buck.cxx") | `CxxLibraryDescription.A          |
    |                                   | bstractCxxLibraryDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxLib                           | ::: block                         |
    | raryDescriptionArg.Builder](CxxLi | Builds instances of type          |
    | braryDescriptionArg.Builder.html  | [`CxxLibraryDescriptionArg`       |
    | "class in com.facebook.buck.cxx") | ](CxxLibraryDescriptionArg.html " |
    |                                   | class in com.facebook.buck.cxx"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxLibrar                        |                                   |
    | yFactory](CxxLibraryFactory.html  |                                   |
    | "class in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CxxLibraryF                      |                                   |
    | lavored](CxxLibraryFlavored.html  |                                   |
    | "class in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CxxLi                            | ::: block                         |
    | braryGroup](CxxLibraryGroup.html  | An action graph representation of |
    | "class in com.facebook.buck.cxx") | a C/C++ library from the target   |
    |                                   | graph, providing the various      |
    |                                   | interfaces to make it consumable  |
    |                                   | by C/C++ preprocessing and native |
    |                                   | linkable rules.                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxLibraryImplicitFlavors        |                                   |
    | ](CxxLibraryImplicitFlavors.html  |                                   |
    | "class in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CxxLibraryMetadataFactory        |                                   |
    | ](CxxLibraryMetadataFactory.html  |                                   |
    | "class in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CxxLink](CxxLink.html            | ::: block                         |
    | "class in com.facebook.buck.cxx") | A BuildRule for linking c++       |
    |                                   | objects.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxLink.Impl](CxxLink.Impl.html  | ::: block                         |
    | "class in com.facebook.buck.cxx") | Buildable implementation of       |
    |                                   | CxxLink.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxLinkableEn                    |                                   |
    | hancer](CxxLinkableEnhancer.html  |                                   |
    | "class in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CxxLinkAndCompileRu              |                                   |
    | les](CxxLinkAndCompileRules.html  |                                   |
    | "class in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Cxx                              |                                   |
    | LinkOptions](CxxLinkOptions.html  |                                   |
    | "class in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CxxLocationMacroExpande          |                                   |
    | r](CxxLocationMacroExpander.html  |                                   |
    | "class in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CxxP                             |                                   |
    | recompiledHeaderDescription](CxxP |                                   |
    | recompiledHeaderDescription.html  |                                   |
    | "class in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CxxPrecomp                       | ::: block                         |
    | iledHeaderDescriptionArg](CxxPrec | Immutable implementation of       |
    | ompiledHeaderDescriptionArg.html  | `CxxPrecomp                       |
    | "class in com.facebook.buck.cxx") | iledHeaderDescription.AbstractCxx |
    |                                   | PrecompiledHeaderDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxPrecompiledHeaderDescri       | ::: block                         |
    | ptionArg.Builder](CxxPrecompiledH | Builds instances of type          |
    | eaderDescriptionArg.Builder.html  | [`CxxPrecompil                    |
    | "class in com.facebook.buck.cxx") | edHeaderDescriptionArg`](CxxPreco |
    |                                   | mpiledHeaderDescriptionArg.html " |
    |                                   | class in com.facebook.buck.cxx"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxPrecompiledHeaderTemplate](C  | ::: block                         |
    | xxPrecompiledHeaderTemplate.html  | Represents a precompilable header |
    | "class in com.facebook.buck.cxx") | file, along with dependencies.    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxPr                            | ::: block                         |
    | efixHeader](CxxPrefixHeader.html  | Represents a header file          |
    | "class in com.facebook.buck.cxx") | mentioned in a \`prefix_header\`  |
    |                                   | param in a cxx library/binary     |
    |                                   | rule.                             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxPrepareForLink                | ::: block                         |
    | Step](CxxPrepareForLinkStep.html  | Prepares argfile for the          |
    | "class in com.facebook.buck.cxx") | CxxLinkStep, so all arguments to  |
    |                                   | the linker will be stored in a    |
    |                                   | single file.                      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxPreproce                      |                                   |
    | ssables](CxxPreprocessables.html  |                                   |
    | "class in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CxxPreprocessAndCompi            | ::: block                         |
    | le](CxxPreprocessAndCompile.html  | A build rule which preprocesses   |
    | "class in com.facebook.buck.cxx") | and/or compiles a C/C++ source in |
    |                                   | a single step.                    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxPreprocessor                  | ::: block                         |
    | Input](CxxPreprocessorInput.html  | The components that get           |
    | "class in com.facebook.buck.cxx") | contributed to a top-level run of |
    |                                   | the C++ preprocessor.             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxPreprocessorInput.Builder](C  |                                   |
    | xxPreprocessorInput.Builder.html  |                                   |
    | "class in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [C                                |                                   |
    | xxRawHeaders](CxxRawHeaders.html  |                                   |
    | "class in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CxxSource](CxxSource.html        | ::: block                         |
    | "class in com.facebook.buck.cxx") | Describes a source file written   |
    |                                   | in the C programming language or  |
    |                                   | a derivative (C++, Objective-C,   |
    |                                   | Objective-C++, etc.) and the      |
    |                                   | various paths it uses from input  |
    |                                   | to output.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxSourceRuleFa                  |                                   |
    | ctory](CxxSourceRuleFactory.html  |                                   |
    | "class in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Cxx                              | ::: block                         |
    | SourceTypes](CxxSourceTypes.html  | Utilities for working with C-like |
    | "class in com.facebook.buck.cxx") | source types.                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxStrip](CxxStrip.html          | ::: block                         |
    | "class in com.facebook.buck.cxx") | Controls how strip tool is        |
    |                                   | invoked.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxSymlinkTreeHea                | ::: block                         |
    | ders](CxxSymlinkTreeHeaders.html  | Encapsulates headers modeled      |
    | "class in com.facebook.buck.cxx") | using a                           |
    |                                   | [`HeaderSymlinkTree`](toolchain/H |
    |                                   | eaderSymlinkTree.html "class in c |
    |                                   | om.facebook.buck.cxx.toolchain"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxTest](CxxTest.html            | ::: block                         |
    | "class in com.facebook.buck.cxx") | A no-op                           |
    |                                   | [`BuildRule`](../core             |
    |                                   | /rules/BuildRule.html "interface  |
    |                                   | in com.facebook.buck.core.rules") |
    |                                   | which houses the logic to run and |
    |                                   | form the results for C/C++ tests. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxTestDesc                      |                                   |
    | ription](CxxTestDescription.html  |                                   |
    | "class in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CxxTestDescriptio                | ::: block                         |
    | nArg](CxxTestDescriptionArg.html  | Immutable implementation of       |
    | "class in com.facebook.buck.cxx") | `CxxTestDescriptio                |
    |                                   | n.AbstractCxxTestDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | CxxTestDescriptionArg.Builder](Cx | Builds instances of type          |
    | xTestDescriptionArg.Builder.html  | [`CxxTestDescriptionA             |
    | "class in com.facebook.buck.cxx") | rg`](CxxTestDescriptionArg.html " |
    |                                   | class in com.facebook.buck.cxx"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxTh                            | ::: block                         |
    | inLTOIndex](CxxThinLTOIndex.html  | A BuildRule for linking c++       |
    | "class in com.facebook.buck.cxx") | objects.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxThinLTOIndex                  | ::: block                         |
    | .Impl](CxxThinLTOIndex.Impl.html  | Buildable implementation of       |
    | "class in com.facebook.buck.cxx") | CxxLink.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxThinLTOI                      | ::: block                         |
    | ndexArg](CxxThinLTOIndexArg.html  | Holds an argument specifying the  |
    | "class in com.facebook.buck.cxx") | location of a thinLTO index file  |
    |                                   | for optimization                  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [C                                | ::: block                         |
    | xxThinLTOOpt](CxxThinLTOOpt.html  | A build rule which runs the opt   |
    | "class in com.facebook.buck.cxx") | phase of an incremental ThinLTO   |
    |                                   | build                             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxThinLTOO                      | ::: block                         |
    | pt.Impl](CxxThinLTOOpt.Impl.html  | Buildable implementation for      |
    | "class in com.facebook.buck.cxx") | CxxThinLTOOpt.                    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxToolchainDescripti            | ::: block                         |
    | on](CxxToolchainDescription.html  | Defines a cxx_toolchain rule that |
    | "class in com.facebook.buck.cxx") | allows a                          |
    |                                   | [`CxxPlatform`](toolchai          |
    |                                   | n/CxxPlatform.html "interface in  |
    |                                   | com.facebook.buck.cxx.toolchain") |
    |                                   | to be configured as a build       |
    |                                   | target.                           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxToolchainDescriptionArg]      | ::: block                         |
    | (CxxToolchainDescriptionArg.html  | This is roughly analagous to the  |
    | "class in com.facebook.buck.cxx") | configuration provided by         |
    |                                   | `CxxBuckConfig`.                  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxToolcha                       | ::: block                         |
    | inDescriptionArg.Builder](CxxTool | Builds instances of type          |
    | chainDescriptionArg.Builder.html  | [`CxxToolchainDescriptionArg`](   |
    | "class in com.facebook.buck.cxx") | CxxToolchainDescriptionArg.html " |
    |                                   | class in com.facebook.buck.cxx"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxToolFlags](CxxToolFlags.html  | ::: block                         |
    | "class in com.facebook.buck.cxx") | Tracks flags passed to the        |
    |                                   | preprocessor or compiler.         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DepsBuilder](DepsBuilder.html    | ::: block                         |
    | "class in com.facebook.buck.cxx") | Builder suitable for generating   |
    |                                   | the dependency list of a build    |
    |                                   | rule.                             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ExplicitCxxTool                  | ::: block                         |
    | Flags](ExplicitCxxToolFlags.html  | `CxxToolFlags` implementation     |
    | "class in com.facebook.buck.cxx") | where the flags are stored        |
    |                                   | explicitly as lists.              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ExplicitCxxToolFlags.Builder](E  |                                   |
    | xplicitCxxToolFlags.Builder.html  |                                   |
    | "class in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [FrameworkDependen                | ::: block                         |
    | cies](FrameworkDependencies.html  | Metadata query for collecting     |
    | "class in com.facebook.buck.cxx") | framework dependencies to include |
    |                                   | in a bundle.                      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [He                               |                                   |
    | aderSymlinkTreeWithHeaderMap](Hea |                                   |
    | derSymlinkTreeWithHeaderMap.html  |                                   |
    | "class in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [LinkableListFilterFactory        | ::: block                         |
    | ](LinkableListFilterFactory.html  | Factory for the creation of       |
    | "class in com.facebook.buck.cxx") | [`LinkableListFilter`](tool       |
    |                                   | chain/nativelink/LinkableListFilt |
    |                                   | er.html "interface in com.faceboo |
    |                                   | k.buck.cxx.toolchain.nativelink") |
    |                                   | which can be used to filter the   |
    |                                   | libraries which an executable     |
    |                                   | (e.g., binary, shared library,    |
    |                                   | Mach-O bundle) links against.     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [MachoDylibS                      | ::: block                         |
    | tubRule](MachoDylibStubRule.html  | Rule which creates a scrubbed     |
    | "class in com.facebook.buck.cxx") | dylib stub from a dylib.          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [MachoDylibStubRuleFactory        | ::: block                         |
    | ](MachoDylibStubRuleFactory.html  | Factor which can create rules for |
    | "class in com.facebook.buck.cxx") | scrubbed dylib stubs              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Mach                             | ::: block                         |
    | oDylibStubScrubContentsStep](Mach | Resets all addresses in a dylib   |
    | oDylibStubScrubContentsStep.html  | stub, so that if the ABI of a     |
    | "class in com.facebook.buck.cxx") | dylib stays the same, the dylib   |
    |                                   | stub itself will be identical on  |
    |                                   | disk.                             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | MachoScrubContentSectionsStep](Ma | Uses the strip tool to remove the |
    | choScrubContentSectionsStep.html  | contents (i.e., compiled code)    |
    | "class in com.facebook.buck.cxx") | from a dylib.                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NoopDebugPathSaniti              | ::: block                         |
    | zer](NoopDebugPathSanitizer.html  | This                              |
    | "class in com.facebook.buck.cxx") | [                                 |
    |                                   | `DebugPathSanitizer`](toolchain/D |
    |                                   | ebugPathSanitizer.html "class in  |
    |                                   | com.facebook.buck.cxx.toolchain") |
    |                                   | pretty much doesn\'t do anything. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Omnibus](Omnibus.html            |                                   |
    | "class in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Omnibus.OmnibusLibrarie          |                                   |
    | s](Omnibus.OmnibusLibraries.html  |                                   |
    | "class in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [OmnibusRoots](OmnibusRoots.html  | ::: block                         |
    | "class in com.facebook.buck.cxx") | A helper class for building the   |
    |                                   | included and excluded omnibus     |
    |                                   | roots to pass to the omnibus      |
    |                                   | builder.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [OmnibusRoots.Bu                  |                                   |
    | ilder](OmnibusRoots.Builder.html  |                                   |
    | "class in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [PrebuiltCxx                      |                                   |
    | Library](PrebuiltCxxLibrary.html  |                                   |
    | "class in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [                                 |                                   |
    | PrebuiltCxxLibraryDescription](Pr |                                   |
    | ebuiltCxxLibraryDescription.html  |                                   |
    | "class in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Prebui                           | ::: block                         |
    | ltCxxLibraryDescriptionArg](Prebu | Immutable implementation of       |
    | iltCxxLibraryDescriptionArg.html  | `Prebui                           |
    | "class in com.facebook.buck.cxx") | ltCxxLibraryDescription.AbstractP |
    |                                   | rebuiltCxxLibraryDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PrebuiltCxxLibraryDesc           | ::: block                         |
    | riptionArg.Builder](PrebuiltCxxLi | Builds instances of type          |
    | braryDescriptionArg.Builder.html  | [`Prebuilt                        |
    | "class in com.facebook.buck.cxx") | CxxLibraryDescriptionArg`](Prebui |
    |                                   | ltCxxLibraryDescriptionArg.html " |
    |                                   | class in com.facebook.buck.cxx"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PrebuiltCx                       |                                   |
    | xLibraryGroupDescription](Prebuil |                                   |
    | tCxxLibraryGroupDescription.html  |                                   |
    | "class in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [PrebuiltCxxLibraryGroupDesc      | ::: block                         |
    | ription.CustomPrebuiltCxxLibrary] | An action graph representation of |
    | (PrebuiltCxxLibraryGroupDescripti | a custom prebuilt C/C++ library   |
    | on.CustomPrebuiltCxxLibrary.html  | from the target graph, providing  |
    | "class in com.facebook.buck.cxx") | the various interfaces to make it |
    |                                   | consumable by C/C++ preprocessing |
    |                                   | and native linkable rules.        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PrebuiltCxxLibra                 | ::: block                         |
    | ryGroupDescriptionArg](PrebuiltCx | Immutable implementation of       |
    | xLibraryGroupDescriptionArg.html  | `PrebuiltCxxLibra                 |
    | "class in com.facebook.buck.cxx") | ryGroupDescription.AbstractPrebui |
    |                                   | ltCxxLibraryGroupDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PrebuiltCxxLibraryGroupDescripti | ::: block                         |
    | onArg.Builder](PrebuiltCxxLibrary | Builds instances of type          |
    | GroupDescriptionArg.Builder.html  | [`PrebuiltCxxLibrary              |
    | "class in com.facebook.buck.cxx") | GroupDescriptionArg`](PrebuiltCxx |
    |                                   | LibraryGroupDescriptionArg.html " |
    |                                   | class in com.facebook.buck.cxx"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PreInclude](PreInclude.html      | ::: block                         |
    | "class in com.facebook.buck.cxx") | Represents a precompilable header |
    |                                   | file, along with dependencies.    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Preproces                        |                                   |
    | sorFlags](PreprocessorFlags.html  |                                   |
    | "class in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [PreprocessorFlags.Builder        |                                   |
    | ](PreprocessorFlags.Builder.html  |                                   |
    | "class in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Relat                            | ::: block                         |
    | iveLinkArg](RelativeLinkArg.html  | Relative link arg.                |
    | "class in com.facebook.buck.cxx") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [TransitiveCx                     | ::: block                         |
    | xPreprocessorInputCache](Transiti | Transitive C++ preprocessor input |
    | veCxxPreprocessorInputCache.html  | cache                             |
    | "class in com.facebook.buck.cxx") | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Enum                              | Description                       |
    +===================================+===================================+
    | [CxxInferEnhancer.InferFlavors](C | ::: block                         |
    | xxInferEnhancer.InferFlavors.html | Flavors affixed to a library or   |
    |  "enum in com.facebook.buck.cxx") | binary rule to run infer.         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxLibrar                        |                                   |
    | yDescription.MetadataType](CxxLib |                                   |
    | raryDescription.MetadataType.html |                                   |
    |  "enum in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CxxLibraryDescription.Type       |                                   |
    | ](CxxLibraryDescription.Type.html |                                   |
    |  "enum in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [C                                |                                   |
    | xxPreprocessables.IncludeType](Cx |                                   |
    | xPreprocessables.IncludeType.html |                                   |
    |  "enum in com.facebook.buck.cxx") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Cx                               |                                   |
    | xSource.Type](CxxSource.Type.html |                                   |
    |  "enum in com.facebook.buck.cxx") |                                   |
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
