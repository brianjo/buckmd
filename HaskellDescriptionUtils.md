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
-   [Package](package-summary.html)
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
[Package]{.packageLabelInType} [com.facebook.buck.features.haskell](package-summary.html)
:::

## Class HaskellDescriptionUtils {#class-haskelldescriptionutils .title title="Class HaskellDescriptionUtils"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.haskell.HaskellDescriptionUtils

::: description
-   

    ------------------------------------------------------------------------

        public class HaskellDescriptionUtils
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected            | `createCompileFlags   | ::: block             |
        | static com.facebook.b | ​(ActionGraphBuilder g | Create common Haskell |
        | uck.features.haskell. | raphBuilder,          | compile flags used by |
        | HaskellCompilerFlags` |           com.google. | HaskellCompileRule or |
        |                       | common.collect.Immuta | H                     |
        |                       | bleSet<BuildRule> dep | askellHaddockLibRule. |
        |                       | s,                    | :::                   |
        |                       | com.facebook.buck.fea |                       |
        |                       | tures.haskell.Haskell |                       |
        |                       | Platform platform,    |                       |
        |                       |                 Linke |                       |
        |                       | r.LinkableDepType dep |                       |
        |                       | Type,                 |                       |
        |                       |    boolean hsProfile, |                       |
        |                       |                    co |                       |
        |                       | m.google.common.colle |                       |
        |                       | ct.ImmutableList<Stri |                       |
        |                       | ng> additionalFlags)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `c                    | ::: block             |
        | atic HaskellLinkRule` | reateLinkRule​(BuildTa | Create a Haskell link |
        |                       | rget target,          | rule that links the   |
        |                       |       ProjectFilesyst | given inputs to a     |
        |                       | em projectFilesystem, | executable or shared  |
        |                       |                BuildR | library and pulls in  |
        |                       | uleParams baseParams, | transitive native     |
        |                       |                Action | linkable deps from    |
        |                       | GraphBuilder graphBui | the given dep roots.  |
        |                       | lder,               c | :::                   |
        |                       | om.facebook.buck.feat |                       |
        |                       | ures.haskell.HaskellP |                       |
        |                       | latform platform,     |                       |
        |                       |            Linker.Lin |                       |
        |                       | kType linkType,       |                       |
        |                       |          com.google.c |                       |
        |                       | ommon.collect.Immutab |                       |
        |                       | leList<Arg> linkerFla |                       |
        |                       | gs,               Ite |                       |
        |                       | rable<Arg> linkerInpu |                       |
        |                       | ts,               Ite |                       |
        |                       | rable<? extends Nativ |                       |
        |                       | eLinkableGroup> deps, |                       |
        |                       |                com.go |                       |
        |                       | ogle.common.collect.I |                       |
        |                       | mmutableSet<BuildTarg |                       |
        |                       | et> linkWholeDeps,    |                       |
        |                       |             Linker.Li |                       |
        |                       | nkableDepType depType |                       |
        |                       | ,               Path  |                       |
        |                       | outputPath,           |                       |
        |                       |      Optional<String> |                       |
        |                       |  soname,              |                       |
        |                       |   boolean hsProfile)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protecte             | `getComp              |                       |
        | d static BuildTarget` | ileBuildTarget​(BuildT |                       |
        |                       | arget target,         |                       |
        |                       |               com.fac |                       |
        |                       | ebook.buck.features.h |                       |
        |                       | askell.HaskellPlatfor |                       |
        |                       | m platform,           |                       |
        |                       |             Linker.Li |                       |
        |                       | nkableDepType depType |                       |
        |                       | ,                     |                       |
        |                       |   boolean hsProfile)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `getParseTim          | ::: block             |
        |                       | eDeps​(TargetConfigura | Accumulate parse-time |
        |                       | tion targetConfigurat | deps needed by        |
        |                       | ion,                  | Haskell descriptions  |
        |                       | Iterable<com.facebook | in depsBuilder.       |
        |                       | .buck.features.haskel | :::                   |
        |                       | l.HaskellPlatform> pl |                       |
        |                       | atforms,              |                       |
        |                       |     com.google.common |                       |
        |                       | .collect.ImmutableCol |                       |
        |                       | lection.Builder<Build |                       |
        |                       | Target> depsBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `stati                | `r                    |                       |
        | c HaskellCompileRule` | equireCompileRule​(Bui |                       |
        |                       | ldTarget buildTarget, |                       |
        |                       |                    Pr |                       |
        |                       | ojectFilesystem proje |                       |
        |                       | ctFilesystem,         |                       |
        |                       |            BuildRuleP |                       |
        |                       | arams params,         |                       |
        |                       |            ActionGrap |                       |
        |                       | hBuilder graphBuilder |                       |
        |                       | ,                   c |                       |
        |                       | om.google.common.coll |                       |
        |                       | ect.ImmutableSet<Buil |                       |
        |                       | dRule> deps,          |                       |
        |                       |           com.faceboo |                       |
        |                       | k.buck.features.haske |                       |
        |                       | ll.HaskellPlatform pl |                       |
        |                       | atform,               |                       |
        |                       |      Linker.LinkableD |                       |
        |                       | epType depType,       |                       |
        |                       |              boolean  |                       |
        |                       | hsProfile,            |                       |
        |                       |         Optional<Stri |                       |
        |                       | ng> main,             |                       |
        |                       |        Optional<com.f |                       |
        |                       | acebook.buck.features |                       |
        |                       | .haskell.HaskellPacka |                       |
        |                       | geInfo> packageInfo,  |                       |
        |                       |                   com |                       |
        |                       | .google.common.collec |                       |
        |                       | t.ImmutableList<Strin |                       |
        |                       | g> flags,             |                       |
        |                       |        com.facebook.b |                       |
        |                       | uck.features.haskell. |                       |
        |                       | HaskellSources srcs)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `requireGhciRule​(     | ::: block             |
        | atic HaskellGhciRule` | BuildTarget buildTarg | Give a rule that will |
        |                       | et,                Pr | result in a ghci      |
        |                       | ojectFilesystem proje | session for the       |
        |                       | ctFilesystem,         | target                |
        |                       |         BuildRulePara | :::                   |
        |                       | ms params,            |                       |
        |                       |      CellPathResolver |                       |
        |                       |  cellPathResolver,    |                       |
        |                       |              ActionGr |                       |
        |                       | aphBuilder graphBuild |                       |
        |                       | er,                co |                       |
        |                       | m.facebook.buck.featu |                       |
        |                       | res.haskell.HaskellPl |                       |
        |                       | atform platform,      |                       |
        |                       |            CxxBuckCon |                       |
        |                       | fig cxxBuckConfig,    |                       |
        |                       |              com.goog |                       |
        |                       | le.common.collect.Imm |                       |
        |                       | utableSortedSet<Build |                       |
        |                       | Target> argDeps,      |                       |
        |                       |            PatternMat |                       |
        |                       | chedCollection<com.go |                       |
        |                       | ogle.common.collect.I |                       |
        |                       | mmutableSortedSet<Bui |                       |
        |                       | ldTarget>> argPlatfor |                       |
        |                       | mDeps,                |                       |
        |                       |  SourceSortedSet argS |                       |
        |                       | rcs,                c |                       |
        |                       | om.google.common.coll |                       |
        |                       | ect.ImmutableSortedSe |                       |
        |                       | t<BuildTarget> argPre |                       |
        |                       | loadDeps,             |                       |
        |                       |     PatternMatchedCol |                       |
        |                       | lection<com.google.co |                       |
        |                       | mmon.collect.Immutabl |                       |
        |                       | eSortedSet<BuildTarge |                       |
        |                       | t>> argPlatformPreloa |                       |
        |                       | dDeps,                |                       |
        |                       |  com.google.common.co |                       |
        |                       | llect.ImmutableList<S |                       |
        |                       | tring> argCompilerFla |                       |
        |                       | gs,                Op |                       |
        |                       | tional<BuildTarget> a |                       |
        |                       | rgGhciBinDep,         |                       |
        |                       |         Optional<Sour |                       |
        |                       | cePath> argGhciInit,  |                       |
        |                       |                com.go |                       |
        |                       | ogle.common.collect.I |                       |
        |                       | mmutableList<SourcePa |                       |
        |                       | th> argExtraScriptTem |                       |
        |                       | plates,               |                       |
        |                       |   boolean hsProfile)` |                       |
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

        []{#createCompileFlags(com.facebook.buck.core.rules.ActionGraphBuilder,com.google.common.collect.ImmutableSet,com.facebook.buck.features.haskell.HaskellPlatform,com.facebook.buck.cxx.toolchain.linker.Linker.LinkableDepType,boolean,com.google.common.collect.ImmutableList)}

        -   #### createCompileFlags

            ``` methodSignature
            protected static com.facebook.buck.features.haskell.HaskellCompilerFlags createCompileFlags​(ActionGraphBuilder graphBuilder,
                                                                                                        com.google.common.collect.ImmutableSet<BuildRule> deps,
                                                                                                        com.facebook.buck.features.haskell.HaskellPlatform platform,
                                                                                                        Linker.LinkableDepType depType,
                                                                                                        boolean hsProfile,
                                                                                                        com.google.common.collect.ImmutableList<String> additionalFlags)
            ```

            ::: block
            Create common Haskell compile flags used by
            HaskellCompileRule or HaskellHaddockLibRule.
            :::

        []{#getCompileBuildTarget(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.features.haskell.HaskellPlatform,com.facebook.buck.cxx.toolchain.linker.Linker.LinkableDepType,boolean)}

        -   #### getCompileBuildTarget

            ``` methodSignature
            protected static BuildTarget getCompileBuildTarget​(BuildTarget target,
                                                               com.facebook.buck.features.haskell.HaskellPlatform platform,
                                                               Linker.LinkableDepType depType,
                                                               boolean hsProfile)
            ```

        []{#requireCompileRule(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.rules.ActionGraphBuilder,com.google.common.collect.ImmutableSet,com.facebook.buck.features.haskell.HaskellPlatform,com.facebook.buck.cxx.toolchain.linker.Linker.LinkableDepType,boolean,java.util.Optional,java.util.Optional,com.google.common.collect.ImmutableList,com.facebook.buck.features.haskell.HaskellSources)}

        -   #### requireCompileRule

            ``` methodSignature
            public static HaskellCompileRule requireCompileRule​(BuildTarget buildTarget,
                                                                ProjectFilesystem projectFilesystem,
                                                                BuildRuleParams params,
                                                                ActionGraphBuilder graphBuilder,
                                                                com.google.common.collect.ImmutableSet<BuildRule> deps,
                                                                com.facebook.buck.features.haskell.HaskellPlatform platform,
                                                                Linker.LinkableDepType depType,
                                                                boolean hsProfile,
                                                                Optional<String> main,
                                                                Optional<com.facebook.buck.features.haskell.HaskellPackageInfo> packageInfo,
                                                                com.google.common.collect.ImmutableList<String> flags,
                                                                com.facebook.buck.features.haskell.HaskellSources srcs)
            ```

        []{#createLinkRule(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.features.haskell.HaskellPlatform,com.facebook.buck.cxx.toolchain.linker.Linker.LinkType,com.google.common.collect.ImmutableList,java.lang.Iterable,java.lang.Iterable,com.google.common.collect.ImmutableSet,com.facebook.buck.cxx.toolchain.linker.Linker.LinkableDepType,java.nio.file.Path,java.util.Optional,boolean)}

        -   #### createLinkRule

            ``` methodSignature
            public static HaskellLinkRule createLinkRule​(BuildTarget target,
                                                         ProjectFilesystem projectFilesystem,
                                                         BuildRuleParams baseParams,
                                                         ActionGraphBuilder graphBuilder,
                                                         com.facebook.buck.features.haskell.HaskellPlatform platform,
                                                         Linker.LinkType linkType,
                                                         com.google.common.collect.ImmutableList<Arg> linkerFlags,
                                                         Iterable<Arg> linkerInputs,
                                                         Iterable<? extends NativeLinkableGroup> deps,
                                                         com.google.common.collect.ImmutableSet<BuildTarget> linkWholeDeps,
                                                         Linker.LinkableDepType depType,
                                                         Path outputPath,
                                                         Optional<String> soname,
                                                         boolean hsProfile)
            ```

            ::: block
            Create a Haskell link rule that links the given inputs to a
            executable or shared library and pulls in transitive native
            linkable deps from the given dep roots.
            :::

        []{#getParseTimeDeps(com.facebook.buck.core.model.TargetConfiguration,java.lang.Iterable,com.google.common.collect.ImmutableCollection.Builder)}

        -   #### getParseTimeDeps

            ``` methodSignature
            public static void getParseTimeDeps​(TargetConfiguration targetConfiguration,
                                                Iterable<com.facebook.buck.features.haskell.HaskellPlatform> platforms,
                                                com.google.common.collect.ImmutableCollection.Builder<BuildTarget> depsBuilder)
            ```

            ::: block
            Accumulate parse-time deps needed by Haskell descriptions in
            depsBuilder.
            :::

        []{#requireGhciRule(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.cell.CellPathResolver,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.features.haskell.HaskellPlatform,com.facebook.buck.cxx.config.CxxBuckConfig,com.google.common.collect.ImmutableSortedSet,com.facebook.buck.rules.coercer.PatternMatchedCollection,com.facebook.buck.rules.coercer.SourceSortedSet,com.google.common.collect.ImmutableSortedSet,com.facebook.buck.rules.coercer.PatternMatchedCollection,com.google.common.collect.ImmutableList,java.util.Optional,java.util.Optional,com.google.common.collect.ImmutableList,boolean)}

        -   #### requireGhciRule

            ``` methodSignature
            public static HaskellGhciRule requireGhciRule​(BuildTarget buildTarget,
                                                          ProjectFilesystem projectFilesystem,
                                                          BuildRuleParams params,
                                                          CellPathResolver cellPathResolver,
                                                          ActionGraphBuilder graphBuilder,
                                                          com.facebook.buck.features.haskell.HaskellPlatform platform,
                                                          CxxBuckConfig cxxBuckConfig,
                                                          com.google.common.collect.ImmutableSortedSet<BuildTarget> argDeps,
                                                          PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> argPlatformDeps,
                                                          SourceSortedSet argSrcs,
                                                          com.google.common.collect.ImmutableSortedSet<BuildTarget> argPreloadDeps,
                                                          PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> argPlatformPreloadDeps,
                                                          com.google.common.collect.ImmutableList<String> argCompilerFlags,
                                                          Optional<BuildTarget> argGhciBinDep,
                                                          Optional<SourcePath> argGhciInit,
                                                          com.google.common.collect.ImmutableList<SourcePath> argExtraScriptTemplates,
                                                          boolean hsProfile)
            ```

            ::: block
            Give a rule that will result in a ghci session for the
            target
            :::
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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
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
