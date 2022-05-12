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
# Package com.facebook.buck.cxx.toolchain {#package-com.facebook.buck.cxx.toolchain .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [Archi                            | ::: block                         |
    | ver](Archiver.html "interface in  | Interface for a c/c++ archiver.   |
    | com.facebook.buck.cxx.toolchain") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ArchiverProvider](Arc            |                                   |
    | hiverProvider.html "interface in  |                                   |
    | com.facebook.buck.cxx.toolchain") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Compi                            | ::: block                         |
    | ler](Compiler.html "interface in  | Interface for a c/c++ compiler.   |
    | com.facebook.buck.cxx.toolchain") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxPlatform                      | ::: block                         |
    | ](CxxPlatform.html "interface in  | Interface describing a C/C++      |
    | com.facebook.buck.cxx.toolchain") | toolchain and platform to build   |
    |                                   | for.                              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxPlatformsSupplier](CxxPlat    | ::: block                         |
    | formsSupplier.html "interface in  | A toolchain that provides CXX     |
    | com.facebook.buck.cxx.toolchain") | platforms.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HasSystemFramewo                 | ::: block                         |
    | rkAndLibraries](HasSystemFramewor | Constructor args which specify    |
    | kAndLibraries.html "interface in  | system framework and library      |
    | com.facebook.buck.cxx.toolchain") | fields.                           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PathShortener](                  | ::: block                         |
    | PathShortener.html "interface in  | A function that may shorten a     |
    | com.facebook.buck.cxx.toolchain") | given path using variou           |
    |                                   | strategies.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Preprocessor]                    | ::: block                         |
    | (Preprocessor.html "interface in  | Interface for a c/c++             |
    | com.facebook.buck.cxx.toolchain") | preprocessor.                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Provid                           | ::: block                         |
    | erBackedCxxPlatform](ProviderBack | Identifies                        |
    | edCxxPlatform.html "interface in  | [                                 |
    | com.facebook.buck.cxx.toolchain") | `UnresolvedCxxPlatform`](Unresolv |
    |                                   | edCxxPlatform.html "interface in  |
    |                                   | com.facebook.buck.cxx.toolchain") |
    |                                   | provided by Buck rule.            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ProvidesCxxPlatform](Provid      | ::: block                         |
    | esCxxPlatform.html "interface in  | Tags objects that can provide a   |
    | com.facebook.buck.cxx.toolchain") | [`CxxPlatform`]                   |
    |                                   | (CxxPlatform.html "interface in c |
    |                                   | om.facebook.buck.cxx.toolchain"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [SharedLibraryI                   | ::: block                         |
    | nterfaceFactory](SharedLibraryInt | Factory class which produces a    |
    | erfaceFactory.html "interface in  | [`BuildRule`](../../core          |
    | com.facebook.buck.cxx.toolchain") | /rules/BuildRule.html "interface  |
    |                                   | in com.facebook.buck.core.rules") |
    |                                   | that generates a shared library   |
    |                                   | interface.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [SharedLibrar                     |                                   |
    | yInterfaceParams](SharedLibraryIn |                                   |
    | terfaceParams.html "interface in  |                                   |
    | com.facebook.buck.cxx.toolchain") |                                   |
    +-----------------------------------+-----------------------------------+
    | [SymbolNameTool](S                | ::: block                         |
    | ymbolNameTool.html "interface in  | Provides methods to extract       |
    | com.facebook.buck.cxx.toolchain") | symbol names from native formats  |
    |                                   | (e.g.                             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [UnresolvedCxxPlatform](Unresolv  | ::: block                         |
    | edCxxPlatform.html "interface in  | Used by descriptions to properly  |
    | com.facebook.buck.cxx.toolchain") | handle                            |
    |                                   | [`CxxPlatform`]                   |
    |                                   | (CxxPlatform.html "interface in c |
    |                                   | om.facebook.buck.cxx.toolchain"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [BsdArch                          | ::: block                         |
    | iver](BsdArchiver.html "class in  | Archiver implementation for a     |
    | com.facebook.buck.cxx.toolchain") | BSD-based toolchain.              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildRuleR                       | ::: block                         |
    | esolverCacheByTargetConfiguration | Custom cache to use with          |
    | ](BuildRuleResolverCacheByTargetC | [`CxxToolProvider`                |
    | onfiguration.html "class in com.f | ](CxxToolProvider.html "class in  |
    | acebook.buck.cxx.toolchain")\<T\> | com.facebook.buck.cxx.toolchain") |
    |                                   | and similar classes that need to  |
    |                                   | cache build rules for a given     |
    |                                   | build rule resolver and target    |
    |                                   | configuration.                    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ClangClCompiler                  | ::: block                         |
    | ](ClangClCompiler.html "class in  | Subclass of WindowsCompiler with  |
    | com.facebook.buck.cxx.toolchain") | overrides specific for clang-cl.  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ClangClPreprocessor](Cl          | ::: block                         |
    | angClPreprocessor.html "class in  | Preprocessor implementation for   |
    | com.facebook.buck.cxx.toolchain") | compilations using clang-cl.      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ClangCompil                      |                                   |
    | er](ClangCompiler.html "class in  |                                   |
    | com.facebook.buck.cxx.toolchain") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ClangPreprocessor](              | ::: block                         |
    | ClangPreprocessor.html "class in  | Preprocessor implementation for   |
    | com.facebook.buck.cxx.toolchain") | the Clang toolchain.              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ClangWindowsArchiver](Cla        | ::: block                         |
    | ngWindowsArchiver.html "class in  | Archiver implementation for the   |
    | com.facebook.buck.cxx.toolchain") | Clang for Windows toolchain.      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ClangWindowsCompiler](Cla        | ::: block                         |
    | ngWindowsCompiler.html "class in  | Compiler implementation for the   |
    | com.facebook.buck.cxx.toolchain") | Clang for Windows toolchain.      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | ClangWindowsPreprocessor](ClangWi | Preprocessor implementation for   |
    | ndowsPreprocessor.html "class in  | the Clang toolchain.              |
    | com.facebook.buck.cxx.toolchain") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CompilerProvider]                |                                   |
    | (CompilerProvider.html "class in  |                                   |
    | com.facebook.buck.cxx.toolchain") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CxxFlavorSanitizer](C            |                                   |
    | xxFlavorSanitizer.html "class in  |                                   |
    | com.facebook.buck.cxx.toolchain") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CxxPlatform.Builder](Cx          |                                   |
    | xPlatform.Builder.html "class in  |                                   |
    | com.facebook.buck.cxx.toolchain") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CxxPlatformsProvider](Cxx        |                                   |
    | PlatformsProvider.html "class in  |                                   |
    | com.facebook.buck.cxx.toolchain") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CxxToolProvider](Cxx             | ::: block                         |
    | ToolProvider.html "class in com.f | A provide for the                 |
    | acebook.buck.cxx.toolchain")\<T\> | [`Preprocessor`]                  |
    |                                   | (Preprocessor.html "interface in  |
    |                                   | com.facebook.buck.cxx.toolchain") |
    |                                   | and                               |
    |                                   | [`Compil                          |
    |                                   | er`](Compiler.html "interface in  |
    |                                   | com.facebook.buck.cxx.toolchain") |
    |                                   | C/C++ drivers.                    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxToolTypeInferer](C            | ::: block                         |
    | xxToolTypeInferer.html "class in  | Utilities for inferring the       |
    | com.facebook.buck.cxx.toolchain") | [`CxxToolProvider.Type`](Cx       |
    |                                   | xToolProvider.Type.html "enum in  |
    |                                   | com.facebook.buck.cxx.toolchain") |
    |                                   | of a cxx tool.                    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DebugPathSanitizer](D            | ::: block                         |
    | ebugPathSanitizer.html "class in  | Encapsulates all the logic to     |
    | com.facebook.buck.cxx.toolchain") | sanitize debug paths in native    |
    |                                   | code.                             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DefaultCompiler                  | ::: block                         |
    | ](DefaultCompiler.html "class in  | Default implementation of the     |
    | com.facebook.buck.cxx.toolchain") | Compiler interface.               |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ElfSharedLibra                   |                                   |
    | ryInterfaceParams](ElfSharedLibra |                                   |
    | ryInterfaceParams.html "class in  |                                   |
    | com.facebook.buck.cxx.toolchain") |                                   |
    +-----------------------------------+-----------------------------------+
    | [FasterPatte                      | ::: block                         |
    | rn](FasterPattern.html "class in  | Pattern-like object which is      |
    | com.facebook.buck.cxx.toolchain") | compatible with Pattern but       |
    |                                   | faster at handling simpler        |
    |                                   | patterns like `.*foo.*`.          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [GccComp                          |                                   |
    | iler](GccCompiler.html "class in  |                                   |
    | com.facebook.buck.cxx.toolchain") |                                   |
    +-----------------------------------+-----------------------------------+
    | [GccPreprocessor                  | ::: block                         |
    | ](GccPreprocessor.html "class in  | Preprocessor implementation for a |
    | com.facebook.buck.cxx.toolchain") | gcc toolchain.                    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [GnuArch                          | ::: block                         |
    | iver](GnuArchiver.html "class in  | Archiver implementation for gcc.  |
    | com.facebook.buck.cxx.toolchain") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HeaderSymlinkTree](              |                                   |
    | HeaderSymlinkTree.html "class in  |                                   |
    | com.facebook.buck.cxx.toolchain") |                                   |
    +-----------------------------------+-----------------------------------+
    | [HeaderSymlin                     |                                   |
    | kTreeWithModuleMap](HeaderSymlink |                                   |
    | TreeWithModuleMap.html "class in  |                                   |
    | com.facebook.buck.cxx.toolchain") |                                   |
    +-----------------------------------+-----------------------------------+
    | [HeaderVerification](H            | ::: block                         |
    | eaderVerification.html "class in  | Defines how to handle headers     |
    | com.facebook.buck.cxx.toolchain") | that get included during the      |
    |                                   | build but aren\'t explicitly      |
    |                                   | tracked in any build files.       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [InferBuckConfig                  | ::: block                         |
    | ](InferBuckConfig.html "class in  | Infer support for Cxx             |
    | com.facebook.buck.cxx.toolchain") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [MachoDylibStubParams](Mac        | ::: block                         |
    | hoDylibStubParams.html "class in  | Represents the params needed to   |
    | com.facebook.buck.cxx.toolchain") | create scrubbed dylib stubs.      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PosixNmSymbolNameTool](Posi      | ::: block                         |
    | xNmSymbolNameTool.html "class in  | A                                 |
    | com.facebook.buck.cxx.toolchain") | [`SymbolNameTool`](S              |
    |                                   | ymbolNameTool.html "interface in  |
    |                                   | com.facebook.buck.cxx.toolchain") |
    |                                   | implementation using a            |
    |                                   | POSIX-compliant \`nm\` utility    |
    |                                   | (                                 |
    |                                   | http://pubs.opengroup.org/onlinep |
    |                                   | ubs/009696699/utilities/nm.html). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Prefix                           | ::: block                         |
    | MapDebugPathSanitizer](PrefixMapD | This sanitizer works by depending |
    | ebugPathSanitizer.html "class in  | on the compiler\'s                |
    | com.facebook.buck.cxx.toolchain") | -fdebug-prefix-map flag to        |
    |                                   | properly ensure that the output   |
    |                                   | only contains references to the   |
    |                                   | mapped-to paths (i.e.             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PreprocessorProvider](Pre        |                                   |
    | processorProvider.html "class in  |                                   |
    | com.facebook.buck.cxx.toolchain") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ProviderBasedUnresol             | ::: block                         |
    | vedCxxPlatform](ProviderBasedUnre | Used to provide a                 |
    | solvedCxxPlatform.html "class in  | [`CxxPlatform`                    |
    | com.facebook.buck.cxx.toolchain") | ](CxxPlatform.html "interface in  |
    |                                   | com.facebook.buck.cxx.toolchain") |
    |                                   | that is specified as a            |
    |                                   | cxx_toolchain build target.       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [WindowsArchiver                  | ::: block                         |
    | ](WindowsArchiver.html "class in  | Archiver implementation for the   |
    | com.facebook.buck.cxx.toolchain") | Windows toolchain.                |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [WindowsCompiler                  |                                   |
    | ](WindowsCompiler.html "class in  |                                   |
    | com.facebook.buck.cxx.toolchain") |                                   |
    +-----------------------------------+-----------------------------------+
    | [WindowsMl64Compiler](Wi          | ::: block                         |
    | ndowsMl64Compiler.html "class in  | A bridge to MASM for x64          |
    | com.facebook.buck.cxx.toolchain") | (ml64.exe)                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [WindowsPreprocessor](Wi          | ::: block                         |
    | ndowsPreprocessor.html "class in  | Preprocessor implementation for   |
    | com.facebook.buck.cxx.toolchain") | the Windows toolchain.            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Enum                              | Description                       |
    +===================================+===================================+
    | [ArchiveContent                   | ::: block                         |
    | s](ArchiveContents.html "enum in  | How this archive packages its     |
    | com.facebook.buck.cxx.toolchain") | contents.                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ArchiverProvider.Lega            | ::: block                         |
    | cyArchiverType](ArchiverProvider. | .buckconfig accepts this and we   |
    | LegacyArchiverType.html "enum in  | combine it with the current       |
    | com.facebook.buck.cxx.toolchain") | platform to determine the         |
    |                                   | archiver type.                    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ArchiverProvider.Type](Arc       | ::: block                         |
    | hiverProvider.Type.html "enum in  | Optional type that can be         |
    | com.facebook.buck.cxx.toolchain") | specified by cxx.archiver_type to |
    |                                   | indicate the given archiver is    |
    |                                   | llvm-lib.                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxToolProvider.Type](Cx         |                                   |
    | xToolProvider.Type.html "enum in  |                                   |
    | com.facebook.buck.cxx.toolchain") |                                   |
    +-----------------------------------+-----------------------------------+
    | [DependencyTrackingMode](Depe     | ::: block                         |
    | ndencyTrackingMode.html "enum in  | Describes the underlying          |
    | com.facebook.buck.cxx.toolchain") | mechanism to track dependencies   |
    |                                   | for a cxx compilation unit.       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Head                             |                                   |
    | erMode](HeaderMode.html "enum in  |                                   |
    | com.facebook.buck.cxx.toolchain") |                                   |
    +-----------------------------------+-----------------------------------+
    | [HeaderVerification.Mode](Heade   |                                   |
    | rVerification.Mode.html "enum in  |                                   |
    | com.facebook.buck.cxx.toolchain") |                                   |
    +-----------------------------------+-----------------------------------+
    | [HeaderVisibility                 |                                   |
    | ](HeaderVisibility.html "enum in  |                                   |
    | com.facebook.buck.cxx.toolchain") |                                   |
    +-----------------------------------+-----------------------------------+
    | [LinkerMapM                       | ::: block                         |
    | ode](LinkerMapMode.html "enum in  | Defines if linker map should be   |
    | com.facebook.buck.cxx.toolchain") | generated or not.                 |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PicType](PicType.html "enum in   | ::: block                         |
    | com.facebook.buck.cxx.toolchain") | Different compilation modes for   |
    |                                   | PIC (position-independent code)   |
    |                                   | and PDC (position-dependent       |
    |                                   | code).                            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [SharedLibraryInte                |                                   |
    | rfaceParams.Kind](SharedLibraryIn |                                   |
    | terfaceParams.Kind.html "enum in  |                                   |
    | com.facebook.buck.cxx.toolchain") |                                   |
    +-----------------------------------+-----------------------------------+
    | [SharedLibraryInte                | ::: block                         |
    | rfaceParams.Type](SharedLibraryIn | The configured mode for shared    |
    | terfaceParams.Type.html "enum in  | library interfaces.               |
    | com.facebook.buck.cxx.toolchain") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Stri                             | ::: block                         |
    | pStyle](StripStyle.html "enum in  | Defines the level of symbol       |
    | com.facebook.buck.cxx.toolchain") | stripping to be performed on the  |
    |                                   | linked product of the build.      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | ToolType](ToolType.html "enum in  | Enumerates possible external      |
    | com.facebook.buck.cxx.toolchain") | tools used in building C/C++      |
    |                                   | programs.                         |
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
