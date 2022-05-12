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
[Package]{.packageLabelInType} [com.facebook.buck.cxx](package-summary.html)
:::

## Class CxxLibraryDescription {#class-cxxlibrarydescription .title title="Class CxxLibraryDescription"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.CxxLibraryDescription

::: description
-   

    All Implemented Interfaces:
    :   `ImplicitDepsInferringDescription<CxxLibraryDescription.CommonArg>`,
        `ImplicitFlavorsInferringDescription`,
        `BaseDescription<CxxLibraryDescriptionArg>`,
        `Description<CxxLibraryDescriptionArg>`,
        `MetadataProvidingDescription<CxxLibraryDescriptionArg>`,
        `Flavored`,
        `DescriptionWithTargetGraph<CxxLibraryDescriptionArg>`,
        `VersionPropagator<CxxLibraryDescriptionArg>`

    ------------------------------------------------------------------------

        public class CxxLibraryDescription
        extends Object
        implements DescriptionWithTargetGraph<CxxLibraryDescriptionArg>, ImplicitDepsInferringDescription<CxxLibraryDescription.CommonArg>, ImplicitFlavorsInferringDescription, Flavored, MetadataProvidingDescription<CxxLibraryDescriptionArg>, VersionPropagator<CxxLibraryDescriptionArg>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static interface `   | `CxxLibraryD          |                       |
        |                       | escription.CommonArg` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `CxxLibraryDesc       |                       |
        |                       | ription.MetadataType` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static interface `   | `CxxLibraryDescripti  | ::: block             |
        |                       | on.TransitiveCxxPrepr | This is a hack to     |
        |                       | ocessorInputFunction` | allow fine grained    |
        |                       |                       | control over how the  |
        |                       |                       | transitive            |
        |                       |                       | `  C                  |
        |                       |                       | xxPreprocessorInput`s |
        |                       |                       | are found.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `CxxLib               |                       |
        |                       | raryDescription.Type` |                       |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                           Field                 Description
          ----------------------------------------------------------- --------------------- -------------
          `static FlavorDomain<HeaderMode>`                           `HEADER_MODE`          
          `static FlavorDomain<HeaderVisibility>`                     `HEADER_VISIBILITY`    
          `static FlavorDomain<CxxLibraryDescription.Type>`           `LIBRARY_TYPE`         
          `static FlavorDomain<CxxLibraryDescription.MetadataType>`   `METADATA_TYPE`        

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                    Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `CxxLibraryDescription​(CxxLibraryImplicitFlavors cxxLibraryImplicitFlavors,                      CxxLibraryFlavored cxxLibraryFlavored,                      CxxLibraryFactory cxxLibraryFactory,                      CxxLibraryMetadataFactory cxxLibraryMetadataFactory)`    

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
        | `BuildRule`           | `c                    | ::: block             |
        |                       | reateBuildRule​(BuildR | Create a              |
        |                       | uleCreationContextWit | [`B                   |
        |                       | hTargetGraph context, | uildRule`](../core/ru |
        |                       |                 Build | les/BuildRule.html "i |
        |                       | Target buildTarget,   | nterface in com.faceb |
        |                       |               BuildRu | ook.buck.core.rules") |
        |                       | leParams params,      | for the given         |
        |                       |            CxxLibrary | [`BuildRuleP          |
        |                       | DescriptionArg args)` | arams`](../core/rules |
        |                       |                       | /BuildRuleParams.html |
        |                       |                       |  "class in com.facebo |
        |                       |                       | ok.buck.core.rules"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `<U> Optional<U>`     | `createMetadata​(Build |                       |
        |                       | Target buildTarget,   |                       |
        |                       |              ActionGr |                       |
        |                       | aphBuilder graphBuild |                       |
        |                       | er,               Cel |                       |
        |                       | lPathResolver cellRoo |                       |
        |                       | ts,               Cxx |                       |
        |                       | LibraryDescriptionArg |                       |
        |                       |  args,                |                       |
        |                       | Optional<com.google.c |                       |
        |                       | ommon.collect.Immutab |                       |
        |                       | leMap<BuildTarget,​Ver |                       |
        |                       | sion>> selectedVersio |                       |
        |                       | ns,               Cla |                       |
        |                       | ss<U> metadataClass)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `                     |                       |
        |                       | findDepsForTargetFrom |                       |
        |                       | ConstructorArgs​(Build |                       |
        |                       | Target buildTarget,   |                       |
        |                       |                       |                       |
        |                       |               CellNam |                       |
        |                       | eResolver cellRoots,  |                       |
        |                       |                       |                       |
        |                       |                CxxLib |                       |
        |                       | raryDescription.Commo |                       |
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
        | `Class<CxxLi          | `get                  | ::: block             |
        | braryDescriptionArg>` | ConstructorArgType()` | The type of the       |
        |                       |                       | constructor argument  |
        |                       |                       | that is used by this  |
        |                       |                       | description to create |
        |                       |                       | a rule                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Optional<Map. | `getLibType​(Buil      |                       |
        | Entry<Flavor,​CxxLibra | dTarget buildTarget)` |                       |
        | ryDescription.Type>>` |                       |                       |
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
        | `static Optional<C    | `queryMetad           | ::: block             |
        | xxPreprocessorInput>` | ataCxxPreprocessorInp | Convenience function  |
        |                       | ut​(ActionGraphBuilder | to query the          |
        |                       |  graphBuilder,        | [`CxxPreprocessorInpu |
        |                       |                       | t`](CxxPreprocessorIn |
        |                       |       BuildTarget bas | put.html "class in co |
        |                       | eTarget,              | m.facebook.buck.cxx") |
        |                       |                       | metadata of a target. |
        |                       | CxxPlatform platform, | :::                   |
        |                       |                       |                       |
        |                       |              HeaderVi |                       |
        |                       | sibility visibility)` |                       |
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
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#LIBRARY_TYPE}

        -   #### LIBRARY_TYPE

                public static final FlavorDomain<CxxLibraryDescription.Type> LIBRARY_TYPE

        []{#METADATA_TYPE}

        -   #### METADATA_TYPE

                public static final FlavorDomain<CxxLibraryDescription.MetadataType> METADATA_TYPE

        []{#HEADER_VISIBILITY}

        -   #### HEADER_VISIBILITY

                public static final FlavorDomain<HeaderVisibility> HEADER_VISIBILITY

        []{#HEADER_MODE}

        -   #### HEADER_MODE

                public static final FlavorDomain<HeaderMode> HEADER_MODE
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.cxx.CxxLibraryImplicitFlavors,com.facebook.buck.cxx.CxxLibraryFlavored,com.facebook.buck.cxx.CxxLibraryFactory,com.facebook.buck.cxx.CxxLibraryMetadataFactory)}

        -   #### CxxLibraryDescription

                public CxxLibraryDescription​(CxxLibraryImplicitFlavors cxxLibraryImplicitFlavors,
                                             CxxLibraryFlavored cxxLibraryFlavored,
                                             CxxLibraryFactory cxxLibraryFactory,
                                             CxxLibraryMetadataFactory cxxLibraryMetadataFactory)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

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

        []{#getConstructorArgType()}

        -   #### getConstructorArgType

            ``` methodSignature
            public Class<CxxLibraryDescriptionArg> getConstructorArgType()
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
                interface `BaseDescription<CxxLibraryDescriptionArg>`

        []{#createBuildRule(com.facebook.buck.core.rules.BuildRuleCreationContextWithTargetGraph,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.cxx.CxxLibraryDescriptionArg)}

        -   #### createBuildRule

            ``` methodSignature
            public BuildRule createBuildRule​(BuildRuleCreationContextWithTargetGraph context,
                                             BuildTarget buildTarget,
                                             BuildRuleParams params,
                                             CxxLibraryDescriptionArg args)
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
                interface `DescriptionWithTargetGraph<CxxLibraryDescriptionArg>`
            :   `args` - A constructor argument, of type as returned by
                [`BaseDescription.getConstructorArgType()`](../core/description/BaseDescription.html#getConstructorArgType()).

            [Returns:]{.returnLabel}
            :   The
                [`BuildRule`](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
                that describes the default flavour of the rule being
                described.

        []{#getLibType(com.facebook.buck.core.model.BuildTarget)}

        -   #### getLibType

            ``` methodSignature
            public static Optional<Map.Entry<Flavor,​CxxLibraryDescription.Type>> getLibType​(BuildTarget buildTarget)
            ```

        []{#findDepsForTargetFromConstructorArgs(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.cxx.CxxLibraryDescription.CommonArg,com.google.common.collect.ImmutableCollection.Builder,com.google.common.collect.ImmutableCollection.Builder)}

        -   #### findDepsForTargetFromConstructorArgs

            ``` methodSignature
            public void findDepsForTargetFromConstructorArgs​(BuildTarget buildTarget,
                                                             CellNameResolver cellRoots,
                                                             CxxLibraryDescription.CommonArg constructorArg,
                                                             com.google.common.collect.ImmutableCollection.Builder<BuildTarget> extraDepsBuilder,
                                                             com.google.common.collect.ImmutableCollection.Builder<BuildTarget> targetGraphOnlyDepsBuilder)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `findDepsForTargetFromConstructorArgs` in
                interface `ImplicitDepsInferringDescription<CxxLibraryDescription.CommonArg>`

        []{#queryMetadataCxxPreprocessorInput(com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.cxx.toolchain.HeaderVisibility)}

        -   #### queryMetadataCxxPreprocessorInput

            ``` methodSignature
            public static Optional<CxxPreprocessorInput> queryMetadataCxxPreprocessorInput​(ActionGraphBuilder graphBuilder,
                                                                                           BuildTarget baseTarget,
                                                                                           CxxPlatform platform,
                                                                                           HeaderVisibility visibility)
            ```

            ::: block
            Convenience function to query the
            [`CxxPreprocessorInput`](CxxPreprocessorInput.html "class in com.facebook.buck.cxx")
            metadata of a target.
            Use this function instead of constructing the BuildTarget
            manually.
            :::

        []{#createMetadata(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.cell.CellPathResolver,com.facebook.buck.cxx.CxxLibraryDescriptionArg,java.util.Optional,java.lang.Class)}

        -   #### createMetadata

            ``` methodSignature
            public <U> Optional<U> createMetadata​(BuildTarget buildTarget,
                                                  ActionGraphBuilder graphBuilder,
                                                  CellPathResolver cellRoots,
                                                  CxxLibraryDescriptionArg args,
                                                  Optional<com.google.common.collect.ImmutableMap<BuildTarget,​Version>> selectedVersions,
                                                  Class<U> metadataClass)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createMetadata` in
                interface `MetadataProvidingDescription<CxxLibraryDescriptionArg>`

        []{#addImplicitFlavors(com.google.common.collect.ImmutableSortedSet,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### addImplicitFlavors

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<Flavor> addImplicitFlavors​(com.google.common.collect.ImmutableSortedSet<Flavor> argDefaultFlavors,
                                                                                           TargetConfiguration toolchainTargetConfiguration)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `addImplicitFlavors` in
                interface `ImplicitFlavorsInferringDescription`

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
                interface `Description<CxxLibraryDescriptionArg>`

            [Specified by:]{.overrideSpecifyLabel}
            :   `producesCacheableSubgraph` in
                interface `DescriptionWithTargetGraph<CxxLibraryDescriptionArg>`
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
