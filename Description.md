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
[Package]{.packageLabelInType} [com.facebook.buck.core.description](package-summary.html)
:::

## Interface Description\<T extends [ConstructorArg](arg/ConstructorArg.html "interface in com.facebook.buck.core.description.arg")\> {#interface-descriptiont-extends-constructorarg .title title="Interface Description"}
:::

::: contentContainer
::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `T` - the argument type for the description to construct the
        [`BuildRule`](../rules/BuildRule.html "interface in com.facebook.buck.core.rules")

    ```{=html}
    <!-- -->
    ```

    All Superinterfaces:
    :   `BaseDescription<T>`

    ```{=html}
    <!-- -->
    ```

    All Known Subinterfaces:
    :   `DescriptionWithTargetGraph<T>`,
        `JsBundleOutputsDescription<T>`,
        `LegacyProviderCompatibleDescription<T>`, `RuleDescription<T>`,
        `RuleDescriptionWithInstanceName<T>`, `VersionPropagator<A>`,
        `VersionRoot<A>`

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
        `LegacyToolchainRuleDescription`, `LuaBinaryDescription`,
        `LuaLibraryDescription`, `NdkLibraryDescription`,
        `NdkToolchainDescription`, `OcamlBinaryDescription`,
        `OcamlLibraryDescription`, `PrebuiltAppleFrameworkDescription`,
        `PrebuiltCxxLibraryDescription`,
        `PrebuiltCxxLibraryGroupDescription`,
        `PrebuiltDotnetLibraryDescription`,
        `PrebuiltDotnetLibraryRuleDescription`,
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
        `ShTestDescription`, `SkylarkDescription`,
        `SwiftLibraryDescription`, `SwiftToolchainDescription`,
        `TestSuiteDescription`, `VersionedAliasDescription`,
        `WorkerToolDescription`, `XcodePostbuildScriptDescription`,
        `XcodePrebuildScriptDescription`,
        `XcodeWorkspaceConfigDescription`, `ZipFileDescription`

    ------------------------------------------------------------------------

        public interface Description<T extends ConstructorArg>
        extends BaseDescription<T>

    ::: block
    Contains information regarding a specific
    [`TargetNode`](../model/targetgraph/TargetNode.html "interface in com.facebook.buck.core.model.targetgraph")
    and the logic to create the corresponding
    [`BuildRule`](../rules/BuildRule.html "interface in com.facebook.buck.core.rules")
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `produce              | ::: block             |
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
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.BaseDescription}

            ### Methods inherited from interface com.facebook.buck.core.description.[BaseDescription](BaseDescription.html "interface in com.facebook.buck.core.description")

            `getConfigurationDeps, getConstructorArgType`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#producesCacheableSubgraph()}

        -   #### producesCacheableSubgraph

            ``` methodSignature
            boolean producesCacheableSubgraph()
            ```

            ::: block
            Whether or not the build rule subgraph produced by this
            `Description` is safe to cache in
            [`IncrementalActionGraphGenerator`](../model/actiongraph/computation/IncrementalActionGraphGenerator.html "class in com.facebook.buck.core.model.actiongraph.computation")
            for incremental action graph generation.
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
