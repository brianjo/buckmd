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
-   Field \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.cxx](package-summary.html)
:::

## Class CxxLinkableEnhancer {#class-cxxlinkableenhancer .title title="Class CxxLinkableEnhancer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.CxxLinkableEnhancer

::: description
-   

    ------------------------------------------------------------------------

        public class CxxLinkableEnhancer
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static CxxLink`      | `cr                   |                       |
        |                       | eateCxxLinkableBuildR |                       |
        |                       | ule​(CellPathResolver  |                       |
        |                       | cellPathResolver,     |                       |
        |                       |                       |                       |
        |                       |   CxxBuckConfig cxxBu |                       |
        |                       | ckConfig,             |                       |
        |                       |                CxxPla |                       |
        |                       | tform cxxPlatform,    |                       |
        |                       |                       |                       |
        |                       |    ProjectFilesystem  |                       |
        |                       | projectFilesystem,    |                       |
        |                       |                       |                       |
        |                       |    BuildRuleResolver  |                       |
        |                       | ruleResolver,         |                       |
        |                       |                    Bu |                       |
        |                       | ildTarget target,     |                       |
        |                       |                       |                       |
        |                       |   Path output,        |                       |
        |                       |                     c |                       |
        |                       | om.google.common.coll |                       |
        |                       | ect.ImmutableMap<Stri |                       |
        |                       | ng,​Path> extraOutputs |                       |
        |                       | ,                     |                       |
        |                       |        com.google.com |                       |
        |                       | mon.collect.Immutable |                       |
        |                       | List<Arg> args,       |                       |
        |                       |                       |                       |
        |                       | Linker.LinkableDepTyp |                       |
        |                       | e runtimeDepType,     |                       |
        |                       |                       |                       |
        |                       |   CxxLinkOptions link |                       |
        |                       | Options,              |                       |
        |                       |               Optiona |                       |
        |                       | l<LinkOutputPostproce |                       |
        |                       | ssor> postprocessor)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static CxxLink`      | `createCxxLinkableBu  | ::: block             |
        |                       | ildRule​(CxxBuckConfig | Construct a           |
        |                       |  cxxBuckConfig,       | [`CxxLink`](CxxL      |
        |                       |                       | ink.html "class in co |
        |                       | CxxPlatform cxxPlatfo | m.facebook.buck.cxx") |
        |                       | rm,                   | rule that builds a    |
        |                       |          ProjectFiles | native linkable from  |
        |                       | ystem projectFilesyst | top-level input       |
        |                       | em,                   | objects and a         |
        |                       |          ActionGraphB | dependency tree of    |
        |                       | uilder graphBuilder,  | [`                    |
        |                       |                       | NativeLinkableGroup`] |
        |                       |      BuildTarget targ | (toolchain/nativelink |
        |                       | et,                   | /NativeLinkableGroup. |
        |                       |          Linker.LinkT | html "interface in co |
        |                       | ype linkType,         | m.facebook.buck.cxx.t |
        |                       |                    Op | oolchain.nativelink") |
        |                       | tional<String> soname | dependencies.         |
        |                       | ,                     | :::                   |
        |                       |        Path output,   |                       |
        |                       |                       |                       |
        |                       |     com.google.common |                       |
        |                       | .collect.ImmutableLis |                       |
        |                       | t<String> extraOutput |                       |
        |                       | Names,                |                       |
        |                       |             Linker.Li |                       |
        |                       | nkableDepType depType |                       |
        |                       | ,                     |                       |
        |                       |        Optional<Linka |                       |
        |                       | bleListFilter> linkab |                       |
        |                       | leListFilter,         |                       |
        |                       |                    Cx |                       |
        |                       | xLinkOptions linkOpti |                       |
        |                       | ons,                  |                       |
        |                       |           Iterable<?  |                       |
        |                       | extends NativeLinkabl |                       |
        |                       | e> nativeLinkableDeps |                       |
        |                       | ,                     |                       |
        |                       |        Optional<Linke |                       |
        |                       | r.CxxRuntimeType> cxx |                       |
        |                       | RuntimeType,          |                       |
        |                       |                   Opt |                       |
        |                       | ional<SourcePath> bun |                       |
        |                       | dleLoader,            |                       |
        |                       |                 com.g |                       |
        |                       | oogle.common.collect. |                       |
        |                       | ImmutableSet<BuildTar |                       |
        |                       | get> blacklist,       |                       |
        |                       |                       |                       |
        |                       | com.google.common.col |                       |
        |                       | lect.ImmutableSet<Bui |                       |
        |                       | ldTarget> linkWholeDe |                       |
        |                       | ps,                   |                       |
        |                       |          NativeLinkab |                       |
        |                       | leInput immediateLink |                       |
        |                       | ableInput,            |                       |
        |                       |                 Optio |                       |
        |                       | nal<LinkOutputPostpro |                       |
        |                       | cessor> postprocessor |                       |
        |                       | ,                     |                       |
        |                       |        CellPathResolv |                       |
        |                       | er cellPathResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static CxxLink`      | `createCxxLink        |                       |
        |                       | ableSharedBuildRule​(C |                       |
        |                       | xxBuckConfig cxxBuckC |                       |
        |                       | onfig,                |                       |
        |                       |                   Cxx |                       |
        |                       | Platform cxxPlatform, |                       |
        |                       |                       |                       |
        |                       |             ProjectFi |                       |
        |                       | lesystem projectFiles |                       |
        |                       | ystem,                |                       |
        |                       |                   Bui |                       |
        |                       | ldRuleResolver ruleRe |                       |
        |                       | solver,               |                       |
        |                       |                    Bu |                       |
        |                       | ildTarget target,     |                       |
        |                       |                       |                       |
        |                       |         Path output,  |                       |
        |                       |                       |                       |
        |                       |            com.google |                       |
        |                       | .common.collect.Immut |                       |
        |                       | ableMap<String,​Path>  |                       |
        |                       | extraOutputs,         |                       |
        |                       |                       |                       |
        |                       |     Optional<String>  |                       |
        |                       | soname,               |                       |
        |                       |                    co |                       |
        |                       | m.google.common.colle |                       |
        |                       | ct.ImmutableList<? ex |                       |
        |                       | tends Arg> args,      |                       |
        |                       |                       |                       |
        |                       |        CellPathResolv |                       |
        |                       | er cellPathResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `cre                  | ::: block             |
        | atic CxxThinLTOIndex` | ateCxxThinLTOIndexBui | Generate build rule   |
        |                       | ldRule​(CxxBuckConfig  | for the indexing step |
        |                       | cxxBuckConfig,        | of an incremental     |
        |                       |                       | ThinLTO build         |
        |                       |    CxxPlatform cxxPla | :::                   |
        |                       | tform,                |                       |
        |                       |                 Proje |                       |
        |                       | ctFilesystem projectF |                       |
        |                       | ilesystem,            |                       |
        |                       |                     A |                       |
        |                       | ctionGraphBuilder gra |                       |
        |                       | phBuilder,            |                       |
        |                       |                     B |                       |
        |                       | uildTarget target,    |                       |
        |                       |                       |                       |
        |                       |        Path output,   |                       |
        |                       |                       |                       |
        |                       |         Linker.Linkab |                       |
        |                       | leDepType depType,    |                       |
        |                       |                       |                       |
        |                       |        Optional<Linka |                       |
        |                       | bleListFilter> linkab |                       |
        |                       | leListFilter,         |                       |
        |                       |                       |                       |
        |                       |   Iterable<? extends  |                       |
        |                       | NativeLinkable> nativ |                       |
        |                       | eLinkableDeps,        |                       |
        |                       |                       |                       |
        |                       |    Optional<Linker.Cx |                       |
        |                       | xRuntimeType> cxxRunt |                       |
        |                       | imeType,              |                       |
        |                       |                   com |                       |
        |                       | .google.common.collec |                       |
        |                       | t.ImmutableSet<BuildT |                       |
        |                       | arget> blacklist,     |                       |
        |                       |                       |                       |
        |                       |       com.google.comm |                       |
        |                       | on.collect.ImmutableS |                       |
        |                       | et<BuildTarget> linkW |                       |
        |                       | holeDeps,             |                       |
        |                       |                    Na |                       |
        |                       | tiveLinkableInput imm |                       |
        |                       | ediateLinkableInput)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com.google    | `derive               | ::: block             |
        | .common.collect.Immut | SupplementaryOutputPa | Derive supplementary  |
        | ableMap<String,​Path>` | thsFromMainOutputPath | output paths based on |
        |                       | ​(Path output,         | the main output path. |
        |                       |                       | :::                   |
        |                       |                     I |                       |
        |                       | terable<String> suppl |                       |
        |                       | ementaryOutputNames)` |                       |
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
    -   []{#method.detail}

        ### Method Detail

        []{#createCxxThinLTOIndexBuildRule(com.facebook.buck.cxx.config.CxxBuckConfig,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.model.BuildTarget,java.nio.file.Path,com.facebook.buck.cxx.toolchain.linker.Linker.LinkableDepType,java.util.Optional,java.lang.Iterable,java.util.Optional,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableSet,com.facebook.buck.cxx.toolchain.nativelink.NativeLinkableInput)}

        -   #### createCxxThinLTOIndexBuildRule

            ``` methodSignature
            public static CxxThinLTOIndex createCxxThinLTOIndexBuildRule​(CxxBuckConfig cxxBuckConfig,
                                                                         CxxPlatform cxxPlatform,
                                                                         ProjectFilesystem projectFilesystem,
                                                                         ActionGraphBuilder graphBuilder,
                                                                         BuildTarget target,
                                                                         Path output,
                                                                         Linker.LinkableDepType depType,
                                                                         Optional<LinkableListFilter> linkableListFilter,
                                                                         Iterable<? extends NativeLinkable> nativeLinkableDeps,
                                                                         Optional<Linker.CxxRuntimeType> cxxRuntimeType,
                                                                         com.google.common.collect.ImmutableSet<BuildTarget> blacklist,
                                                                         com.google.common.collect.ImmutableSet<BuildTarget> linkWholeDeps,
                                                                         NativeLinkableInput immediateLinkableInput)
            ```

            ::: block
            Generate build rule for the indexing step of an incremental
            ThinLTO build
            :::

        []{#createCxxLinkableBuildRule(com.facebook.buck.core.cell.CellPathResolver,com.facebook.buck.cxx.config.CxxBuckConfig,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.core.model.BuildTarget,java.nio.file.Path,com.google.common.collect.ImmutableMap,com.google.common.collect.ImmutableList,com.facebook.buck.cxx.toolchain.linker.Linker.LinkableDepType,com.facebook.buck.cxx.CxxLinkOptions,java.util.Optional)}

        -   #### createCxxLinkableBuildRule

            ``` methodSignature
            public static CxxLink createCxxLinkableBuildRule​(CellPathResolver cellPathResolver,
                                                             CxxBuckConfig cxxBuckConfig,
                                                             CxxPlatform cxxPlatform,
                                                             ProjectFilesystem projectFilesystem,
                                                             BuildRuleResolver ruleResolver,
                                                             BuildTarget target,
                                                             Path output,
                                                             com.google.common.collect.ImmutableMap<String,​Path> extraOutputs,
                                                             com.google.common.collect.ImmutableList<Arg> args,
                                                             Linker.LinkableDepType runtimeDepType,
                                                             CxxLinkOptions linkOptions,
                                                             Optional<LinkOutputPostprocessor> postprocessor)
            ```

        []{#createCxxLinkableBuildRule(com.facebook.buck.cxx.config.CxxBuckConfig,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.cxx.toolchain.linker.Linker.LinkType,java.util.Optional,java.nio.file.Path,com.google.common.collect.ImmutableList,com.facebook.buck.cxx.toolchain.linker.Linker.LinkableDepType,java.util.Optional,com.facebook.buck.cxx.CxxLinkOptions,java.lang.Iterable,java.util.Optional,java.util.Optional,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableSet,com.facebook.buck.cxx.toolchain.nativelink.NativeLinkableInput,java.util.Optional,com.facebook.buck.core.cell.CellPathResolver)}

        -   #### createCxxLinkableBuildRule

            ``` methodSignature
            public static CxxLink createCxxLinkableBuildRule​(CxxBuckConfig cxxBuckConfig,
                                                             CxxPlatform cxxPlatform,
                                                             ProjectFilesystem projectFilesystem,
                                                             ActionGraphBuilder graphBuilder,
                                                             BuildTarget target,
                                                             Linker.LinkType linkType,
                                                             Optional<String> soname,
                                                             Path output,
                                                             com.google.common.collect.ImmutableList<String> extraOutputNames,
                                                             Linker.LinkableDepType depType,
                                                             Optional<LinkableListFilter> linkableListFilter,
                                                             CxxLinkOptions linkOptions,
                                                             Iterable<? extends NativeLinkable> nativeLinkableDeps,
                                                             Optional<Linker.CxxRuntimeType> cxxRuntimeType,
                                                             Optional<SourcePath> bundleLoader,
                                                             com.google.common.collect.ImmutableSet<BuildTarget> blacklist,
                                                             com.google.common.collect.ImmutableSet<BuildTarget> linkWholeDeps,
                                                             NativeLinkableInput immediateLinkableInput,
                                                             Optional<LinkOutputPostprocessor> postprocessor,
                                                             CellPathResolver cellPathResolver)
            ```

            ::: block
            Construct a
            [`CxxLink`](CxxLink.html "class in com.facebook.buck.cxx")
            rule that builds a native linkable from top-level input
            objects and a dependency tree of
            [`NativeLinkableGroup`](toolchain/nativelink/NativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink")
            dependencies.
            :::

            [Parameters:]{.paramLabel}
            :   `nativeLinkableDeps` - library dependencies that the
                linkable links in
            :   `immediateLinkableInput` - framework and libraries of
                the linkable itself
            :   `cellPathResolver` -

        []{#createCxxLinkableSharedBuildRule(com.facebook.buck.cxx.config.CxxBuckConfig,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.core.model.BuildTarget,java.nio.file.Path,com.google.common.collect.ImmutableMap,java.util.Optional,com.google.common.collect.ImmutableList,com.facebook.buck.core.cell.CellPathResolver)}

        -   #### createCxxLinkableSharedBuildRule

            ``` methodSignature
            public static CxxLink createCxxLinkableSharedBuildRule​(CxxBuckConfig cxxBuckConfig,
                                                                   CxxPlatform cxxPlatform,
                                                                   ProjectFilesystem projectFilesystem,
                                                                   BuildRuleResolver ruleResolver,
                                                                   BuildTarget target,
                                                                   Path output,
                                                                   com.google.common.collect.ImmutableMap<String,​Path> extraOutputs,
                                                                   Optional<String> soname,
                                                                   com.google.common.collect.ImmutableList<? extends Arg> args,
                                                                   CellPathResolver cellPathResolver)
            ```

        []{#deriveSupplementaryOutputPathsFromMainOutputPath(java.nio.file.Path,java.lang.Iterable)}

        -   #### deriveSupplementaryOutputPathsFromMainOutputPath

            ``` methodSignature
            public static com.google.common.collect.ImmutableMap<String,​Path> deriveSupplementaryOutputPathsFromMainOutputPath​(Path output,
                                                                                                                                     Iterable<String> supplementaryOutputNames)
            ```

            ::: block
            Derive supplementary output paths based on the main output
            path.
            :::

            [Parameters:]{.paramLabel}
            :   `output` - main output path.
            :   `supplementaryOutputNames` - supplementary output names.

            [Returns:]{.returnLabel}
            :   Map of names to supplementary output paths.
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
-   Field \| 
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
