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

## Interface Toolchain {#interface-toolchain .title title="Interface Toolchain"}
:::

::: contentContainer
::: description
-   

    All Known Subinterfaces:
    :   `AdbToolchain`, `AndroidBuildToolsLocation`,
        `AndroidSdkLocation`, `AppleDeveloperDirectoryForTestsProvider`,
        `AppleDeveloperDirectoryProvider`, `AppleSdkLocation`,
        `AppleToolchainProvider`, `CodeSignIdentityStore`,
        `ComparableToolchain`, `CxxPlatformsSupplier`, `Downloader`,
        `DxToolchain`, `HaskellPlatformsProvider`, `InferToolchain`,
        `JavacOptionsProvider`, `JavaCxxPlatformProvider`,
        `JavaToolchain`, `LuaPlatformsProvider`, `PexToolProvider`,
        `PythonInterpreter`, `PythonPlatformsProvider`, `RustToolchain`,
        `SwiftPlatformsProvider`, `ToolchainWithCapability`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AndroidNdk`, `AndroidPlatformTarget`,
        `AppleCxxPlatformsProvider`, `BaseToolchain`,
        `CxxPlatformsProvider`, `DefaultPexToolProvider`,
        `ExplodingDownloader`, `GoToolchain`, `HttpDownloader`,
        `JavaOptionsProvider`, `NdkCxxPlatformsProvider`,
        `OnDiskMavenDownloader`, `ProvisioningProfileStore`,
        `PythonInterpreterFromConfig`, `RemoteMavenDownloader`,
        `RetryingDownloader`, `StackedDownloader`

    ------------------------------------------------------------------------

        public interface Toolchain

    ::: block
    Interface indicating that the class is a toolchain.
    Use
    [`ToolchainProvider`](ToolchainProvider.html "interface in com.facebook.buck.core.toolchain")
    to get a toolchain by a name.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method        Description
          ------------------- ------------- -------------
          `String`            `getName()`    

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

        []{#getName()}

        -   #### getName

            ``` methodSignature
            String getName()
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
