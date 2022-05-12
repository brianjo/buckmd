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

<div>

-   Summary: 
-   [Nested](#nested.class.summary) \| 
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
::: subTitle
[Package]{.packageLabelInType} [com.facebook.buck.apple](package-summary.html)
:::

## Class AppleBinaryDescriptionArg {#class-applebinarydescriptionarg .title title="Class AppleBinaryDescriptionArg"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.AppleBinaryDescriptionArg

::: description
-   

    All Implemented Interfaces:
    :   `AppleNativeTargetDescriptionArg`, `HasEntitlementsFile`,
        `BuildRuleArg`, `ConstructorArg`, `DataTransferObject`,
        `HasContacts`, `HasDeclaredDeps`, `HasDefaultPlatform`,
        `HasTests`, `HasDefaultFlavors`, `CxxConstructorArg`,
        `CxxLibraryDescription.CommonArg`, `LinkableCxxConstructorArg`,
        `HasSystemFrameworkAndLibraries`, `SwiftCommonArg`

    ------------------------------------------------------------------------

        @ParametersAreNonnullByDefault
        @Generated("org.immutables.processor.ProxyProcessor")
        @Immutable
        @CheckReturnValue
        public final class AppleBinaryDescriptionArg
        extends Object

    ::: block
    Immutable implementation of
    `AppleBinaryDescription.AbstractAppleBinaryDescriptionArg`.
    Use the builder to create immutable instances:
    `AppleBinaryDescriptionArg.builder()`.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `AppleBinaryDe        | ::: block             |
        |                       | scriptionArg.Builder` | Builds instances of   |
        |                       |                       | type                  |
        |                       |                       | [`AppleBinary         |
        |                       |                       | DescriptionArg`](Appl |
        |                       |                       | eBinaryDescriptionArg |
        |                       |                       | .html "class in com.f |
        |                       |                       | acebook.buck.apple"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.core.description.arg.BuildRuleArg}

            ### Fields inherited from interface com.facebook.buck.core.description.arg.[BuildRuleArg](../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")

            `DEFAULT_TARGET_PLATFORM_PARAM_NAME`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static AppleBinaryDe | `builder()`           | ::: block             |
        | scriptionArg.Builder` |                       | Creates a builder for |
        |                       |                       | [`AppleBinary         |
        |                       |                       | DescriptionArg`](Appl |
        |                       |                       | eBinaryDescriptionArg |
        |                       |                       | .html "class in com.f |
        |                       |                       | acebook.buck.apple"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `eq                   | ::: block             |
        |                       | uals​(Object another)` | This instance is      |
        |                       |                       | equal to all          |
        |                       |                       | instances of          |
        |                       |                       | `Apple                |
        |                       |                       | BinaryDescriptionArg` |
        |                       |                       | that have equal       |
        |                       |                       | attribute values.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getBridgingHeader()` | ::: block             |
        | Optional<SourcePath>` |                       | These fields are      |
        |                       |                       | passed through to     |
        |                       |                       | SwiftLibrary for      |
        |                       |                       | mixed C/Swift         |
        |                       |                       | targets; they are not |
        |                       |                       | used otherwise.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `getCanBeAsset()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `co                   | `getCompatibleWith()` | ::: block             |
        | m.google.common.colle |                       | A list of             |
        | ct.ImmutableList<Unco |                       | `config_setting` a    |
        | nfiguredBuildTarget>` |                       | target is compatible  |
        |                       |                       | with.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getCompilerFlags()`  |                       |
        | n.collect.ImmutableLi |                       |                       |
        | st<StringWithMacros>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `co                   | `getConfigs()`        |                       |
        | m.google.common.colle |                       |                       |
        | ct.ImmutableSortedMap |                       |                       |
        | <String,​com.google.co |                       |                       |
        | mmon.collect.Immutabl |                       |                       |
        | eMap<String,​String>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getContacts()`       |                       |
        | common.collect.Immuta |                       |                       |
        | bleSortedSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `CxxDeps`             | `getCxxDeps()`        | ::: block             |
        |                       |                       | Override parent       |
        |                       |                       | class\'s deps to      |
        |                       |                       | include exported      |
        |                       |                       | deps.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Li          | `getCxxRuntimeType()` |                       |
        | nker.CxxRuntimeType>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getDefaultFlavors()` |                       |
        | common.collect.Immuta |                       |                       |
        | bleSortedSet<Flavor>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Flavor>`    | `                     |                       |
        |                       | getDefaultPlatform()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `getDefaults()`       |                       |
        | ommon.collect.Immutab |                       |                       |
        | leMap<String,​Flavor>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Unco        | `getDef               | ::: block             |
        | nfiguredBuildTarget>` | aultTargetPlatform()` | The name of build     |
        |                       |                       | target default        |
        |                       |                       | \"new\" platform: it  |
        |                       |                       | is used when a        |
        |                       |                       | platform is not       |
        |                       |                       | specified either      |
        |                       |                       | globally or in a      |
        |                       |                       | target which used     |
        |                       |                       | this target as a      |
        |                       |                       | dependency.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getDeps()`           |                       |
        | n.collect.ImmutableSo |                       |                       |
        | rtedSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `g                    |                       |
        | Optional<SourcePath>` | etEntitlementsFile()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getExecutableName()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `CxxDeps`             | `                     |                       |
        |                       | getExportedCxxDeps()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getExportedDeps()`   |                       |
        | n.collect.ImmutableSo |                       |                       |
        | rtedSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourceSortedSet`     | `                     |                       |
        |                       | getExportedHeaders()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPreproc           | `getE                 |                       |
        | essables.IncludeType` | xportedHeaderStyle()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.co        | `g                    |                       |
        | mmon.collect.Immutabl | etExportedLangPlatfor |                       |
        | eMap<CxxSource.Type,​P | mPreprocessorFlags()` |                       |
        | atternMatchedCollecti |                       |                       |
        | on<com.google.common. |                       |                       |
        | collect.ImmutableList |                       |                       |
        | <StringWithMacros>>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.goog             | `getExportedLan       |                       |
        | le.common.collect.Imm | gPreprocessorFlags()` |                       |
        | utableMap<CxxSource.T |                       |                       |
        | ype,​com.google.common |                       |                       |
        | .collect.ImmutableLis |                       |                       |
        | t<StringWithMacros>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getE                 |                       |
        | n.collect.ImmutableLi | xportedLinkerFlags()` |                       |
        | st<StringWithMacros>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getEx                |                       |
        | PatternMatchedCollect | portedPlatformDeps()` |                       |
        | ion<com.google.common |                       |                       |
        | .collect.ImmutableSor |                       |                       |
        | tedSet<BuildTarget>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getExpor             |                       |
        | PatternMatchedCollect | tedPlatformHeaders()` |                       |
        | ion<SourceSortedSet>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getExportedP         |                       |
        | PatternMatchedCollect | latformLinkerFlags()` |                       |
        | ion<com.google.common |                       |                       |
        | .collect.ImmutableLis |                       |                       |
        | t<StringWithMacros>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getExportedPlatfor   |                       |
        | PatternMatchedCollect | mPreprocessorFlags()` |                       |
        | ion<com.google.common |                       |                       |
        | .collect.ImmutableLis |                       |                       |
        | t<StringWithMacros>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getExpor             |                       |
        | n.collect.ImmutableLi | tedPostLinkerFlags()` |                       |
        | st<StringWithMacros>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getExportedPostP     |                       |
        | PatternMatchedCollect | latformLinkerFlags()` |                       |
        | ion<com.google.common |                       |                       |
        | .collect.ImmutableLis |                       |                       |
        | t<StringWithMacros>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getExporte           |                       |
        | n.collect.ImmutableLi | dPreprocessorFlags()` |                       |
        | st<StringWithMacros>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `                     | ::: block             |
        | .common.collect.Immut | getExtraXcodeFiles()` | extra_xcode_sources   |
        | ableList<SourcePath>` |                       | will add the files to |
        |                       |                       | the list of files in  |
        |                       |                       | the project and       |
        |                       |                       | won\'t add them to an |
        |                       |                       | Xcode target.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `ge                   | ::: block             |
        | .common.collect.Immut | tExtraXcodeSources()` | extra_xcode_sources   |
        | ableList<SourcePath>` |                       | will add the files to |
        |                       |                       | the list of files to  |
        |                       |                       | be compiled in the    |
        |                       |                       | Xcode target.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getFatLto()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `getForceStatic()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.   | `getFrameworks()`     |                       |
        | collect.ImmutableSort |                       |                       |
        | edSet<FrameworkPath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `                     |                       |
        |                       | getHeaderNamespace()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `g                    |                       |
        |                       | etHeaderPathPrefix()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourceSortedSet`     | `getHeaders()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `get                  | ::: block             |
        | common.collect.Immuta | IncludeDirectories()` | A list of include     |
        | bleSortedSet<String>` |                       | directories to be     |
        |                       |                       | added to the compile  |
        |                       |                       | command for compiling |
        |                       |                       | this cxx target.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getInfoPlist()`      |                       |
        | Optional<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `getInfo              |                       |
        | ommon.collect.Immutab | PlistSubstitutions()` |                       |
        | leMap<String,​String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getLabels()`         |                       |
        | common.collect.Immuta |                       |                       |
        | bleSortedSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.goog             | `ge                   |                       |
        | le.common.collect.Imm | tLangCompilerFlags()` |                       |
        | utableMap<CxxSource.T |                       |                       |
        | ype,​com.google.common |                       |                       |
        | .collect.ImmutableLis |                       |                       |
        | t<StringWithMacros>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.co        | `getLangPla           |                       |
        | mmon.collect.Immutabl | tformCompilerFlags()` |                       |
        | eMap<CxxSource.Type,​P |                       |                       |
        | atternMatchedCollecti |                       |                       |
        | on<com.google.common. |                       |                       |
        | collect.ImmutableList |                       |                       |
        | <StringWithMacros>>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.co        | `getLangPlatfor       |                       |
        | mmon.collect.Immutabl | mPreprocessorFlags()` |                       |
        | eMap<CxxSource.Type,​P |                       |                       |
        | atternMatchedCollecti |                       |                       |
        | on<com.google.common. |                       |                       |
        | collect.ImmutableList |                       |                       |
        | <StringWithMacros>>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.goog             | `getLan               |                       |
        | le.common.collect.Imm | gPreprocessorFlags()` |                       |
        | utableMap<CxxSource.T |                       |                       |
        | ype,​com.google.common |                       |                       |
        | .collect.ImmutableLis |                       |                       |
        | t<StringWithMacros>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.   | `getLibraries()`      |                       |
        | collect.ImmutableSort |                       |                       |
        | edSet<FrameworkPath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getLicenses()`       |                       |
        | e.common.collect.Immu |                       |                       |
        | tableSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `get                  |                       |
        | ogle.common.collect.I | LinkerExtraOutputs()` |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getLinkerFlags()`    |                       |
        | n.collect.ImmutableLi |                       |                       |
        | st<StringWithMacros>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getLinkGroup()`      | ::: block             |
        |                       |                       | Defines the link      |
        |                       |                       | group.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional             | `getLinkGroupMap()`   | ::: block             |
        | <com.google.common.co |                       | Defines the list of   |
        | llect.ImmutableList<C |                       | link group mappings.  |
        | xxLinkGroupMapping>>` |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Lin         | `getLinkStyle()`      |                       |
        | ker.LinkableDepType>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `getLinkWhole()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Opt                  | `getModulemapMode()`  | ::: block             |
        | ional<ModuleMapMode>` |                       | A modulemap mode, to  |
        |                       |                       | override the one      |
        |                       |                       | specified in          |
        |                       |                       | .buckconfig.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getModuleName()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getName()`           | ::: block             |
        |                       |                       | Each rule has a name  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getPla               |                       |
        | PatternMatchedCollect | tformCompilerFlags()` |                       |
        | ion<com.google.common |                       |                       |
        | .collect.ImmutableLis |                       |                       |
        | t<StringWithMacros>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getPlatformDeps()`   |                       |
        | PatternMatchedCollect |                       |                       |
        | ion<com.google.common |                       |                       |
        | .collect.ImmutableSor |                       |                       |
        | tedSet<BuildTarget>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `                     |                       |
        | PatternMatchedCollect | getPlatformHeaders()` |                       |
        | ion<SourceSortedSet>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getP                 |                       |
        | PatternMatchedCollect | latformLinkerFlags()` |                       |
        | ion<com.google.common |                       |                       |
        | .collect.ImmutableLis |                       |                       |
        | t<StringWithMacros>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getPlatfor           |                       |
        | PatternMatchedCollect | mPreprocessorFlags()` |                       |
        | ion<com.google.common |                       |                       |
        | .collect.ImmutableLis |                       |                       |
        | t<StringWithMacros>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Patt                 | `getPlatformSrcs()`   |                       |
        | ernMatchedCollection< |                       |                       |
        | com.google.common.col |                       |                       |
        | lect.ImmutableSortedS |                       |                       |
        | et<SourceWithFlags>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `                     |                       |
        | n.collect.ImmutableLi | getPostLinkerFlags()` |                       |
        | st<StringWithMacros>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getPostP             |                       |
        | PatternMatchedCollect | latformLinkerFlags()` |                       |
        | ion<com.google.common |                       |                       |
        | .collect.ImmutableLis |                       |                       |
        | t<StringWithMacros>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `ge                   |                       |
        | Optional<SourcePath>` | tPrecompiledHeader()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<NativeLi    | `g                    |                       |
        | nkableGroup.Linkage>` | etPreferredLinkage()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getPrefixHeader()`   |                       |
        | Optional<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `ge                   |                       |
        | n.collect.ImmutableLi | tPreprocessorFlags()` |                       |
        | st<StringWithMacros>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `CxxDeps`             | `getPrivateCxxDeps()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getPublic            | ::: block             |
        | common.collect.Immuta | IncludeDirectories()` | A list of include     |
        | bleSortedSet<String>` |                       | directories to be     |
        |                       |                       | added to the compile  |
        |                       |                       | command for compiling |
        |                       |                       | this cxx target and   |
        |                       |                       | every target that     |
        |                       |                       | depends on it.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getPublicSystem      | ::: block             |
        | common.collect.Immuta | IncludeDirectories()` | A list of include     |
        | bleSortedSet<String>` |                       | directories to be     |
        |                       |                       | added to the compile  |
        |                       |                       | command for compiling |
        |                       |                       | this cxx target and   |
        |                       |                       | every target that     |
        |                       |                       | depends on it.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.comm      | `getRawHeaders()`     | ::: block             |
        | on.collect.ImmutableS |                       | Raw headers are       |
        | ortedSet<SourcePath>` |                       | headers which are     |
        |                       |                       | used as they are (via |
        |                       |                       | compilation flags).   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getSoname()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.co | `getSrcs()`           |                       |
        | llect.ImmutableSorted |                       |                       |
        | Set<SourceWithFlags>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getSta               |                       |
        |                       | ticLibraryBasename()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Pattern>`   | `getSuppo             |                       |
        |                       | rtedPlatformsRegex()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `getSup               |                       |
        |                       | portsMergedLinking()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `get                  |                       |
        | n.collect.ImmutableLi | SwiftCompilerFlags()` |                       |
        | st<StringWithMacros>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getSwiftVersion()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `g                    | ::: block             |
        |                       | etTargetSdkVersion()` | The minimum OS        |
        |                       |                       | version for which     |
        |                       |                       | this target should be |
        |                       |                       | built.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getTests()`          |                       |
        | n.collect.ImmutableSo |                       |                       |
        | rtedSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getThinLto()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `getXcodePriv         |                       |
        |                       | ateHeadersSymlinks()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `getXcodePub          |                       |
        |                       | licHeadersSymlinks()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          | ::: block             |
        |                       |                       | Computes a hash code  |
        |                       |                       | from attributes:      |
        |                       |                       | `infoPlist`,          |
        |                       |                       | `inf                  |
        |                       |                       | oPlistSubstitutions`, |
        |                       |                       | `configs`,            |
        |                       |                       | `headerPathPrefix`,   |
        |                       |                       | `modular`,            |
        |                       |                       | `modulemapMode`,      |
        |                       |                       | `targetSdkVersion`,   |
        |                       |                       | `exportedHeaders`,    |
        |                       |                       | `expo                 |
        |                       |                       | rtedPlatformHeaders`, |
        |                       |                       | `export               |
        |                       |                       | edPreprocessorFlags`, |
        |                       |                       | `exportedPlatfo       |
        |                       |                       | rmPreprocessorFlags`, |
        |                       |                       | `exportedLa           |
        |                       |                       | ngPreprocessorFlags`, |
        |                       |                       | `exportedLangPlatfo   |
        |                       |                       | rmPreprocessorFlags`, |
        |                       |                       | `                     |
        |                       |                       | exportedLinkerFlags`, |
        |                       |                       | `expo                 |
        |                       |                       | rtedPostLinkerFlags`, |
        |                       |                       | `exported             |
        |                       |                       | PlatformLinkerFlags`, |
        |                       |                       | `exportedPost         |
        |                       |                       | PlatformLinkerFlags`, |
        |                       |                       | `exportedDeps`,       |
        |                       |                       | `e                    |
        |                       |                       | xportedPlatformDeps`, |
        |                       |                       | `supp                 |
        |                       |                       | ortedPlatformsRegex`, |
        |                       |                       | `soname`,             |
        |                       |                       | `st                   |
        |                       |                       | aticLibraryBasename`, |
        |                       |                       | `forceStatic`,        |
        |                       |                       | `linkWhole`,          |
        |                       |                       | `canBeAsset`,         |
        |                       |                       | `preferredLinkage`,   |
        |                       |                       | `xcodePu              |
        |                       |                       | blicHeadersSymlinks`, |
        |                       |                       | `xcodePri             |
        |                       |                       | vateHeadersSymlinks`, |
        |                       |                       | `extraXcodeSources`,  |
        |                       |                       | `extraXcodeFiles`,    |
        |                       |                       | `reexportAl           |
        |                       |                       | lHeaderDependencies`, |
        |                       |                       | `bridgingHeader`,     |
        |                       |                       | `moduleName`,         |
        |                       |                       | `publi                |
        |                       |                       | cIncludeDirectories`, |
        |                       |                       | `publicSyste          |
        |                       |                       | mIncludeDirectories`, |
        |                       |                       | `exportedCxxDeps`,    |
        |                       |                       | `cxxDeps`,            |
        |                       |                       | `                     |
        |                       |                       | exportedHeaderStyle`, |
        |                       |                       | `su                   |
        |                       |                       | pportsMergedLinking`, |
        |                       |                       | `linkStyle`,          |
        |                       |                       | `linkGroupMap`,       |
        |                       |                       | `linkGroup`,          |
        |                       |                       | `thinLto`, `fatLto`,  |
        |                       |                       | `srcs`,               |
        |                       |                       | `platformSrcs`,       |
        |                       |                       | `headers`,            |
        |                       |                       | `rawHeaders`,         |
        |                       |                       | `includeDirectories`, |
        |                       |                       | `platformHeaders`,    |
        |                       |                       | `prefixHeader`,       |
        |                       |                       | `precompiledHeader`,  |
        |                       |                       | `compilerFlags`,      |
        |                       |                       | `langCompilerFlags`,  |
        |                       |                       | `langPl               |
        |                       |                       | atformCompilerFlags`, |
        |                       |                       | `pl                   |
        |                       |                       | atformCompilerFlags`, |
        |                       |                       | `preprocessorFlags`,  |
        |                       |                       | `platfo               |
        |                       |                       | rmPreprocessorFlags`, |
        |                       |                       | `la                   |
        |                       |                       | ngPreprocessorFlags`, |
        |                       |                       | `langPlatfo           |
        |                       |                       | rmPreprocessorFlags`, |
        |                       |                       | `linkerFlags`,        |
        |                       |                       | `postLinkerFlags`,    |
        |                       |                       | `linkerExtraOutputs`, |
        |                       |                       | `                     |
        |                       |                       | platformLinkerFlags`, |
        |                       |                       | `executableName`,     |
        |                       |                       | `post                 |
        |                       |                       | PlatformLinkerFlags`, |
        |                       |                       | `platformDeps`,       |
        |                       |                       | `headerNamespace`,    |
        |                       |                       | `cxxRuntimeType`,     |
        |                       |                       | `defaults`,           |
        |                       |                       | `defaultFlavors`,     |
        |                       |                       | `privateCxxDeps`,     |
        |                       |                       | `licenses`, `labels`, |
        |                       |                       | `de                   |
        |                       |                       | faultTargetPlatform`, |
        |                       |                       | `compatibleWith`,     |
        |                       |                       | `name`, `deps`,       |
        |                       |                       | `defaultPlatform`,    |
        |                       |                       | `tests`,              |
        |                       |                       | `frameworks`,         |
        |                       |                       | `libraries`,          |
        |                       |                       | `swiftCompilerFlags`, |
        |                       |                       | `swiftVersion`,       |
        |                       |                       | `contacts`,           |
        |                       |                       | `entitlementsFile`.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isModular()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `isReexportAll        | ::: block             |
        |                       | HeaderDependencies()` | Controls whether the  |
        |                       |                       | headers of            |
        |                       |                       | dependencies in       |
        |                       |                       | \"deps\" is           |
        |                       |                       | re-exported for       |
        |                       |                       | compiling targets     |
        |                       |                       | that depend on this   |
        |                       |                       | one.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          | ::: block             |
        |                       |                       | Prints the immutable  |
        |                       |                       | value                 |
        |                       |                       | `Apple                |
        |                       |                       | BinaryDescriptionArg` |
        |                       |                       | with attribute        |
        |                       |                       | values.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.apple.AppleNativeTargetDescriptionArg}

            ### Methods inherited from interface com.facebook.buck.apple.[AppleNativeTargetDescriptionArg](AppleNativeTargetDescriptionArg.html "interface in com.facebook.buck.apple")

            `checkModularUsage`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.BuildRuleArg}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[BuildRuleArg](../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")

            `labelsContainsAnyOf`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.CxxConstructorArg}

            ### Methods inherited from interface com.facebook.buck.cxx.[CxxConstructorArg](../cxx/CxxConstructorArg.html "interface in com.facebook.buck.cxx")

            `checkDuplicateSources`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.CxxLibraryDescription.CommonArg}

            ### Methods inherited from interface com.facebook.buck.cxx.[CxxLibraryDescription.CommonArg](../cxx/CxxLibraryDescription.CommonArg.html "interface in com.facebook.buck.cxx")

            `checkHeadersUsage`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getInfoPlist()}

        -   #### getInfoPlist

            ``` methodSignature
            public Optional<SourcePath> getInfoPlist()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `infoPlist` attribute

        []{#getInfoPlistSubstitutions()}

        -   #### getInfoPlistSubstitutions

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​String> getInfoPlistSubstitutions()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `infoPlistSubstitutions` attribute

        []{#getConfigs()}

        -   #### getConfigs

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedMap<String,​com.google.common.collect.ImmutableMap<String,​String>> getConfigs()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getConfigs` in
                interface `AppleNativeTargetDescriptionArg`

            [Returns:]{.returnLabel}
            :   The value of the `configs` attribute

        []{#getHeaderPathPrefix()}

        -   #### getHeaderPathPrefix

            ``` methodSignature
            public Optional<String> getHeaderPathPrefix()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getHeaderPathPrefix` in
                interface `AppleNativeTargetDescriptionArg`

            [Returns:]{.returnLabel}
            :   The value of the `headerPathPrefix` attribute

        []{#isModular()}

        -   #### isModular

            ``` methodSignature
            public boolean isModular()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isModular` in
                interface `AppleNativeTargetDescriptionArg`

            [Returns:]{.returnLabel}
            :   The value of the `modular` attribute

        []{#getModulemapMode()}

        -   #### getModulemapMode

            ``` methodSignature
            public Optional<ModuleMapMode> getModulemapMode()
            ```

            ::: block
            A modulemap mode, to override the one specified in
            .buckconfig.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getModulemapMode` in
                interface `AppleNativeTargetDescriptionArg`

        []{#getTargetSdkVersion()}

        -   #### getTargetSdkVersion

            ``` methodSignature
            public Optional<String> getTargetSdkVersion()
            ```

            ::: block
            The minimum OS version for which this target should be
            built. If set, this will override the config-level option.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTargetSdkVersion` in
                interface `AppleNativeTargetDescriptionArg`

        []{#getExportedHeaders()}

        -   #### getExportedHeaders

            ``` methodSignature
            public SourceSortedSet getExportedHeaders()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExportedHeaders` in
                interface `CxxLibraryDescription.CommonArg`

            [Returns:]{.returnLabel}
            :   The value of the `exportedHeaders` attribute

        []{#getExportedPlatformHeaders()}

        -   #### getExportedPlatformHeaders

            ``` methodSignature
            public PatternMatchedCollection<SourceSortedSet> getExportedPlatformHeaders()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExportedPlatformHeaders` in
                interface `CxxLibraryDescription.CommonArg`

            [Returns:]{.returnLabel}
            :   The value of the `exportedPlatformHeaders` attribute

        []{#getExportedPreprocessorFlags()}

        -   #### getExportedPreprocessorFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<StringWithMacros> getExportedPreprocessorFlags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExportedPreprocessorFlags` in
                interface `CxxLibraryDescription.CommonArg`

            [Returns:]{.returnLabel}
            :   The value of the `exportedPreprocessorFlags` attribute

        []{#getExportedPlatformPreprocessorFlags()}

        -   #### getExportedPlatformPreprocessorFlags

            ``` methodSignature
            public PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> getExportedPlatformPreprocessorFlags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExportedPlatformPreprocessorFlags` in
                interface `CxxLibraryDescription.CommonArg`

            [Returns:]{.returnLabel}
            :   The value of the `exportedPlatformPreprocessorFlags`
                attribute

        []{#getExportedLangPreprocessorFlags()}

        -   #### getExportedLangPreprocessorFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<CxxSource.Type,​com.google.common.collect.ImmutableList<StringWithMacros>> getExportedLangPreprocessorFlags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExportedLangPreprocessorFlags` in
                interface `CxxLibraryDescription.CommonArg`

            [Returns:]{.returnLabel}
            :   The value of the `exportedLangPreprocessorFlags`
                attribute

        []{#getExportedLangPlatformPreprocessorFlags()}

        -   #### getExportedLangPlatformPreprocessorFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<CxxSource.Type,​PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> getExportedLangPlatformPreprocessorFlags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExportedLangPlatformPreprocessorFlags` in
                interface `CxxLibraryDescription.CommonArg`

            [Returns:]{.returnLabel}
            :   The value of the `exportedLangPlatformPreprocessorFlags`
                attribute

        []{#getExportedLinkerFlags()}

        -   #### getExportedLinkerFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<StringWithMacros> getExportedLinkerFlags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExportedLinkerFlags` in
                interface `CxxLibraryDescription.CommonArg`

            [Returns:]{.returnLabel}
            :   The value of the `exportedLinkerFlags` attribute

        []{#getExportedPostLinkerFlags()}

        -   #### getExportedPostLinkerFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<StringWithMacros> getExportedPostLinkerFlags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExportedPostLinkerFlags` in
                interface `CxxLibraryDescription.CommonArg`

            [Returns:]{.returnLabel}
            :   The value of the `exportedPostLinkerFlags` attribute

        []{#getExportedPlatformLinkerFlags()}

        -   #### getExportedPlatformLinkerFlags

            ``` methodSignature
            public PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> getExportedPlatformLinkerFlags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExportedPlatformLinkerFlags` in
                interface `CxxLibraryDescription.CommonArg`

            [Returns:]{.returnLabel}
            :   The value of the `exportedPlatformLinkerFlags` attribute

        []{#getExportedPostPlatformLinkerFlags()}

        -   #### getExportedPostPlatformLinkerFlags

            ``` methodSignature
            public PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> getExportedPostPlatformLinkerFlags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExportedPostPlatformLinkerFlags` in
                interface `CxxLibraryDescription.CommonArg`

            [Returns:]{.returnLabel}
            :   The value of the `exportedPostPlatformLinkerFlags`
                attribute

        []{#getExportedDeps()}

        -   #### getExportedDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildTarget> getExportedDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExportedDeps` in
                interface `CxxLibraryDescription.CommonArg`

            [Returns:]{.returnLabel}
            :   The value of the `exportedDeps` attribute

        []{#getExportedPlatformDeps()}

        -   #### getExportedPlatformDeps

            ``` methodSignature
            public PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> getExportedPlatformDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExportedPlatformDeps` in
                interface `CxxLibraryDescription.CommonArg`

            [Returns:]{.returnLabel}
            :   The value of the `exportedPlatformDeps` attribute

        []{#getSupportedPlatformsRegex()}

        -   #### getSupportedPlatformsRegex

            ``` methodSignature
            public Optional<Pattern> getSupportedPlatformsRegex()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSupportedPlatformsRegex` in
                interface `CxxLibraryDescription.CommonArg`

            [Returns:]{.returnLabel}
            :   The value of the `supportedPlatformsRegex` attribute

        []{#getSoname()}

        -   #### getSoname

            ``` methodSignature
            public Optional<String> getSoname()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSoname` in
                interface `CxxLibraryDescription.CommonArg`

            [Returns:]{.returnLabel}
            :   The value of the `soname` attribute

        []{#getStaticLibraryBasename()}

        -   #### getStaticLibraryBasename

            ``` methodSignature
            public Optional<String> getStaticLibraryBasename()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getStaticLibraryBasename` in
                interface `CxxLibraryDescription.CommonArg`

            [Returns:]{.returnLabel}
            :   The value of the `staticLibraryBasename` attribute

        []{#getForceStatic()}

        -   #### getForceStatic

            ``` methodSignature
            public Optional<Boolean> getForceStatic()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getForceStatic` in
                interface `CxxLibraryDescription.CommonArg`

            [Returns:]{.returnLabel}
            :   The value of the `forceStatic` attribute

        []{#getLinkWhole()}

        -   #### getLinkWhole

            ``` methodSignature
            public Optional<Boolean> getLinkWhole()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLinkWhole` in
                interface `CxxLibraryDescription.CommonArg`

            [Returns:]{.returnLabel}
            :   The value of the `linkWhole` attribute

        []{#getCanBeAsset()}

        -   #### getCanBeAsset

            ``` methodSignature
            public Optional<Boolean> getCanBeAsset()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCanBeAsset` in
                interface `CxxLibraryDescription.CommonArg`

            [Returns:]{.returnLabel}
            :   The value of the `canBeAsset` attribute

        []{#getPreferredLinkage()}

        -   #### getPreferredLinkage

            ``` methodSignature
            public Optional<NativeLinkableGroup.Linkage> getPreferredLinkage()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPreferredLinkage` in
                interface `CxxLibraryDescription.CommonArg`

            [Returns:]{.returnLabel}
            :   The value of the `preferredLinkage` attribute

        []{#getXcodePublicHeadersSymlinks()}

        -   #### getXcodePublicHeadersSymlinks

            ``` methodSignature
            public Optional<Boolean> getXcodePublicHeadersSymlinks()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getXcodePublicHeadersSymlinks` in
                interface `CxxLibraryDescription.CommonArg`

            [Returns:]{.returnLabel}
            :   The value of the `xcodePublicHeadersSymlinks` attribute

        []{#getXcodePrivateHeadersSymlinks()}

        -   #### getXcodePrivateHeadersSymlinks

            ``` methodSignature
            public Optional<Boolean> getXcodePrivateHeadersSymlinks()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getXcodePrivateHeadersSymlinks` in
                interface `CxxLibraryDescription.CommonArg`

            [Returns:]{.returnLabel}
            :   The value of the `xcodePrivateHeadersSymlinks` attribute

        []{#getExtraXcodeSources()}

        -   #### getExtraXcodeSources

            ``` methodSignature
            public com.google.common.collect.ImmutableList<SourcePath> getExtraXcodeSources()
            ```

            ::: block
            extra_xcode_sources will add the files to the list of files
            to be compiled in the Xcode target.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExtraXcodeSources` in
                interface `CxxLibraryDescription.CommonArg`

        []{#getExtraXcodeFiles()}

        -   #### getExtraXcodeFiles

            ``` methodSignature
            public com.google.common.collect.ImmutableList<SourcePath> getExtraXcodeFiles()
            ```

            ::: block
            extra_xcode_sources will add the files to the list of files
            in the project and won\'t add them to an Xcode target.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExtraXcodeFiles` in
                interface `CxxLibraryDescription.CommonArg`

        []{#isReexportAllHeaderDependencies()}

        -   #### isReexportAllHeaderDependencies

            ``` methodSignature
            public Optional<Boolean> isReexportAllHeaderDependencies()
            ```

            ::: block
            Controls whether the headers of dependencies in \"deps\" is
            re-exported for compiling targets that depend on this one.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `isReexportAllHeaderDependencies` in
                interface `CxxLibraryDescription.CommonArg`

        []{#getBridgingHeader()}

        -   #### getBridgingHeader

            ``` methodSignature
            public Optional<SourcePath> getBridgingHeader()
            ```

            ::: block
            These fields are passed through to SwiftLibrary for mixed
            C/Swift targets; they are not used otherwise.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBridgingHeader` in
                interface `CxxLibraryDescription.CommonArg`

        []{#getModuleName()}

        -   #### getModuleName

            ``` methodSignature
            public Optional<String> getModuleName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getModuleName` in
                interface `CxxLibraryDescription.CommonArg`

            [Returns:]{.returnLabel}
            :   The value of the `moduleName` attribute

        []{#getPublicIncludeDirectories()}

        -   #### getPublicIncludeDirectories

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<String> getPublicIncludeDirectories()
            ```

            ::: block
            A list of include directories to be added to the compile
            command for compiling this cxx target and every target that
            depends on it.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPublicIncludeDirectories` in
                interface `CxxLibraryDescription.CommonArg`

            [Returns:]{.returnLabel}
            :   a list of public (exported) include paths for this cxx
                target.

        []{#getPublicSystemIncludeDirectories()}

        -   #### getPublicSystemIncludeDirectories

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<String> getPublicSystemIncludeDirectories()
            ```

            ::: block
            A list of include directories to be added to the compile
            command for compiling this cxx target and every target that
            depends on it.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPublicSystemIncludeDirectories` in
                interface `CxxLibraryDescription.CommonArg`

            [Returns:]{.returnLabel}
            :   a list of public (exported) include paths for this cxx
                target.

        []{#getExportedCxxDeps()}

        -   #### getExportedCxxDeps

            ``` methodSignature
            public CxxDeps getExportedCxxDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExportedCxxDeps` in
                interface `CxxLibraryDescription.CommonArg`

            [Returns:]{.returnLabel}
            :   C/C++ deps which are propagated to dependents.

        []{#getCxxDeps()}

        -   #### getCxxDeps

            ``` methodSignature
            public CxxDeps getCxxDeps()
            ```

            ::: block
            Override parent class\'s deps to include exported deps.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCxxDeps` in interface `CxxConstructorArg`

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCxxDeps` in
                interface `CxxLibraryDescription.CommonArg`

            [Returns:]{.returnLabel}
            :   the C/C++ deps this rule builds against.

        []{#getExportedHeaderStyle()}

        -   #### getExportedHeaderStyle

            ``` methodSignature
            public CxxPreprocessables.IncludeType getExportedHeaderStyle()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExportedHeaderStyle` in
                interface `CxxLibraryDescription.CommonArg`

            [Returns:]{.returnLabel}
            :   how exported headers from this rule should be included
                by dependents.

        []{#getSupportsMergedLinking()}

        -   #### getSupportsMergedLinking

            ``` methodSignature
            public Optional<Boolean> getSupportsMergedLinking()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSupportsMergedLinking` in
                interface `CxxLibraryDescription.CommonArg`

            [Returns:]{.returnLabel}
            :   The value of the `supportsMergedLinking` attribute

        []{#getLinkStyle()}

        -   #### getLinkStyle

            ``` methodSignature
            public Optional<Linker.LinkableDepType> getLinkStyle()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLinkStyle` in interface `LinkableCxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `linkStyle` attribute

        []{#getLinkGroupMap()}

        -   #### getLinkGroupMap

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableList<CxxLinkGroupMapping>> getLinkGroupMap()
            ```

            ::: block
            Defines the list of link group mappings. Targets\'
            membership in a group is defined by the order of the list,
            so if more than one mapping matches a single target, the
            group would be the one defined by the first match.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLinkGroupMap` in
                interface `LinkableCxxConstructorArg`

        []{#getLinkGroup()}

        -   #### getLinkGroup

            ``` methodSignature
            public Optional<String> getLinkGroup()
            ```

            ::: block
            Defines the link group. When linking executable code, only
            static libraries which belong to the same group would be
            linked into the executable.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLinkGroup` in interface `LinkableCxxConstructorArg`

        []{#getThinLto()}

        -   #### getThinLto

            ``` methodSignature
            public boolean getThinLto()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getThinLto` in interface `LinkableCxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `thinLto` attribute

        []{#getFatLto()}

        -   #### getFatLto

            ``` methodSignature
            public boolean getFatLto()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFatLto` in interface `LinkableCxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `fatLto` attribute

        []{#getSrcs()}

        -   #### getSrcs

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<SourceWithFlags> getSrcs()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSrcs` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `srcs` attribute

        []{#getPlatformSrcs()}

        -   #### getPlatformSrcs

            ``` methodSignature
            public PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<SourceWithFlags>> getPlatformSrcs()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPlatformSrcs` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `platformSrcs` attribute

        []{#getHeaders()}

        -   #### getHeaders

            ``` methodSignature
            public SourceSortedSet getHeaders()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getHeaders` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `headers` attribute

        []{#getRawHeaders()}

        -   #### getRawHeaders

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<SourcePath> getRawHeaders()
            ```

            ::: block
            Raw headers are headers which are used as they are (via
            compilation flags). Buck doesn\'t copy them or create
            symlinks for them. They are public (since managed by
            compilation flags).
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRawHeaders` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   a list of raw headers

        []{#getIncludeDirectories()}

        -   #### getIncludeDirectories

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<String> getIncludeDirectories()
            ```

            ::: block
            A list of include directories to be added to the compile
            command for compiling this cxx target.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getIncludeDirectories` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   a list of private include paths for this cxx target.

        []{#getPlatformHeaders()}

        -   #### getPlatformHeaders

            ``` methodSignature
            public PatternMatchedCollection<SourceSortedSet> getPlatformHeaders()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPlatformHeaders` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `platformHeaders` attribute

        []{#getPrefixHeader()}

        -   #### getPrefixHeader

            ``` methodSignature
            public Optional<SourcePath> getPrefixHeader()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPrefixHeader` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `prefixHeader` attribute

        []{#getPrecompiledHeader()}

        -   #### getPrecompiledHeader

            ``` methodSignature
            public Optional<SourcePath> getPrecompiledHeader()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPrecompiledHeader` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `precompiledHeader` attribute

        []{#getCompilerFlags()}

        -   #### getCompilerFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<StringWithMacros> getCompilerFlags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCompilerFlags` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `compilerFlags` attribute

        []{#getLangCompilerFlags()}

        -   #### getLangCompilerFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<CxxSource.Type,​com.google.common.collect.ImmutableList<StringWithMacros>> getLangCompilerFlags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLangCompilerFlags` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `langCompilerFlags` attribute

        []{#getLangPlatformCompilerFlags()}

        -   #### getLangPlatformCompilerFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<CxxSource.Type,​PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> getLangPlatformCompilerFlags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLangPlatformCompilerFlags` in
                interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `langPlatformCompilerFlags` attribute

        []{#getPlatformCompilerFlags()}

        -   #### getPlatformCompilerFlags

            ``` methodSignature
            public PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> getPlatformCompilerFlags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPlatformCompilerFlags` in
                interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `platformCompilerFlags` attribute

        []{#getPreprocessorFlags()}

        -   #### getPreprocessorFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<StringWithMacros> getPreprocessorFlags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPreprocessorFlags` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `preprocessorFlags` attribute

        []{#getPlatformPreprocessorFlags()}

        -   #### getPlatformPreprocessorFlags

            ``` methodSignature
            public PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> getPlatformPreprocessorFlags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPlatformPreprocessorFlags` in
                interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `platformPreprocessorFlags` attribute

        []{#getLangPreprocessorFlags()}

        -   #### getLangPreprocessorFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<CxxSource.Type,​com.google.common.collect.ImmutableList<StringWithMacros>> getLangPreprocessorFlags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLangPreprocessorFlags` in
                interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `langPreprocessorFlags` attribute

        []{#getLangPlatformPreprocessorFlags()}

        -   #### getLangPlatformPreprocessorFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<CxxSource.Type,​PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> getLangPlatformPreprocessorFlags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLangPlatformPreprocessorFlags` in
                interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `langPlatformPreprocessorFlags`
                attribute

        []{#getLinkerFlags()}

        -   #### getLinkerFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<StringWithMacros> getLinkerFlags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLinkerFlags` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `linkerFlags` attribute

        []{#getPostLinkerFlags()}

        -   #### getPostLinkerFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<StringWithMacros> getPostLinkerFlags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPostLinkerFlags` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `postLinkerFlags` attribute

        []{#getLinkerExtraOutputs()}

        -   #### getLinkerExtraOutputs

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getLinkerExtraOutputs()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLinkerExtraOutputs` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `linkerExtraOutputs` attribute

        []{#getPlatformLinkerFlags()}

        -   #### getPlatformLinkerFlags

            ``` methodSignature
            public PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> getPlatformLinkerFlags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPlatformLinkerFlags` in
                interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `platformLinkerFlags` attribute

        []{#getExecutableName()}

        -   #### getExecutableName

            ``` methodSignature
            public Optional<String> getExecutableName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExecutableName` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `executableName` attribute

        []{#getPostPlatformLinkerFlags()}

        -   #### getPostPlatformLinkerFlags

            ``` methodSignature
            public PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> getPostPlatformLinkerFlags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPostPlatformLinkerFlags` in
                interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `postPlatformLinkerFlags` attribute

        []{#getPlatformDeps()}

        -   #### getPlatformDeps

            ``` methodSignature
            public PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> getPlatformDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPlatformDeps` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `platformDeps` attribute

        []{#getHeaderNamespace()}

        -   #### getHeaderNamespace

            ``` methodSignature
            public Optional<String> getHeaderNamespace()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getHeaderNamespace` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `headerNamespace` attribute

        []{#getCxxRuntimeType()}

        -   #### getCxxRuntimeType

            ``` methodSignature
            public Optional<Linker.CxxRuntimeType> getCxxRuntimeType()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCxxRuntimeType` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `cxxRuntimeType` attribute

        []{#getDefaults()}

        -   #### getDefaults

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​Flavor> getDefaults()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDefaults` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   The value of the `defaults` attribute

        []{#getDefaultFlavors()}

        -   #### getDefaultFlavors

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<Flavor> getDefaultFlavors()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDefaultFlavors` in interface `CxxConstructorArg`

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDefaultFlavors` in interface `HasDefaultFlavors`

            [Returns:]{.returnLabel}
            :   The computed-at-construction value of the
                `defaultFlavors` attribute

        []{#getPrivateCxxDeps()}

        -   #### getPrivateCxxDeps

            ``` methodSignature
            public CxxDeps getPrivateCxxDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPrivateCxxDeps` in interface `CxxConstructorArg`

            [Returns:]{.returnLabel}
            :   C/C++ deps which are \*not\* propagated to dependents.

        []{#getLicenses()}

        -   #### getLicenses

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<SourcePath> getLicenses()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLicenses` in interface `BuildRuleArg`

            [Returns:]{.returnLabel}
            :   The value of the `licenses` attribute

        []{#getLabels()}

        -   #### getLabels

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<String> getLabels()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLabels` in interface `BuildRuleArg`

            [Returns:]{.returnLabel}
            :   The value of the `labels` attribute

        []{#getDefaultTargetPlatform()}

        -   #### getDefaultTargetPlatform

            ``` methodSignature
            public Optional<UnconfiguredBuildTarget> getDefaultTargetPlatform()
            ```

            ::: block
            The name of build target default \"new\" platform: it is
            used when a platform is not specified either globally or in
            a target which used this target as a dependency.
            The value is a build target, but we specify it as string,
            because this function is not actually called, but the attr
            is fetched by name from the raw (unconfigured) target node.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDefaultTargetPlatform` in interface `BuildRuleArg`

        []{#getCompatibleWith()}

        -   #### getCompatibleWith

            ``` methodSignature
            public com.google.common.collect.ImmutableList<UnconfiguredBuildTarget> getCompatibleWith()
            ```

            ::: block
            A list of `config_setting` a target is compatible with.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCompatibleWith` in interface `BuildRuleArg`

        []{#getName()}

        -   #### getName

            ``` methodSignature
            public String getName()
            ```

            ::: block
            Each rule has a name
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getName` in interface `ConstructorArg`

        []{#getDeps()}

        -   #### getDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildTarget> getDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDeps` in interface `HasDeclaredDeps`

            [Returns:]{.returnLabel}
            :   The value of the `deps` attribute

        []{#getDefaultPlatform()}

        -   #### getDefaultPlatform

            ``` methodSignature
            public Optional<Flavor> getDefaultPlatform()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDefaultPlatform` in interface `HasDefaultPlatform`

            [Returns:]{.returnLabel}
            :   If present, the default platform with which to build
                this target if none are provided on the command line.

        []{#getTests()}

        -   #### getTests

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildTarget> getTests()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTests` in interface `HasTests`

            [Returns:]{.returnLabel}
            :   A list of tests of this target.

        []{#getFrameworks()}

        -   #### getFrameworks

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<FrameworkPath> getFrameworks()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFrameworks` in
                interface `HasSystemFrameworkAndLibraries`

            [Returns:]{.returnLabel}
            :   The value of the `frameworks` attribute

        []{#getLibraries()}

        -   #### getLibraries

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<FrameworkPath> getLibraries()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLibraries` in
                interface `HasSystemFrameworkAndLibraries`

            [Returns:]{.returnLabel}
            :   The value of the `libraries` attribute

        []{#getSwiftCompilerFlags()}

        -   #### getSwiftCompilerFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<StringWithMacros> getSwiftCompilerFlags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSwiftCompilerFlags` in interface `SwiftCommonArg`

            [Returns:]{.returnLabel}
            :   The value of the `swiftCompilerFlags` attribute

        []{#getSwiftVersion()}

        -   #### getSwiftVersion

            ``` methodSignature
            public Optional<String> getSwiftVersion()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSwiftVersion` in interface `SwiftCommonArg`

            [Returns:]{.returnLabel}
            :   The value of the `swiftVersion` attribute

        []{#getContacts()}

        -   #### getContacts

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<String> getContacts()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getContacts` in interface `HasContacts`

            [Returns:]{.returnLabel}
            :   The value of the `contacts` attribute

        []{#getEntitlementsFile()}

        -   #### getEntitlementsFile

            ``` methodSignature
            public Optional<SourcePath> getEntitlementsFile()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getEntitlementsFile` in interface `HasEntitlementsFile`

            [Returns:]{.returnLabel}
            :   The value of the `entitlementsFile` attribute

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(@Nullable
                                  Object another)
            ```

            ::: block
            This instance is equal to all instances of
            `AppleBinaryDescriptionArg` that have equal attribute
            values.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

            [Returns:]{.returnLabel}
            :   `true` if `this` is equal to `another` instance

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            ::: block
            Computes a hash code from attributes: `infoPlist`,
            `infoPlistSubstitutions`, `configs`, `headerPathPrefix`,
            `modular`, `modulemapMode`, `targetSdkVersion`,
            `exportedHeaders`, `exportedPlatformHeaders`,
            `exportedPreprocessorFlags`,
            `exportedPlatformPreprocessorFlags`,
            `exportedLangPreprocessorFlags`,
            `exportedLangPlatformPreprocessorFlags`,
            `exportedLinkerFlags`, `exportedPostLinkerFlags`,
            `exportedPlatformLinkerFlags`,
            `exportedPostPlatformLinkerFlags`, `exportedDeps`,
            `exportedPlatformDeps`, `supportedPlatformsRegex`, `soname`,
            `staticLibraryBasename`, `forceStatic`, `linkWhole`,
            `canBeAsset`, `preferredLinkage`,
            `xcodePublicHeadersSymlinks`, `xcodePrivateHeadersSymlinks`,
            `extraXcodeSources`, `extraXcodeFiles`,
            `reexportAllHeaderDependencies`, `bridgingHeader`,
            `moduleName`, `publicIncludeDirectories`,
            `publicSystemIncludeDirectories`, `exportedCxxDeps`,
            `cxxDeps`, `exportedHeaderStyle`, `supportsMergedLinking`,
            `linkStyle`, `linkGroupMap`, `linkGroup`, `thinLto`,
            `fatLto`, `srcs`, `platformSrcs`, `headers`, `rawHeaders`,
            `includeDirectories`, `platformHeaders`, `prefixHeader`,
            `precompiledHeader`, `compilerFlags`, `langCompilerFlags`,
            `langPlatformCompilerFlags`, `platformCompilerFlags`,
            `preprocessorFlags`, `platformPreprocessorFlags`,
            `langPreprocessorFlags`, `langPlatformPreprocessorFlags`,
            `linkerFlags`, `postLinkerFlags`, `linkerExtraOutputs`,
            `platformLinkerFlags`, `executableName`,
            `postPlatformLinkerFlags`, `platformDeps`,
            `headerNamespace`, `cxxRuntimeType`, `defaults`,
            `defaultFlavors`, `privateCxxDeps`, `licenses`, `labels`,
            `defaultTargetPlatform`, `compatibleWith`, `name`, `deps`,
            `defaultPlatform`, `tests`, `frameworks`, `libraries`,
            `swiftCompilerFlags`, `swiftVersion`, `contacts`,
            `entitlementsFile`.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`

            [Returns:]{.returnLabel}
            :   hashCode value

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            ::: block
            Prints the immutable value `AppleBinaryDescriptionArg` with
            attribute values.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

            [Returns:]{.returnLabel}
            :   A string representation of the value

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static AppleBinaryDescriptionArg.Builder builder()
            ```

            ::: block
            Creates a builder for
            [`AppleBinaryDescriptionArg`](AppleBinaryDescriptionArg.html "class in com.facebook.buck.apple").
            :::

            [Returns:]{.returnLabel}
            :   A new AppleBinaryDescriptionArg builder
    :::
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

<div>

-   Summary: 
-   [Nested](#nested.class.summary) \| 
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
