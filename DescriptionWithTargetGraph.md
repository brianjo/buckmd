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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules](package-summary.html)
:::

## Interface DescriptionWithTargetGraph\<T extends [BuildRuleArg](../description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")\> {#interface-descriptionwithtargetgrapht-extends-buildrulearg .title title="Interface DescriptionWithTargetGraph"}
:::

::: contentContainer
::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `T` - The object describing the parameters to be passed to the
        [`BuildRule`](BuildRule.html "interface in com.facebook.buck.core.rules").
        How this is processed is described in the class level javadoc of
        [`ConstructorArgMarshaller`](../../rules/coercer/ConstructorArgMarshaller.html "interface in com.facebook.buck.rules.coercer").

    ```{=html}
    <!-- -->
    ```

    All Superinterfaces:
    :   `BaseDescription<T>`, `Description<T>`

    ```{=html}
    <!-- -->
    ```

    All Known Subinterfaces:
    :   `JsBundleOutputsDescription<T>`,
        `LegacyProviderCompatibleDescription<T>`,
        `VersionPropagator<A>`, `VersionRoot<A>`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AbstractGenruleDescription`, `AndroidAarDescription`,
        `AndroidAppModularityDescription`, `AndroidBinaryDescription`,
        `AndroidBuildConfigDescription`, `AndroidBundleDescription`,
        `AndroidInstrumentationApkDescription`,
        `AndroidInstrumentationTestDescription`,
        `AndroidLibraryDescription`, `AndroidManifestDescription`,
        `AndroidPrebuiltAarDescription`, `AndroidResourceDescription`,
        `ApkGenruleDescription`, `AppleAssetCatalogDescription`,
        `AppleBinaryDescription`, `AppleBundleDescription`,
        `AppleLibraryDescription`, `ApplePackageDescription`,
        `AppleResourceDescription`, `AppleTestDescription`,
        `AppleToolchainDescription`, `AppleToolchainSetDescription`,
        `CgoLibraryDescription`, `CommandAliasDescription`,
        `CoreDataModelDescription`, `CsharpLibraryDescription`,
        `CxxBinaryDescription`, `CxxGenruleDescription`,
        `CxxLibraryDescription`, `CxxLuaExtensionDescription`,
        `CxxPrecompiledHeaderDescription`,
        `CxxPythonExtensionDescription`, `CxxTestDescription`,
        `CxxToolchainDescription`, `DBinaryDescription`,
        `DLibraryDescription`, `DTestDescription`,
        `ExportFileDescription`, `ExternalTestRunnerDescription`,
        `FilegroupDescription`, `GenAidlDescription`,
        `GenruleDescription`, `GoBinaryDescription`,
        `GoLibraryDescription`, `GoTestDescription`,
        `GoTestRunnerDescription`, `GroovyLibraryDescription`,
        `GroovyTestDescription`, `GwtBinaryDescription`,
        `HalideLibraryDescription`, `HaskellBinaryDescription`,
        `HaskellGhciDescription`, `HaskellHaddockDescription`,
        `HaskellLibraryDescription`,
        `HaskellPrebuiltLibraryDescription`, `HttpArchiveDescription`,
        `HttpFileDescription`, `JarGenruleDescription`,
        `JavaAnnotationProcessorDescription`, `JavaBinaryDescription`,
        `JavaLibraryDescription`, `JavaPluginDescription`,
        `JavaTestDescription`, `JavaTestRunnerDescription`,
        `JsBundleDescription`, `JsBundleGenruleDescription`,
        `JsLibraryDescription`, `KeystoreDescription`,
        `KotlinLibraryDescription`, `KotlinTestDescription`,
        `LuaBinaryDescription`, `LuaLibraryDescription`,
        `NdkLibraryDescription`, `NdkToolchainDescription`,
        `OcamlBinaryDescription`, `OcamlLibraryDescription`,
        `PrebuiltAppleFrameworkDescription`,
        `PrebuiltCxxLibraryDescription`,
        `PrebuiltCxxLibraryGroupDescription`,
        `PrebuiltDotnetLibraryDescription`,
        `PrebuiltGoLibraryDescription`, `PrebuiltJarDescription`,
        `PrebuiltNativeLibraryDescription`,
        `PrebuiltOcamlLibraryDescription`,
        `PrebuiltPythonLibraryDescription`,
        `PrebuiltRustLibraryDescription`, `PythonBinaryDescription`,
        `PythonLibraryDescription`, `PythonTestDescription`,
        `PythonTestRunnerDescription`, `RemoteFileDescription`,
        `RobolectricTestDescription`, `RustBinaryDescription`,
        `RustLibraryDescription`, `RustTestDescription`,
        `ScalaLibraryDescription`, `ScalaTestDescription`,
        `SceneKitAssetsDescription`, `ShBinaryDescription`,
        `ShTestDescription`, `SwiftLibraryDescription`,
        `SwiftToolchainDescription`, `TestSuiteDescription`,
        `VersionedAliasDescription`, `WorkerToolDescription`,
        `XcodePostbuildScriptDescription`,
        `XcodePrebuildScriptDescription`,
        `XcodeWorkspaceConfigDescription`, `ZipFileDescription`

    ------------------------------------------------------------------------

        public interface DescriptionWithTargetGraph<T extends BuildRuleArg>
        extends Description<T>

    ::: block
    The Source of Truth about a
    [`BuildRule`](BuildRule.html "interface in com.facebook.buck.core.rules"),
    providing mechanisms to expose the arguments that rules derived from
    the Buildable take and providing a factory for those BuildRules. It
    is expected that instances of this class are stateless.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `BuildRule`           | `createBuildRule​(Buil | ::: block             |
        |                       | dRuleCreationContextW | Create a              |
        |                       | ithTargetGraph contex | [`BuildRul            |
        |                       | t,                Bui | e`](BuildRule.html "i |
        |                       | ldTarget buildTarget, | nterface in com.faceb |
        |                       |                 Build | ook.buck.core.rules") |
        |                       | RuleParams params,    | for the given         |
        |                       |              T args)` | [`BuildRuleParams`]   |
        |                       |                       | (BuildRuleParams.html |
        |                       |                       |  "class in com.facebo |
        |                       |                       | ok.buck.core.rules"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `produce              | ::: block             |
        |                       | sCacheableSubgraph()` | Whether or not the    |
        |                       |                       | build rule subgraph   |
        |                       |                       | produced by this      |
        |                       |                       | `Description` is safe |
        |                       |                       | to cache in           |
        |                       |                       | [`                    |
        |                       |                       | IncrementalActionGrap |
        |                       |                       | hGenerator`](../model |
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

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.BaseDescription}

            ### Methods inherited from interface com.facebook.buck.core.description.[BaseDescription](../description/BaseDescription.html "interface in com.facebook.buck.core.description")

            `getConfigurationDeps, getConstructorArgType`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createBuildRule(com.facebook.buck.core.rules.BuildRuleCreationContextWithTargetGraph,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.description.arg.BuildRuleArg)}
        []{#createBuildRule(com.facebook.buck.core.rules.BuildRuleCreationContextWithTargetGraph,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.BuildRuleParams,T)}

        -   #### createBuildRule

            ``` methodSignature
            BuildRule createBuildRule​(BuildRuleCreationContextWithTargetGraph context,
                                      BuildTarget buildTarget,
                                      BuildRuleParams params,
                                      T args)
            ```

            ::: block
            Create a
            [`BuildRule`](BuildRule.html "interface in com.facebook.buck.core.rules")
            for the given
            [`BuildRuleParams`](BuildRuleParams.html "class in com.facebook.buck.core.rules").
            Note that the
            [`BuildTarget`](../model/BuildTarget.html "class in com.facebook.buck.core.model")
            referred to in the `params` contains the
            [`Flavor`](../model/Flavor.html "interface in com.facebook.buck.core.model")
            to create.
            :::

            [Parameters:]{.paramLabel}
            :   `buildTarget` -
            :   `args` - A constructor argument, of type as returned by
                [`BaseDescription.getConstructorArgType()`](../description/BaseDescription.html#getConstructorArgType()).

            [Returns:]{.returnLabel}
            :   The
                [`BuildRule`](BuildRule.html "interface in com.facebook.buck.core.rules")
                that describes the default flavour of the rule being
                described.

        []{#producesCacheableSubgraph()}

        -   #### producesCacheableSubgraph

            ``` methodSignature
            default boolean producesCacheableSubgraph()
            ```

            ::: block
            Whether or not the build rule subgraph produced by this
            `Description` is safe to cache in
            [`IncrementalActionGraphGenerator`](../model/actiongraph/computation/IncrementalActionGraphGenerator.html "class in com.facebook.buck.core.model.actiongraph.computation")
            for incremental action graph generation.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `producesCacheableSubgraph` in
                interface `Description<T extends BuildRuleArg>`
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
