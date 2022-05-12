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
[Package]{.packageLabelInType} [com.facebook.buck.features.haskell](package-summary.html)
:::

## Class HaskellGhciDescription {#class-haskellghcidescription .title title="Class HaskellGhciDescription"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.haskell.HaskellGhciDescription

::: description
-   

    All Implemented Interfaces:
    :   `ImplicitDepsInferringDescription<com.facebook.buck.features.haskell.HaskellGhciDescription.AbstractHaskellGhciDescriptionArg>`,
        `BaseDescription<HaskellGhciDescriptionArg>`,
        `Description<HaskellGhciDescriptionArg>`,
        `DescriptionWithTargetGraph<HaskellGhciDescriptionArg>`,
        `VersionRoot<HaskellGhciDescriptionArg>`

    ------------------------------------------------------------------------

        public class HaskellGhciDescription
        extends Object
        implements DescriptionWithTargetGraph<HaskellGhciDescriptionArg>, ImplicitDepsInferringDescription<com.facebook.buck.features.haskell.HaskellGhciDescription.AbstractHaskellGhciDescriptionArg>, VersionRoot<HaskellGhciDescriptionArg>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                        Description
          ------------------------------------------------------------------------------------------------------------------ -------------
          `HaskellGhciDescription​(ToolchainProvider toolchainProvider,                       CxxBuckConfig cxxBuckConfig)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `BuildRule`           | `cr                   | ::: block             |
        |                       | eateBuildRule​(BuildRu | Create a              |
        |                       | leCreationContextWith | [`Buil                |
        |                       | TargetGraph context,  | dRule`](../../core/ru |
        |                       |                BuildT | les/BuildRule.html "i |
        |                       | arget buildTarget,    | nterface in com.faceb |
        |                       |              BuildRul | ook.buck.core.rules") |
        |                       | eParams params,       | for the given         |
        |                       |           HaskellGhci | [`BuildRulePara       |
        |                       | DescriptionArg args)` | ms`](../../core/rules |
        |                       |                       | /BuildRuleParams.html |
        |                       |                       |  "class in com.facebo |
        |                       |                       | ok.buck.core.rules"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `findDepsForTargetF   |                       |
        |                       | romConstructorArgs​(Bu |                       |
        |                       | ildTarget buildTarget |                       |
        |                       | ,                     |                       |
        |                       |                  Cell |                       |
        |                       | NameResolver cellRoot |                       |
        |                       | s,                    |                       |
        |                       |                   com |                       |
        |                       | .facebook.buck.featur |                       |
        |                       | es.haskell.HaskellGhc |                       |
        |                       | iDescription.Abstract |                       |
        |                       | HaskellGhciDescriptio |                       |
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
        | `Class<Haskel         | `get                  | ::: block             |
        | lGhciDescriptionArg>` | ConstructorArgType()` | The type of the       |
        |                       |                       | constructor argument  |
        |                       |                       | that is used by this  |
        |                       |                       | description to create |
        |                       |                       | a rule                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `ge                   |                       |
        | ic com.facebook.buck. | tOmnibusSpec​(BuildTar |                       |
        | features.haskell.Hask | get baseTarget,       |                       |
        | ellGhciDescription.Ha |          ActionGraphB |                       |
        | skellGhciOmnibusSpec` | uilder graphBuilder,  |                       |
        |                       |               com.goo |                       |
        |                       | gle.common.collect.Im |                       |
        |                       | mutableList<? extends |                       |
        |                       |  NativeLinkable> omni |                       |
        |                       | busRoots,             |                       |
        |                       |    com.google.common. |                       |
        |                       | collect.ImmutableList |                       |
        |                       | <? extends NativeLink |                       |
        |                       | able> excludedRoots)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Path`         | `getSoLibsRelDir​(Bui  | ::: block             |
        |                       | ldTarget baseTarget)` | Give the relative     |
        |                       |                       | path from the omnibus |
        |                       |                       | to its shared library |
        |                       |                       | directory.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static BuildRule`    | `requireOmnibus       | ::: block             |
        |                       | SharedObject​(CellPath | Give a rule for an    |
        |                       | Resolver cellPathReso | omnibus object to be  |
        |                       | lver,                 | loaded into a ghci    |
        |                       |            BuildTarge | session               |
        |                       | t baseTarget,         | :::                   |
        |                       |                    Pr |                       |
        |                       | ojectFilesystem proje |                       |
        |                       | ctFilesystem,         |                       |
        |                       |                    Ac |                       |
        |                       | tionGraphBuilder grap |                       |
        |                       | hBuilder,             |                       |
        |                       |                CxxPla |                       |
        |                       | tform cxxPlatform,    |                       |
        |                       |                       |                       |
        |                       |    CxxBuckConfig cxxB |                       |
        |                       | uckConfig,            |                       |
        |                       |                 Itera |                       |
        |                       | ble<NativeLinkable> b |                       |
        |                       | ody,                  |                       |
        |                       |           Iterable<Na |                       |
        |                       | tiveLinkable> deps,   |                       |
        |                       |                       |                       |
        |                       |     com.google.common |                       |
        |                       | .collect.ImmutableLis |                       |
        |                       | t<Arg> extraLdFlags)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.BaseDescription}

            ### Methods inherited from interface com.facebook.buck.core.description.[BaseDescription](../../core/description/BaseDescription.html "interface in com.facebook.buck.core.description")

            `getConfigurationDeps`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.DescriptionWithTargetGraph}

            ### Methods inherited from interface com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")

            `producesCacheableSubgraph`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.versions.VersionRoot}

            ### Methods inherited from interface com.facebook.buck.versions.[VersionRoot](../../versions/VersionRoot.html "interface in com.facebook.buck.versions")

            `isVersionRoot`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.toolchain.ToolchainProvider,com.facebook.buck.cxx.config.CxxBuckConfig)}

        -   #### HaskellGhciDescription

                public HaskellGhciDescription​(ToolchainProvider toolchainProvider,
                                              CxxBuckConfig cxxBuckConfig)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getConstructorArgType()}

        -   #### getConstructorArgType

            ``` methodSignature
            public Class<HaskellGhciDescriptionArg> getConstructorArgType()
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
                interface `BaseDescription<HaskellGhciDescriptionArg>`

        []{#getOmnibusSpec(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableList)}

        -   #### getOmnibusSpec

            ``` methodSignature
            public static com.facebook.buck.features.haskell.HaskellGhciDescription.HaskellGhciOmnibusSpec getOmnibusSpec​(BuildTarget baseTarget,
                                                                                                                          ActionGraphBuilder graphBuilder,
                                                                                                                          com.google.common.collect.ImmutableList<? extends NativeLinkable> omnibusRoots,
                                                                                                                          com.google.common.collect.ImmutableList<? extends NativeLinkable> excludedRoots)
            ```

            [Parameters:]{.paramLabel}
            :   `omnibusRoots` - roots of the graph of nodes (including
                transitive deps) to include in the omnibus link.
            :   `excludedRoots` - roots of a the graph of nodes
                (including transitive deps) that cannot be included in
                the omnibus link.

            [Returns:]{.returnLabel}
            :   the `HaskellGhciDescription.HaskellGhciOmnibusSpec`
                describing the omnibus link.

        []{#getSoLibsRelDir(com.facebook.buck.core.model.BuildTarget)}

        -   #### getSoLibsRelDir

            ``` methodSignature
            public static Path getSoLibsRelDir​(BuildTarget baseTarget)
            ```

            ::: block
            Give the relative path from the omnibus to its shared
            library directory. Expose this to enable setting -rpath.
            :::

        []{#requireOmnibusSharedObject(com.facebook.buck.core.cell.CellPathResolver,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.cxx.config.CxxBuckConfig,java.lang.Iterable,java.lang.Iterable,com.google.common.collect.ImmutableList)}

        -   #### requireOmnibusSharedObject

            ``` methodSignature
            public static BuildRule requireOmnibusSharedObject​(CellPathResolver cellPathResolver,
                                                               BuildTarget baseTarget,
                                                               ProjectFilesystem projectFilesystem,
                                                               ActionGraphBuilder graphBuilder,
                                                               CxxPlatform cxxPlatform,
                                                               CxxBuckConfig cxxBuckConfig,
                                                               Iterable<NativeLinkable> body,
                                                               Iterable<NativeLinkable> deps,
                                                               com.google.common.collect.ImmutableList<Arg> extraLdFlags)
            ```

            ::: block
            Give a rule for an omnibus object to be loaded into a ghci
            session
            :::

        []{#createBuildRule(com.facebook.buck.core.rules.BuildRuleCreationContextWithTargetGraph,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.features.haskell.HaskellGhciDescriptionArg)}

        -   #### createBuildRule

            ``` methodSignature
            public BuildRule createBuildRule​(BuildRuleCreationContextWithTargetGraph context,
                                             BuildTarget buildTarget,
                                             BuildRuleParams params,
                                             HaskellGhciDescriptionArg args)
            ```

            ::: block
            [Description copied from
            interface: `DescriptionWithTargetGraph`]{.descfrmTypeLabel}
            :::

            ::: block
            Create a
            [`BuildRule`](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
            for the given
            [`BuildRuleParams`](../../core/rules/BuildRuleParams.html "class in com.facebook.buck.core.rules").
            Note that the
            [`BuildTarget`](../../core/model/BuildTarget.html "class in com.facebook.buck.core.model")
            referred to in the `params` contains the
            [`Flavor`](../../core/model/Flavor.html "interface in com.facebook.buck.core.model")
            to create.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `createBuildRule` in
                interface `DescriptionWithTargetGraph<HaskellGhciDescriptionArg>`
            :   `args` - A constructor argument, of type as returned by
                [`BaseDescription.getConstructorArgType()`](../../core/description/BaseDescription.html#getConstructorArgType()).

            [Returns:]{.returnLabel}
            :   The
                [`BuildRule`](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
                that describes the default flavour of the rule being
                described.

        []{#findDepsForTargetFromConstructorArgs(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.features.haskell.HaskellGhciDescription.AbstractHaskellGhciDescriptionArg,com.google.common.collect.ImmutableCollection.Builder,com.google.common.collect.ImmutableCollection.Builder)}

        -   #### findDepsForTargetFromConstructorArgs

            ``` methodSignature
            public void findDepsForTargetFromConstructorArgs​(BuildTarget buildTarget,
                                                             CellNameResolver cellRoots,
                                                             com.facebook.buck.features.haskell.HaskellGhciDescription.AbstractHaskellGhciDescriptionArg constructorArg,
                                                             com.google.common.collect.ImmutableCollection.Builder<BuildTarget> extraDepsBuilder,
                                                             com.google.common.collect.ImmutableCollection.Builder<BuildTarget> targetGraphOnlyDepsBuilder)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `findDepsForTargetFromConstructorArgs` in
                interface `ImplicitDepsInferringDescription<com.facebook.buck.features.haskell.HaskellGhciDescription.AbstractHaskellGhciDescriptionArg>`
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
