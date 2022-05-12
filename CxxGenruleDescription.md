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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
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

## Class CxxGenruleDescription {#class-cxxgenruledescription .title title="Class CxxGenruleDescription"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.shell.AbstractGenruleDescription](../shell/AbstractGenruleDescription.html "class in com.facebook.buck.shell")\<[CxxGenruleDescriptionArg](CxxGenruleDescriptionArg.html "class in com.facebook.buck.cxx")\>

    -   -   com.facebook.buck.cxx.CxxGenruleDescription

::: description
-   

    All Implemented Interfaces:
    :   `ImplicitDepsInferringDescription<CxxGenruleDescriptionArg>`,
        `BaseDescription<CxxGenruleDescriptionArg>`,
        `Description<CxxGenruleDescriptionArg>`, `Flavored`,
        `DescriptionWithTargetGraph<CxxGenruleDescriptionArg>`,
        `VersionPropagator<CxxGenruleDescriptionArg>`

    ------------------------------------------------------------------------

        public class CxxGenruleDescription
        extends AbstractGenruleDescription<CxxGenruleDescriptionArg>
        implements Flavored, VersionPropagator<CxxGenruleDescriptionArg>, ImplicitDepsInferringDescription<CxxGenruleDescriptionArg>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.shell.AbstractGenruleDescription}

            ### Nested classes/interfaces inherited from class com.facebook.buck.shell.[AbstractGenruleDescription](../shell/AbstractGenruleDescription.html "class in com.facebook.buck.shell")

            `AbstractGenruleDescription.CommonArg`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.shell.AbstractGenruleDescription}

            ### Fields inherited from class com.facebook.buck.shell.[AbstractGenruleDescription](../shell/AbstractGenruleDescription.html "class in com.facebook.buck.shell")

            `buckConfig, enableSandbox, sandboxExecutionStrategy, toolchainProvider`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                          Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `CxxGenruleDescription​(ToolchainProvider toolchainProvider,                      BuckConfig buckConfig,                      CxxBuckConfig cxxBuckConfig,                      SandboxExecutionStrategy sandboxExecutionStrategy)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected BuildRule` | `createBuildRule​(B    |                       |
        |                       | uildTarget buildTarge |                       |
        |                       | t,                Pro |                       |
        |                       | jectFilesystem projec |                       |
        |                       | tFilesystem,          |                       |
        |                       |        BuildRuleParam |                       |
        |                       | s params,             |                       |
        |                       |     ActionGraphBuilde |                       |
        |                       | r graphBuilder,       |                       |
        |                       |           CxxGenruleD |                       |
        |                       | escriptionArg args,   |                       |
        |                       |               Optiona |                       |
        |                       | l<Arg> cmd,           |                       |
        |                       |       Optional<Arg> b |                       |
        |                       | ash,                O |                       |
        |                       | ptional<Arg> cmdExe)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildRule`           | `c                    | ::: block             |
        |                       | reateBuildRule​(BuildR | Create a              |
        |                       | uleCreationContextWit | [`B                   |
        |                       | hTargetGraph context, | uildRule`](../core/ru |
        |                       |                 Build | les/BuildRule.html "i |
        |                       | Target buildTarget,   | nterface in com.faceb |
        |                       |               BuildRu | ook.buck.core.rules") |
        |                       | leParams params,      | for the given         |
        |                       |            CxxGenrule | [`BuildRuleP          |
        |                       | DescriptionArg args)` | arams`](../core/rules |
        |                       |                       | /BuildRuleParams.html |
        |                       |                       |  "class in com.facebo |
        |                       |                       | ok.buck.core.rules"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `findDepsForTar       |                       |
        |                       | getFromConstructorArg |                       |
        |                       | s​(BuildTarget buildTa |                       |
        |                       | rget,                 |                       |
        |                       |                       |                       |
        |                       | CellNameResolver cell |                       |
        |                       | Roots,                |                       |
        |                       |                       |                       |
        |                       |  CxxGenruleDescriptio |                       |
        |                       | nArg constructorArg,  |                       |
        |                       |                       |                       |
        |                       |                com.go |                       |
        |                       | ogle.common.collect.I |                       |
        |                       | mmutableCollection.Bu |                       |
        |                       | ilder<BuildTarget> ex |                       |
        |                       | traDepsBuilder,       |                       |
        |                       |                       |                       |
        |                       |           com.google. |                       |
        |                       | common.collect.Immuta |                       |
        |                       | bleCollection.Builder |                       |
        |                       | <BuildTarget> targetG |                       |
        |                       | raphOnlyDepsBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static SourcePath`   | `fixupSourcePa        |                       |
        |                       | th​(ActionGraphBuilder |                       |
        |                       |  graphBuilder,        |                       |
        |                       |          CxxPlatform  |                       |
        |                       | platform,             |                       |
        |                       |     SourcePath path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com.google    | `fixupSourcePaths​(Ac  |                       |
        | .common.collect.Immut | tionGraphBuilder grap |                       |
        | ableList<SourcePath>` | hBuilder,             |                       |
        |                       |      CxxPlatform cxxP |                       |
        |                       | latform,              |                       |
        |                       |     com.google.common |                       |
        |                       | .collect.ImmutableLis |                       |
        |                       | t<SourcePath> paths)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `s                    | `fixupSourcePaths​(Act |                       |
        | tatic <T> com.google. | ionGraphBuilder graph |                       |
        | common.collect.Immuta | Builder,              |                       |
        | bleMap<T,​SourcePath>` |     CxxPlatform cxxPl |                       |
        |                       | atform,               |                       |
        |                       |    com.google.common. |                       |
        |                       | collect.ImmutableMap< |                       |
        |                       | T,​SourcePath> paths)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `s                    | `fix                  |                       |
        | tatic com.google.comm | upSourcePaths​(ActionG |                       |
        | on.collect.ImmutableS | raphBuilder graphBuil |                       |
        | ortedSet<SourcePath>` | der,                  |                       |
        |                       | CxxPlatform cxxPlatfo |                       |
        |                       | rm,                 c |                       |
        |                       | om.google.common.coll |                       |
        |                       | ect.ImmutableSortedSe |                       |
        |                       | t<SourcePath> paths)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Class<CxxGe          | `get                  | ::: block             |
        | nruleDescriptionArg>` | ConstructorArgType()` | The type of the       |
        |                       |                       | constructor argument  |
        |                       |                       | that is used by this  |
        |                       |                       | description to create |
        |                       |                       | a rule                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected            | `getMa                |                       |
        | Optional<com.google.c | croHandler​(BuildTarge |                       |
        | ommon.collect.Immutab | t buildTarget,        |                       |
        | leList<MacroExpander< |          ProjectFiles |                       |
        | ? extends Macro,​?>>>` | ystem filesystem,     |                       |
        |                       |             BuildRule |                       |
        |                       | Resolver resolver,    |                       |
        |                       |              TargetGr |                       |
        |                       | aph targetGraph,      |                       |
        |                       |            CxxGenrule |                       |
        |                       | DescriptionArg args)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `h                    |                       |
        |                       | asFlavors​(com.google. |                       |
        |                       | common.collect.Immuta |                       |
        |                       | bleSet<Flavor> flavor |                       |
        |                       | s,           TargetCo |                       |
        |                       | nfiguration toolchain |                       |
        |                       | TargetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `produce              | ::: block             |
        |                       | sCacheableSubgraph()` | Whether or not the    |
        |                       |                       | build rule subgraph   |
        |                       |                       | produced by this      |
        |                       |                       | `Description` is safe |
        |                       |                       | to cache in           |
        |                       |                       | [`Incre               |
        |                       |                       | mentalActionGraphGene |
        |                       |                       | rator`](../core/model |
        |                       |                       | /actiongraph/computat |
        |                       |                       | ion/IncrementalAction |
        |                       |                       | GraphGenerator.html " |
        |                       |                       | class in com.facebook |
        |                       |                       | .buck.core.model.acti |
        |                       |                       | ongraph.computation") |
        |                       |                       | for incremental       |
        |                       |                       | action graph          |
        |                       |                       | generation.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `wrapsCxxGenrule​(So   |                       |
        |                       | urcePathRuleFinder ru |                       |
        |                       | leFinder,             |                       |
        |                       |     SourcePath path)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.shell.AbstractGenruleDescription}

            ### Methods inherited from class com.facebook.buck.shell.[AbstractGenruleDescription](../shell/AbstractGenruleDescription.html "class in com.facebook.buck.shell")

            `canExecuteRemotely, createBuildRule, getAndroidToolsOptional, getGenruleType`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.BaseDescription}

            ### Methods inherited from interface com.facebook.buck.core.description.[BaseDescription](../core/description/BaseDescription.html "interface in com.facebook.buck.core.description")

            `getConfigurationDeps`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.model.Flavored}

            ### Methods inherited from interface com.facebook.buck.core.model.[Flavored](../core/model/Flavored.html "interface in com.facebook.buck.core.model")

            `flavorDomains`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.toolchain.ToolchainProvider,com.facebook.buck.core.config.BuckConfig,com.facebook.buck.cxx.config.CxxBuckConfig,com.facebook.buck.sandbox.SandboxExecutionStrategy)}

        -   #### CxxGenruleDescription

                public CxxGenruleDescription​(ToolchainProvider toolchainProvider,
                                             BuckConfig buckConfig,
                                             CxxBuckConfig cxxBuckConfig,
                                             SandboxExecutionStrategy sandboxExecutionStrategy)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#wrapsCxxGenrule(com.facebook.buck.core.rules.SourcePathRuleFinder,com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### wrapsCxxGenrule

            ``` methodSignature
            public static boolean wrapsCxxGenrule​(SourcePathRuleFinder ruleFinder,
                                                  SourcePath path)
            ```

        []{#fixupSourcePath(com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### fixupSourcePath

            ``` methodSignature
            public static SourcePath fixupSourcePath​(ActionGraphBuilder graphBuilder,
                                                     CxxPlatform platform,
                                                     SourcePath path)
            ```

            [Returns:]{.returnLabel}
            :   a new
                [`BuildTargetSourcePath`](../core/sourcepath/BuildTargetSourcePath.html "interface in com.facebook.buck.core.sourcepath")
                for an existing
                [`BuildTargetSourcePath`](../core/sourcepath/BuildTargetSourcePath.html "interface in com.facebook.buck.core.sourcepath")
                which refers to a
                [`CxxGenrule`](CxxGenrule.html "class in com.facebook.buck.cxx")
                with the given `platform` flavor applied.

        []{#fixupSourcePaths(com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.cxx.toolchain.CxxPlatform,com.google.common.collect.ImmutableList)}

        -   #### fixupSourcePaths

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<SourcePath> fixupSourcePaths​(ActionGraphBuilder graphBuilder,
                                                                                               CxxPlatform cxxPlatform,
                                                                                               com.google.common.collect.ImmutableList<SourcePath> paths)
            ```

        []{#fixupSourcePaths(com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.cxx.toolchain.CxxPlatform,com.google.common.collect.ImmutableSortedSet)}

        -   #### fixupSourcePaths

            ``` methodSignature
            public static com.google.common.collect.ImmutableSortedSet<SourcePath> fixupSourcePaths​(ActionGraphBuilder graphBuilder,
                                                                                                    CxxPlatform cxxPlatform,
                                                                                                    com.google.common.collect.ImmutableSortedSet<SourcePath> paths)
            ```

        []{#fixupSourcePaths(com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.cxx.toolchain.CxxPlatform,com.google.common.collect.ImmutableMap)}

        -   #### fixupSourcePaths

            ``` methodSignature
            public static <T> com.google.common.collect.ImmutableMap<T,​SourcePath> fixupSourcePaths​(ActionGraphBuilder graphBuilder,
                                                                                                          CxxPlatform cxxPlatform,
                                                                                                          com.google.common.collect.ImmutableMap<T,​SourcePath> paths)
            ```

        []{#getConstructorArgType()}

        -   #### getConstructorArgType

            ``` methodSignature
            public Class<CxxGenruleDescriptionArg> getConstructorArgType()
            ```

            ::: block
            [Description copied from
            interface: `BaseDescription`]{.descfrmTypeLabel}
            :::

            ::: block
            The type of the constructor argument that is used by this
            description to create a rule
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getConstructorArgType` in
                interface `BaseDescription<CxxGenruleDescriptionArg>`

        []{#hasFlavors(com.google.common.collect.ImmutableSet,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### hasFlavors

            ``` methodSignature
            public boolean hasFlavors​(com.google.common.collect.ImmutableSet<Flavor> flavors,
                                      TargetConfiguration toolchainTargetConfiguration)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `hasFlavors` in interface `Flavored`

            [Parameters:]{.paramLabel}
            :   `flavors` - The set of
                [`Flavor`](../core/model/Flavor.html "interface in com.facebook.buck.core.model")s
                to consider. All must match.

            [Returns:]{.returnLabel}
            :   Whether a
                [`BuildRule`](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
                of the given
                [`Flavor`](../core/model/Flavor.html "interface in com.facebook.buck.core.model")
                can be created.

        []{#getMacroHandler(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.core.model.targetgraph.TargetGraph,com.facebook.buck.cxx.CxxGenruleDescriptionArg)}

        -   #### getMacroHandler

            ``` methodSignature
            protected Optional<com.google.common.collect.ImmutableList<MacroExpander<? extends Macro,​?>>> getMacroHandler​(BuildTarget buildTarget,
                                                                                                                                ProjectFilesystem filesystem,
                                                                                                                                BuildRuleResolver resolver,
                                                                                                                                TargetGraph targetGraph,
                                                                                                                                CxxGenruleDescriptionArg args)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `getMacroHandler` in
                class `AbstractGenruleDescription<CxxGenruleDescriptionArg>`

            [Returns:]{.returnLabel}
            :   the
                [`MacroExpander`](../rules/macros/MacroExpander.html "interface in com.facebook.buck.rules.macros")s
                which apply to the macros in this description.

        []{#createBuildRule(com.facebook.buck.core.rules.BuildRuleCreationContextWithTargetGraph,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.cxx.CxxGenruleDescriptionArg)}

        -   #### createBuildRule

            ``` methodSignature
            public BuildRule createBuildRule​(BuildRuleCreationContextWithTargetGraph context,
                                             BuildTarget buildTarget,
                                             BuildRuleParams params,
                                             CxxGenruleDescriptionArg args)
            ```

            ::: block
            [Description copied from
            interface: `DescriptionWithTargetGraph`]{.descfrmTypeLabel}
            :::

            ::: block
            Create a
            [`BuildRule`](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
            for the given
            [`BuildRuleParams`](../core/rules/BuildRuleParams.html "class in com.facebook.buck.core.rules").
            Note that the
            [`BuildTarget`](../core/model/BuildTarget.html "class in com.facebook.buck.core.model")
            referred to in the `params` contains the
            [`Flavor`](../core/model/Flavor.html "interface in com.facebook.buck.core.model")
            to create.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `createBuildRule` in
                interface `DescriptionWithTargetGraph<CxxGenruleDescriptionArg>`

            [Overrides:]{.overrideSpecifyLabel}
            :   `createBuildRule` in
                class `AbstractGenruleDescription<CxxGenruleDescriptionArg>`
            :   `args` - A constructor argument, of type as returned by
                [`BaseDescription.getConstructorArgType()`](../core/description/BaseDescription.html#getConstructorArgType()).

            [Returns:]{.returnLabel}
            :   The
                [`BuildRule`](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
                that describes the default flavour of the rule being
                described.

        []{#createBuildRule(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.cxx.CxxGenruleDescriptionArg,java.util.Optional,java.util.Optional,java.util.Optional)}

        -   #### createBuildRule

            ``` methodSignature
            protected BuildRule createBuildRule​(BuildTarget buildTarget,
                                                ProjectFilesystem projectFilesystem,
                                                BuildRuleParams params,
                                                ActionGraphBuilder graphBuilder,
                                                CxxGenruleDescriptionArg args,
                                                Optional<Arg> cmd,
                                                Optional<Arg> bash,
                                                Optional<Arg> cmdExe)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createBuildRule` in
                class `AbstractGenruleDescription<CxxGenruleDescriptionArg>`

        []{#findDepsForTargetFromConstructorArgs(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.cxx.CxxGenruleDescriptionArg,com.google.common.collect.ImmutableCollection.Builder,com.google.common.collect.ImmutableCollection.Builder)}

        -   #### findDepsForTargetFromConstructorArgs

            ``` methodSignature
            public void findDepsForTargetFromConstructorArgs​(BuildTarget buildTarget,
                                                             CellNameResolver cellRoots,
                                                             CxxGenruleDescriptionArg constructorArg,
                                                             com.google.common.collect.ImmutableCollection.Builder<BuildTarget> extraDepsBuilder,
                                                             com.google.common.collect.ImmutableCollection.Builder<BuildTarget> targetGraphOnlyDepsBuilder)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `findDepsForTargetFromConstructorArgs` in
                interface `ImplicitDepsInferringDescription<CxxGenruleDescriptionArg>`

            [Overrides:]{.overrideSpecifyLabel}
            :   `findDepsForTargetFromConstructorArgs` in
                class `AbstractGenruleDescription<CxxGenruleDescriptionArg>`

        []{#producesCacheableSubgraph()}

        -   #### producesCacheableSubgraph

            ``` methodSignature
            public boolean producesCacheableSubgraph()
            ```

            ::: block
            [Description copied from
            interface: `DescriptionWithTargetGraph`]{.descfrmTypeLabel}
            :::

            ::: block
            Whether or not the build rule subgraph produced by this
            `Description` is safe to cache in
            [`IncrementalActionGraphGenerator`](../core/model/actiongraph/computation/IncrementalActionGraphGenerator.html "class in com.facebook.buck.core.model.actiongraph.computation")
            for incremental action graph generation.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `producesCacheableSubgraph` in
                interface `Description<CxxGenruleDescriptionArg>`

            [Specified by:]{.overrideSpecifyLabel}
            :   `producesCacheableSubgraph` in
                interface `DescriptionWithTargetGraph<CxxGenruleDescriptionArg>`
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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
