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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Class AndroidBuckConfig {#class-androidbuckconfig .title title="Class AndroidBuckConfig"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.AndroidBuckConfig

::: description
-   

    ------------------------------------------------------------------------

        public class AndroidBuckConfig
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `AndroidBuckConfig    | ::: block             |
        |                       | .NdkSearchOrderEntry` | Values acceptable for |
        |                       |                       | ndk.ndk_search_order. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                         Field                                   Description
          --------------------------------------------------------- --------------------------------------- -------------
          `static String`                                           `PATH_ENTRY_IN_ADB_PATH_SEARCH_ORDER`    
          `static String`                                           `SDK_ENTRY_IN_ADB_PATH_SEARCH_ORDER`     
          `static com.google.common.collect.ImmutableSet<String>`   `VALID_ABI_KEYS`                         

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                    Description
          ------------------------------------------------------------------------------ -------------
          `AndroidBuckConfig​(BuckConfig delegate,                  Platform platform)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Op                   | `getAapt2Override()`  | ::: block             |
        | tional<ToolProvider>` |                       | Returns the tool      |
        |                       |                       | provider to the       |
        |                       |                       | platform specific     |
        |                       |                       | aapt2 executable that |
        |                       |                       | is overridden by the  |
        |                       |                       | current project.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getAap               | ::: block             |
        |                       | tNoResourceRemoval()` | Whether to disable    |
        |                       |                       | resource removal in   |
        |                       |                       | aapt2.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Op                   | `getAaptOverride()`   | ::: block             |
        | tional<java.util.func |                       | Returns the path to   |
        | tion.Supplier<Tool>>` |                       | the platform specific |
        |                       |                       | aapt executable that  |
        |                       |                       | is overridden by the  |
        |                       |                       | current project.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Path>`      | `getAdbOverride()`    | ::: block             |
        |                       |                       | Returns the path to   |
        |                       |                       | the adb executable    |
        |                       |                       | overridden by the     |
        |                       |                       | current project.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getAdbSearchOrder()` | ::: block             |
        | ogle.common.collect.I |                       | Defines the order to  |
        | mmutableList<String>` |                       | search for the adb    |
        |                       |                       | executable: a list    |
        |                       |                       | consisting of the     |
        |                       |                       | elements \'\',        |
        |                       |                       | representing the      |
        |                       |                       | first adb on the      |
        |                       |                       | system PATH, or \'\', |
        |                       |                       | representing the adb  |
        |                       |                       | in the platform-tools |
        |                       |                       | directory of the      |
        |                       |                       | currently configured  |
        |                       |                       | Android SDK location. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Integer`             | `getAdbTimeout()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getAndroi            |                       |
        |                       | dCompileSdkVersion()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `ge                   |                       |
        |                       | tBuildToolsVersion()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getExtraNdkCFlags()` |                       |
        | ogle.common.collect.I |                       |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `g                    |                       |
        | ogle.common.collect.I | etExtraNdkCxxFlags()` |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `                     |                       |
        | ogle.common.collect.I | getExtraNdkLdFlags()` |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getFail              | ::: block             |
        |                       | OnLegacyAaptErrors()` | Whether to fail (vs   |
        |                       |                       | warn) on legacy aapt2 |
        |                       |                       | compile errors.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `                     | ::: block             |
        |                       | getNdkAppPlatformForC | Returns the CPU       |
        |                       | puAbi​(String cpuAbi)` | specific app          |
        |                       |                       | platform, or the      |
        |                       |                       | fallback one if set.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `                     |                       |
        |                       | getNdkClangVersion()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optio                | `getNdkCompiler()`    |                       |
        | nal<NdkCompilerType>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `getNdkCp             |                       |
        | ommon.collect.Immutab | uAbiAppPlatformMap()` |                       |
        | leMap<String,​String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getNdkCpuAbiF        |                       |
        |                       | allbackAppPlatform()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Opti                 | `getNdkCpuAbis()`     |                       |
        | onal<com.google.commo |                       |                       |
        | n.collect.ImmutableSe |                       |                       |
        | t<NdkTargetArchAbi>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Opt                  | `getNdkCxxRuntime()`  |                       |
        | ional<NdkCxxRuntime>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optiona              | `ge                   |                       |
        | l<NdkCxxRuntimeType>` | tNdkCxxRuntimeType()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `O                    | `g                    | ::: block             |
        | ptional<BuildTarget>` | etNdkCxxToolchainTarg | Gets the              |
        |                       | etForAbi​(NdkTargetArc | ndk_toolchain target  |
        |                       | hAbi cpuAbi,          | for the abi if it is  |
        |                       |                       | specified in the      |
        |                       |  TargetConfiguration  | config.               |
        |                       | targetConfiguration)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getNdkGccVersion()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getNdkPath()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `ge                   |                       |
        |                       | tNdkRepositoryPath()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getNdkSearchOrder()` | ::: block             |
        | n.collect.ImmutableLi |                       | Defines the order of  |
        | st<AndroidBuckConfig. |                       | search of the Android |
        | NdkSearchOrderEntry>` |                       | NDK.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `ge                   |                       |
        |                       | tNdkUnifiedHeaders()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getNdkVersion()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `O                    | `getRedexTarget       |                       |
        | ptional<BuildTarget>` | ​(TargetConfiguration  |                       |
        |                       | targetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Tool`                | `getRedexTool​(BuildR  |                       |
        |                       | uleResolver buildRule |                       |
        |                       | Resolver,             |                       |
        |                       |  TargetConfiguration  |                       |
        |                       | targetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getSdkPath()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getSdkPathConfi      | ::: block             |
        |                       | gOptionFromSearchOrde | Given the entry to    |
        |                       | rEntry​(String entry)` | from the order of     |
        |                       |                       | search of the Android |
        |                       |                       | SDK location returns  |
        |                       |                       | the name of the       |
        |                       |                       | configuration option  |
        |                       |                       | that contains SDK     |
        |                       |                       | path if the entry     |
        |                       |                       | instructs to get that |
        |                       |                       | value from            |
        |                       |                       | `.buckconfig` (i.e.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `get                  | ::: block             |
        | ogle.common.collect.I | SdkPathSearchOrder()` | Defines the order of  |
        | mmutableList<String>` |                       | search of the path to |
        |                       |                       | Android SDK.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `getSki               | ::: block             |
        |                       | pCrunchPngsDefault()` | Whether to skip       |
        |                       |                       | crunching pngs by     |
        |                       |                       | default in aapt2      |
        |                       |                       | compile.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isGrayscaleImag      |                       |
        |                       | eProcessingEnabled()` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
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

        []{#PATH_ENTRY_IN_ADB_PATH_SEARCH_ORDER}

        -   #### PATH_ENTRY_IN_ADB_PATH_SEARCH_ORDER

                public static final String PATH_ENTRY_IN_ADB_PATH_SEARCH_ORDER

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.android.AndroidBuckConfig.PATH_ENTRY_IN_ADB_PATH_SEARCH_ORDER)

        []{#SDK_ENTRY_IN_ADB_PATH_SEARCH_ORDER}

        -   #### SDK_ENTRY_IN_ADB_PATH_SEARCH_ORDER

                public static final String SDK_ENTRY_IN_ADB_PATH_SEARCH_ORDER

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.android.AndroidBuckConfig.SDK_ENTRY_IN_ADB_PATH_SEARCH_ORDER)

        []{#VALID_ABI_KEYS}

        -   #### VALID_ABI_KEYS

                public static final com.google.common.collect.ImmutableSet<String> VALID_ABI_KEYS
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.config.BuckConfig,com.facebook.buck.util.environment.Platform)}

        -   #### AndroidBuckConfig

                public AndroidBuckConfig​(BuckConfig delegate,
                                         Platform platform)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getSkipCrunchPngsDefault()}

        -   #### getSkipCrunchPngsDefault

            ``` methodSignature
            public Optional<Boolean> getSkipCrunchPngsDefault()
            ```

            ::: block
            Whether to skip crunching pngs by default in aapt2 compile.
            :::

        []{#getFailOnLegacyAaptErrors()}

        -   #### getFailOnLegacyAaptErrors

            ``` methodSignature
            public boolean getFailOnLegacyAaptErrors()
            ```

            ::: block
            Whether to fail (vs warn) on legacy aapt2 compile errors.
            :::

        []{#getAaptNoResourceRemoval()}

        -   #### getAaptNoResourceRemoval

            ``` methodSignature
            public boolean getAaptNoResourceRemoval()
            ```

            ::: block
            Whether to disable resource removal in aapt2.
            :::

        []{#getAndroidCompileSdkVersion()}

        -   #### getAndroidCompileSdkVersion

            ``` methodSignature
            public Optional<String> getAndroidCompileSdkVersion()
            ```

        []{#getBuildToolsVersion()}

        -   #### getBuildToolsVersion

            ``` methodSignature
            public Optional<String> getBuildToolsVersion()
            ```

        []{#getAdbOverride()}

        -   #### getAdbOverride

            ``` methodSignature
            public Optional<Path> getAdbOverride()
            ```

            ::: block
            Returns the path to the adb executable overridden by the
            current project. If not specified, the
            [`getAdbSearchOrder()`](#getAdbSearchOrder()) will be used
            to find adb.
            :::

        []{#getAdbSearchOrder()}

        -   #### getAdbSearchOrder

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getAdbSearchOrder()
            ```

            ::: block
            Defines the order to search for the adb executable: a list
            consisting of the elements \'\', representing the first adb
            on the system PATH, or \'\', representing the adb in the
            platform-tools directory of the currently configured Android
            SDK location.
            :::

        []{#getAdbTimeout()}

        -   #### getAdbTimeout

            ``` methodSignature
            public Integer getAdbTimeout()
            ```

        []{#getSdkPath()}

        -   #### getSdkPath

            ``` methodSignature
            public Optional<String> getSdkPath()
            ```

        []{#getSdkPathSearchOrder()}

        -   #### getSdkPathSearchOrder

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getSdkPathSearchOrder()
            ```

            ::: block
            Defines the order of search of the path to Android SDK.
            The order is the list of elements that can either be
            `<CONFIG>` (to indicate the entry from `.buckconfig`) or the
            name of an environment variable that contains path to
            Android SDK (for example, `ANDROID_SDK`).

            If nothing is specified in `.buckconfig` the default order
            is: `ANDROID_SDK`, `ANDROID_HOME`, `ANDROID_SDK_ROOT`,
            `<CONFIG>`
            :::

        []{#getSdkPathConfigOptionFromSearchOrderEntry(java.lang.String)}

        -   #### getSdkPathConfigOptionFromSearchOrderEntry

            ``` methodSignature
            public Optional<String> getSdkPathConfigOptionFromSearchOrderEntry​(String entry)
            ```

            ::: block
            Given the entry to from the order of search of the Android
            SDK location returns the name of the configuration option
            that contains SDK path if the entry instructs to get that
            value from `.buckconfig` (i.e. it\'s `<CONFIG>`) or
            `Optional.empty()` in other cases.
            :::

        []{#getNdkVersion()}

        -   #### getNdkVersion

            ``` methodSignature
            public Optional<String> getNdkVersion()
            ```

        []{#getNdkPath()}

        -   #### getNdkPath

            ``` methodSignature
            public Optional<String> getNdkPath()
            ```

        []{#getNdkRepositoryPath()}

        -   #### getNdkRepositoryPath

            ``` methodSignature
            public Optional<String> getNdkRepositoryPath()
            ```

        []{#getNdkSearchOrder()}

        -   #### getNdkSearchOrder

            ``` methodSignature
            public com.google.common.collect.ImmutableList<AndroidBuckConfig.NdkSearchOrderEntry> getNdkSearchOrder()
            ```

            ::: block
            Defines the order of search of the Android NDK.
            The order is the list of elements that can either be
            `<NDK_REPOSITORY_CONFIG>` to indicate the entry
            `ndk.ndk_repo_path` from `.buckconfig`,
            `  <NDK_DIRECTORY_CONFIG>` to indicate the entry
            `ndk.ndk_path` from `.buckconfig`, or the name of an
            environment variable that contains path to Android NDK
            (`ANDROID_NDK`, `NDK_HOME` or `ANDROID_NDK_REPOSITORY`).

            If nothing is specified in `.buckconfig` the default order
            is: `  ANDROID_NDK_REPOSITORY`, `ANDROID_NDK`, `NDK_HOME`,
            `  <NDK_REPOSITORY_CONFIG>`, `<NDK_DIRECTORY_CONFIG>`
            :::

        []{#getNdkCpuAbiFallbackAppPlatform()}

        -   #### getNdkCpuAbiFallbackAppPlatform

            ``` methodSignature
            public Optional<String> getNdkCpuAbiFallbackAppPlatform()
            ```

        []{#getNdkCpuAbiAppPlatformMap()}

        -   #### getNdkCpuAbiAppPlatformMap

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​String> getNdkCpuAbiAppPlatformMap()
            ```

        []{#getNdkCpuAbis()}

        -   #### getNdkCpuAbis

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableSet<NdkTargetArchAbi>> getNdkCpuAbis()
            ```

        []{#getNdkCompiler()}

        -   #### getNdkCompiler

            ``` methodSignature
            public Optional<NdkCompilerType> getNdkCompiler()
            ```

        []{#getNdkGccVersion()}

        -   #### getNdkGccVersion

            ``` methodSignature
            public Optional<String> getNdkGccVersion()
            ```

        []{#getNdkClangVersion()}

        -   #### getNdkClangVersion

            ``` methodSignature
            public Optional<String> getNdkClangVersion()
            ```

        []{#getNdkCxxRuntime()}

        -   #### getNdkCxxRuntime

            ``` methodSignature
            public Optional<NdkCxxRuntime> getNdkCxxRuntime()
            ```

        []{#getNdkCxxRuntimeType()}

        -   #### getNdkCxxRuntimeType

            ``` methodSignature
            public Optional<NdkCxxRuntimeType> getNdkCxxRuntimeType()
            ```

        []{#getExtraNdkCFlags()}

        -   #### getExtraNdkCFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getExtraNdkCFlags()
            ```

        []{#getExtraNdkCxxFlags()}

        -   #### getExtraNdkCxxFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getExtraNdkCxxFlags()
            ```

        []{#getExtraNdkLdFlags()}

        -   #### getExtraNdkLdFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getExtraNdkLdFlags()
            ```

        []{#getNdkUnifiedHeaders()}

        -   #### getNdkUnifiedHeaders

            ``` methodSignature
            public Optional<Boolean> getNdkUnifiedHeaders()
            ```

        []{#isGrayscaleImageProcessingEnabled()}

        -   #### isGrayscaleImageProcessingEnabled

            ``` methodSignature
            public boolean isGrayscaleImageProcessingEnabled()
            ```

        []{#getNdkAppPlatformForCpuAbi(java.lang.String)}

        -   #### getNdkAppPlatformForCpuAbi

            ``` methodSignature
            public Optional<String> getNdkAppPlatformForCpuAbi​(String cpuAbi)
            ```

            ::: block
            Returns the CPU specific app platform, or the fallback one
            if set. If neither are set, returns \`Optional.empty\`
            instead of a default value so callers can determine the
            difference between user-set and buck defaults.
            :::

        []{#getNdkCxxToolchainTargetForAbi(com.facebook.buck.android.toolchain.ndk.NdkTargetArchAbi,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getNdkCxxToolchainTargetForAbi

            ``` methodSignature
            public Optional<BuildTarget> getNdkCxxToolchainTargetForAbi​(NdkTargetArchAbi cpuAbi,
                                                                        TargetConfiguration targetConfiguration)
            ```

            ::: block
            Gets the ndk_toolchain target for the abi if it is specified
            in the config.
            :::

        []{#getAaptOverride()}

        -   #### getAaptOverride

            ``` methodSignature
            public Optional<java.util.function.Supplier<Tool>> getAaptOverride()
            ```

            ::: block
            Returns the path to the platform specific aapt executable
            that is overridden by the current project. If not specified,
            the Android platform aapt will be used.
            :::

        []{#getAapt2Override()}

        -   #### getAapt2Override

            ``` methodSignature
            public Optional<ToolProvider> getAapt2Override()
            ```

            ::: block
            Returns the tool provider to the platform specific aapt2
            executable that is overridden by the current project. If not
            specified, the Android platform aapt will be used.
            :::

        []{#getRedexTarget(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getRedexTarget

            ``` methodSignature
            public Optional<BuildTarget> getRedexTarget​(TargetConfiguration targetConfiguration)
            ```

        []{#getRedexTool(com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getRedexTool

            ``` methodSignature
            public Tool getRedexTool​(BuildRuleResolver buildRuleResolver,
                                     TargetConfiguration targetConfiguration)
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
