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

## Interface BaseDescription\<T extends [ConstructorArg](arg/ConstructorArg.html "interface in com.facebook.buck.core.description.arg")\> {#interface-basedescriptiont-extends-constructorarg .title title="Interface BaseDescription"}
:::

::: contentContainer
::: description
-   

    All Known Subinterfaces:
    :   `ConfigurationRuleDescription<T,​R>`, `Description<T>`,
        `DescriptionWithTargetGraph<T>`,
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
        `AndroidPlatformDescription`, `AndroidPrebuiltAarDescription`,
        `AndroidResourceDescription`, `ApkGenruleDescription`,
        `AppleAssetCatalogDescription`, `AppleBinaryDescription`,
        `AppleBundleDescription`, `AppleLibraryDescription`,
        `ApplePackageDescription`, `AppleResourceDescription`,
        `AppleTestDescription`, `AppleToolchainDescription`,
        `AppleToolchainSetDescription`, `CgoLibraryDescription`,
        `CommandAliasDescription`, `ConfigSettingDescription`,
        `ConstraintSettingDescription`, `ConstraintValueDescription`,
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
        `OcamlLibraryDescription`, `PlatformDescription`,
        `PrebuiltAppleFrameworkDescription`,
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

        public interface BaseDescription<T extends ConstructorArg>

    ::: block
    Description common to both build and config rule types.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `default com.google   | `getConf              |                       |
        | .common.collect.Immut | igurationDeps​(T arg)` |                       |
        | ableSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Class<T>`            | `get                  | ::: block             |
        |                       | ConstructorArgType()` | The type of the       |
        |                       |                       | constructor argument  |
        |                       |                       | that is used by this  |
        |                       |                       | description to create |
        |                       |                       | a rule                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getConstructorArgType()}

        -   #### getConstructorArgType

            ``` methodSignature
            Class<T> getConstructorArgType()
            ```

            ::: block
            The type of the constructor argument that is used by this
            description to create a rule
            :::

        []{#getConfigurationDeps(com.facebook.buck.core.description.arg.ConstructorArg)}
        []{#getConfigurationDeps(T)}

        -   #### getConfigurationDeps

            ``` methodSignature
            default com.google.common.collect.ImmutableSet<BuildTarget> getConfigurationDeps​(T arg)
            ```

            [Returns:]{.returnLabel}
            :   a set of configuration targets declared in a given
                constructor argument.
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
