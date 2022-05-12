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
-   Nested \| 
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.cxx](package-summary.html)
:::

## Class CxxDescriptionEnhancer {#class-cxxdescriptionenhancer .title title="Class CxxDescriptionEnhancer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.CxxDescriptionEnhancer

::: description
-   

    ------------------------------------------------------------------------

        public class CxxDescriptionEnhancer
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                                                Description
          ------------------- ---------------------------------------------------- -------------
          `static Flavor`     `BINARY_WITH_SHARED_LIBRARIES_SYMLINK_TREE_FLAVOR`    
          `static Flavor`     `CXX_LINK_BINARY_FLAVOR`                              
          `static Flavor`     `CXX_LINK_MAP_FLAVOR`                                 
          `static Flavor`     `CXX_LINK_THININDEX_FLAVOR`                           
          `static Flavor`     `EXPORTED_HEADER_SYMLINK_TREE_FLAVOR`                 
          `static Flavor`     `HEADER_SYMLINK_TREE_FLAVOR`                          
          `static Flavor`     `INCREMENTAL_THINLTO`                                 
          `static Flavor`     `MACH_O_BUNDLE_FLAVOR`                                
          `static Flavor`     `SHARED_FLAVOR`                                       
          `static Flavor`     `SHARED_INTERFACE_FLAVOR`                             
          `static Flavor`     `SHARED_LIBRARY_SYMLINK_TREE_FLAVOR`                  
          `static Flavor`     `STATIC_FLAVOR`                                       
          `static Flavor`     `STATIC_PIC_FLAVOR`                                   

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static               | `collectCxxPreproces  |                       |
        |  com.google.common.co | sorInput​(BuildTarget  |                       |
        | llect.ImmutableList<C | target,               |                       |
        | xxPreprocessorInput>` |               CxxPlat |                       |
        |                       | form cxxPlatform,     |                       |
        |                       |                       |                       |
        |                       |    ActionGraphBuilder |                       |
        |                       |  graphBuilder,        |                       |
        |                       |                       |                       |
        |                       | Iterable<BuildRule> d |                       |
        |                       | eps,                  |                       |
        |                       |            com.google |                       |
        |                       | .common.collect.Immut |                       |
        |                       | ableMultimap<CxxSourc |                       |
        |                       | e.Type,​? extends Arg> |                       |
        |                       |  preprocessorFlags,   |                       |
        |                       |                       |                       |
        |                       |      com.google.commo |                       |
        |                       | n.collect.ImmutableLi |                       |
        |                       | st<HeaderSymlinkTree> |                       |
        |                       |  headerSymlinkTrees,  |                       |
        |                       |                       |                       |
        |                       |       com.google.comm |                       |
        |                       | on.collect.ImmutableS |                       |
        |                       | et<FrameworkPath> fra |                       |
        |                       | meworks,              |                       |
        |                       |                Iterab |                       |
        |                       | le<CxxPreprocessorInp |                       |
        |                       | ut> cxxPreprocessorIn |                       |
        |                       | putFromDeps,          |                       |
        |                       |                    co |                       |
        |                       | m.google.common.colle |                       |
        |                       | ct.ImmutableSortedSet |                       |
        |                       | <SourcePath> rawHeade |                       |
        |                       | rs,                   |                       |
        |                       |           com.google. |                       |
        |                       | common.collect.Immuta |                       |
        |                       | bleSortedSet<String>  |                       |
        |                       | includeDirectories,   |                       |
        |                       |                       |                       |
        |                       |      ProjectFilesyste |                       |
        |                       | m projectFilesystem)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Cx            | `                     |                       |
        | xLinkAndCompileRules` | createBuildRuleForCxx |                       |
        |                       | ThinLtoBinary​(BuildTa |                       |
        |                       | rget target,          |                       |
        |                       |                       |                       |
        |                       |      ProjectFilesyste |                       |
        |                       | m projectFilesystem,  |                       |
        |                       |                       |                       |
        |                       |              ActionGr |                       |
        |                       | aphBuilder graphBuild |                       |
        |                       | er,                   |                       |
        |                       |                  Cell |                       |
        |                       | PathResolver cellRoot |                       |
        |                       | s,                    |                       |
        |                       |                 CxxBu |                       |
        |                       | ckConfig cxxBuckConfi |                       |
        |                       | g,                    |                       |
        |                       |                 CxxPl |                       |
        |                       | atform cxxPlatform,   |                       |
        |                       |                       |                       |
        |                       |             CxxBinary |                       |
        |                       | Description.CommonArg |                       |
        |                       |  args,                |                       |
        |                       |                     c |                       |
        |                       | om.google.common.coll |                       |
        |                       | ect.ImmutableSet<Buil |                       |
        |                       | dTarget> extraDeps,   |                       |
        |                       |                       |                       |
        |                       |             Optional< |                       |
        |                       | StripStyle> stripStyl |                       |
        |                       | e,                    |                       |
        |                       |                 Optio |                       |
        |                       | nal<LinkerMapMode> fl |                       |
        |                       | avoredLinkerMapMode)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Cx            | `cre                  |                       |
        | xLinkAndCompileRules` | ateBuildRulesForCxxBi |                       |
        |                       | nary​(BuildTarget targ |                       |
        |                       | et,                   |                       |
        |                       |            ProjectFil |                       |
        |                       | esystem projectFilesy |                       |
        |                       | stem,                 |                       |
        |                       |              ActionGr |                       |
        |                       | aphBuilder graphBuild |                       |
        |                       | er,                   |                       |
        |                       |            CellPathRe |                       |
        |                       | solver cellRoots,     |                       |
        |                       |                       |                       |
        |                       |     CxxBuckConfig cxx |                       |
        |                       | BuckConfig,           |                       |
        |                       |                    Cx |                       |
        |                       | xPlatform cxxPlatform |                       |
        |                       | ,                     |                       |
        |                       |          com.google.c |                       |
        |                       | ommon.collect.Immutab |                       |
        |                       | leMap<String,​CxxSourc |                       |
        |                       | e> srcs,              |                       |
        |                       |                 com.g |                       |
        |                       | oogle.common.collect. |                       |
        |                       | ImmutableMap<Path,​Sou |                       |
        |                       | rcePath> headers,     |                       |
        |                       |                       |                       |
        |                       |     SortedSet<BuildRu |                       |
        |                       | le> deps,             |                       |
        |                       |                  com. |                       |
        |                       | google.common.collect |                       |
        |                       | .ImmutableSet<BuildTa |                       |
        |                       | rget> linkWholeDeps,  |                       |
        |                       |                       |                       |
        |                       |        Optional<Strip |                       |
        |                       | Style> stripStyle,    |                       |
        |                       |                       |                       |
        |                       |      Optional<LinkerM |                       |
        |                       | apMode> flavoredLinke |                       |
        |                       | rMapMode,             |                       |
        |                       |                  Link |                       |
        |                       | er.LinkableDepType li |                       |
        |                       | nkStyle,              |                       |
        |                       |                 Optio |                       |
        |                       | nal<LinkableListFilte |                       |
        |                       | r> linkableListFilter |                       |
        |                       | ,                     |                       |
        |                       |          CxxLinkOptio |                       |
        |                       | ns linkOptions,       |                       |
        |                       |                       |                       |
        |                       |   com.google.common.c |                       |
        |                       | ollect.ImmutableList< |                       |
        |                       | StringWithMacros> pre |                       |
        |                       | processorFlags,       |                       |
        |                       |                       |                       |
        |                       |   PatternMatchedColle |                       |
        |                       | ction<com.google.comm |                       |
        |                       | on.collect.ImmutableL |                       |
        |                       | ist<StringWithMacros> |                       |
        |                       | > platformPreprocesso |                       |
        |                       | rFlags,               |                       |
        |                       |                com.go |                       |
        |                       | ogle.common.collect.I |                       |
        |                       | mmutableMap<CxxSource |                       |
        |                       | .Type,​com.google.comm |                       |
        |                       | on.collect.ImmutableL |                       |
        |                       | ist<StringWithMacros> |                       |
        |                       | > langPreprocessorFla |                       |
        |                       | gs,                   |                       |
        |                       |            com.google |                       |
        |                       | .common.collect.Immut |                       |
        |                       | ableMap<CxxSource.Typ |                       |
        |                       | e,​PatternMatchedColle |                       |
        |                       | ction<com.google.comm |                       |
        |                       | on.collect.ImmutableL |                       |
        |                       | ist<StringWithMacros> |                       |
        |                       | >> langPlatformPrepro |                       |
        |                       | cessorFlags,          |                       |
        |                       |                     c |                       |
        |                       | om.google.common.coll |                       |
        |                       | ect.ImmutableSortedSe |                       |
        |                       | t<FrameworkPath> fram |                       |
        |                       | eworks,               |                       |
        |                       |                com.go |                       |
        |                       | ogle.common.collect.I |                       |
        |                       | mmutableSortedSet<Fra |                       |
        |                       | meworkPath> libraries |                       |
        |                       | ,                     |                       |
        |                       |          com.google.c |                       |
        |                       | ommon.collect.Immutab |                       |
        |                       | leList<StringWithMacr |                       |
        |                       | os> compilerFlags,    |                       |
        |                       |                       |                       |
        |                       |      com.google.commo |                       |
        |                       | n.collect.ImmutableMa |                       |
        |                       | p<CxxSource.Type,​com. |                       |
        |                       | google.common.collect |                       |
        |                       | .ImmutableList<String |                       |
        |                       | WithMacros>> langComp |                       |
        |                       | ilerFlags,            |                       |
        |                       |                   Pat |                       |
        |                       | ternMatchedCollection |                       |
        |                       | <com.google.common.co |                       |
        |                       | llect.ImmutableList<S |                       |
        |                       | tringWithMacros>> pla |                       |
        |                       | tformCompilerFlags,   |                       |
        |                       |                       |                       |
        |                       |       com.google.comm |                       |
        |                       | on.collect.ImmutableM |                       |
        |                       | ap<CxxSource.Type,​Pat |                       |
        |                       | ternMatchedCollection |                       |
        |                       | <com.google.common.co |                       |
        |                       | llect.ImmutableList<S |                       |
        |                       | tringWithMacros>>> la |                       |
        |                       | ngPlatformCompilerFla |                       |
        |                       | gs,                   |                       |
        |                       |            Optional<S |                       |
        |                       | ourcePath> prefixHead |                       |
        |                       | er,                   |                       |
        |                       |            Optional<S |                       |
        |                       | ourcePath> precompile |                       |
        |                       | dHeader,              |                       |
        |                       |                 com.g |                       |
        |                       | oogle.common.collect. |                       |
        |                       | ImmutableList<StringW |                       |
        |                       | ithMacros> linkerFlag |                       |
        |                       | s,                    |                       |
        |                       |           com.google. |                       |
        |                       | common.collect.Immuta |                       |
        |                       | bleList<String> linke |                       |
        |                       | rExtraOutputs,        |                       |
        |                       |                       |                       |
        |                       |  PatternMatchedCollec |                       |
        |                       | tion<com.google.commo |                       |
        |                       | n.collect.ImmutableLi |                       |
        |                       | st<StringWithMacros>> |                       |
        |                       |  platformLinkerFlags, |                       |
        |                       |                       |                       |
        |                       |         Optional<Link |                       |
        |                       | er.CxxRuntimeType> cx |                       |
        |                       | xRuntimeType,         |                       |
        |                       |                       |                       |
        |                       | com.google.common.col |                       |
        |                       | lect.ImmutableSortedS |                       |
        |                       | et<SourcePath> rawHea |                       |
        |                       | ders,                 |                       |
        |                       |              com.goog |                       |
        |                       | le.common.collect.Imm |                       |
        |                       | utableSortedSet<Strin |                       |
        |                       | g> includeDirectories |                       |
        |                       | ,                     |                       |
        |                       |          Optional<Str |                       |
        |                       | ing> outputRootName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Cx            | `                     |                       |
        | xLinkAndCompileRules` | createBuildRulesForCx |                       |
        |                       | xBinaryDescriptionArg |                       |
        |                       | ​(TargetGraph targetGr |                       |
        |                       | aph,                  |                       |
        |                       |                       |                       |
        |                       |      BuildTarget targ |                       |
        |                       | et,                   |                       |
        |                       |                       |                       |
        |                       |     ProjectFilesystem |                       |
        |                       |  projectFilesystem,   |                       |
        |                       |                       |                       |
        |                       |                     A |                       |
        |                       | ctionGraphBuilder gra |                       |
        |                       | phBuilder,            |                       |
        |                       |                       |                       |
        |                       |            CellPathRe |                       |
        |                       | solver cellRoots,     |                       |
        |                       |                       |                       |
        |                       |                   Cxx |                       |
        |                       | BuckConfig cxxBuckCon |                       |
        |                       | fig,                  |                       |
        |                       |                       |                       |
        |                       |      CxxPlatform cxxP |                       |
        |                       | latform,              |                       |
        |                       |                       |                       |
        |                       |          CxxBinaryDes |                       |
        |                       | cription.CommonArg ar |                       |
        |                       | gs,                   |                       |
        |                       |                       |                       |
        |                       |     com.google.common |                       |
        |                       | .collect.ImmutableSet |                       |
        |                       | <BuildTarget> extraDe |                       |
        |                       | ps,                   |                       |
        |                       |                       |                       |
        |                       |     Optional<StripSty |                       |
        |                       | le> stripStyle,       |                       |
        |                       |                       |                       |
        |                       |                 Optio |                       |
        |                       | nal<LinkerMapMode> fl |                       |
        |                       | avoredLinkerMapMode)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Opti          | `crea                 |                       |
        | onal<com.facebook.buc | teCompilationDatabase |                       |
        | k.cxx.CxxCompilationD | Dependencies​(BuildTar |                       |
        | atabaseDependencies>` | get buildTarget,      |                       |
        |                       |                       |                       |
        |                       |             FlavorDom |                       |
        |                       | ain<?> platforms,     |                       |
        |                       |                       |                       |
        |                       |              ActionGr |                       |
        |                       | aphBuilder graphBuild |                       |
        |                       | er,                   |                       |
        |                       |                     c |                       |
        |                       | om.google.common.coll |                       |
        |                       | ect.ImmutableSortedSe |                       |
        |                       | t<BuildTarget> deps)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static BuildTarget`  | `c                    |                       |
        |                       | reateCxxLinkTarget​(Bu |                       |
        |                       | ildTarget target,     |                       |
        |                       |                 Optio |                       |
        |                       | nal<LinkerMapMode> fl |                       |
        |                       | avoredLinkerMapMode)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static CxxStrip`     | `                     |                       |
        |                       | createCxxStripRule​(Bu |                       |
        |                       | ildTarget baseBuildTa |                       |
        |                       | rget,                 |                       |
        |                       |    ProjectFilesystem  |                       |
        |                       | projectFilesystem,    |                       |
        |                       |                 Actio |                       |
        |                       | nGraphBuilder graphBu |                       |
        |                       | ilder,                |                       |
        |                       |     StripStyle stripS |                       |
        |                       | tyle,                 |                       |
        |                       |    boolean isCacheabl |                       |
        |                       | e,                    |                       |
        |                       | BuildRule unstrippedB |                       |
        |                       | inaryRule,            |                       |
        |                       |         CxxPlatform c |                       |
        |                       | xxPlatform,           |                       |
        |                       |          Optional<Str |                       |
        |                       | ing> outputRootName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `createHeaderSym      |                       |
        | ic HeaderSymlinkTree` | linkTree​(BuildTarget  |                       |
        |                       | buildTarget,          |                       |
        |                       |                Projec |                       |
        |                       | tFilesystem projectFi |                       |
        |                       | lesystem,             |                       |
        |                       |             BuildRule |                       |
        |                       | Resolver resolver,    |                       |
        |                       |                       |                       |
        |                       | CxxPlatform cxxPlatfo |                       |
        |                       | rm,                   |                       |
        |                       |       com.google.comm |                       |
        |                       | on.collect.ImmutableM |                       |
        |                       | ap<Path,​SourcePath> h |                       |
        |                       | eaders,               |                       |
        |                       |           HeaderVisib |                       |
        |                       | ility headerVisibilit |                       |
        |                       | y,                    |                       |
        |                       |      boolean shouldCr |                       |
        |                       | eateHeadersSymlinks)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `c                    |                       |
        | ic HeaderSymlinkTree` | reateHeaderSymlinkTre |                       |
        |                       | e​(BuildTarget buildTa |                       |
        |                       | rget,                 |                       |
        |                       |         ProjectFilesy |                       |
        |                       | stem projectFilesyste |                       |
        |                       | m,                    |                       |
        |                       |      HeaderMode mode, |                       |
        |                       |                       |                       |
        |                       |    com.google.common. |                       |
        |                       | collect.ImmutableMap< |                       |
        |                       | Path,​SourcePath> head |                       |
        |                       | ers,                  |                       |
        |                       |        HeaderVisibili |                       |
        |                       | ty headerVisibility,  |                       |
        |                       |                       |                       |
        |                       |   Flavor... flavors)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static BuildTarget`  | `createHeaderSym      |                       |
        |                       | linkTreeTarget​(BuildT |                       |
        |                       | arget target,         |                       |
        |                       |                       |                       |
        |                       |  HeaderVisibility hea |                       |
        |                       | derVisibility,        |                       |
        |                       |                       |                       |
        |                       |   Flavor... flavors)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static BuildRule`    | `c                    |                       |
        |                       | reateLinkMap​(BuildTar |                       |
        |                       | get target,           |                       |
        |                       |     ProjectFilesystem |                       |
        |                       |  projectFilesystem,   |                       |
        |                       |             SourcePat |                       |
        |                       | hRuleFinder ruleFinde |                       |
        |                       | r,              CxxLi |                       |
        |                       | nkAndCompileRules cxx |                       |
        |                       | LinkAndCompileRules)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static BuildTarget`  | `createS              |                       |
        |                       | haredLibraryBuildTarg |                       |
        |                       | et​(BuildTarget target |                       |
        |                       | ,                     |                       |
        |                       |            Flavor pla |                       |
        |                       | tform,                |                       |
        |                       |                 Linke |                       |
        |                       | r.LinkType linkType)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `createSharedLi       | ::: block             |
        | ic MappedSymlinkTree` | brarySymlinkTree​(Buil | Build a               |
        |                       | dTarget baseBuildTarg | [`HeaderSymlin        |
        |                       | et,                   | kTree`](toolchain/Hea |
        |                       |              ProjectF | derSymlinkTree.html " |
        |                       | ilesystem filesystem, | class in com.facebook |
        |                       |                       | .buck.cxx.toolchain") |
        |                       |           ActionGraph | of all the shared     |
        |                       | Builder graphBuilder, | libraries found via   |
        |                       |                       | the top-level rule\'s |
        |                       |           CxxPlatform | transitive            |
        |                       |  cxxPlatform,         | dependencies.         |
        |                       |                       | :::                   |
        |                       |   Iterable<? extends  |                       |
        |                       | BuildRule> deps,      |                       |
        |                       |                       |                       |
        |                       |      java.util.functi |                       |
        |                       | on.Function<? super B |                       |
        |                       | uildRule,​Optional<Ite |                       |
        |                       | rable<? extends Build |                       |
        |                       | Rule>>> passthrough)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static BuildTarget`  | `creat                |                       |
        |                       | eSharedLibrarySymlink |                       |
        |                       | TreeTarget​(BuildTarge |                       |
        |                       | t target,             |                       |
        |                       |                       |                       |
        |                       |     Flavor platform)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static BuildTarget`  | `createStaticLib      |                       |
        |                       | raryBuildTarget​(Build |                       |
        |                       | Target target,        |                       |
        |                       |                       |                       |
        |                       |    Flavor platform,   |                       |
        |                       |                       |                       |
        |                       |         PicType pic)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static BuildRule`    | `createUberCompi      |                       |
        |                       | lationDatabase​(BuildT |                       |
        |                       | arget buildTarget,    |                       |
        |                       |                       |                       |
        |                       |       ProjectFilesyst |                       |
        |                       | em projectFilesystem, |                       |
        |                       |                       |                       |
        |                       |          ActionGraphB |                       |
        |                       | uilder graphBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Flavor`       | `fl                   |                       |
        |                       | avorForLinkableDepTyp |                       |
        |                       | e​(Linker.LinkableDepT |                       |
        |                       | ype linkableDepType)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `framewo              |                       |
        | AddsToRuleKeyFunction | rkPathToSearchPath​(Cx |                       |
        | <FrameworkPath,​Path>` | xPlatform cxxPlatform |                       |
        |                       | ,                     |                       |
        |                       |       SourcePathResol |                       |
        |                       | verAdapter resolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `getDefaultSharedLibr | ::: block             |
        |                       | arySoname​(BuildTarget | Default shared        |
        |                       |  target,              | library soname for a  |
        |                       |                  CxxP | target                |
        |                       | latform platform,     | :::                   |
        |                       |                       |                       |
        |                       |      ProjectFilesyste |                       |
        |                       | m projectFilesystem)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static HeaderMode`   | `getHeaderModeForPl   |                       |
        |                       | atform​(BuildRuleResol |                       |
        |                       | ver resolver,         |                       |
        |                       |                  Targ |                       |
        |                       | etConfiguration targe |                       |
        |                       | tConfiguration,       |                       |
        |                       |                    Cx |                       |
        |                       | xPlatform cxxPlatform |                       |
        |                       | ,                     |                       |
        |                       |      boolean shouldCr |                       |
        |                       | eateHeadersSymlinks)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Flavor`       | `getHeaderSymlinkTree |                       |
        |                       | Flavor​(HeaderVisibili |                       |
        |                       | ty headerVisibility)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Path`         | `getHeaderSym         |                       |
        |                       | linkTreePath​(ProjectF |                       |
        |                       | ilesystem filesystem, |                       |
        |                       |                       |                       |
        |                       |     BuildTarget targe |                       |
        |                       | t,                    |                       |
        |                       |       HeaderVisibilit |                       |
        |                       | y headerVisibility,   |                       |
        |                       |                       |                       |
        |                       |   Flavor... flavors)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Path`         | `getSharedLibr        |                       |
        |                       | aryPath​(ProjectFilesy |                       |
        |                       | stem filesystem,      |                       |
        |                       |                 Build |                       |
        |                       | Target sharedLibraryT |                       |
        |                       | arget,                |                       |
        |                       |       String soname)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `getSharedLib         |                       |
        |                       | rarySoname​(Optional<S |                       |
        |                       | tring> declaredSoname |                       |
        |                       | ,                     |                       |
        |                       |    BuildTarget target |                       |
        |                       | ,                     |                       |
        |                       |    CxxPlatform platfo |                       |
        |                       | rm,                   |                       |
        |                       |      ProjectFilesyste |                       |
        |                       | m projectFilesystem)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Path`         | `getSharedLibra       |                       |
        |                       | rySymlinkTreePath​(Pro |                       |
        |                       | jectFilesystem filesy |                       |
        |                       | stem,                 |                       |
        |                       |                 Build |                       |
        |                       | Target target,        |                       |
        |                       |                       |                       |
        |                       |     Flavor platform)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `getStaticLibrary     |                       |
        |                       | Basename​(BuildTarget  |                       |
        |                       | target,               |                       |
        |                       |            String suf |                       |
        |                       | fix,                  |                       |
        |                       |         boolean uniqu |                       |
        |                       | eLibraryNameEnabled)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `getS                 |                       |
        |                       | taticLibraryName​(Buil |                       |
        |                       | dTarget target,       |                       |
        |                       |                Option |                       |
        |                       | al<String> staticLibr |                       |
        |                       | aryBasename,          |                       |
        |                       |             String ex |                       |
        |                       | tension,              |                       |
        |                       |         boolean uniqu |                       |
        |                       | eLibraryNameEnabled)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `getStaticLibraryNa   | ::: block             |
        |                       | me​(BuildTarget target | Returns static        |
        |                       | ,                     | library name          |
        |                       |  Optional<String> sta | :::                   |
        |                       | ticLibraryBasename,   |                       |
        |                       |                    St |                       |
        |                       | ring extension,       |                       |
        |                       |                String |                       |
        |                       |  suffix,              |                       |
        |                       |         boolean uniqu |                       |
        |                       | eLibraryNameEnabled)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Strin         | `getStringWi          |                       |
        | gWithMacrosConverter` | thMacrosArgsConverter |                       |
        |                       | ​(BuildTarget target,  |                       |
        |                       |                       |                       |
        |                       |            CellPathRe |                       |
        |                       | solver cellPathResolv |                       |
        |                       | er,                   |                       |
        |                       |                Action |                       |
        |                       | GraphBuilder graphBui |                       |
        |                       | lder,                 |                       |
        |                       |                  CxxP |                       |
        |                       | latform cxxPlatform)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `normalizeModuleNam   |                       |
        |                       | e​(String moduleName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `s                    | `                     |                       |
        | tatic com.google.comm | parseCxxSources​(Build |                       |
        | on.collect.ImmutableM | Target buildTarget,   |                       |
        | ap<String,​CxxSource>` |               ActionG |                       |
        |                       | raphBuilder graphBuil |                       |
        |                       | der,                C |                       |
        |                       | xxPlatform cxxPlatfor |                       |
        |                       | m,                Cxx |                       |
        |                       | ConstructorArg args)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `s                    | `parseCxxSource       |                       |
        | tatic com.google.comm | s​(BuildTarget buildTa |                       |
        | on.collect.ImmutableM | rget,                 |                       |
        | ap<String,​CxxSource>` | ActionGraphBuilder gr |                       |
        |                       | aphBuilder,           |                       |
        |                       |       CxxPlatform cxx |                       |
        |                       | Platform,             |                       |
        |                       |     com.google.common |                       |
        |                       | .collect.ImmutableSor |                       |
        |                       | tedSet<SourceWithFlag |                       |
        |                       | s> srcs,              |                       |
        |                       |    PatternMatchedColl |                       |
        |                       | ection<com.google.com |                       |
        |                       | mon.collect.Immutable |                       |
        |                       | SortedSet<SourceWithF |                       |
        |                       | lags>> platformSrcs)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `parseExportedHead    |                       |
        | static com.google.com | ers​(BuildTarget build |                       |
        | mon.collect.Immutable | Target,               |                       |
        | Map<Path,​SourcePath>` |        ActionGraphBui |                       |
        |                       | lder graphBuilder,    |                       |
        |                       |                   Pro |                       |
        |                       | jectFilesystem projec |                       |
        |                       | tFilesystem,          |                       |
        |                       |             Optional< |                       |
        |                       | CxxPlatform> cxxPlatf |                       |
        |                       | orm,                  |                       |
        |                       |     CxxLibraryDescrip |                       |
        |                       | tion.CommonArg args)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `parse                |                       |
        | static com.google.com | ExportedPlatformHeade |                       |
        | mon.collect.Immutable | rs​(BuildTarget buildT |                       |
        | Map<Path,​SourcePath>` | arget,                |                       |
        |                       |               ActionG |                       |
        |                       | raphBuilder graphBuil |                       |
        |                       | der,                  |                       |
        |                       |             ProjectFi |                       |
        |                       | lesystem projectFiles |                       |
        |                       | ystem,                |                       |
        |                       |               CxxPlat |                       |
        |                       | form cxxPlatform,     |                       |
        |                       |                       |                       |
        |                       |     CxxLibraryDescrip |                       |
        |                       | tion.CommonArg args)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `parse                |                       |
        | static com.google.com | Headers​(BuildTarget b |                       |
        | mon.collect.Immutable | uildTarget,           |                       |
        | Map<Path,​SourcePath>` |    ActionGraphBuilder |                       |
        |                       |  graphBuilder,        |                       |
        |                       |       ProjectFilesyst |                       |
        |                       | em projectFilesystem, |                       |
        |                       |              Optional |                       |
        |                       | <CxxPlatform> cxxPlat |                       |
        |                       | form,             Cxx |                       |
        |                       | ConstructorArg args)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `requir               |                       |
        | ic HeaderSymlinkTree` | eHeaderSymlinkTree​(Bu |                       |
        |                       | ildTarget buildTarget |                       |
        |                       | ,                     |                       |
        |                       |      ProjectFilesyste |                       |
        |                       | m projectFilesystem,  |                       |
        |                       |                       |                       |
        |                       |    ActionGraphBuilder |                       |
        |                       |  graphBuilder,        |                       |
        |                       |                   Cxx |                       |
        |                       | Platform cxxPlatform, |                       |
        |                       |                       |                       |
        |                       |     com.google.common |                       |
        |                       | .collect.ImmutableMap |                       |
        |                       | <Path,​SourcePath> hea |                       |
        |                       | ders,                 |                       |
        |                       |          HeaderVisibi |                       |
        |                       | lity headerVisibility |                       |
        |                       | ,                     |                       |
        |                       |      boolean shouldCr |                       |
        |                       | eateHeadersSymlinks)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `requireShar          |                       |
        | ic MappedSymlinkTree` | edLibrarySymlinkTree​( |                       |
        |                       | BuildTarget buildTarg |                       |
        |                       | et,                   |                       |
        |                       |               Project |                       |
        |                       | Filesystem filesystem |                       |
        |                       | ,                     |                       |
        |                       |             ActionGra |                       |
        |                       | phBuilder graphBuilde |                       |
        |                       | r,                    |                       |
        |                       |              CxxPlatf |                       |
        |                       | orm cxxPlatform,      |                       |
        |                       |                       |                       |
        |                       |       Iterable<? exte |                       |
        |                       | nds BuildRule> deps)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#INCREMENTAL_THINLTO}

        -   #### INCREMENTAL_THINLTO

                public static final Flavor INCREMENTAL_THINLTO

        []{#HEADER_SYMLINK_TREE_FLAVOR}

        -   #### HEADER_SYMLINK_TREE_FLAVOR

                public static final Flavor HEADER_SYMLINK_TREE_FLAVOR

        []{#EXPORTED_HEADER_SYMLINK_TREE_FLAVOR}

        -   #### EXPORTED_HEADER_SYMLINK_TREE_FLAVOR

                public static final Flavor EXPORTED_HEADER_SYMLINK_TREE_FLAVOR

        []{#STATIC_FLAVOR}

        -   #### STATIC_FLAVOR

                public static final Flavor STATIC_FLAVOR

        []{#STATIC_PIC_FLAVOR}

        -   #### STATIC_PIC_FLAVOR

                public static final Flavor STATIC_PIC_FLAVOR

        []{#SHARED_FLAVOR}

        -   #### SHARED_FLAVOR

                public static final Flavor SHARED_FLAVOR

        []{#SHARED_INTERFACE_FLAVOR}

        -   #### SHARED_INTERFACE_FLAVOR

                public static final Flavor SHARED_INTERFACE_FLAVOR

        []{#MACH_O_BUNDLE_FLAVOR}

        -   #### MACH_O\_BUNDLE_FLAVOR

                public static final Flavor MACH_O_BUNDLE_FLAVOR

        []{#SHARED_LIBRARY_SYMLINK_TREE_FLAVOR}

        -   #### SHARED_LIBRARY_SYMLINK_TREE_FLAVOR

                public static final Flavor SHARED_LIBRARY_SYMLINK_TREE_FLAVOR

        []{#BINARY_WITH_SHARED_LIBRARIES_SYMLINK_TREE_FLAVOR}

        -   #### BINARY_WITH_SHARED_LIBRARIES_SYMLINK_TREE_FLAVOR

                public static final Flavor BINARY_WITH_SHARED_LIBRARIES_SYMLINK_TREE_FLAVOR

        []{#CXX_LINK_BINARY_FLAVOR}

        -   #### CXX_LINK_BINARY_FLAVOR

                public static final Flavor CXX_LINK_BINARY_FLAVOR

        []{#CXX_LINK_THININDEX_FLAVOR}

        -   #### CXX_LINK_THININDEX_FLAVOR

                public static final Flavor CXX_LINK_THININDEX_FLAVOR

        []{#CXX_LINK_MAP_FLAVOR}

        -   #### CXX_LINK_MAP_FLAVOR

                public static final Flavor CXX_LINK_MAP_FLAVOR
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getHeaderModeForPlatform(com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.cxx.toolchain.CxxPlatform,boolean)}

        -   #### getHeaderModeForPlatform

            ``` methodSignature
            public static HeaderMode getHeaderModeForPlatform​(BuildRuleResolver resolver,
                                                              TargetConfiguration targetConfiguration,
                                                              CxxPlatform cxxPlatform,
                                                              boolean shouldCreateHeadersSymlinks)
            ```

        []{#createHeaderSymlinkTree(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.cxx.toolchain.HeaderMode,com.google.common.collect.ImmutableMap,com.facebook.buck.cxx.toolchain.HeaderVisibility,com.facebook.buck.core.model.Flavor...)}

        -   #### createHeaderSymlinkTree

            ``` methodSignature
            public static HeaderSymlinkTree createHeaderSymlinkTree​(BuildTarget buildTarget,
                                                                    ProjectFilesystem projectFilesystem,
                                                                    HeaderMode mode,
                                                                    com.google.common.collect.ImmutableMap<Path,​SourcePath> headers,
                                                                    HeaderVisibility headerVisibility,
                                                                    Flavor... flavors)
            ```

        []{#createHeaderSymlinkTree(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.cxx.toolchain.CxxPlatform,com.google.common.collect.ImmutableMap,com.facebook.buck.cxx.toolchain.HeaderVisibility,boolean)}

        -   #### createHeaderSymlinkTree

            ``` methodSignature
            public static HeaderSymlinkTree createHeaderSymlinkTree​(BuildTarget buildTarget,
                                                                    ProjectFilesystem projectFilesystem,
                                                                    BuildRuleResolver resolver,
                                                                    CxxPlatform cxxPlatform,
                                                                    com.google.common.collect.ImmutableMap<Path,​SourcePath> headers,
                                                                    HeaderVisibility headerVisibility,
                                                                    boolean shouldCreateHeadersSymlinks)
            ```

        []{#requireHeaderSymlinkTree(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.cxx.toolchain.CxxPlatform,com.google.common.collect.ImmutableMap,com.facebook.buck.cxx.toolchain.HeaderVisibility,boolean)}

        -   #### requireHeaderSymlinkTree

            ``` methodSignature
            public static HeaderSymlinkTree requireHeaderSymlinkTree​(BuildTarget buildTarget,
                                                                     ProjectFilesystem projectFilesystem,
                                                                     ActionGraphBuilder graphBuilder,
                                                                     CxxPlatform cxxPlatform,
                                                                     com.google.common.collect.ImmutableMap<Path,​SourcePath> headers,
                                                                     HeaderVisibility headerVisibility,
                                                                     boolean shouldCreateHeadersSymlinks)
            ```

        []{#createHeaderSymlinkTreeTarget(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.cxx.toolchain.HeaderVisibility,com.facebook.buck.core.model.Flavor...)}

        -   #### createHeaderSymlinkTreeTarget

            ``` methodSignature
            public static BuildTarget createHeaderSymlinkTreeTarget​(BuildTarget target,
                                                                    HeaderVisibility headerVisibility,
                                                                    Flavor... flavors)
            ```

            [Returns:]{.returnLabel}
            :   the
                [`BuildTarget`](../core/model/BuildTarget.html "class in com.facebook.buck.core.model")
                to use for the
                [`BuildRule`](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
                generating the symlink tree of headers.

        []{#getHeaderSymlinkTreePath(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.cxx.toolchain.HeaderVisibility,com.facebook.buck.core.model.Flavor...)}

        -   #### getHeaderSymlinkTreePath

            ``` methodSignature
            public static Path getHeaderSymlinkTreePath​(ProjectFilesystem filesystem,
                                                        BuildTarget target,
                                                        HeaderVisibility headerVisibility,
                                                        Flavor... flavors)
            ```

            [Returns:]{.returnLabel}
            :   the absolute
                [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
                to use for the symlink tree of headers.

        []{#getHeaderSymlinkTreeFlavor(com.facebook.buck.cxx.toolchain.HeaderVisibility)}

        -   #### getHeaderSymlinkTreeFlavor

            ``` methodSignature
            public static Flavor getHeaderSymlinkTreeFlavor​(HeaderVisibility headerVisibility)
            ```

        []{#parseHeaders(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.io.filesystem.ProjectFilesystem,java.util.Optional,com.facebook.buck.cxx.CxxConstructorArg)}

        -   #### parseHeaders

            ``` methodSignature
            public static com.google.common.collect.ImmutableMap<Path,​SourcePath> parseHeaders​(BuildTarget buildTarget,
                                                                                                     ActionGraphBuilder graphBuilder,
                                                                                                     ProjectFilesystem projectFilesystem,
                                                                                                     Optional<CxxPlatform> cxxPlatform,
                                                                                                     CxxConstructorArg args)
            ```

            [Returns:]{.returnLabel}
            :   a map of header locations to input
                [`SourcePath`](../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
                objects formed by parsing the input
                [`SourcePath`](../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
                objects for the \"headers\" parameter.

        []{#parseExportedHeaders(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.io.filesystem.ProjectFilesystem,java.util.Optional,com.facebook.buck.cxx.CxxLibraryDescription.CommonArg)}

        -   #### parseExportedHeaders

            ``` methodSignature
            public static com.google.common.collect.ImmutableMap<Path,​SourcePath> parseExportedHeaders​(BuildTarget buildTarget,
                                                                                                             ActionGraphBuilder graphBuilder,
                                                                                                             ProjectFilesystem projectFilesystem,
                                                                                                             Optional<CxxPlatform> cxxPlatform,
                                                                                                             CxxLibraryDescription.CommonArg args)
            ```

            [Returns:]{.returnLabel}
            :   a map of header locations to input
                [`SourcePath`](../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
                objects formed by parsing the input
                [`SourcePath`](../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
                objects for the \"exportedHeaders\" parameter.

        []{#parseExportedPlatformHeaders(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.cxx.CxxLibraryDescription.CommonArg)}

        -   #### parseExportedPlatformHeaders

            ``` methodSignature
            public static com.google.common.collect.ImmutableMap<Path,​SourcePath> parseExportedPlatformHeaders​(BuildTarget buildTarget,
                                                                                                                     ActionGraphBuilder graphBuilder,
                                                                                                                     ProjectFilesystem projectFilesystem,
                                                                                                                     CxxPlatform cxxPlatform,
                                                                                                                     CxxLibraryDescription.CommonArg args)
            ```

            [Returns:]{.returnLabel}
            :   a map of header locations to input
                [`SourcePath`](../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
                objects formed by parsing the input
                [`SourcePath`](../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
                objects for the \"exportedHeaders\" parameter.

        []{#parseCxxSources(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.cxx.CxxConstructorArg)}

        -   #### parseCxxSources

            ``` methodSignature
            public static com.google.common.collect.ImmutableMap<String,​CxxSource> parseCxxSources​(BuildTarget buildTarget,
                                                                                                         ActionGraphBuilder graphBuilder,
                                                                                                         CxxPlatform cxxPlatform,
                                                                                                         CxxConstructorArg args)
            ```

            [Returns:]{.returnLabel}
            :   a list
                [`CxxSource`](CxxSource.html "class in com.facebook.buck.cxx")
                objects formed by parsing the input
                [`SourcePath`](../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
                objects for the \"srcs\" parameter.

        []{#parseCxxSources(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.cxx.toolchain.CxxPlatform,com.google.common.collect.ImmutableSortedSet,com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### parseCxxSources

            ``` methodSignature
            public static com.google.common.collect.ImmutableMap<String,​CxxSource> parseCxxSources​(BuildTarget buildTarget,
                                                                                                         ActionGraphBuilder graphBuilder,
                                                                                                         CxxPlatform cxxPlatform,
                                                                                                         com.google.common.collect.ImmutableSortedSet<SourceWithFlags> srcs,
                                                                                                         PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<SourceWithFlags>> platformSrcs)
            ```

        []{#collectCxxPreprocessorInput(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder,java.lang.Iterable,com.google.common.collect.ImmutableMultimap,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableSet,java.lang.Iterable,com.google.common.collect.ImmutableSortedSet,com.google.common.collect.ImmutableSortedSet,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### collectCxxPreprocessorInput

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<CxxPreprocessorInput> collectCxxPreprocessorInput​(BuildTarget target,
                                                                                                                    CxxPlatform cxxPlatform,
                                                                                                                    ActionGraphBuilder graphBuilder,
                                                                                                                    Iterable<BuildRule> deps,
                                                                                                                    com.google.common.collect.ImmutableMultimap<CxxSource.Type,​? extends Arg> preprocessorFlags,
                                                                                                                    com.google.common.collect.ImmutableList<HeaderSymlinkTree> headerSymlinkTrees,
                                                                                                                    com.google.common.collect.ImmutableSet<FrameworkPath> frameworks,
                                                                                                                    Iterable<CxxPreprocessorInput> cxxPreprocessorInputFromDeps,
                                                                                                                    com.google.common.collect.ImmutableSortedSet<SourcePath> rawHeaders,
                                                                                                                    com.google.common.collect.ImmutableSortedSet<String> includeDirectories,
                                                                                                                    ProjectFilesystem projectFilesystem)
            ```

        []{#createStaticLibraryBuildTarget(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.model.Flavor,com.facebook.buck.cxx.toolchain.PicType)}

        -   #### createStaticLibraryBuildTarget

            ``` methodSignature
            public static BuildTarget createStaticLibraryBuildTarget​(BuildTarget target,
                                                                     Flavor platform,
                                                                     PicType pic)
            ```

        []{#createSharedLibraryBuildTarget(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.model.Flavor,com.facebook.buck.cxx.toolchain.linker.Linker.LinkType)}

        -   #### createSharedLibraryBuildTarget

            ``` methodSignature
            public static BuildTarget createSharedLibraryBuildTarget​(BuildTarget target,
                                                                     Flavor platform,
                                                                     Linker.LinkType linkType)
            ```

        []{#getStaticLibraryName(com.facebook.buck.core.model.BuildTarget,java.util.Optional,java.lang.String,boolean)}

        -   #### getStaticLibraryName

            ``` methodSignature
            public static String getStaticLibraryName​(BuildTarget target,
                                                      Optional<String> staticLibraryBasename,
                                                      String extension,
                                                      boolean uniqueLibraryNameEnabled)
            ```

        []{#getStaticLibraryBasename(com.facebook.buck.core.model.BuildTarget,java.lang.String,boolean)}

        -   #### getStaticLibraryBasename

            ``` methodSignature
            public static String getStaticLibraryBasename​(BuildTarget target,
                                                          String suffix,
                                                          boolean uniqueLibraryNameEnabled)
            ```

        []{#getStaticLibraryName(com.facebook.buck.core.model.BuildTarget,java.util.Optional,java.lang.String,java.lang.String,boolean)}

        -   #### getStaticLibraryName

            ``` methodSignature
            public static String getStaticLibraryName​(BuildTarget target,
                                                      Optional<String> staticLibraryBasename,
                                                      String extension,
                                                      String suffix,
                                                      boolean uniqueLibraryNameEnabled)
            ```

            ::: block
            Returns static library name
            :::

        []{#getSharedLibrarySoname(java.util.Optional,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### getSharedLibrarySoname

            ``` methodSignature
            public static String getSharedLibrarySoname​(Optional<String> declaredSoname,
                                                        BuildTarget target,
                                                        CxxPlatform platform,
                                                        ProjectFilesystem projectFilesystem)
            ```

        []{#getDefaultSharedLibrarySoname(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### getDefaultSharedLibrarySoname

            ``` methodSignature
            public static String getDefaultSharedLibrarySoname​(BuildTarget target,
                                                               CxxPlatform platform,
                                                               ProjectFilesystem projectFilesystem)
            ```

            ::: block
            Default shared library soname for a target
            :::

        []{#getSharedLibraryPath(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget,java.lang.String)}

        -   #### getSharedLibraryPath

            ``` methodSignature
            public static Path getSharedLibraryPath​(ProjectFilesystem filesystem,
                                                    BuildTarget sharedLibraryTarget,
                                                    String soname)
            ```

        []{#createCxxLinkTarget(com.facebook.buck.core.model.BuildTarget,java.util.Optional)}

        -   #### createCxxLinkTarget

            ``` methodSignature
            public static BuildTarget createCxxLinkTarget​(BuildTarget target,
                                                          Optional<LinkerMapMode> flavoredLinkerMapMode)
            ```

        []{#frameworkPathToSearchPath(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### frameworkPathToSearchPath

            ``` methodSignature
            public static AddsToRuleKeyFunction<FrameworkPath,​Path> frameworkPathToSearchPath​(CxxPlatform cxxPlatform,
                                                                                                    SourcePathResolverAdapter resolver)
            ```

            [Returns:]{.returnLabel}
            :   a function that transforms the
                [`FrameworkPath`](../rules/coercer/FrameworkPath.html "class in com.facebook.buck.rules.coercer")
                to search paths with any embedded macros expanded.

        []{#createBuildRuleForCxxThinLtoBinary(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.cell.CellPathResolver,com.facebook.buck.cxx.config.CxxBuckConfig,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.cxx.CxxBinaryDescription.CommonArg,com.google.common.collect.ImmutableSet,java.util.Optional,java.util.Optional)}

        -   #### createBuildRuleForCxxThinLtoBinary

            ``` methodSignature
            public static CxxLinkAndCompileRules createBuildRuleForCxxThinLtoBinary​(BuildTarget target,
                                                                                    ProjectFilesystem projectFilesystem,
                                                                                    ActionGraphBuilder graphBuilder,
                                                                                    CellPathResolver cellRoots,
                                                                                    CxxBuckConfig cxxBuckConfig,
                                                                                    CxxPlatform cxxPlatform,
                                                                                    CxxBinaryDescription.CommonArg args,
                                                                                    com.google.common.collect.ImmutableSet<BuildTarget> extraDeps,
                                                                                    Optional<StripStyle> stripStyle,
                                                                                    Optional<LinkerMapMode> flavoredLinkerMapMode)
            ```

        []{#createBuildRulesForCxxBinaryDescriptionArg(com.facebook.buck.core.model.targetgraph.TargetGraph,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.cell.CellPathResolver,com.facebook.buck.cxx.config.CxxBuckConfig,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.cxx.CxxBinaryDescription.CommonArg,com.google.common.collect.ImmutableSet,java.util.Optional,java.util.Optional)}

        -   #### createBuildRulesForCxxBinaryDescriptionArg

            ``` methodSignature
            public static CxxLinkAndCompileRules createBuildRulesForCxxBinaryDescriptionArg​(TargetGraph targetGraph,
                                                                                            BuildTarget target,
                                                                                            ProjectFilesystem projectFilesystem,
                                                                                            ActionGraphBuilder graphBuilder,
                                                                                            CellPathResolver cellRoots,
                                                                                            CxxBuckConfig cxxBuckConfig,
                                                                                            CxxPlatform cxxPlatform,
                                                                                            CxxBinaryDescription.CommonArg args,
                                                                                            com.google.common.collect.ImmutableSet<BuildTarget> extraDeps,
                                                                                            Optional<StripStyle> stripStyle,
                                                                                            Optional<LinkerMapMode> flavoredLinkerMapMode)
            ```

        []{#createBuildRulesForCxxBinary(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.cell.CellPathResolver,com.facebook.buck.cxx.config.CxxBuckConfig,com.facebook.buck.cxx.toolchain.CxxPlatform,com.google.common.collect.ImmutableMap,com.google.common.collect.ImmutableMap,java.util.SortedSet,com.google.common.collect.ImmutableSet,java.util.Optional,java.util.Optional,com.facebook.buck.cxx.toolchain.linker.Linker.LinkableDepType,java.util.Optional,com.facebook.buck.cxx.CxxLinkOptions,com.google.common.collect.ImmutableList,com.facebook.buck.rules.coercer.PatternMatchedCollection,com.google.common.collect.ImmutableMap,com.google.common.collect.ImmutableMap,com.google.common.collect.ImmutableSortedSet,com.google.common.collect.ImmutableSortedSet,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableMap,com.facebook.buck.rules.coercer.PatternMatchedCollection,com.google.common.collect.ImmutableMap,java.util.Optional,java.util.Optional,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableList,com.facebook.buck.rules.coercer.PatternMatchedCollection,java.util.Optional,com.google.common.collect.ImmutableSortedSet,com.google.common.collect.ImmutableSortedSet,java.util.Optional)}

        -   #### createBuildRulesForCxxBinary

            ``` methodSignature
            public static CxxLinkAndCompileRules createBuildRulesForCxxBinary​(BuildTarget target,
                                                                              ProjectFilesystem projectFilesystem,
                                                                              ActionGraphBuilder graphBuilder,
                                                                              CellPathResolver cellRoots,
                                                                              CxxBuckConfig cxxBuckConfig,
                                                                              CxxPlatform cxxPlatform,
                                                                              com.google.common.collect.ImmutableMap<String,​CxxSource> srcs,
                                                                              com.google.common.collect.ImmutableMap<Path,​SourcePath> headers,
                                                                              SortedSet<BuildRule> deps,
                                                                              com.google.common.collect.ImmutableSet<BuildTarget> linkWholeDeps,
                                                                              Optional<StripStyle> stripStyle,
                                                                              Optional<LinkerMapMode> flavoredLinkerMapMode,
                                                                              Linker.LinkableDepType linkStyle,
                                                                              Optional<LinkableListFilter> linkableListFilter,
                                                                              CxxLinkOptions linkOptions,
                                                                              com.google.common.collect.ImmutableList<StringWithMacros> preprocessorFlags,
                                                                              PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> platformPreprocessorFlags,
                                                                              com.google.common.collect.ImmutableMap<CxxSource.Type,​com.google.common.collect.ImmutableList<StringWithMacros>> langPreprocessorFlags,
                                                                              com.google.common.collect.ImmutableMap<CxxSource.Type,​PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> langPlatformPreprocessorFlags,
                                                                              com.google.common.collect.ImmutableSortedSet<FrameworkPath> frameworks,
                                                                              com.google.common.collect.ImmutableSortedSet<FrameworkPath> libraries,
                                                                              com.google.common.collect.ImmutableList<StringWithMacros> compilerFlags,
                                                                              com.google.common.collect.ImmutableMap<CxxSource.Type,​com.google.common.collect.ImmutableList<StringWithMacros>> langCompilerFlags,
                                                                              PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> platformCompilerFlags,
                                                                              com.google.common.collect.ImmutableMap<CxxSource.Type,​PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> langPlatformCompilerFlags,
                                                                              Optional<SourcePath> prefixHeader,
                                                                              Optional<SourcePath> precompiledHeader,
                                                                              com.google.common.collect.ImmutableList<StringWithMacros> linkerFlags,
                                                                              com.google.common.collect.ImmutableList<String> linkerExtraOutputs,
                                                                              PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> platformLinkerFlags,
                                                                              Optional<Linker.CxxRuntimeType> cxxRuntimeType,
                                                                              com.google.common.collect.ImmutableSortedSet<SourcePath> rawHeaders,
                                                                              com.google.common.collect.ImmutableSortedSet<String> includeDirectories,
                                                                              Optional<String> outputRootName)
            ```

        []{#createCxxStripRule(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.cxx.toolchain.StripStyle,boolean,com.facebook.buck.core.rules.BuildRule,com.facebook.buck.cxx.toolchain.CxxPlatform,java.util.Optional)}

        -   #### createCxxStripRule

            ``` methodSignature
            public static CxxStrip createCxxStripRule​(BuildTarget baseBuildTarget,
                                                      ProjectFilesystem projectFilesystem,
                                                      ActionGraphBuilder graphBuilder,
                                                      StripStyle stripStyle,
                                                      boolean isCacheable,
                                                      BuildRule unstrippedBinaryRule,
                                                      CxxPlatform cxxPlatform,
                                                      Optional<String> outputRootName)
            ```

        []{#createUberCompilationDatabase(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### createUberCompilationDatabase

            ``` methodSignature
            public static BuildRule createUberCompilationDatabase​(BuildTarget buildTarget,
                                                                  ProjectFilesystem projectFilesystem,
                                                                  ActionGraphBuilder graphBuilder)
            ```

        []{#createCompilationDatabaseDependencies(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.model.FlavorDomain,com.facebook.buck.core.rules.ActionGraphBuilder,com.google.common.collect.ImmutableSortedSet)}

        -   #### createCompilationDatabaseDependencies

            ``` methodSignature
            public static Optional<com.facebook.buck.cxx.CxxCompilationDatabaseDependencies> createCompilationDatabaseDependencies​(BuildTarget buildTarget,
                                                                                                                                   FlavorDomain<?> platforms,
                                                                                                                                   ActionGraphBuilder graphBuilder,
                                                                                                                                   com.google.common.collect.ImmutableSortedSet<BuildTarget> deps)
            ```

        []{#createSharedLibrarySymlinkTreeTarget(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.model.Flavor)}

        -   #### createSharedLibrarySymlinkTreeTarget

            ``` methodSignature
            public static BuildTarget createSharedLibrarySymlinkTreeTarget​(BuildTarget target,
                                                                           Flavor platform)
            ```

            [Returns:]{.returnLabel}
            :   the
                [`BuildTarget`](../core/model/BuildTarget.html "class in com.facebook.buck.core.model")
                to use for the
                [`BuildRule`](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
                generating the symlink tree of shared libraries.

        []{#getSharedLibrarySymlinkTreePath(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.model.Flavor)}

        -   #### getSharedLibrarySymlinkTreePath

            ``` methodSignature
            public static Path getSharedLibrarySymlinkTreePath​(ProjectFilesystem filesystem,
                                                               BuildTarget target,
                                                               Flavor platform)
            ```

            [Returns:]{.returnLabel}
            :   the
                [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
                to use for the symlink tree of headers.

        []{#createSharedLibrarySymlinkTree(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.cxx.toolchain.CxxPlatform,java.lang.Iterable,java.util.function.Function)}

        -   #### createSharedLibrarySymlinkTree

            ``` methodSignature
            public static MappedSymlinkTree createSharedLibrarySymlinkTree​(BuildTarget baseBuildTarget,
                                                                           ProjectFilesystem filesystem,
                                                                           ActionGraphBuilder graphBuilder,
                                                                           CxxPlatform cxxPlatform,
                                                                           Iterable<? extends BuildRule> deps,
                                                                           java.util.function.Function<? super BuildRule,​Optional<Iterable<? extends BuildRule>>> passthrough)
            ```

            ::: block
            Build a
            [`HeaderSymlinkTree`](toolchain/HeaderSymlinkTree.html "class in com.facebook.buck.cxx.toolchain")
            of all the shared libraries found via the top-level rule\'s
            transitive dependencies.
            :::

        []{#requireSharedLibrarySymlinkTree(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.cxx.toolchain.CxxPlatform,java.lang.Iterable)}

        -   #### requireSharedLibrarySymlinkTree

            ``` methodSignature
            public static MappedSymlinkTree requireSharedLibrarySymlinkTree​(BuildTarget buildTarget,
                                                                            ProjectFilesystem filesystem,
                                                                            ActionGraphBuilder graphBuilder,
                                                                            CxxPlatform cxxPlatform,
                                                                            Iterable<? extends BuildRule> deps)
            ```

        []{#flavorForLinkableDepType(com.facebook.buck.cxx.toolchain.linker.Linker.LinkableDepType)}

        -   #### flavorForLinkableDepType

            ``` methodSignature
            public static Flavor flavorForLinkableDepType​(Linker.LinkableDepType linkableDepType)
            ```

        []{#getStringWithMacrosArgsConverter(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.cell.CellPathResolver,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.cxx.toolchain.CxxPlatform)}

        -   #### getStringWithMacrosArgsConverter

            ``` methodSignature
            public static StringWithMacrosConverter getStringWithMacrosArgsConverter​(BuildTarget target,
                                                                                     CellPathResolver cellPathResolver,
                                                                                     ActionGraphBuilder graphBuilder,
                                                                                     CxxPlatform cxxPlatform)
            ```

            [Returns:]{.returnLabel}
            :   a
                [`StringWithMacrosConverter`](../rules/macros/StringWithMacrosConverter.html "class in com.facebook.buck.rules.macros")
                to use when converting C/C++ flags.

        []{#normalizeModuleName(java.lang.String)}

        -   #### normalizeModuleName

            ``` methodSignature
            public static String normalizeModuleName​(String moduleName)
            ```

        []{#createLinkMap(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.SourcePathRuleFinder,com.facebook.buck.cxx.CxxLinkAndCompileRules)}

        -   #### createLinkMap

            ``` methodSignature
            public static BuildRule createLinkMap​(BuildTarget target,
                                                  ProjectFilesystem projectFilesystem,
                                                  SourcePathRuleFinder ruleFinder,
                                                  CxxLinkAndCompileRules cxxLinkAndCompileRules)
            ```

            [Returns:]{.returnLabel}
            :   a
                [`BuildRule`](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
                that produces a single file that contains linker map
                produced during the linking process.

            [Throws:]{.throwsLabel}
            :   `HumanReadableException` - if the linked does not
                support linker maps.
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
-   Nested \| 
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
