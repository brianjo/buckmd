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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.apple](package-summary.html)
:::

## Class AppleConfig {#class-appleconfig .title title="Class AppleConfig"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.AppleConfig

::: description
-   

    All Implemented Interfaces:
    :   `ConfigView<BuckConfig>`

    ------------------------------------------------------------------------

        public class AppleConfig
        extends Object
        implements ConfigView<BuckConfig>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                          Field                          Description
          ---------------------------------------------------------- ------------------------------ -------------
          `static String`                                            `APPLE_SECTION`                 
          `static String`                                            `BUILD_SCRIPT`                  
          `static com.google.common.collect.ImmutableList<String>`   `DEFAULT_IDENTITIES_COMMAND`    
          `static com.google.common.collect.ImmutableList<String>`   `DEFAULT_READ_COMMAND`          
          `static String`                                            `LINK_SCRUB_CONCURRENTLY`       

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `addCe                |                       |
        |                       | llPathToIquotePath()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `AppleAssetCa         | `asse                 |                       |
        | talog.ValidationType` | tCatalogValidation()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `buildScriptPath()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `cache                |                       |
        |                       | BundlesAndPackages()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ja                   | `getAp                | ::: block             |
        | va.util.function.Supp | pleDeveloperDirectory | If specified, the     |
        | lier<Optional<Path>>` | Supplier​(ProcessExecu | value of              |
        |                       | tor processExecutor)` | `[apple]              |
        |                       |                       |  xcode_developer_dir` |
        |                       |                       | wrapped in a          |
        |                       |                       | `Supplier`.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Path>`      | `getAppleDevice       |                       |
        |                       | HelperAbsolutePath()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `O                    | `getAppleDeviceH      | ::: block             |
        | ptional<BuildTarget>` | elperTarget​(Optional< | Query buckconfig for  |
        |                       | TargetConfiguration>  | device helper target. |
        |                       | targetConfiguration)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `O                    | `getAp                |                       |
        | ptional<BuildTarget>` | pleToolchainSetTarget |                       |
        |                       | ​(TargetConfiguration  |                       |
        |                       | targetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getCodeSig           |                       |
        | ogle.common.collect.I | nIdentitiesCommand()` |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ToolProvider`        | `g                    |                       |
        |                       | etCodesignProvider()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `java.time.Duration`  | `                     | ::: block             |
        |                       | getCodesignTimeout()` | Specify the maximum   |
        |                       |                       | code-signing time     |
        |                       |                       | before timing out.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleDebugFormat`    | `getDefaultDebugInf   |                       |
        |                       | oFormatForBinaries()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `AppleDebugFormat`    | `getDefaultDebugInfo  |                       |
        |                       | FormatForLibraries()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `AppleDebugFormat`    | `getDefaultDebug      |                       |
        |                       | InfoFormatForTests()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuckConfig`          | `getDelegate()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.                 | `get                  |                       |
        | google.common.collect | ExtraPlatformPaths()` |                       |
        | .ImmutableList<Path>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.                 | `getE                 |                       |
        | google.common.collect | xtraToolchainPaths()` |                       |
        | .ImmutableList<Path>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getForc              |                       |
        |                       | eLoadLibraryPath​(bool |                       |
        |                       | ean isFocusedTarget)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getIdbPath()`        | ::: block             |
        |                       |                       | Gets the path to the  |
        |                       |                       | executable file of    |
        |                       |                       | idb                   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Op                   | `getPackage           | ::: block             |
        | tional<com.facebook.b | ConfigForPlatform​(App | Returns the custom    |
        | uck.apple.AppleConfig | lePlatform platform)` | packager command      |
        | .ApplePackageConfig>` |                       | specified in the      |
        |                       |                       | config, if defined.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getProvisioning      |                       |
        | ogle.common.collect.I | ProfileReadCommand()` |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getProvisionin       |                       |
        |                       | gProfileSearchPath()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `ge                   |                       |
        |                       | tTargetSdkVersion​(App |                       |
        |                       | lePlatform platform)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getTestLogDirectoryE |                       |
        |                       | nvironmentVariable()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getTestLogLevel()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getTestLogLevelE     |                       |
        |                       | nvironmentVariable()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<com.goo     | `get                  |                       |
        | gle.common.collect.Im | ToolchainsOverrideFor |                       |
        | mutableList<String>>` | SDKName​(String name)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getXcodeDevelope     |                       |
        |                       | rDirectoryForTests()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getXcodeDisab        |                       |
        |                       | leParallelizeBuild()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getXcodeToolN        |                       |
        |                       | ame​(String toolName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Path>`      | `getXcodeToolReplacem |                       |
        |                       | ent​(String toolName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getXcodeToolVersion​( |                       |
        |                       | String toolName,      |                       |
        |                       |                String |                       |
        |                       |  defaultToolVersion)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getX                 |                       |
        | ogle.common.collect.I | ctestPlatformNames()` |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getXctoolDefaultDe   |                       |
        |                       | stinationSpecifier()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Path>`      | `getXctoolPath()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Long>`      | `getXcto              |                       |
        |                       | olStutterTimeoutMs()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `O                    | `getXctoolZipTarget   |                       |
        | ptional<BuildTarget>` | ​(TargetConfiguration  |                       |
        |                       | targetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ZipCompressionLevel` | `getZ                 |                       |
        |                       | ipCompressionLevel()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `linkAllObjC()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ModuleMapMode`       | `moduleMapMode()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static AppleConfig`  | `of​(                  |                       |
        |                       | BuckConfig delegate)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `shellPath()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `shouldAddLink        |                       |
        |                       | edLibrariesAsFlags()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `sh                   |                       |
        |                       | ouldAddLinkerFlagsFor |                       |
        |                       | LinkWholeLibraries()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `shouldGenerateHead   |                       |
        |                       | erSymlinkTreesOnly()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `shouldGenerateMiss   |                       |
        |                       | ingUmbrellaHeaders()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `shouldIncludeShar    |                       |
        |                       | edLibraryResources()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `shouldLin            |                       |
        |                       | kScrubConcurrently()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `sho                  |                       |
        |                       | uldLinkSystemSwift()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `shouldMergeHeader    |                       |
        |                       | MapsInXcodeProject()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `shouldUseHeader      |                       |
        |                       | MapsInXcodeProject()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `shouldUs             |                       |
        |                       | eModernBuildSystem()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `shou                 |                       |
        |                       | ldUseSwiftDelegate()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `shouldVer            |                       |
        |                       | ifyBundleResources()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `shou                 |                       |
        |                       | ldWorkAroundDsymutilL |                       |
        |                       | TOStackOverflowBug()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `us                   |                       |
        |                       | eDryRunCodeSigning()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `useEntitlementsWh    |                       |
        |                       | enAdhocCodeSigning()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `useF                 |                       |
        |                       | lavoredCxxSections()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `useIdb()`            | ::: block             |
        |                       |                       | Determines whether to |
        |                       |                       | use idb install       |
        |                       |                       | functions or simctl;  |
        |                       |                       | current default is to |
        |                       |                       | not use idb           |
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
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#DEFAULT_IDENTITIES_COMMAND}

        -   #### DEFAULT_IDENTITIES_COMMAND

                public static final com.google.common.collect.ImmutableList<String> DEFAULT_IDENTITIES_COMMAND

        []{#DEFAULT_READ_COMMAND}

        -   #### DEFAULT_READ_COMMAND

                public static final com.google.common.collect.ImmutableList<String> DEFAULT_READ_COMMAND

        []{#APPLE_SECTION}

        -   #### APPLE_SECTION

                public static final String APPLE_SECTION

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.apple.AppleConfig.APPLE_SECTION)

        []{#BUILD_SCRIPT}

        -   #### BUILD_SCRIPT

                public static final String BUILD_SCRIPT

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.apple.AppleConfig.BUILD_SCRIPT)

        []{#LINK_SCRUB_CONCURRENTLY}

        -   #### LINK_SCRUB_CONCURRENTLY

                public static final String LINK_SCRUB_CONCURRENTLY

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.apple.AppleConfig.LINK_SCRUB_CONCURRENTLY)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#of(com.facebook.buck.core.config.BuckConfig)}

        -   #### of

            ``` methodSignature
            public static AppleConfig of​(BuckConfig delegate)
            ```

        []{#getDelegate()}

        -   #### getDelegate

            ``` methodSignature
            public BuckConfig getDelegate()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDelegate` in interface `ConfigView<BuckConfig>`

        []{#getAppleDeveloperDirectorySupplier(com.facebook.buck.util.ProcessExecutor)}

        -   #### getAppleDeveloperDirectorySupplier

            ``` methodSignature
            public java.util.function.Supplier<Optional<Path>> getAppleDeveloperDirectorySupplier​(ProcessExecutor processExecutor)
            ```

            ::: block
            If specified, the value of `[apple] xcode_developer_dir`
            wrapped in a `Supplier`. Otherwise, this returns a
            `Supplier` that lazily runs `xcode-select --print-path` and
            caches the result.
            :::

        []{#getIdbPath()}

        -   #### getIdbPath

            ``` methodSignature
            public Path getIdbPath()
            ```

            ::: block
            Gets the path to the executable file of idb
            :::

            [Returns:]{.returnLabel}
            :   a custom path if it was passed in the config, the
                default path otherwise

        []{#useIdb()}

        -   #### useIdb

            ``` methodSignature
            public boolean useIdb()
            ```

            ::: block
            Determines whether to use idb install functions or simctl;
            current default is to not use idb
            :::

            [Returns:]{.returnLabel}
            :   true it is supposed to use idb, false otherwise

        []{#getXcodeDeveloperDirectoryForTests()}

        -   #### getXcodeDeveloperDirectoryForTests

            ``` methodSignature
            public Optional<String> getXcodeDeveloperDirectoryForTests()
            ```

        []{#getExtraToolchainPaths()}

        -   #### getExtraToolchainPaths

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Path> getExtraToolchainPaths()
            ```

        []{#getExtraPlatformPaths()}

        -   #### getExtraPlatformPaths

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Path> getExtraPlatformPaths()
            ```

        []{#getAppleToolchainSetTarget(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getAppleToolchainSetTarget

            ``` methodSignature
            public Optional<BuildTarget> getAppleToolchainSetTarget​(TargetConfiguration targetConfiguration)
            ```

        []{#getTargetSdkVersion(com.facebook.buck.apple.toolchain.ApplePlatform)}

        -   #### getTargetSdkVersion

            ``` methodSignature
            public Optional<String> getTargetSdkVersion​(ApplePlatform platform)
            ```

        []{#getXctestPlatformNames()}

        -   #### getXctestPlatformNames

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getXctestPlatformNames()
            ```

        []{#getXctoolPath()}

        -   #### getXctoolPath

            ``` methodSignature
            public Optional<Path> getXctoolPath()
            ```

        []{#getXctoolZipTarget(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getXctoolZipTarget

            ``` methodSignature
            public Optional<BuildTarget> getXctoolZipTarget​(TargetConfiguration targetConfiguration)
            ```

        []{#getCodesignProvider()}

        -   #### getCodesignProvider

            ``` methodSignature
            public ToolProvider getCodesignProvider()
            ```

        []{#getCodesignTimeout()}

        -   #### getCodesignTimeout

            ``` methodSignature
            public java.time.Duration getCodesignTimeout()
            ```

            ::: block
            Specify the maximum code-signing time before timing out.
            :::

        []{#getXctoolDefaultDestinationSpecifier()}

        -   #### getXctoolDefaultDestinationSpecifier

            ``` methodSignature
            public Optional<String> getXctoolDefaultDestinationSpecifier()
            ```

        []{#getXctoolStutterTimeoutMs()}

        -   #### getXctoolStutterTimeoutMs

            ``` methodSignature
            public Optional<Long> getXctoolStutterTimeoutMs()
            ```

        []{#getXcodeDisableParallelizeBuild()}

        -   #### getXcodeDisableParallelizeBuild

            ``` methodSignature
            public boolean getXcodeDisableParallelizeBuild()
            ```

        []{#useDryRunCodeSigning()}

        -   #### useDryRunCodeSigning

            ``` methodSignature
            public boolean useDryRunCodeSigning()
            ```

        []{#cacheBundlesAndPackages()}

        -   #### cacheBundlesAndPackages

            ``` methodSignature
            public boolean cacheBundlesAndPackages()
            ```

        []{#linkAllObjC()}

        -   #### linkAllObjC

            ``` methodSignature
            public boolean linkAllObjC()
            ```

        []{#getZipCompressionLevel()}

        -   #### getZipCompressionLevel

            ``` methodSignature
            public ZipCompressionLevel getZipCompressionLevel()
            ```

        []{#getAppleDeviceHelperAbsolutePath()}

        -   #### getAppleDeviceHelperAbsolutePath

            ``` methodSignature
            public Optional<Path> getAppleDeviceHelperAbsolutePath()
            ```

        []{#getAppleDeviceHelperTarget(java.util.Optional)}

        -   #### getAppleDeviceHelperTarget

            ``` methodSignature
            public Optional<BuildTarget> getAppleDeviceHelperTarget​(Optional<TargetConfiguration> targetConfiguration)
            ```

            ::: block
            Query buckconfig for device helper target.
            :::

        []{#getProvisioningProfileSearchPath()}

        -   #### getProvisioningProfileSearchPath

            ``` methodSignature
            public Path getProvisioningProfileSearchPath()
            ```

        []{#shouldUseHeaderMapsInXcodeProject()}

        -   #### shouldUseHeaderMapsInXcodeProject

            ``` methodSignature
            public boolean shouldUseHeaderMapsInXcodeProject()
            ```

        []{#shouldMergeHeaderMapsInXcodeProject()}

        -   #### shouldMergeHeaderMapsInXcodeProject

            ``` methodSignature
            public boolean shouldMergeHeaderMapsInXcodeProject()
            ```

        []{#shouldGenerateHeaderSymlinkTreesOnly()}

        -   #### shouldGenerateHeaderSymlinkTreesOnly

            ``` methodSignature
            public boolean shouldGenerateHeaderSymlinkTreesOnly()
            ```

        []{#shouldGenerateMissingUmbrellaHeaders()}

        -   #### shouldGenerateMissingUmbrellaHeaders

            ``` methodSignature
            public boolean shouldGenerateMissingUmbrellaHeaders()
            ```

        []{#shouldUseSwiftDelegate()}

        -   #### shouldUseSwiftDelegate

            ``` methodSignature
            public boolean shouldUseSwiftDelegate()
            ```

        []{#shouldVerifyBundleResources()}

        -   #### shouldVerifyBundleResources

            ``` methodSignature
            public boolean shouldVerifyBundleResources()
            ```

        []{#shouldAddLinkedLibrariesAsFlags()}

        -   #### shouldAddLinkedLibrariesAsFlags

            ``` methodSignature
            public boolean shouldAddLinkedLibrariesAsFlags()
            ```

        []{#shouldLinkSystemSwift()}

        -   #### shouldLinkSystemSwift

            ``` methodSignature
            public boolean shouldLinkSystemSwift()
            ```

        []{#shouldIncludeSharedLibraryResources()}

        -   #### shouldIncludeSharedLibraryResources

            ``` methodSignature
            public boolean shouldIncludeSharedLibraryResources()
            ```

        []{#shouldAddLinkerFlagsForLinkWholeLibraries()}

        -   #### shouldAddLinkerFlagsForLinkWholeLibraries

            ``` methodSignature
            public boolean shouldAddLinkerFlagsForLinkWholeLibraries()
            ```

        []{#getForceLoadLibraryPath(boolean)}

        -   #### getForceLoadLibraryPath

            ``` methodSignature
            public String getForceLoadLibraryPath​(boolean isFocusedTarget)
            ```

        []{#assetCatalogValidation()}

        -   #### assetCatalogValidation

            ``` methodSignature
            public AppleAssetCatalog.ValidationType assetCatalogValidation()
            ```

        []{#getTestLogDirectoryEnvironmentVariable()}

        -   #### getTestLogDirectoryEnvironmentVariable

            ``` methodSignature
            public String getTestLogDirectoryEnvironmentVariable()
            ```

        []{#getTestLogLevelEnvironmentVariable()}

        -   #### getTestLogLevelEnvironmentVariable

            ``` methodSignature
            public String getTestLogLevelEnvironmentVariable()
            ```

        []{#getTestLogLevel()}

        -   #### getTestLogLevel

            ``` methodSignature
            public String getTestLogLevel()
            ```

        []{#getDefaultDebugInfoFormatForBinaries()}

        -   #### getDefaultDebugInfoFormatForBinaries

            ``` methodSignature
            public AppleDebugFormat getDefaultDebugInfoFormatForBinaries()
            ```

        []{#getDefaultDebugInfoFormatForTests()}

        -   #### getDefaultDebugInfoFormatForTests

            ``` methodSignature
            public AppleDebugFormat getDefaultDebugInfoFormatForTests()
            ```

        []{#getDefaultDebugInfoFormatForLibraries()}

        -   #### getDefaultDebugInfoFormatForLibraries

            ``` methodSignature
            public AppleDebugFormat getDefaultDebugInfoFormatForLibraries()
            ```

        []{#getProvisioningProfileReadCommand()}

        -   #### getProvisioningProfileReadCommand

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getProvisioningProfileReadCommand()
            ```

        []{#getCodeSignIdentitiesCommand()}

        -   #### getCodeSignIdentitiesCommand

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getCodeSignIdentitiesCommand()
            ```

        []{#getPackageConfigForPlatform(com.facebook.buck.apple.toolchain.ApplePlatform)}

        -   #### getPackageConfigForPlatform

            ``` methodSignature
            public Optional<com.facebook.buck.apple.AppleConfig.ApplePackageConfig> getPackageConfigForPlatform​(ApplePlatform platform)
            ```

            ::: block
            Returns the custom packager command specified in the config,
            if defined.
            This is translated into the config value of
            `apple.PLATFORMNAME_packager_command`.
            :::

            [Parameters:]{.paramLabel}
            :   `platform` - the platform to query.

            [Returns:]{.returnLabel}
            :   the custom packager command specified in the config, if
                defined.

        []{#getToolchainsOverrideForSDKName(java.lang.String)}

        -   #### getToolchainsOverrideForSDKName

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableList<String>> getToolchainsOverrideForSDKName​(String name)
            ```

        []{#getXcodeToolReplacement(java.lang.String)}

        -   #### getXcodeToolReplacement

            ``` methodSignature
            public Optional<Path> getXcodeToolReplacement​(String toolName)
            ```

        []{#getXcodeToolName(java.lang.String)}

        -   #### getXcodeToolName

            ``` methodSignature
            public String getXcodeToolName​(String toolName)
            ```

        []{#getXcodeToolVersion(java.lang.String,java.lang.String)}

        -   #### getXcodeToolVersion

            ``` methodSignature
            public String getXcodeToolVersion​(String toolName,
                                              String defaultToolVersion)
            ```

        []{#useFlavoredCxxSections()}

        -   #### useFlavoredCxxSections

            ``` methodSignature
            public boolean useFlavoredCxxSections()
            ```

            [Returns:]{.returnLabel}
            :   whether to extend C/C++ platforms using config settings
                in `cxx#` sections instead of the unflavored `cxx`
                section.

        []{#addCellPathToIquotePath()}

        -   #### addCellPathToIquotePath

            ``` methodSignature
            public boolean addCellPathToIquotePath()
            ```

            [Returns:]{.returnLabel}
            :   whether to add the cell path to the \`-iquote\` path for
                all compilations.

        []{#shouldWorkAroundDsymutilLTOStackOverflowBug()}

        -   #### shouldWorkAroundDsymutilLTOStackOverflowBug

            ``` methodSignature
            public boolean shouldWorkAroundDsymutilLTOStackOverflowBug()
            ```

        []{#moduleMapMode()}

        -   #### moduleMapMode

            ``` methodSignature
            public ModuleMapMode moduleMapMode()
            ```

            [Returns:]{.returnLabel}
            :   The module map mode to use for modular libraries.

        []{#shellPath()}

        -   #### shellPath

            ``` methodSignature
            public Path shellPath()
            ```

        []{#buildScriptPath()}

        -   #### buildScriptPath

            ``` methodSignature
            public Path buildScriptPath()
            ```

        []{#useEntitlementsWhenAdhocCodeSigning()}

        -   #### useEntitlementsWhenAdhocCodeSigning

            ``` methodSignature
            public boolean useEntitlementsWhenAdhocCodeSigning()
            ```

            [Returns:]{.returnLabel}
            :   whether entitlements should be used during adhoc code
                signing phase (adhoc is used on simulator and macOS
                platforms).

        []{#shouldUseModernBuildSystem()}

        -   #### shouldUseModernBuildSystem

            ``` methodSignature
            public boolean shouldUseModernBuildSystem()
            ```

        []{#shouldLinkScrubConcurrently()}

        -   #### shouldLinkScrubConcurrently

            ``` methodSignature
            public boolean shouldLinkScrubConcurrently()
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
-   Nested \| 
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
