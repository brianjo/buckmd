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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Interface AndroidGraphEnhancerArgs {#interface-androidgraphenhancerargs .title title="Interface AndroidGraphEnhancerArgs"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `HasApplicationModuleBlacklist`,
        `HasDuplicateAndroidResourceTypes`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AndroidBinaryDescriptionArg`, `AndroidBundleDescriptionArg`

    ------------------------------------------------------------------------

        public interface AndroidGraphEnhancerArgs
        extends HasDuplicateAndroidResourceTypes, HasApplicationModuleBlacklist
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.android.HasDuplicateAndroidResourceTypes}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.android.[HasDuplicateAndroidResourceTypes](HasDuplicateAndroidResourceTypes.html "interface in com.facebook.buck.android")

            `HasDuplicateAndroidResourceTypes.DuplicateResourceBehaviour`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `d                    | `getAaptMode()`       |                       |
        | efault com.facebook.b |                       |                       |
        | uck.android.AaptMode` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getAd                |                       |
        | ogle.common.collect.I | ditionalAaptParams()` |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<co          | `getAndroi            |                       |
        | m.facebook.buck.andro | dSdkProguardConfig()` |                       |
        | id.ProGuardObfuscateS |                       |                       |
        | tep.SdkProguardType>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getApplic            |                       |
        | n.collect.ImmutableMa | ationModuleConfigs()` |                       |
        | p<String,​com.google.c |                       |                       |
        | ommon.collect.Immutab |                       |                       |
        | leList<BuildTarget>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getApplication       |                       |
        | Optional<com.google.c | ModuleDependencies()` |                       |
        | ommon.collect.Immutab |                       |                       |
        | leMap<String,​com.goog |                       |                       |
        | le.common.collect.Imm |                       |                       |
        | utableList<String>>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default Set<String>` | `getApplicationM      |                       |
        |                       | odulesWithManifest()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default Set<String>` | `getApplicationMo     |                       |
        |                       | dulesWithResources()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Set<BuildTarget>`    | `getApplic            |                       |
        |                       | ationModuleTargets()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `defau                | `ge                   |                       |
        | lt BuildConfigFields` | tBuildConfigValues()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getBui               |                       |
        | Optional<SourcePath>` | ldConfigValuesFile()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Set<TargetCpuType>`  | `getCpuFilters()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getDexR              |                       |
        | Optional<SourcePath>` | eorderDataDumpFile()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `get                  |                       |
        | Optional<SourcePath>` | DexReorderToolFile()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default String`      | `getDexTool()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `getDisablePreDex()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default com.g        | `getExtr              |                       |
        | oogle.common.collect. | aFilteredResources()` |                       |
        | ImmutableSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `getIsCacheable()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getK                 |                       |
        |                       | eepResourcePattern()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.g                | `getLocales()`        |                       |
        | oogle.common.collect. |                       |                       |
        | ImmutableSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getLocal             |                       |
        |                       | izedStringFileName()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getManifest()`       |                       |
        | Optional<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `def                  | `                     |                       |
        | ault ManifestEntries` | getManifestEntries()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `g                    |                       |
        | Optional<SourcePath>` | etManifestSkeleton()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getModu              |                       |
        | Optional<SourcePath>` | leManifestSkeleton()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `O                    | `getNativeLibrary     |                       |
        | ptional<BuildTarget>` | MergeCodeGenerator()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `O                    | `getNati              |                       |
        | ptional<BuildTarget>` | veLibraryMergeGlue()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getNativeLibraryMer  |                       |
        | Optional<com.google.c | geLocalizedSymbols()` |                       |
        | ommon.collect.Immutab |                       |                       |
        | leSortedSet<String>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Map<S                | `getNat               |                       |
        | tring,​List<Pattern>>` | iveLibraryMergeMap()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `O                    | `                     |                       |
        | ptional<BuildTarget>` | getNativeLibraryProgu |                       |
        |                       | ardConfigGenerator()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getNoDx()`           |                       |
        | .common.collect.Immut |                       |                       |
        | ableSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default int`         | `get                  |                       |
        |                       | OptimizationPasses()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getPackageType()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Option               | `getPost              |                       |
        | al<StringWithMacros>` | FilterResourcesCmd()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Option               | `getPreproc           |                       |
        | al<StringWithMacros>` | essJavaClassesBash()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getProguardConfig()` |                       |
        | Optional<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `List<String>`        | `                     |                       |
        |                       | getProguardJvmArgs()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.goo              | `ge                   |                       |
        | gle.common.collect.Im | tRelinkerWhitelist()` |                       |
        | mutableList<Pattern>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default com          | `getR                 |                       |
        | .facebook.buck.androi | esourceCompression()` |                       |
        | d.ResourcesFilter.Res |                       |                       |
        | ourceCompressionMode` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getRe                |                       |
        |                       | sourceUnionPackage()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `ge                   |                       |
        |                       | tUseDynamicFeature()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `isAa                 | ::: block             |
        |                       | pt2LocaleFiltering()` | Whether to filter     |
        |                       |                       | locales using aapt2.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `isAllowRDot          |                       |
        |                       | JavaInSecondaryDex()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `isBu                 |                       |
        |                       | ildStringSourceMap()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `isEnableRelinker()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `isIgnore             |                       |
        |                       | AaptProguardConfig()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `isInclu              |                       |
        |                       | desVectorDrawables()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `isNoAutoA            |                       |
        |                       | ddOverlayResources()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `isNoAu               |                       |
        |                       | toVersionResources()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `isNoVersionTr        |                       |
        |                       | ansitionsResources()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `isReor               |                       |
        |                       | derClassesIntraDex()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `isSkipCrunchPngs()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `isSkipProguard()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `isTrimResourceIds()` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.HasApplicationModuleBlacklist}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[HasApplicationModuleBlacklist](../core/description/arg/HasApplicationModuleBlacklist.html "interface in com.facebook.buck.core.description.arg")

            `getApplicationModuleBlacklist, withApplicationModuleBlacklist`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.android.HasDuplicateAndroidResourceTypes}

            ### Methods inherited from interface com.facebook.buck.android.[HasDuplicateAndroidResourceTypes](HasDuplicateAndroidResourceTypes.html "interface in com.facebook.buck.android")

            `getAllowedDuplicateResourceTypes, getBannedDuplicateResourceTypes, getDuplicateResourceBehavior, getDuplicateResourceWhitelist, getEffectiveBannedDuplicateResourceTypes`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getManifest()}

        -   #### getManifest

            ``` methodSignature
            Optional<SourcePath> getManifest()
            ```

        []{#getManifestSkeleton()}

        -   #### getManifestSkeleton

            ``` methodSignature
            Optional<SourcePath> getManifestSkeleton()
            ```

        []{#getModuleManifestSkeleton()}

        -   #### getModuleManifestSkeleton

            ``` methodSignature
            Optional<SourcePath> getModuleManifestSkeleton()
            ```

        []{#getPackageType()}

        -   #### getPackageType

            ``` methodSignature
            Optional<String> getPackageType()
            ```

        []{#getNoDx()}

        -   #### getNoDx

            ``` methodSignature
            com.google.common.collect.ImmutableSet<BuildTarget> getNoDx()
            ```

        []{#getDisablePreDex()}

        -   #### getDisablePreDex

            ``` methodSignature
            @Default
            default boolean getDisablePreDex()
            ```

        []{#getAndroidSdkProguardConfig()}

        -   #### getAndroidSdkProguardConfig

            ``` methodSignature
            Optional<com.facebook.buck.android.ProGuardObfuscateStep.SdkProguardType> getAndroidSdkProguardConfig()
            ```

        []{#getOptimizationPasses()}

        -   #### getOptimizationPasses

            ``` methodSignature
            @Default
            default int getOptimizationPasses()
            ```

        []{#getProguardJvmArgs()}

        -   #### getProguardJvmArgs

            ``` methodSignature
            List<String> getProguardJvmArgs()
            ```

        []{#getProguardConfig()}

        -   #### getProguardConfig

            ``` methodSignature
            Optional<SourcePath> getProguardConfig()
            ```

        []{#getResourceCompression()}

        -   #### getResourceCompression

            ``` methodSignature
            @Default
            default com.facebook.buck.android.ResourcesFilter.ResourceCompressionMode getResourceCompression()
            ```

        []{#isSkipCrunchPngs()}

        -   #### isSkipCrunchPngs

            ``` methodSignature
            Optional<Boolean> isSkipCrunchPngs()
            ```

        []{#isIncludesVectorDrawables()}

        -   #### isIncludesVectorDrawables

            ``` methodSignature
            @Default
            default boolean isIncludesVectorDrawables()
            ```

        []{#isNoAutoVersionResources()}

        -   #### isNoAutoVersionResources

            ``` methodSignature
            @Default
            default boolean isNoAutoVersionResources()
            ```

        []{#isNoVersionTransitionsResources()}

        -   #### isNoVersionTransitionsResources

            ``` methodSignature
            @Default
            default boolean isNoVersionTransitionsResources()
            ```

        []{#isNoAutoAddOverlayResources()}

        -   #### isNoAutoAddOverlayResources

            ``` methodSignature
            @Default
            default boolean isNoAutoAddOverlayResources()
            ```

        []{#getApplicationModuleTargets()}

        -   #### getApplicationModuleTargets

            ``` methodSignature
            Set<BuildTarget> getApplicationModuleTargets()
            ```

        []{#getApplicationModuleConfigs()}

        -   #### getApplicationModuleConfigs

            ``` methodSignature
            com.google.common.collect.ImmutableMap<String,​com.google.common.collect.ImmutableList<BuildTarget>> getApplicationModuleConfigs()
            ```

        []{#getApplicationModulesWithResources()}

        -   #### getApplicationModulesWithResources

            ``` methodSignature
            @Default
            default Set<String> getApplicationModulesWithResources()
            ```

        []{#getApplicationModulesWithManifest()}

        -   #### getApplicationModulesWithManifest

            ``` methodSignature
            @Default
            default Set<String> getApplicationModulesWithManifest()
            ```

        []{#getApplicationModuleDependencies()}

        -   #### getApplicationModuleDependencies

            ``` methodSignature
            Optional<com.google.common.collect.ImmutableMap<String,​com.google.common.collect.ImmutableList<String>>> getApplicationModuleDependencies()
            ```

        []{#getIsCacheable()}

        -   #### getIsCacheable

            ``` methodSignature
            @Default
            default boolean getIsCacheable()
            ```

        []{#getAdditionalAaptParams()}

        -   #### getAdditionalAaptParams

            ``` methodSignature
            com.google.common.collect.ImmutableList<String> getAdditionalAaptParams()
            ```

        []{#getAaptMode()}

        -   #### getAaptMode

            ``` methodSignature
            @Default
            default com.facebook.buck.android.AaptMode getAaptMode()
            ```

        []{#isTrimResourceIds()}

        -   #### isTrimResourceIds

            ``` methodSignature
            @Default
            default boolean isTrimResourceIds()
            ```

        []{#isAllowRDotJavaInSecondaryDex()}

        -   #### isAllowRDotJavaInSecondaryDex

            ``` methodSignature
            @Default
            default boolean isAllowRDotJavaInSecondaryDex()
            ```

        []{#getKeepResourcePattern()}

        -   #### getKeepResourcePattern

            ``` methodSignature
            Optional<String> getKeepResourcePattern()
            ```

        []{#getResourceUnionPackage()}

        -   #### getResourceUnionPackage

            ``` methodSignature
            Optional<String> getResourceUnionPackage()
            ```

        []{#getLocales()}

        -   #### getLocales

            ``` methodSignature
            com.google.common.collect.ImmutableSet<String> getLocales()
            ```

        []{#isAapt2LocaleFiltering()}

        -   #### isAapt2LocaleFiltering

            ``` methodSignature
            @Default
            default boolean isAapt2LocaleFiltering()
            ```

            ::: block
            Whether to filter locales using aapt2.
            :::

        []{#getLocalizedStringFileName()}

        -   #### getLocalizedStringFileName

            ``` methodSignature
            Optional<String> getLocalizedStringFileName()
            ```

        []{#isBuildStringSourceMap()}

        -   #### isBuildStringSourceMap

            ``` methodSignature
            @Default
            default boolean isBuildStringSourceMap()
            ```

        []{#isIgnoreAaptProguardConfig()}

        -   #### isIgnoreAaptProguardConfig

            ``` methodSignature
            @Default
            default boolean isIgnoreAaptProguardConfig()
            ```

        []{#getCpuFilters()}

        -   #### getCpuFilters

            ``` methodSignature
            Set<TargetCpuType> getCpuFilters()
            ```

        []{#getPreprocessJavaClassesBash()}

        -   #### getPreprocessJavaClassesBash

            ``` methodSignature
            Optional<StringWithMacros> getPreprocessJavaClassesBash()
            ```

        []{#isReorderClassesIntraDex()}

        -   #### isReorderClassesIntraDex

            ``` methodSignature
            @Default
            default boolean isReorderClassesIntraDex()
            ```

        []{#getDexTool()}

        -   #### getDexTool

            ``` methodSignature
            @Default
            default String getDexTool()
            ```

        []{#getDexReorderToolFile()}

        -   #### getDexReorderToolFile

            ``` methodSignature
            Optional<SourcePath> getDexReorderToolFile()
            ```

        []{#getDexReorderDataDumpFile()}

        -   #### getDexReorderDataDumpFile

            ``` methodSignature
            Optional<SourcePath> getDexReorderDataDumpFile()
            ```

        []{#getNativeLibraryMergeMap()}

        -   #### getNativeLibraryMergeMap

            ``` methodSignature
            Map<String,​List<Pattern>> getNativeLibraryMergeMap()
            ```

        []{#getNativeLibraryMergeGlue()}

        -   #### getNativeLibraryMergeGlue

            ``` methodSignature
            Optional<BuildTarget> getNativeLibraryMergeGlue()
            ```

        []{#getNativeLibraryMergeCodeGenerator()}

        -   #### getNativeLibraryMergeCodeGenerator

            ``` methodSignature
            Optional<BuildTarget> getNativeLibraryMergeCodeGenerator()
            ```

        []{#getNativeLibraryMergeLocalizedSymbols()}

        -   #### getNativeLibraryMergeLocalizedSymbols

            ``` methodSignature
            Optional<com.google.common.collect.ImmutableSortedSet<String>> getNativeLibraryMergeLocalizedSymbols()
            ```

        []{#getNativeLibraryProguardConfigGenerator()}

        -   #### getNativeLibraryProguardConfigGenerator

            ``` methodSignature
            Optional<BuildTarget> getNativeLibraryProguardConfigGenerator()
            ```

        []{#isEnableRelinker()}

        -   #### isEnableRelinker

            ``` methodSignature
            @Default
            default boolean isEnableRelinker()
            ```

        []{#getRelinkerWhitelist()}

        -   #### getRelinkerWhitelist

            ``` methodSignature
            com.google.common.collect.ImmutableList<Pattern> getRelinkerWhitelist()
            ```

        []{#getManifestEntries()}

        -   #### getManifestEntries

            ``` methodSignature
            @Default
            default ManifestEntries getManifestEntries()
            ```

        []{#getBuildConfigValues()}

        -   #### getBuildConfigValues

            ``` methodSignature
            @Default
            default BuildConfigFields getBuildConfigValues()
            ```

        []{#getPostFilterResourcesCmd()}

        -   #### getPostFilterResourcesCmd

            ``` methodSignature
            Optional<StringWithMacros> getPostFilterResourcesCmd()
            ```

        []{#getBuildConfigValuesFile()}

        -   #### getBuildConfigValuesFile

            ``` methodSignature
            Optional<SourcePath> getBuildConfigValuesFile()
            ```

        []{#isSkipProguard()}

        -   #### isSkipProguard

            ``` methodSignature
            @Default
            default boolean isSkipProguard()
            ```

        []{#getUseDynamicFeature()}

        -   #### getUseDynamicFeature

            ``` methodSignature
            @Default
            default boolean getUseDynamicFeature()
            ```

        []{#getExtraFilteredResources()}

        -   #### getExtraFilteredResources

            ``` methodSignature
            @Default
            default com.google.common.collect.ImmutableSet<String> getExtraFilteredResources()
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
