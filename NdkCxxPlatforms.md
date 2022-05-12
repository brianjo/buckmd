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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.android.toolchain.ndk.impl](package-summary.html)
:::

## Class NdkCxxPlatforms {#class-ndkcxxplatforms .title title="Class NdkCxxPlatforms"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.toolchain.ndk.impl.NdkCxxPlatforms

::: description
-   

    ------------------------------------------------------------------------

        public class NdkCxxPlatforms
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `                     | ::: block             |
        |                       | NdkCxxPlatforms.Host` | The OS and            |
        |                       |                       | Architecture that     |
        |                       |                       | we\'re building on.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `NdkCxxPlatf          | ::: block             |
        |                       | orms.ToolchainTarget` | The toolchains name   |
        |                       |                       | for the platform      |
        |                       |                       | being targeted.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `static String`       | `BUILD_HOST_SUBST`    | ::: block             |
        |                       |                       | Magic string we       |
        |                       |                       | substitute into debug |
        |                       |                       | paths in place of the |
        |                       |                       | build-host name,      |
        |                       |                       | erasing the           |
        |                       |                       | difference between    |
        |                       |                       | say, building on      |
        |                       |                       | Darwin and building   |
        |                       |                       | on Linux.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static com.go        | `D                    | ::: block             |
        | ogle.common.collect.I | EFAULT_COMMON_CFLAGS` | Defaults for c and    |
        | mmutableList<String>` |                       | c++ flags             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static com.go        | `DEFAULT_C            | ::: block             |
        | ogle.common.collect.I | OMMON_COMPILER_FLAGS` | Flags used when       |
        | mmutableList<String>` |                       | compiling either C or |
        |                       |                       | C++ sources.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static com.go        | `DEF                  |                       |
        | ogle.common.collect.I | AULT_COMMON_CPPFLAGS` |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com.go        | `DEF                  |                       |
        | ogle.common.collect.I | AULT_COMMON_CXXFLAGS` |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com.go        | `DEFAU                |                       |
        | ogle.common.collect.I | LT_COMMON_CXXPPFLAGS` |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com.go        | `DE                   | ::: block             |
        | ogle.common.collect.I | FAULT_COMMON_LDFLAGS` | Default linker flags  |
        | mmutableList<String>` |                       | added by the NDK.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `DEFAULT              |                       |
        |                       | _TARGET_APP_PLATFORM` |                       |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static String`       | `getDef               |                       |
        |                       | aultClangVersionForNd |                       |
        |                       | k​(String ndkVersion)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `getDef               |                       |
        | atic NdkCompilerType` | aultCompilerTypeForNd |                       |
        |                       | k​(String ndkVersion)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getD                 |                       |
        | static NdkCxxRuntime` | efaultCxxRuntimeForNd |                       |
        |                       | k​(String ndkVersion)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `getD                 |                       |
        |                       | efaultGccVersionForNd |                       |
        |                       | k​(String ndkVersion)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `getPlatforms​(        | ::: block             |
        | atic com.google.commo | CxxBuckConfig config, | Gets all the          |
        | n.collect.ImmutableMa |              AndroidB | unresolved            |
        | p<TargetCpuType,​Unres | uckConfig androidConf | [`NdkCxxPlatf         |
        | olvedNdkCxxPlatform>` | ig,             Proje | orm`](../NdkCxxPlatfo |
        |                       | ctFilesystem filesyst | rm.html "interface in |
        |                       | em,             Targe |  com.facebook.buck.an |
        |                       | tConfiguration target | droid.toolchain.ndk") |
        |                       | Configuration,        | based on the          |
        |                       |       Platform platfo | buckconfig.           |
        |                       | rm,             Toolc | :::                   |
        |                       | hainProvider toolchai |                       |
        |                       | nProvider,            |                       |
        |                       |   String ndkVersion)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `getPlatforms         |                       |
        | atic com.google.commo | ​(CxxBuckConfig config |                       |
        | n.collect.ImmutableMa | ,             Android |                       |
        | p<TargetCpuType,​Unres | BuckConfig androidCon |                       |
        | olvedNdkCxxPlatform>` | fig,             Proj |                       |
        |                       | ectFilesystem filesys |                       |
        |                       | tem,             Path |                       |
        |                       |  ndkRoot,             |                       |
        |                       |  NdkCxxPlatformCompil |                       |
        |                       | er compiler,          |                       |
        |                       |     NdkCxxRuntime cxx |                       |
        |                       | Runtime,              |                       |
        |                       | NdkCxxRuntimeType run |                       |
        |                       | timeType,             |                       |
        |                       |  Set<NdkTargetArchAbi |                       |
        |                       | > cpuAbis,            |                       |
        |                       |   Platform platform)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `getPlatforms​(CxxB    |                       |
        | atic com.google.commo | uckConfig config,     |                       |
        | n.collect.ImmutableMa |          AndroidBuckC |                       |
        | p<TargetCpuType,​Unres | onfig androidConfig,  |                       |
        | olvedNdkCxxPlatform>` |             ProjectFi |                       |
        |                       | lesystem filesystem,  |                       |
        |                       |             Path ndkR |                       |
        |                       | oot,             NdkC |                       |
        |                       | xxPlatformCompiler co |                       |
        |                       | mpiler,             N |                       |
        |                       | dkCxxRuntime cxxRunti |                       |
        |                       | me,             NdkCx |                       |
        |                       | xRuntimeType runtimeT |                       |
        |                       | ype,             Set< |                       |
        |                       | NdkTargetArchAbi> cpu |                       |
        |                       | Abis,             Pla |                       |
        |                       | tform platform,       |                       |
        |                       |        ExecutableFind |                       |
        |                       | er executableFinder,  |                       |
        |                       |             boolean s |                       |
        |                       | trictToolchainPaths)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `isSup                |                       |
        |                       | portedConfiguration​(P |                       |
        |                       | ath ndkRoot,          |                       |
        |                       |                 NdkCx |                       |
        |                       | xRuntime cxxRuntime)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
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

        []{#BUILD_HOST_SUBST}

        -   #### BUILD_HOST_SUBST

                public static final String BUILD_HOST_SUBST

            ::: block
            Magic string we substitute into debug paths in place of the
            build-host name, erasing the difference between say,
            building on Darwin and building on Linux.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../../constant-values.html#com.facebook.buck.android.toolchain.ndk.impl.NdkCxxPlatforms.BUILD_HOST_SUBST)

        []{#DEFAULT_TARGET_APP_PLATFORM}

        -   #### DEFAULT_TARGET_APP_PLATFORM

                public static final String DEFAULT_TARGET_APP_PLATFORM

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../../constant-values.html#com.facebook.buck.android.toolchain.ndk.impl.NdkCxxPlatforms.DEFAULT_TARGET_APP_PLATFORM)

        []{#DEFAULT_COMMON_CFLAGS}

        -   #### DEFAULT_COMMON_CFLAGS

                public static final com.google.common.collect.ImmutableList<String> DEFAULT_COMMON_CFLAGS

            ::: block
            Defaults for c and c++ flags
            :::

        []{#DEFAULT_COMMON_CXXFLAGS}

        -   #### DEFAULT_COMMON_CXXFLAGS

                public static final com.google.common.collect.ImmutableList<String> DEFAULT_COMMON_CXXFLAGS

        []{#DEFAULT_COMMON_CPPFLAGS}

        -   #### DEFAULT_COMMON_CPPFLAGS

                public static final com.google.common.collect.ImmutableList<String> DEFAULT_COMMON_CPPFLAGS

        []{#DEFAULT_COMMON_CXXPPFLAGS}

        -   #### DEFAULT_COMMON_CXXPPFLAGS

                public static final com.google.common.collect.ImmutableList<String> DEFAULT_COMMON_CXXPPFLAGS

        []{#DEFAULT_COMMON_COMPILER_FLAGS}

        -   #### DEFAULT_COMMON_COMPILER_FLAGS

                public static final com.google.common.collect.ImmutableList<String> DEFAULT_COMMON_COMPILER_FLAGS

            ::: block
            Flags used when compiling either C or C++ sources.
            :::

        []{#DEFAULT_COMMON_LDFLAGS}

        -   #### DEFAULT_COMMON_LDFLAGS

                public static final com.google.common.collect.ImmutableList<String> DEFAULT_COMMON_LDFLAGS

            ::: block
            Default linker flags added by the NDK.
            :::
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getDefaultCompilerTypeForNdk(java.lang.String)}

        -   #### getDefaultCompilerTypeForNdk

            ``` methodSignature
            public static NdkCompilerType getDefaultCompilerTypeForNdk​(String ndkVersion)
            ```

        []{#getDefaultCxxRuntimeForNdk(java.lang.String)}

        -   #### getDefaultCxxRuntimeForNdk

            ``` methodSignature
            public static NdkCxxRuntime getDefaultCxxRuntimeForNdk​(String ndkVersion)
            ```

        []{#getDefaultGccVersionForNdk(java.lang.String)}

        -   #### getDefaultGccVersionForNdk

            ``` methodSignature
            public static String getDefaultGccVersionForNdk​(String ndkVersion)
            ```

        []{#getDefaultClangVersionForNdk(java.lang.String)}

        -   #### getDefaultClangVersionForNdk

            ``` methodSignature
            public static String getDefaultClangVersionForNdk​(String ndkVersion)
            ```

        []{#isSupportedConfiguration(java.nio.file.Path,com.facebook.buck.android.toolchain.ndk.NdkCxxRuntime)}

        -   #### isSupportedConfiguration

            ``` methodSignature
            public static boolean isSupportedConfiguration​(Path ndkRoot,
                                                           NdkCxxRuntime cxxRuntime)
            ```

        []{#getPlatforms(com.facebook.buck.cxx.config.CxxBuckConfig,com.facebook.buck.android.AndroidBuckConfig,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.util.environment.Platform,com.facebook.buck.core.toolchain.ToolchainProvider,java.lang.String)}

        -   #### getPlatforms

            ``` methodSignature
            public static com.google.common.collect.ImmutableMap<TargetCpuType,​UnresolvedNdkCxxPlatform> getPlatforms​(CxxBuckConfig config,
                                                                                                                            AndroidBuckConfig androidConfig,
                                                                                                                            ProjectFilesystem filesystem,
                                                                                                                            TargetConfiguration targetConfiguration,
                                                                                                                            Platform platform,
                                                                                                                            ToolchainProvider toolchainProvider,
                                                                                                                            String ndkVersion)
            ```

            ::: block
            Gets all the unresolved
            [`NdkCxxPlatform`](../NdkCxxPlatform.html "interface in com.facebook.buck.android.toolchain.ndk")
            based on the buckconfig.
            :::

        []{#getPlatforms(com.facebook.buck.cxx.config.CxxBuckConfig,com.facebook.buck.android.AndroidBuckConfig,com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path,com.facebook.buck.android.toolchain.ndk.NdkCxxPlatformCompiler,com.facebook.buck.android.toolchain.ndk.NdkCxxRuntime,com.facebook.buck.android.toolchain.ndk.NdkCxxRuntimeType,java.util.Set,com.facebook.buck.util.environment.Platform)}

        -   #### getPlatforms

            ``` methodSignature
            public static com.google.common.collect.ImmutableMap<TargetCpuType,​UnresolvedNdkCxxPlatform> getPlatforms​(CxxBuckConfig config,
                                                                                                                            AndroidBuckConfig androidConfig,
                                                                                                                            ProjectFilesystem filesystem,
                                                                                                                            Path ndkRoot,
                                                                                                                            NdkCxxPlatformCompiler compiler,
                                                                                                                            NdkCxxRuntime cxxRuntime,
                                                                                                                            NdkCxxRuntimeType runtimeType,
                                                                                                                            Set<NdkTargetArchAbi> cpuAbis,
                                                                                                                            Platform platform)
            ```

        []{#getPlatforms(com.facebook.buck.cxx.config.CxxBuckConfig,com.facebook.buck.android.AndroidBuckConfig,com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path,com.facebook.buck.android.toolchain.ndk.NdkCxxPlatformCompiler,com.facebook.buck.android.toolchain.ndk.NdkCxxRuntime,com.facebook.buck.android.toolchain.ndk.NdkCxxRuntimeType,java.util.Set,com.facebook.buck.util.environment.Platform,com.facebook.buck.io.ExecutableFinder,boolean)}

        -   #### getPlatforms

            ``` methodSignature
            public static com.google.common.collect.ImmutableMap<TargetCpuType,​UnresolvedNdkCxxPlatform> getPlatforms​(CxxBuckConfig config,
                                                                                                                            AndroidBuckConfig androidConfig,
                                                                                                                            ProjectFilesystem filesystem,
                                                                                                                            Path ndkRoot,
                                                                                                                            NdkCxxPlatformCompiler compiler,
                                                                                                                            NdkCxxRuntime cxxRuntime,
                                                                                                                            NdkCxxRuntimeType runtimeType,
                                                                                                                            Set<NdkTargetArchAbi> cpuAbis,
                                                                                                                            Platform platform,
                                                                                                                            ExecutableFinder executableFinder,
                                                                                                                            boolean strictToolchainPaths)
            ```

            [Returns:]{.returnLabel}
            :   the map holding the available
                [`NdkCxxPlatform`](../NdkCxxPlatform.html "interface in com.facebook.buck.android.toolchain.ndk")s.
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   [Nested](#nested.class.summary) \| 
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
