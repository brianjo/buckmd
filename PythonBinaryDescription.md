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
[Package]{.packageLabelInType} [com.facebook.buck.features.python](package-summary.html)
:::

## Class PythonBinaryDescription {#class-pythonbinarydescription .title title="Class PythonBinaryDescription"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.python.PythonBinaryDescription

::: description
-   

    All Implemented Interfaces:
    :   `ImplicitDepsInferringDescription<com.facebook.buck.features.python.PythonBinaryDescription.AbstractPythonBinaryDescriptionArg>`,
        `BaseDescription<PythonBinaryDescriptionArg>`,
        `Description<PythonBinaryDescriptionArg>`,
        `DescriptionWithTargetGraph<PythonBinaryDescriptionArg>`,
        `VersionRoot<PythonBinaryDescriptionArg>`

    ------------------------------------------------------------------------

        public class PythonBinaryDescription
        extends Object
        implements DescriptionWithTargetGraph<PythonBinaryDescriptionArg>, ImplicitDepsInferringDescription<com.facebook.buck.features.python.PythonBinaryDescription.AbstractPythonBinaryDescriptionArg>, VersionRoot<PythonBinaryDescriptionArg>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                    Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `PythonBinaryDescription​(ToolchainProvider toolchainProvider,                        PythonBuckConfig pythonBuckConfig,                        CxxBuckConfig cxxBuckConfig)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `                     | `addM                 |                       |
        | static com.google.com | issingInitModules​(com |                       |
        | mon.collect.Immutable | .google.common.collec |                       |
        | Map<Path,​SourcePath>` | t.ImmutableMap<Path,​S |                       |
        |                       | ourcePath> modules,   |                       |
        |                       |                     S |                       |
        |                       | ourcePath emptyInit)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `PythonBinary`        | `cre                  | ::: block             |
        |                       | ateBuildRule​(BuildRul | Create a              |
        |                       | eCreationContextWithT | [`Buil                |
        |                       | argetGraph context,   | dRule`](../../core/ru |
        |                       |               BuildTa | les/BuildRule.html "i |
        |                       | rget buildTarget,     | nterface in com.faceb |
        |                       |             BuildRule | ook.buck.core.rules") |
        |                       | Params params,        | for the given         |
        |                       |          PythonBinary | [`BuildRulePara       |
        |                       | DescriptionArg args)` | ms`](../../core/rules |
        |                       |                       | /BuildRuleParams.html |
        |                       |                       |  "class in com.facebo |
        |                       |                       | ok.buck.core.rules"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static SourcePath`   | `createEmptyI         |                       |
        |                       | nitModule​(BuildTarget |                       |
        |                       |  buildTarget,         |                       |
        |                       |               Project |                       |
        |                       | Filesystem projectFil |                       |
        |                       | esystem,              |                       |
        |                       |          ActionGraphB |                       |
        |                       | uilder graphBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `findDepsForTargetFr  |                       |
        |                       | omConstructorArgs​(Bui |                       |
        |                       | ldTarget buildTarget, |                       |
        |                       |                       |                       |
        |                       |                 CellN |                       |
        |                       | ameResolver cellRoots |                       |
        |                       | ,                     |                       |
        |                       |                  com. |                       |
        |                       | facebook.buck.feature |                       |
        |                       | s.python.PythonBinary |                       |
        |                       | Description.AbstractP |                       |
        |                       | ythonBinaryDescriptio |                       |
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
        | `Class<PythonB        | `get                  | ::: block             |
        | inaryDescriptionArg>` | ConstructorArgType()` | The type of the       |
        |                       |                       | constructor argument  |
        |                       |                       | that is used by this  |
        |                       |                       | description to create |
        |                       |                       | a rule                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static BuildTarget`  | `g                    |                       |
        |                       | etEmptyInitTarget​(Bui |                       |
        |                       | ldTarget baseTarget)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `produce              | ::: block             |
        |                       | sCacheableSubgraph()` | Whether or not the    |
        |                       |                       | build rule subgraph   |
        |                       |                       | produced by this      |
        |                       |                       | `Description` is safe |
        |                       |                       | to cache in           |
        |                       |                       | [`Incremen            |
        |                       |                       | talActionGraphGenerat |
        |                       |                       | or`](../../core/model |
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

            ### Methods inherited from interface com.facebook.buck.core.description.[BaseDescription](../../core/description/BaseDescription.html "interface in com.facebook.buck.core.description")

            `getConfigurationDeps`

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

        []{#<init>(com.facebook.buck.core.toolchain.ToolchainProvider,com.facebook.buck.features.python.PythonBuckConfig,com.facebook.buck.cxx.config.CxxBuckConfig)}

        -   #### PythonBinaryDescription

                public PythonBinaryDescription​(ToolchainProvider toolchainProvider,
                                               PythonBuckConfig pythonBuckConfig,
                                               CxxBuckConfig cxxBuckConfig)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getConstructorArgType()}

        -   #### getConstructorArgType

            ``` methodSignature
            public Class<PythonBinaryDescriptionArg> getConstructorArgType()
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
                interface `BaseDescription<PythonBinaryDescriptionArg>`

        []{#getEmptyInitTarget(com.facebook.buck.core.model.BuildTarget)}

        -   #### getEmptyInitTarget

            ``` methodSignature
            public static BuildTarget getEmptyInitTarget​(BuildTarget baseTarget)
            ```

        []{#createEmptyInitModule(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### createEmptyInitModule

            ``` methodSignature
            public static SourcePath createEmptyInitModule​(BuildTarget buildTarget,
                                                           ProjectFilesystem projectFilesystem,
                                                           ActionGraphBuilder graphBuilder)
            ```

        []{#addMissingInitModules(com.google.common.collect.ImmutableMap,com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addMissingInitModules

            ``` methodSignature
            public static com.google.common.collect.ImmutableMap<Path,​SourcePath> addMissingInitModules​(com.google.common.collect.ImmutableMap<Path,​SourcePath> modules,
                                                                                                              SourcePath emptyInit)
            ```

        []{#createBuildRule(com.facebook.buck.core.rules.BuildRuleCreationContextWithTargetGraph,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.features.python.PythonBinaryDescriptionArg)}

        -   #### createBuildRule

            ``` methodSignature
            public PythonBinary createBuildRule​(BuildRuleCreationContextWithTargetGraph context,
                                                BuildTarget buildTarget,
                                                BuildRuleParams params,
                                                PythonBinaryDescriptionArg args)
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
                interface `DescriptionWithTargetGraph<PythonBinaryDescriptionArg>`
            :   `args` - A constructor argument, of type as returned by
                [`BaseDescription.getConstructorArgType()`](../../core/description/BaseDescription.html#getConstructorArgType()).

            [Returns:]{.returnLabel}
            :   The
                [`BuildRule`](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
                that describes the default flavour of the rule being
                described.

        []{#findDepsForTargetFromConstructorArgs(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.features.python.PythonBinaryDescription.AbstractPythonBinaryDescriptionArg,com.google.common.collect.ImmutableCollection.Builder,com.google.common.collect.ImmutableCollection.Builder)}

        -   #### findDepsForTargetFromConstructorArgs

            ``` methodSignature
            public void findDepsForTargetFromConstructorArgs​(BuildTarget buildTarget,
                                                             CellNameResolver cellRoots,
                                                             com.facebook.buck.features.python.PythonBinaryDescription.AbstractPythonBinaryDescriptionArg constructorArg,
                                                             com.google.common.collect.ImmutableCollection.Builder<BuildTarget> extraDepsBuilder,
                                                             com.google.common.collect.ImmutableCollection.Builder<BuildTarget> targetGraphOnlyDepsBuilder)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `findDepsForTargetFromConstructorArgs` in
                interface `ImplicitDepsInferringDescription<com.facebook.buck.features.python.PythonBinaryDescription.AbstractPythonBinaryDescriptionArg>`

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
            [`IncrementalActionGraphGenerator`](../../core/model/actiongraph/computation/IncrementalActionGraphGenerator.html "class in com.facebook.buck.core.model.actiongraph.computation")
            for incremental action graph generation.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `producesCacheableSubgraph` in
                interface `Description<PythonBinaryDescriptionArg>`

            [Specified by:]{.overrideSpecifyLabel}
            :   `producesCacheableSubgraph` in
                interface `DescriptionWithTargetGraph<PythonBinaryDescriptionArg>`
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
