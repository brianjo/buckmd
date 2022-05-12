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

## Class AppleTestDescription {#class-appletestdescription .title title="Class AppleTestDescription"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.AppleTestDescription

::: description
-   

    All Implemented Interfaces:
    :   `AppleLibrarySwiftDelegate`,
        `ImplicitDepsInferringDescription<com.facebook.buck.apple.AppleTestDescription.AbstractAppleTestDescriptionArg>`,
        `BaseDescription<AppleTestDescriptionArg>`,
        `Description<AppleTestDescriptionArg>`,
        `MetadataProvidingDescription<AppleTestDescriptionArg>`,
        `Flavored`,
        `DescriptionWithTargetGraph<AppleTestDescriptionArg>`

    ------------------------------------------------------------------------

        public class AppleTestDescription
        extends Object
        implements DescriptionWithTargetGraph<AppleTestDescriptionArg>, Flavored, ImplicitDepsInferringDescription<com.facebook.buck.apple.AppleTestDescription.AbstractAppleTestDescriptionArg>, MetadataProvidingDescription<AppleTestDescriptionArg>, AppleLibrarySwiftDelegate
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type     Field            Description
          --------------------- ---------------- -------------
          `static UserFlavor`   `COMPILE_DEPS`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                    Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `AppleTestDescription​(ToolchainProvider toolchainProvider,                     XCodeDescriptions xcodeDescriptions,                     AppleConfig appleConfig,                     CxxBuckConfig cxxBuckConfig,                     SwiftBuckConfig swiftBuckConfig,                     AppleLibraryDescription appleLibraryDescription)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `BuildRule`           | `                     | ::: block             |
        |                       | createBuildRule​(Build | Create a              |
        |                       | RuleCreationContextWi | [`B                   |
        |                       | thTargetGraph context | uildRule`](../core/ru |
        |                       | ,                Buil | les/BuildRule.html "i |
        |                       | dTarget buildTarget,  | nterface in com.faceb |
        |                       |                BuildR | ook.buck.core.rules") |
        |                       | uleParams params,     | for the given         |
        |                       |             AppleTest | [`BuildRuleP          |
        |                       | DescriptionArg args)` | arams`](../core/rules |
        |                       |                       | /BuildRuleParams.html |
        |                       |                       |  "class in com.facebo |
        |                       |                       | ok.buck.core.rules"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `<U> Optional<U>`     | `createMetadata​(Buil  |                       |
        |                       | dTarget buildTarget,  |                       |
        |                       |               ActionG |                       |
        |                       | raphBuilder graphBuil |                       |
        |                       | der,               Ce |                       |
        |                       | llPathResolver cellRo |                       |
        |                       | ots,               Ap |                       |
        |                       | pleTestDescriptionArg |                       |
        |                       |  args,                |                       |
        |                       | Optional<com.google.c |                       |
        |                       | ommon.collect.Immutab |                       |
        |                       | leMap<BuildTarget,​Ver |                       |
        |                       | sion>> selectedVersio |                       |
        |                       | ns,               Cla |                       |
        |                       | ss<U> metadataClass)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `fin                  |                       |
        |                       | dDepsForTargetFromCon |                       |
        |                       | structorArgs​(BuildTar |                       |
        |                       | get buildTarget,      |                       |
        |                       |                       |                       |
        |                       |            CellNameRe |                       |
        |                       | solver cellRoots,     |                       |
        |                       |                       |                       |
        |                       |             com.faceb |                       |
        |                       | ook.buck.apple.AppleT |                       |
        |                       | estDescription.Abstra |                       |
        |                       | ctAppleTestDescriptio |                       |
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
        | `Class<Appl           | `get                  | ::: block             |
        | eTestDescriptionArg>` | ConstructorArgType()` | The type of the       |
        |                       |                       | constructor argument  |
        |                       |                       | that is used by this  |
        |                       |                       | description to create |
        |                       |                       | a rule                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.c  | `get                  |                       |
        | ollect.ImmutableSet<C | PreprocessorInputForS |                       |
        | xxPreprocessorInput>` | wift​(BuildTarget buil |                       |
        |                       | dTarget,              |                       |
        |                       |                 Actio |                       |
        |                       | nGraphBuilder graphBu |                       |
        |                       | ilder,                |                       |
        |                       |               CxxPlat |                       |
        |                       | form cxxPlatform,     |                       |
        |                       |                       |                       |
        |                       |     CxxLibraryDescrip |                       |
        |                       | tion.CommonArg args)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `h                    |                       |
        |                       | asFlavors​(com.google. |                       |
        |                       | common.collect.Immuta |                       |
        |                       | bleSet<Flavor> flavor |                       |
        |                       | s,           TargetCo |                       |
        |                       | nfiguration toolchain |                       |
        |                       | TargetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
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

        []{#COMPILE_DEPS}

        -   #### COMPILE_DEPS

                public static final UserFlavor COMPILE_DEPS
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.toolchain.ToolchainProvider,com.facebook.buck.apple.XCodeDescriptions,com.facebook.buck.apple.AppleConfig,com.facebook.buck.cxx.config.CxxBuckConfig,com.facebook.buck.swift.SwiftBuckConfig,com.facebook.buck.apple.AppleLibraryDescription)}

        -   #### AppleTestDescription

                public AppleTestDescription​(ToolchainProvider toolchainProvider,
                                            XCodeDescriptions xcodeDescriptions,
                                            AppleConfig appleConfig,
                                            CxxBuckConfig cxxBuckConfig,
                                            SwiftBuckConfig swiftBuckConfig,
                                            AppleLibraryDescription appleLibraryDescription)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getConstructorArgType()}

        -   #### getConstructorArgType

            ``` methodSignature
            public Class<AppleTestDescriptionArg> getConstructorArgType()
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
                interface `BaseDescription<AppleTestDescriptionArg>`

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

        []{#createBuildRule(com.facebook.buck.core.rules.BuildRuleCreationContextWithTargetGraph,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.apple.AppleTestDescriptionArg)}

        -   #### createBuildRule

            ``` methodSignature
            public BuildRule createBuildRule​(BuildRuleCreationContextWithTargetGraph context,
                                             BuildTarget buildTarget,
                                             BuildRuleParams params,
                                             AppleTestDescriptionArg args)
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
                interface `DescriptionWithTargetGraph<AppleTestDescriptionArg>`
            :   `args` - A constructor argument, of type as returned by
                [`BaseDescription.getConstructorArgType()`](../core/description/BaseDescription.html#getConstructorArgType()).

            [Returns:]{.returnLabel}
            :   The
                [`BuildRule`](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
                that describes the default flavour of the rule being
                described.

        []{#findDepsForTargetFromConstructorArgs(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.apple.AppleTestDescription.AbstractAppleTestDescriptionArg,com.google.common.collect.ImmutableCollection.Builder,com.google.common.collect.ImmutableCollection.Builder)}

        -   #### findDepsForTargetFromConstructorArgs

            ``` methodSignature
            public void findDepsForTargetFromConstructorArgs​(BuildTarget buildTarget,
                                                             CellNameResolver cellRoots,
                                                             com.facebook.buck.apple.AppleTestDescription.AbstractAppleTestDescriptionArg constructorArg,
                                                             com.google.common.collect.ImmutableCollection.Builder<BuildTarget> extraDepsBuilder,
                                                             com.google.common.collect.ImmutableCollection.Builder<BuildTarget> targetGraphOnlyDepsBuilder)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `findDepsForTargetFromConstructorArgs` in
                interface `ImplicitDepsInferringDescription<com.facebook.buck.apple.AppleTestDescription.AbstractAppleTestDescriptionArg>`

        []{#createMetadata(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.cell.CellPathResolver,com.facebook.buck.apple.AppleTestDescriptionArg,java.util.Optional,java.lang.Class)}

        -   #### createMetadata

            ``` methodSignature
            public <U> Optional<U> createMetadata​(BuildTarget buildTarget,
                                                  ActionGraphBuilder graphBuilder,
                                                  CellPathResolver cellRoots,
                                                  AppleTestDescriptionArg args,
                                                  Optional<com.google.common.collect.ImmutableMap<BuildTarget,​Version>> selectedVersions,
                                                  Class<U> metadataClass)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createMetadata` in
                interface `MetadataProvidingDescription<AppleTestDescriptionArg>`

        []{#getPreprocessorInputForSwift(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.cxx.CxxLibraryDescription.CommonArg)}

        -   #### getPreprocessorInputForSwift

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<CxxPreprocessorInput> getPreprocessorInputForSwift​(BuildTarget buildTarget,
                                                                                                             ActionGraphBuilder graphBuilder,
                                                                                                             CxxPlatform cxxPlatform,
                                                                                                             CxxLibraryDescription.CommonArg args)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPreprocessorInputForSwift` in
                interface `AppleLibrarySwiftDelegate`
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
