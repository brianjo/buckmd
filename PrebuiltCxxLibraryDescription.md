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

## Class PrebuiltCxxLibraryDescription {#class-prebuiltcxxlibrarydescription .title title="Class PrebuiltCxxLibraryDescription"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.PrebuiltCxxLibraryDescription

::: description
-   

    All Implemented Interfaces:
    :   `ImplicitDepsInferringDescription<com.facebook.buck.cxx.PrebuiltCxxLibraryDescription.AbstractPrebuiltCxxLibraryDescriptionArg>`,
        `BaseDescription<PrebuiltCxxLibraryDescriptionArg>`,
        `Description<PrebuiltCxxLibraryDescriptionArg>`,
        `DescriptionWithTargetGraph<PrebuiltCxxLibraryDescriptionArg>`,
        `VersionPropagator<PrebuiltCxxLibraryDescriptionArg>`

    ------------------------------------------------------------------------

        public class PrebuiltCxxLibraryDescription
        extends Object
        implements DescriptionWithTargetGraph<PrebuiltCxxLibraryDescriptionArg>, ImplicitDepsInferringDescription<com.facebook.buck.cxx.PrebuiltCxxLibraryDescription.AbstractPrebuiltCxxLibraryDescriptionArg>, VersionPropagator<PrebuiltCxxLibraryDescriptionArg>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                      Description
          -------------------------------------------------------------------------------------------------------------------------------- -------------
          `PrebuiltCxxLibraryDescription​(ToolchainProvider toolchainProvider,                              CxxBuckConfig cxxBuckConfig)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `BuildRule`           | `createBui            | ::: block             |
        |                       | ldRule​(BuildRuleCreat | Create a              |
        |                       | ionContextWithTargetG | [`B                   |
        |                       | raph context,         | uildRule`](../core/ru |
        |                       |         BuildTarget b | les/BuildRule.html "i |
        |                       | uildTarget,           | nterface in com.faceb |
        |                       |       BuildRuleParams | ook.buck.core.rules") |
        |                       |  params,              | for the given         |
        |                       |    PrebuiltCxxLibrary | [`BuildRuleP          |
        |                       | DescriptionArg args)` | arams`](../core/rules |
        |                       |                       | /BuildRuleParams.html |
        |                       |                       |  "class in com.facebo |
        |                       |                       | ok.buck.core.rules"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `findDepsForTargetFr  |                       |
        |                       | omConstructorArgs​(Bui |                       |
        |                       | ldTarget buildTarget, |                       |
        |                       |                       |                       |
        |                       |                 CellN |                       |
        |                       | ameResolver cellRoots |                       |
        |                       | ,                     |                       |
        |                       |                  com. |                       |
        |                       | facebook.buck.cxx.Pre |                       |
        |                       | builtCxxLibraryDescri |                       |
        |                       | ption.AbstractPrebuil |                       |
        |                       | tCxxLibraryDescriptio |                       |
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
        | `Class<PrebuiltCxxLi  | `get                  | ::: block             |
        | braryDescriptionArg>` | ConstructorArgType()` | The type of the       |
        |                       |                       | constructor argument  |
        |                       |                       | that is used by this  |
        |                       |                       | description to create |
        |                       |                       | a rule                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `getSoname​(Buil       |                       |
        |                       | dTarget target,       |                       |
        |                       |     CxxPlatform cxxPl |                       |
        |                       | atform,          Opti |                       |
        |                       | onal<String> soname)` |                       |
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.toolchain.ToolchainProvider,com.facebook.buck.cxx.config.CxxBuckConfig)}

        -   #### PrebuiltCxxLibraryDescription

                public PrebuiltCxxLibraryDescription​(ToolchainProvider toolchainProvider,
                                                     CxxBuckConfig cxxBuckConfig)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getConstructorArgType()}

        -   #### getConstructorArgType

            ``` methodSignature
            public Class<PrebuiltCxxLibraryDescriptionArg> getConstructorArgType()
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
                interface `BaseDescription<PrebuiltCxxLibraryDescriptionArg>`

        []{#getSoname(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.cxx.toolchain.CxxPlatform,java.util.Optional)}

        -   #### getSoname

            ``` methodSignature
            public static String getSoname​(BuildTarget target,
                                           CxxPlatform cxxPlatform,
                                           Optional<String> soname)
            ```

        []{#createBuildRule(com.facebook.buck.core.rules.BuildRuleCreationContextWithTargetGraph,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.cxx.PrebuiltCxxLibraryDescriptionArg)}

        -   #### createBuildRule

            ``` methodSignature
            public BuildRule createBuildRule​(BuildRuleCreationContextWithTargetGraph context,
                                             BuildTarget buildTarget,
                                             BuildRuleParams params,
                                             PrebuiltCxxLibraryDescriptionArg args)
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
                interface `DescriptionWithTargetGraph<PrebuiltCxxLibraryDescriptionArg>`
            :   `args` - A constructor argument, of type as returned by
                [`BaseDescription.getConstructorArgType()`](../core/description/BaseDescription.html#getConstructorArgType()).

            [Returns:]{.returnLabel}
            :   The
                [`BuildRule`](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
                that describes the default flavour of the rule being
                described.

        []{#findDepsForTargetFromConstructorArgs(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.cxx.PrebuiltCxxLibraryDescription.AbstractPrebuiltCxxLibraryDescriptionArg,com.google.common.collect.ImmutableCollection.Builder,com.google.common.collect.ImmutableCollection.Builder)}

        -   #### findDepsForTargetFromConstructorArgs

            ``` methodSignature
            public void findDepsForTargetFromConstructorArgs​(BuildTarget buildTarget,
                                                             CellNameResolver cellRoots,
                                                             com.facebook.buck.cxx.PrebuiltCxxLibraryDescription.AbstractPrebuiltCxxLibraryDescriptionArg constructorArg,
                                                             com.google.common.collect.ImmutableCollection.Builder<BuildTarget> extraDepsBuilder,
                                                             com.google.common.collect.ImmutableCollection.Builder<BuildTarget> targetGraphOnlyDepsBuilder)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `findDepsForTargetFromConstructorArgs` in
                interface `ImplicitDepsInferringDescription<com.facebook.buck.cxx.PrebuiltCxxLibraryDescription.AbstractPrebuiltCxxLibraryDescriptionArg>`

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
                interface `Description<PrebuiltCxxLibraryDescriptionArg>`

            [Specified by:]{.overrideSpecifyLabel}
            :   `producesCacheableSubgraph` in
                interface `DescriptionWithTargetGraph<PrebuiltCxxLibraryDescriptionArg>`
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
