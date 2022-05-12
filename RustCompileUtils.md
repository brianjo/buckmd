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
[Package]{.packageLabelInType} [com.facebook.buck.features.rust](package-summary.html)
:::

## Class RustCompileUtils {#class-rustcompileutils .title title="Class RustCompileUtils"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.rust.RustCompileUtils

::: description
-   

    ------------------------------------------------------------------------

        public class RustCompileUtils
        extends Object

    ::: block
    Utilities to generate various kinds of Rust compilation.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static void`         | `addFeatures​(BuildTa  |                       |
        |                       | rget buildTarget,     |                       |
        |                       |         Iterable<Stri |                       |
        |                       | ng> features,         |                       |
        |                       |     com.google.common |                       |
        |                       | .collect.ImmutableLis |                       |
        |                       | t.Builder<Arg> args)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `addTargetTripleFor   | ::: block             |
        |                       | Flavor​(Flavor flavor, | Add the appropriate   |
        |                       |                       | \--target option to   |
        |                       |     com.google.common | the given rustc args  |
        |                       | .collect.ImmutableLis | if the given flavor   |
        |                       | t.Builder<Arg> args)` | is known.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `createBinary         |                       |
        | ic BinaryWrapperRule` | BuildRule​(BuildTarget |                       |
        |                       |  buildTarget,         |                       |
        |                       |               Project |                       |
        |                       | Filesystem projectFil |                       |
        |                       | esystem,              |                       |
        |                       |          BuildRulePar |                       |
        |                       | ams params,           |                       |
        |                       |             ActionGra |                       |
        |                       | phBuilder graphBuilde |                       |
        |                       | r,                    |                       |
        |                       |    RustBuckConfig rus |                       |
        |                       | tBuckConfig,          |                       |
        |                       |              com.face |                       |
        |                       | book.buck.features.ru |                       |
        |                       | st.RustPlatform rustP |                       |
        |                       | latform,              |                       |
        |                       |          Optional<Str |                       |
        |                       | ing> crateName,       |                       |
        |                       |                 Optio |                       |
        |                       | nal<String> edition,  |                       |
        |                       |                       |                       |
        |                       | com.google.common.col |                       |
        |                       | lect.ImmutableSortedS |                       |
        |                       | et<String> features,  |                       |
        |                       |                       |                       |
        |                       | com.google.common.col |                       |
        |                       | lect.ImmutableSortedM |                       |
        |                       | ap<String,​Arg> enviro |                       |
        |                       | nment,                |                       |
        |                       |        Iterator<Arg>  |                       |
        |                       | rustcFlags,           |                       |
        |                       |             Iterator< |                       |
        |                       | Arg> linkerFlags,     |                       |
        |                       |                   Lin |                       |
        |                       | ker.LinkableDepType l |                       |
        |                       | inkStyle,             |                       |
        |                       |           boolean rpa |                       |
        |                       | th,                   |                       |
        |                       |     com.google.common |                       |
        |                       | .collect.ImmutableSor |                       |
        |                       | tedSet<SourcePath> so |                       |
        |                       | urces,                |                       |
        |                       |        com.google.com |                       |
        |                       | mon.collect.Immutable |                       |
        |                       | SortedMap<SourcePath, |                       |
        |                       | ​String> mappedSources |                       |
        |                       | ,                     |                       |
        |                       |   Optional<String> cr |                       |
        |                       | ateRoot,              |                       |
        |                       |          com.google.c |                       |
        |                       | ommon.collect.Immutab |                       |
        |                       | leSet<String> default |                       |
        |                       | Roots,                |                       |
        |                       |        CrateType crat |                       |
        |                       | eType,                |                       |
        |                       |        Iterable<Build |                       |
        |                       | Rule> deps,           |                       |
        |                       |             com.googl |                       |
        |                       | e.common.collect.Immu |                       |
        |                       | tableMap<String,​Build |                       |
        |                       | Target> depsAliases)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protecte             | `getC                 |                       |
        | d static BuildTarget` | ompileBuildTarget​(Bui |                       |
        |                       | ldTarget target,      |                       |
        |                       |                  CxxP |                       |
        |                       | latform cxxPlatform,  |                       |
        |                       |                       |                       |
        |                       | CrateType crateType)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `getCra               | ::: block             |
        | tic Optional<String>` | teRoot​(SourcePathReso | Given a list of       |
        |                       | lverAdapter resolver, | sources, return the   |
        |                       |              String c | one which is the root |
        |                       | rate,             com | based on the defaults |
        |                       | .google.common.collec | and user parameters.  |
        |                       | t.ImmutableSet<String | :::                   |
        |                       | > defaults,           |                       |
        |                       |    java.util.stream.S |                       |
        |                       | tream<Path> sources)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Li            | `getLi                |                       |
        | nker.LinkableDepType` | nkStyle​(BuildTarget t |                       |
        |                       | arget,             Op |                       |
        |                       | tional<Linker.Linkabl |                       |
        |                       | eDepType> linkStyle)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Strin         | `g                    | ::: block             |
        | gWithMacrosConverter` | etMacroExpander​(Build | Return a macro        |
        |                       | RuleCreationContextWi | expander for a string |
        |                       | thTargetGraph context | with macros           |
        |                       | ,                 Bui | :::                   |
        |                       | ldTarget buildTarget, |                       |
        |                       |                  CxxP |                       |
        |                       | latform cxxPlatform)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static I             | `getPlatformParseTim  |                       |
        | terable<BuildTarget>` | eDeps​(RustToolchain r |                       |
        |                       | ustToolchain,         |                       |
        |                       |                  Buil |                       |
        |                       | dTarget buildTarget,  |                       |
        |                       |                       |                       |
        |                       |    HasDefaultPlatform |                       |
        |                       |  hasDefaultPlatform)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Un            | `getRustP             | ::: block             |
        | resolvedRustPlatform` | latform​(RustToolchain | Gets the              |
        |                       |  rustToolchain,       | [`UnresolvedRustPl    |
        |                       |           BuildTarget | atform`](UnresolvedRu |
        |                       |  target,              | stPlatform.html "inte |
        |                       |    HasDefaultPlatform | rface in com.facebook |
        |                       |  hasDefaultPlatform)` | .buck.features.rust") |
        |                       |                       | for a target.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Ma            | `get                  | ::: block             |
        | p<String,​SourcePath>` | TransitiveRustSharedL | Collect all the       |
        |                       | ibraries​(com.facebook | shared libraries      |
        |                       | .buck.features.rust.R | generated by          |
        |                       | ustPlatform rustPlatf | `RustLinkable`s found |
        |                       | orm,                  | by transitively       |
        |                       |                 Itera | traversing all        |
        |                       | ble<? extends BuildRu | unbroken dependency   |
        |                       | le> inputs,           | chains of             |
        |                       |                       | `RustLinkable`        |
        |                       |   boolean forceRlib)` | objects found via the |
        |                       |                       | passed in             |
        |                       |                       | [`Buil                |
        |                       |                       | dRule`](../../core/ru |
        |                       |                       | les/BuildRule.html "i |
        |                       |                       | nterface in com.faceb |
        |                       |                       | ook.buck.core.rules") |
        |                       |                       | roots.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `requir               |                       |
        | atic RustCompileRule` | eBuild​(BuildTarget bu |                       |
        |                       | ildTarget,            |                       |
        |                       |   ProjectFilesystem p |                       |
        |                       | rojectFilesystem,     |                       |
        |                       |          ActionGraphB |                       |
        |                       | uilder graphBuilder,  |                       |
        |                       |             com.faceb |                       |
        |                       | ook.buck.features.rus |                       |
        |                       | t.RustPlatform rustPl |                       |
        |                       | atform,             R |                       |
        |                       | ustBuckConfig rustCon |                       |
        |                       | fig,             com. |                       |
        |                       | google.common.collect |                       |
        |                       | .ImmutableSortedMap<S |                       |
        |                       | tring,​Arg> environmen |                       |
        |                       | t,             com.go |                       |
        |                       | ogle.common.collect.I |                       |
        |                       | mmutableList<Arg> ext |                       |
        |                       | raFlags,              |                       |
        |                       | com.google.common.col |                       |
        |                       | lect.ImmutableList<Ar |                       |
        |                       | g> extraLinkerFlags,  |                       |
        |                       |             Iterable< |                       |
        |                       | Arg> linkerInputs,    |                       |
        |                       |           String crat |                       |
        |                       | eName,             Cr |                       |
        |                       | ateType crateType,    |                       |
        |                       |           Optional<St |                       |
        |                       | ring> edition,        |                       |
        |                       |       Linker.Linkable |                       |
        |                       | DepType depType,      |                       |
        |                       |         com.google.co |                       |
        |                       | mmon.collect.Immutabl |                       |
        |                       | eSortedMap<SourcePath |                       |
        |                       | ,​Optional<String>> ma |                       |
        |                       | ppedSources,          |                       |
        |                       |     String rootModule |                       |
        |                       | ,             boolean |                       |
        |                       |  forceRlib,           |                       |
        |                       |    boolean preferStat |                       |
        |                       | ic,             Itera |                       |
        |                       | ble<BuildRule> deps,  |                       |
        |                       |             com.googl |                       |
        |                       | e.common.collect.Immu |                       |
        |                       | tableMap<String,​Build |                       |
        |                       | Target> depsAliases,  |                       |
        |                       |             Optional< |                       |
        |                       | String> incremental)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `ruleToCrateN         |                       |
        |                       | ame​(String rulename)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `targetTripleForF     | ::: block             |
        |                       | lavor​(Flavor flavor)` | Given a Rust flavor,  |
        |                       |                       | return a target       |
        |                       |                       | triple or null if     |
        |                       |                       | none known.           |
        |                       |                       | :::                   |
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

        []{#getCompileBuildTarget(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.features.rust.CrateType)}

        -   #### getCompileBuildTarget

            ``` methodSignature
            protected static BuildTarget getCompileBuildTarget​(BuildTarget target,
                                                               CxxPlatform cxxPlatform,
                                                               CrateType crateType)
            ```

        []{#requireBuild(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.features.rust.RustPlatform,com.facebook.buck.features.rust.RustBuckConfig,com.google.common.collect.ImmutableSortedMap,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableList,java.lang.Iterable,java.lang.String,com.facebook.buck.features.rust.CrateType,java.util.Optional,com.facebook.buck.cxx.toolchain.linker.Linker.LinkableDepType,com.google.common.collect.ImmutableSortedMap,java.lang.String,boolean,boolean,java.lang.Iterable,com.google.common.collect.ImmutableMap,java.util.Optional)}

        -   #### requireBuild

            ``` methodSignature
            public static RustCompileRule requireBuild​(BuildTarget buildTarget,
                                                       ProjectFilesystem projectFilesystem,
                                                       ActionGraphBuilder graphBuilder,
                                                       com.facebook.buck.features.rust.RustPlatform rustPlatform,
                                                       RustBuckConfig rustConfig,
                                                       com.google.common.collect.ImmutableSortedMap<String,​Arg> environment,
                                                       com.google.common.collect.ImmutableList<Arg> extraFlags,
                                                       com.google.common.collect.ImmutableList<Arg> extraLinkerFlags,
                                                       Iterable<Arg> linkerInputs,
                                                       String crateName,
                                                       CrateType crateType,
                                                       Optional<String> edition,
                                                       Linker.LinkableDepType depType,
                                                       com.google.common.collect.ImmutableSortedMap<SourcePath,​Optional<String>> mappedSources,
                                                       String rootModule,
                                                       boolean forceRlib,
                                                       boolean preferStatic,
                                                       Iterable<BuildRule> deps,
                                                       com.google.common.collect.ImmutableMap<String,​BuildTarget> depsAliases,
                                                       Optional<String> incremental)
            ```

        []{#getLinkStyle(com.facebook.buck.core.model.BuildTarget,java.util.Optional)}

        -   #### getLinkStyle

            ``` methodSignature
            public static Linker.LinkableDepType getLinkStyle​(BuildTarget target,
                                                              Optional<Linker.LinkableDepType> linkStyle)
            ```

        []{#getRustPlatform(com.facebook.buck.features.rust.RustToolchain,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.description.arg.HasDefaultPlatform)}

        -   #### getRustPlatform

            ``` methodSignature
            public static UnresolvedRustPlatform getRustPlatform​(RustToolchain rustToolchain,
                                                                 BuildTarget target,
                                                                 HasDefaultPlatform hasDefaultPlatform)
            ```

            ::: block
            Gets the
            [`UnresolvedRustPlatform`](UnresolvedRustPlatform.html "interface in com.facebook.buck.features.rust")
            for a target.
            :::

        []{#getPlatformParseTimeDeps(com.facebook.buck.features.rust.RustToolchain,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.description.arg.HasDefaultPlatform)}

        -   #### getPlatformParseTimeDeps

            ``` methodSignature
            public static Iterable<BuildTarget> getPlatformParseTimeDeps​(RustToolchain rustToolchain,
                                                                         BuildTarget buildTarget,
                                                                         HasDefaultPlatform hasDefaultPlatform)
            ```

        []{#createBinaryBuildRule(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.features.rust.RustBuckConfig,com.facebook.buck.features.rust.RustPlatform,java.util.Optional,java.util.Optional,com.google.common.collect.ImmutableSortedSet,com.google.common.collect.ImmutableSortedMap,java.util.Iterator,java.util.Iterator,com.facebook.buck.cxx.toolchain.linker.Linker.LinkableDepType,boolean,com.google.common.collect.ImmutableSortedSet,com.google.common.collect.ImmutableSortedMap,java.util.Optional,com.google.common.collect.ImmutableSet,com.facebook.buck.features.rust.CrateType,java.lang.Iterable,com.google.common.collect.ImmutableMap)}

        -   #### createBinaryBuildRule

            ``` methodSignature
            public static BinaryWrapperRule createBinaryBuildRule​(BuildTarget buildTarget,
                                                                  ProjectFilesystem projectFilesystem,
                                                                  BuildRuleParams params,
                                                                  ActionGraphBuilder graphBuilder,
                                                                  RustBuckConfig rustBuckConfig,
                                                                  com.facebook.buck.features.rust.RustPlatform rustPlatform,
                                                                  Optional<String> crateName,
                                                                  Optional<String> edition,
                                                                  com.google.common.collect.ImmutableSortedSet<String> features,
                                                                  com.google.common.collect.ImmutableSortedMap<String,​Arg> environment,
                                                                  Iterator<Arg> rustcFlags,
                                                                  Iterator<Arg> linkerFlags,
                                                                  Linker.LinkableDepType linkStyle,
                                                                  boolean rpath,
                                                                  com.google.common.collect.ImmutableSortedSet<SourcePath> sources,
                                                                  com.google.common.collect.ImmutableSortedMap<SourcePath,​String> mappedSources,
                                                                  Optional<String> crateRoot,
                                                                  com.google.common.collect.ImmutableSet<String> defaultRoots,
                                                                  CrateType crateType,
                                                                  Iterable<BuildRule> deps,
                                                                  com.google.common.collect.ImmutableMap<String,​BuildTarget> depsAliases)
            ```

        []{#addFeatures(com.facebook.buck.core.model.BuildTarget,java.lang.Iterable,com.google.common.collect.ImmutableList.Builder)}

        -   #### addFeatures

            ``` methodSignature
            public static void addFeatures​(BuildTarget buildTarget,
                                           Iterable<String> features,
                                           com.google.common.collect.ImmutableList.Builder<Arg> args)
            ```

        []{#ruleToCrateName(java.lang.String)}

        -   #### ruleToCrateName

            ``` methodSignature
            public static String ruleToCrateName​(String rulename)
            ```

        []{#getTransitiveRustSharedLibraries(com.facebook.buck.features.rust.RustPlatform,java.lang.Iterable,boolean)}

        -   #### getTransitiveRustSharedLibraries

            ``` methodSignature
            public static Map<String,​SourcePath> getTransitiveRustSharedLibraries​(com.facebook.buck.features.rust.RustPlatform rustPlatform,
                                                                                        Iterable<? extends BuildRule> inputs,
                                                                                        boolean forceRlib)
            ```

            ::: block
            Collect all the shared libraries generated by
            `RustLinkable`s found by transitively traversing all
            unbroken dependency chains of `RustLinkable` objects found
            via the passed in
            [`BuildRule`](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
            roots.
            :::

            [Returns:]{.returnLabel}
            :   a mapping of library name to the library
                [`SourcePath`](../../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath").

        []{#getCrateRoot(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,java.lang.String,com.google.common.collect.ImmutableSet,java.util.stream.Stream)}

        -   #### getCrateRoot

            ``` methodSignature
            public static Optional<String> getCrateRoot​(SourcePathResolverAdapter resolver,
                                                        String crate,
                                                        com.google.common.collect.ImmutableSet<String> defaults,
                                                        java.util.stream.Stream<Path> sources)
            ```

            ::: block
            Given a list of sources, return the one which is the root
            based on the defaults and user parameters.
            :::

            [Parameters:]{.paramLabel}
            :   `resolver` - SourcePathResolverAdapter for rule
            :   `crate` - Name of crate
            :   `defaults` - Default names for this rule (library,
                binary, etc)
            :   `sources` - List of sources

            [Returns:]{.returnLabel}
            :   The unique matching source - if there are not exactly
                one, return Optional.empty

        []{#targetTripleForFlavor(com.facebook.buck.core.model.Flavor)}

        -   #### targetTripleForFlavor

            ``` methodSignature
            @Nullable
            public static String targetTripleForFlavor​(Flavor flavor)
            ```

            ::: block
            Given a Rust flavor, return a target triple or null if none
            known.
            :::

        []{#addTargetTripleForFlavor(com.facebook.buck.core.model.Flavor,com.google.common.collect.ImmutableList.Builder)}

        -   #### addTargetTripleForFlavor

            ``` methodSignature
            public static void addTargetTripleForFlavor​(Flavor flavor,
                                                        com.google.common.collect.ImmutableList.Builder<Arg> args)
            ```

            ::: block
            Add the appropriate \--target option to the given rustc args
            if the given flavor is known.
            :::

        []{#getMacroExpander(com.facebook.buck.core.rules.BuildRuleCreationContextWithTargetGraph,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.cxx.toolchain.CxxPlatform)}

        -   #### getMacroExpander

            ``` methodSignature
            public static StringWithMacrosConverter getMacroExpander​(BuildRuleCreationContextWithTargetGraph context,
                                                                     BuildTarget buildTarget,
                                                                     CxxPlatform cxxPlatform)
            ```

            ::: block
            Return a macro expander for a string with macros
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
