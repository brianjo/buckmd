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
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.apple](package-summary.html)
:::

## Class AppleLibraryDescription {#class-applelibrarydescription .title title="Class AppleLibraryDescription"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.AppleLibraryDescription

::: description
-   

    All Implemented Interfaces:
    :   `ImplicitDepsInferringDescription<com.facebook.buck.apple.AppleLibraryDescription.AbstractAppleLibraryDescriptionArg>`,
        `ImplicitFlavorsInferringDescription`,
        `BaseDescription<AppleLibraryDescriptionArg>`,
        `Description<AppleLibraryDescriptionArg>`,
        `MetadataProvidingDescription<AppleLibraryDescriptionArg>`,
        `Flavored`,
        `DescriptionWithTargetGraph<AppleLibraryDescriptionArg>`,
        `VersionPropagator<AppleLibraryDescriptionArg>`

    ------------------------------------------------------------------------

        public class AppleLibraryDescription
        extends Object
        implements DescriptionWithTargetGraph<AppleLibraryDescriptionArg>, Flavored, ImplicitDepsInferringDescription<com.facebook.buck.apple.AppleLibraryDescription.AbstractAppleLibraryDescriptionArg>, ImplicitFlavorsInferringDescription, MetadataProvidingDescription<AppleLibraryDescriptionArg>, VersionPropagator<AppleLibraryDescriptionArg>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                            Description
          ------------------- -------------------------------- -------------
          `static class `     `AppleLibraryDescription.Type`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                                                     Field             Description
          ------------------------------------------------------------------------------------- ----------------- -------------
          `static FlavorDomain<AppleLibraryDescription.Type>`                                   `LIBRARY_TYPE`     
          `static FlavorDomain<com.facebook.buck.apple.AppleLibraryDescription.MetadataType>`   `METADATA_TYPE`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `AppleLibraryDescription​(ToolchainProvider toolchainProvider,                        XCodeDescriptions xcodeDescriptions,                        SwiftLibraryDescription swiftDelegate,                        AppleConfig appleConfig,                        CxxBuckConfig cxxBuckConfig,                        SwiftBuckConfig swiftBuckConfig,                        CxxLibraryImplicitFlavors cxxLibraryImplicitFlavors,                        CxxLibraryFlavored cxxLibraryFlavored,                        CxxLibraryFactory cxxLibraryFactory,                        CxxLibraryMetadataFactory cxxLibraryMetadataFactory)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.google.          | `addImplicitF         |                       |
        | common.collect.Immuta | lavors​(com.google.com |                       |
        | bleSortedSet<Flavor>` | mon.collect.Immutable |                       |
        |                       | SortedSet<Flavor> arg |                       |
        |                       | DefaultFlavors,       |                       |
        |                       |              TargetCo |                       |
        |                       | nfiguration toolchain |                       |
        |                       | TargetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildRule`           | `cre                  | ::: block             |
        |                       | ateBuildRule​(BuildRul | Create a              |
        |                       | eCreationContextWithT | [`B                   |
        |                       | argetGraph context,   | uildRule`](../core/ru |
        |                       |               BuildTa | les/BuildRule.html "i |
        |                       | rget buildTarget,     | nterface in com.faceb |
        |                       |             BuildRule | ook.buck.core.rules") |
        |                       | Params params,        | for the given         |
        |                       |          AppleLibrary | [`BuildRuleP          |
        |                       | DescriptionArg args)` | arams`](../core/rules |
        |                       |                       | /BuildRuleParams.html |
        |                       |                       |  "class in com.facebo |
        |                       |                       | ok.buck.core.rules"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `<A extends           | `c                    |                       |
        | AppleNativeTargetDesc | reateLibraryBuildRule |                       |
        | riptionArg>BuildRule` | ​(BuildRuleCreationCon |                       |
        |                       | textWithTargetGraph c |                       |
        |                       | ontext,               |                       |
        |                       |          BuildTarget  |                       |
        |                       | buildTarget,          |                       |
        |                       |               BuildRu |                       |
        |                       | leParams params,      |                       |
        |                       |                   Act |                       |
        |                       | ionGraphBuilder graph |                       |
        |                       | Builder,              |                       |
        |                       |           A args,     |                       |
        |                       |                    Op |                       |
        |                       | tional<Linker.Linkabl |                       |
        |                       | eDepType> linkableDep |                       |
        |                       | Type,                 |                       |
        |                       |        Optional<Sourc |                       |
        |                       | ePath> bundleLoader,  |                       |
        |                       |                       |                       |
        |                       |  com.google.common.co |                       |
        |                       | llect.ImmutableSet<Bu |                       |
        |                       | ildTarget> blacklist, |                       |
        |                       |                       |                       |
        |                       |   com.google.common.c |                       |
        |                       | ollect.ImmutableSorte |                       |
        |                       | dSet<BuildTarget> ext |                       |
        |                       | raCxxDeps,            |                       |
        |                       |             CxxLibrar |                       |
        |                       | yDescription.Transiti |                       |
        |                       | veCxxPreprocessorInpu |                       |
        |                       | tFunction transitiveC |                       |
        |                       | xxPreprocessorInput)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `<U> Optional<U>`     | `c                    |                       |
        |                       | reateMetadata​(BuildTa |                       |
        |                       | rget buildTarget,     |                       |
        |                       |            ActionGrap |                       |
        |                       | hBuilder graphBuilder |                       |
        |                       | ,               CellP |                       |
        |                       | athResolver cellRoots |                       |
        |                       | ,               Apple |                       |
        |                       | LibraryDescriptionArg |                       |
        |                       |  args,                |                       |
        |                       | Optional<com.google.c |                       |
        |                       | ommon.collect.Immutab |                       |
        |                       | leMap<BuildTarget,​Ver |                       |
        |                       | sion>> selectedVersio |                       |
        |                       | ns,               Cla |                       |
        |                       | ss<U> metadataClass)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<BuildRule>` | `createSwiftBuildRu   |                       |
        |                       | le​(BuildTarget buildT |                       |
        |                       | arget,                |                       |
        |                       |       ProjectFilesyst |                       |
        |                       | em projectFilesystem, |                       |
        |                       |                       |                       |
        |                       | ActionGraphBuilder gr |                       |
        |                       | aphBuilder,           |                       |
        |                       |            CellPathRe |                       |
        |                       | solver cellRoots,     |                       |
        |                       |                  Appl |                       |
        |                       | eNativeTargetDescript |                       |
        |                       | ionArg args,          |                       |
        |                       |             Optional< |                       |
        |                       | AppleLibrarySwiftDele |                       |
        |                       | gate> swiftDelegate)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `findDepsF            |                       |
        |                       | orTargetFromConstruct |                       |
        |                       | orArgs​(BuildTarget bu |                       |
        |                       | ildTarget,            |                       |
        |                       |                       |                       |
        |                       |      CellNameResolver |                       |
        |                       |  cellRoots,           |                       |
        |                       |                       |                       |
        |                       |       com.facebook.bu |                       |
        |                       | ck.apple.AppleLibrary |                       |
        |                       | Description.AbstractA |                       |
        |                       | ppleLibraryDescriptio |                       |
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
        | `Opt                  | `f                    |                       |
        | ional<com.google.comm | lavorDomains​(TargetCo |                       |
        | on.collect.ImmutableS | nfiguration toolchain |                       |
        | et<FlavorDomain<?>>>` | TargetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Class<AppleLi        | `get                  | ::: block             |
        | braryDescriptionArg>` | ConstructorArgType()` | The type of the       |
        |                       |                       | constructor argument  |
        |                       |                       | that is used by this  |
        |                       |                       | description to create |
        |                       |                       | a rule                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `h                    |                       |
        |                       | asFlavors​(com.google. |                       |
        |                       | common.collect.Immuta |                       |
        |                       | bleSet<Flavor> flavor |                       |
        |                       | s,           TargetCo |                       |
        |                       | nfiguration toolchain |                       |
        |                       | TargetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `isNotStaticallyLinke |                       |
        |                       | dLibraryNode​(TargetNo |                       |
        |                       | de<CxxLibraryDescript |                       |
        |                       | ion.CommonArg> node)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Optional<C    | `underlyingModule     |                       |
        | xxPreprocessorInput>` | CxxPreprocessorInput​( |                       |
        |                       | BuildTarget target,   |                       |
        |                       |                       |                       |
        |                       |               ActionG |                       |
        |                       | raphBuilder graphBuil |                       |
        |                       | der,                  |                       |
        |                       |                     C |                       |
        |                       | xxPlatform platform)` |                       |
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

            ### Methods inherited from interface com.facebook.buck.core.description.[BaseDescription](../core/description/BaseDescription.html "interface in com.facebook.buck.core.description")

            `getConfigurationDeps`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.DescriptionWithTargetGraph}

            ### Methods inherited from interface com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")

            `producesCacheableSubgraph`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#METADATA_TYPE}

        -   #### METADATA_TYPE

                public static final FlavorDomain<com.facebook.buck.apple.AppleLibraryDescription.MetadataType> METADATA_TYPE

        []{#LIBRARY_TYPE}

        -   #### LIBRARY_TYPE

                public static final FlavorDomain<AppleLibraryDescription.Type> LIBRARY_TYPE
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.toolchain.ToolchainProvider,com.facebook.buck.apple.XCodeDescriptions,com.facebook.buck.swift.SwiftLibraryDescription,com.facebook.buck.apple.AppleConfig,com.facebook.buck.cxx.config.CxxBuckConfig,com.facebook.buck.swift.SwiftBuckConfig,com.facebook.buck.cxx.CxxLibraryImplicitFlavors,com.facebook.buck.cxx.CxxLibraryFlavored,com.facebook.buck.cxx.CxxLibraryFactory,com.facebook.buck.cxx.CxxLibraryMetadataFactory)}

        -   #### AppleLibraryDescription

                public AppleLibraryDescription​(ToolchainProvider toolchainProvider,
                                               XCodeDescriptions xcodeDescriptions,
                                               SwiftLibraryDescription swiftDelegate,
                                               AppleConfig appleConfig,
                                               CxxBuckConfig cxxBuckConfig,
                                               SwiftBuckConfig swiftBuckConfig,
                                               CxxLibraryImplicitFlavors cxxLibraryImplicitFlavors,
                                               CxxLibraryFlavored cxxLibraryFlavored,
                                               CxxLibraryFactory cxxLibraryFactory,
                                               CxxLibraryMetadataFactory cxxLibraryMetadataFactory)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getConstructorArgType()}

        -   #### getConstructorArgType

            ``` methodSignature
            public Class<AppleLibraryDescriptionArg> getConstructorArgType()
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
                interface `BaseDescription<AppleLibraryDescriptionArg>`

        []{#flavorDomains(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### flavorDomains

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableSet<FlavorDomain<?>>> flavorDomains​(TargetConfiguration toolchainTargetConfiguration)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `flavorDomains` in interface `Flavored`

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

        []{#createSwiftBuildRule(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.cell.CellPathResolver,com.facebook.buck.apple.AppleNativeTargetDescriptionArg,java.util.Optional)}

        -   #### createSwiftBuildRule

            ``` methodSignature
            public Optional<BuildRule> createSwiftBuildRule​(BuildTarget buildTarget,
                                                            ProjectFilesystem projectFilesystem,
                                                            ActionGraphBuilder graphBuilder,
                                                            CellPathResolver cellRoots,
                                                            AppleNativeTargetDescriptionArg args,
                                                            Optional<AppleLibrarySwiftDelegate> swiftDelegate)
            ```

        []{#createBuildRule(com.facebook.buck.core.rules.BuildRuleCreationContextWithTargetGraph,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.apple.AppleLibraryDescriptionArg)}

        -   #### createBuildRule

            ``` methodSignature
            public BuildRule createBuildRule​(BuildRuleCreationContextWithTargetGraph context,
                                             BuildTarget buildTarget,
                                             BuildRuleParams params,
                                             AppleLibraryDescriptionArg args)
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
                interface `DescriptionWithTargetGraph<AppleLibraryDescriptionArg>`
            :   `args` - A constructor argument, of type as returned by
                [`BaseDescription.getConstructorArgType()`](../core/description/BaseDescription.html#getConstructorArgType()).

            [Returns:]{.returnLabel}
            :   The
                [`BuildRule`](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
                that describes the default flavour of the rule being
                described.

        []{#createLibraryBuildRule(com.facebook.buck.core.rules.BuildRuleCreationContextWithTargetGraph,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.apple.AppleNativeTargetDescriptionArg,java.util.Optional,java.util.Optional,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableSortedSet,com.facebook.buck.cxx.CxxLibraryDescription.TransitiveCxxPreprocessorInputFunction)}
        []{#createLibraryBuildRule(com.facebook.buck.core.rules.BuildRuleCreationContextWithTargetGraph,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.rules.ActionGraphBuilder,A,java.util.Optional,java.util.Optional,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableSortedSet,com.facebook.buck.cxx.CxxLibraryDescription.TransitiveCxxPreprocessorInputFunction)}

        -   #### createLibraryBuildRule

            ``` methodSignature
            public <A extends AppleNativeTargetDescriptionArg> BuildRule createLibraryBuildRule​(BuildRuleCreationContextWithTargetGraph context,
                                                                                                BuildTarget buildTarget,
                                                                                                BuildRuleParams params,
                                                                                                ActionGraphBuilder graphBuilder,
                                                                                                A args,
                                                                                                Optional<Linker.LinkableDepType> linkableDepType,
                                                                                                Optional<SourcePath> bundleLoader,
                                                                                                com.google.common.collect.ImmutableSet<BuildTarget> blacklist,
                                                                                                com.google.common.collect.ImmutableSortedSet<BuildTarget> extraCxxDeps,
                                                                                                CxxLibraryDescription.TransitiveCxxPreprocessorInputFunction transitiveCxxPreprocessorInput)
            ```

            [Parameters:]{.paramLabel}
            :   `bundleLoader` - The binary in which the current library
                will be (dynamically) loaded into.

        []{#createMetadata(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.cell.CellPathResolver,com.facebook.buck.apple.AppleLibraryDescriptionArg,java.util.Optional,java.lang.Class)}

        -   #### createMetadata

            ``` methodSignature
            public <U> Optional<U> createMetadata​(BuildTarget buildTarget,
                                                  ActionGraphBuilder graphBuilder,
                                                  CellPathResolver cellRoots,
                                                  AppleLibraryDescriptionArg args,
                                                  Optional<com.google.common.collect.ImmutableMap<BuildTarget,​Version>> selectedVersions,
                                                  Class<U> metadataClass)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createMetadata` in
                interface `MetadataProvidingDescription<AppleLibraryDescriptionArg>`

        []{#addImplicitFlavors(com.google.common.collect.ImmutableSortedSet,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### addImplicitFlavors

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<Flavor> addImplicitFlavors​(com.google.common.collect.ImmutableSortedSet<Flavor> argDefaultFlavors,
                                                                                           TargetConfiguration toolchainTargetConfiguration)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `addImplicitFlavors` in
                interface `ImplicitFlavorsInferringDescription`

        []{#findDepsForTargetFromConstructorArgs(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.apple.AppleLibraryDescription.AbstractAppleLibraryDescriptionArg,com.google.common.collect.ImmutableCollection.Builder,com.google.common.collect.ImmutableCollection.Builder)}

        -   #### findDepsForTargetFromConstructorArgs

            ``` methodSignature
            public void findDepsForTargetFromConstructorArgs​(BuildTarget buildTarget,
                                                             CellNameResolver cellRoots,
                                                             com.facebook.buck.apple.AppleLibraryDescription.AbstractAppleLibraryDescriptionArg constructorArg,
                                                             com.google.common.collect.ImmutableCollection.Builder<BuildTarget> extraDepsBuilder,
                                                             com.google.common.collect.ImmutableCollection.Builder<BuildTarget> targetGraphOnlyDepsBuilder)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `findDepsForTargetFromConstructorArgs` in
                interface `ImplicitDepsInferringDescription<com.facebook.buck.apple.AppleLibraryDescription.AbstractAppleLibraryDescriptionArg>`

        []{#isNotStaticallyLinkedLibraryNode(com.facebook.buck.core.model.targetgraph.TargetNode)}

        -   #### isNotStaticallyLinkedLibraryNode

            ``` methodSignature
            public static boolean isNotStaticallyLinkedLibraryNode​(TargetNode<CxxLibraryDescription.CommonArg> node)
            ```

        []{#underlyingModuleCxxPreprocessorInput(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.cxx.toolchain.CxxPlatform)}

        -   #### underlyingModuleCxxPreprocessorInput

            ``` methodSignature
            public static Optional<CxxPreprocessorInput> underlyingModuleCxxPreprocessorInput​(BuildTarget target,
                                                                                              ActionGraphBuilder graphBuilder,
                                                                                              CxxPlatform platform)
            ```
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
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
