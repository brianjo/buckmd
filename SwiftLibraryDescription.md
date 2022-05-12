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
[Package]{.packageLabelInType} [com.facebook.buck.swift](package-summary.html)
:::

## Class SwiftLibraryDescription {#class-swiftlibrarydescription .title title="Class SwiftLibraryDescription"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.swift.SwiftLibraryDescription

::: description
-   

    All Implemented Interfaces:
    :   `ImplicitDepsInferringDescription<com.facebook.buck.swift.SwiftLibraryDescription.AbstractSwiftLibraryDescriptionArg>`,
        `BaseDescription<SwiftLibraryDescriptionArg>`,
        `Description<SwiftLibraryDescriptionArg>`, `Flavored`,
        `DescriptionWithTargetGraph<SwiftLibraryDescriptionArg>`

    ------------------------------------------------------------------------

        public class SwiftLibraryDescription
        extends Object
        implements DescriptionWithTargetGraph<SwiftLibraryDescriptionArg>, Flavored, ImplicitDepsInferringDescription<com.facebook.buck.swift.SwiftLibraryDescription.AbstractSwiftLibraryDescriptionArg>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                            Description
          ------------------- -------------------------------- -------------
          `static class `     `SwiftLibraryDescription.Type`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                  Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `SwiftLibraryDescription​(ToolchainProvider toolchainProvider,                        CxxBuckConfig cxxBuckConfig,                        SwiftBuckConfig swiftBuckConfig)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `BuildRule`           | `cre                  | ::: block             |
        |                       | ateBuildRule​(BuildRul | Create a              |
        |                       | eCreationContextWithT | [`B                   |
        |                       | argetGraph context,   | uildRule`](../core/ru |
        |                       |               BuildTa | les/BuildRule.html "i |
        |                       | rget buildTarget,     | nterface in com.faceb |
        |                       |             BuildRule | ook.buck.core.rules") |
        |                       | Params params,        | for the given         |
        |                       |          SwiftLibrary | [`BuildRuleP          |
        |                       | DescriptionArg args)` | arams`](../core/rules |
        |                       |                       | /BuildRuleParams.html |
        |                       |                       |  "class in com.facebo |
        |                       |                       | ok.buck.core.rules"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<BuildRule>` | `createCompani        |                       |
        |                       | onBuildRule​(BuildRule |                       |
        |                       | CreationContextWithTa |                       |
        |                       | rgetGraph context,    |                       |
        |                       |                       |                       |
        |                       |  BuildTarget buildTar |                       |
        |                       | get,                  |                       |
        |                       |         BuildRulePara |                       |
        |                       | ms params,            |                       |
        |                       |               ActionG |                       |
        |                       | raphBuilder graphBuil |                       |
        |                       | der,                  |                       |
        |                       |         CxxLibraryDes |                       |
        |                       | cription.CommonArg ar |                       |
        |                       | gs,                   |                       |
        |                       |        Optional<Strin |                       |
        |                       | g> targetSdkVersion)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static SwiftCompile` | `createSwiftCo        |                       |
        |                       | mpileRule​(CxxPlatform |                       |
        |                       |  cxxPlatform,         |                       |
        |                       |                SwiftP |                       |
        |                       | latform swiftPlatform |                       |
        |                       | ,                     |                       |
        |                       |    SwiftBuckConfig sw |                       |
        |                       | iftBuckConfig,        |                       |
        |                       |                 Build |                       |
        |                       | Target buildTarget,   |                       |
        |                       |                       |                       |
        |                       | ActionGraphBuilder gr |                       |
        |                       | aphBuilder,           |                       |
        |                       |              CellPath |                       |
        |                       | Resolver cellRoots,   |                       |
        |                       |                       |                       |
        |                       | ProjectFilesystem pro |                       |
        |                       | jectFilesystem,       |                       |
        |                       |                  Swif |                       |
        |                       | tLibraryDescriptionAr |                       |
        |                       | g args,               |                       |
        |                       |          Preprocessor |                       |
        |                       |  preprocessor,        |                       |
        |                       |                 Prepr |                       |
        |                       | ocessorFlags preproce |                       |
        |                       | ssFlags,              |                       |
        |                       |           boolean imp |                       |
        |                       | ortUnderlyingModule,  |                       |
        |                       |                       |                       |
        |                       |  Optional<SwiftTarget |                       |
        |                       | Triple> swiftTarget)` |                       |
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
        |                       | ck.swift.SwiftLibrary |                       |
        |                       | Description.AbstractS |                       |
        |                       | wiftLibraryDescriptio |                       |
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
        | `Class<SwiftLi        | `get                  | ::: block             |
        | braryDescriptionArg>` | ConstructorArgType()` | The type of the       |
        |                       |                       | constructor argument  |
        |                       |                       | that is used by this  |
        |                       |                       | description to create |
        |                       |                       | a rule                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.g                | `getSupportedFlavors  |                       |
        | oogle.common.collect. | ​(com.google.common.co |                       |
        | ImmutableSet<Flavor>` | llect.ImmutableSet<Fl |                       |
        |                       | avor> flavors,        |                       |
        |                       |              TargetCo |                       |
        |                       | nfiguration toolchain |                       |
        |                       | TargetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `h                    |                       |
        |                       | asFlavors​(com.google. |                       |
        |                       | common.collect.Immuta |                       |
        |                       | bleSet<Flavor> flavor |                       |
        |                       | s,           TargetCo |                       |
        |                       | nfiguration toolchain |                       |
        |                       | TargetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `isSwiftTarget​(Buil   |                       |
        |                       | dTarget buildTarget)` |                       |
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.toolchain.ToolchainProvider,com.facebook.buck.cxx.config.CxxBuckConfig,com.facebook.buck.swift.SwiftBuckConfig)}

        -   #### SwiftLibraryDescription

                public SwiftLibraryDescription​(ToolchainProvider toolchainProvider,
                                               CxxBuckConfig cxxBuckConfig,
                                               SwiftBuckConfig swiftBuckConfig)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#findDepsForTargetFromConstructorArgs(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.swift.SwiftLibraryDescription.AbstractSwiftLibraryDescriptionArg,com.google.common.collect.ImmutableCollection.Builder,com.google.common.collect.ImmutableCollection.Builder)}

        -   #### findDepsForTargetFromConstructorArgs

            ``` methodSignature
            public void findDepsForTargetFromConstructorArgs​(BuildTarget buildTarget,
                                                             CellNameResolver cellRoots,
                                                             com.facebook.buck.swift.SwiftLibraryDescription.AbstractSwiftLibraryDescriptionArg constructorArg,
                                                             com.google.common.collect.ImmutableCollection.Builder<BuildTarget> extraDepsBuilder,
                                                             com.google.common.collect.ImmutableCollection.Builder<BuildTarget> targetGraphOnlyDepsBuilder)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `findDepsForTargetFromConstructorArgs` in
                interface `ImplicitDepsInferringDescription<com.facebook.buck.swift.SwiftLibraryDescription.AbstractSwiftLibraryDescriptionArg>`

        []{#getConstructorArgType()}

        -   #### getConstructorArgType

            ``` methodSignature
            public Class<SwiftLibraryDescriptionArg> getConstructorArgType()
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
                interface `BaseDescription<SwiftLibraryDescriptionArg>`

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

        []{#createBuildRule(com.facebook.buck.core.rules.BuildRuleCreationContextWithTargetGraph,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.swift.SwiftLibraryDescriptionArg)}

        -   #### createBuildRule

            ``` methodSignature
            public BuildRule createBuildRule​(BuildRuleCreationContextWithTargetGraph context,
                                             BuildTarget buildTarget,
                                             BuildRuleParams params,
                                             SwiftLibraryDescriptionArg args)
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
                interface `DescriptionWithTargetGraph<SwiftLibraryDescriptionArg>`
            :   `args` - A constructor argument, of type as returned by
                [`BaseDescription.getConstructorArgType()`](../core/description/BaseDescription.html#getConstructorArgType()).

            [Returns:]{.returnLabel}
            :   The
                [`BuildRule`](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
                that describes the default flavour of the rule being
                described.

        []{#createCompanionBuildRule(com.facebook.buck.core.rules.BuildRuleCreationContextWithTargetGraph,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.cxx.CxxLibraryDescription.CommonArg,java.util.Optional)}

        -   #### createCompanionBuildRule

            ``` methodSignature
            public Optional<BuildRule> createCompanionBuildRule​(BuildRuleCreationContextWithTargetGraph context,
                                                                BuildTarget buildTarget,
                                                                BuildRuleParams params,
                                                                ActionGraphBuilder graphBuilder,
                                                                CxxLibraryDescription.CommonArg args,
                                                                Optional<String> targetSdkVersion)
            ```

        []{#createSwiftCompileRule(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.swift.toolchain.SwiftPlatform,com.facebook.buck.swift.SwiftBuckConfig,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.cell.CellPathResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.swift.SwiftLibraryDescriptionArg,com.facebook.buck.cxx.toolchain.Preprocessor,com.facebook.buck.cxx.PreprocessorFlags,boolean,java.util.Optional)}

        -   #### createSwiftCompileRule

            ``` methodSignature
            public static SwiftCompile createSwiftCompileRule​(CxxPlatform cxxPlatform,
                                                              SwiftPlatform swiftPlatform,
                                                              SwiftBuckConfig swiftBuckConfig,
                                                              BuildTarget buildTarget,
                                                              ActionGraphBuilder graphBuilder,
                                                              CellPathResolver cellRoots,
                                                              ProjectFilesystem projectFilesystem,
                                                              SwiftLibraryDescriptionArg args,
                                                              Preprocessor preprocessor,
                                                              PreprocessorFlags preprocessFlags,
                                                              boolean importUnderlyingModule,
                                                              Optional<SwiftTargetTriple> swiftTarget)
            ```

        []{#isSwiftTarget(com.facebook.buck.core.model.BuildTarget)}

        -   #### isSwiftTarget

            ``` methodSignature
            public static boolean isSwiftTarget​(BuildTarget buildTarget)
            ```

        []{#getSupportedFlavors(com.google.common.collect.ImmutableSet,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getSupportedFlavors

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<Flavor> getSupportedFlavors​(com.google.common.collect.ImmutableSet<Flavor> flavors,
                                                                                      TargetConfiguration toolchainTargetConfiguration)
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
