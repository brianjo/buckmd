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
[Package]{.packageLabelInType} [com.facebook.buck.core.toolchain](package-summary.html)
:::

## Interface ToolchainFactory\<T extends [Toolchain](Toolchain.html "interface in com.facebook.buck.core.toolchain")\> {#interface-toolchainfactoryt-extends-toolchain .title title="Interface ToolchainFactory"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `AdbToolchainFactory`, `AndroidBuildToolsLocationFactory`,
        `AndroidNdkFactory`, `AndroidPlatformTargetFactory`,
        `AndroidSdkLocationFactory`, `AppleCxxPlatformsProviderFactory`,
        `AppleDeveloperDirectoryForTestsProviderFactory`,
        `AppleDeveloperDirectoryProviderFactory`,
        `AppleSdkLocationFactory`, `AppleToolchainProviderFactory`,
        `CodeSignIdentityStoreFactory`, `CxxPlatformsProviderFactory`,
        `DotnetToolchainSupplier.DotnetToolchainFactory`,
        `DownloaderFactory`, `DxToolchainFactory`, `GoToolchainFactory`,
        `HaskellPlatformsProviderFactory`, `InferToolchainFactory`,
        `JavacOptionsProviderFactory`, `JavaCxxPlatformProviderFactory`,
        `JavaOptionsProviderFactory`, `JavaToolchainFactory`,
        `LuaPlatformsProviderFactory`, `NdkCxxPlatformsProviderFactory`,
        `OcamlToolchainFactory`, `PexToolProviderFactory`,
        `ProvisioningProfileStoreFactory`, `PythonInterpreterFactory`,
        `PythonPlatformsProviderFactory`, `RustToolchainFactory`,
        `SwiftPlatformsProviderFactory`

    ------------------------------------------------------------------------

        public interface ToolchainFactory<T extends Toolchain>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                                                                                     Description
          ------------------- -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `Optional<T>`       `createToolchain​(ToolchainProvider toolchainProvider,                ToolchainCreationContext context,                TargetConfiguration toolchainTargetConfiguration)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createToolchain(com.facebook.buck.core.toolchain.ToolchainProvider,com.facebook.buck.core.toolchain.ToolchainCreationContext,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### createToolchain

            ``` methodSignature
            Optional<T> createToolchain​(ToolchainProvider toolchainProvider,
                                        ToolchainCreationContext context,
                                        TargetConfiguration toolchainTargetConfiguration)
            ```

            [Throws:]{.throwsLabel}
            :   `ToolchainInstantiationException` - when a toolchain
                cannot be created
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
