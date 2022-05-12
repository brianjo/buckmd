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

## Class AndroidBundleDescriptionArg {#class-androidbundledescriptionarg .title title="Class AndroidBundleDescriptionArg"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.AndroidBundleDescriptionArg

::: description
-   

    All Implemented Interfaces:
    :   `AndroidGraphEnhancerArgs`, `HasDuplicateAndroidResourceTypes`,
        `HasExopackageArgs`, `BuildRuleArg`, `ConstructorArg`,
        `DataTransferObject`, `HasApplicationModuleBlacklist`,
        `HasDeclaredDeps`, `HasTests`

    ------------------------------------------------------------------------

        @ParametersAreNonnullByDefault
        @Generated("org.immutables.processor.ProxyProcessor")
        @Immutable
        @CheckReturnValue
        public final class AndroidBundleDescriptionArg
        extends Object

    ::: block
    Immutable implementation of
    `AndroidBundleDescription.AbstractAndroidBundleDescriptionArg`.
    Use the builder to create immutable instances:
    `AndroidBundleDescriptionArg.builder()`.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `AndroidBundleDe      | ::: block             |
        |                       | scriptionArg.Builder` | Builds instances of   |
        |                       |                       | type                  |
        |                       |                       | [`AndroidBundleDesc   |
        |                       |                       | riptionArg`](AndroidB |
        |                       |                       | undleDescriptionArg.h |
        |                       |                       | tml "class in com.fac |
        |                       |                       | ebook.buck.android"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.android.HasDuplicateAndroidResourceTypes}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.android.[HasDuplicateAndroidResourceTypes](HasDuplicateAndroidResourceTypes.html "interface in com.facebook.buck.android")

            `HasDuplicateAndroidResourceTypes.DuplicateResourceBehaviour`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.core.description.arg.BuildRuleArg}

            ### Fields inherited from interface com.facebook.buck.core.description.arg.[BuildRuleArg](../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")

            `DEFAULT_TARGET_PLATFORM_PARAM_NAME`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `s                    | `builder()`           | ::: block             |
        | tatic AndroidBundleDe |                       | Creates a builder for |
        | scriptionArg.Builder` |                       | [`AndroidBundleDesc   |
        |                       |                       | riptionArg`](AndroidB |
        |                       |                       | undleDescriptionArg.h |
        |                       |                       | tml "class in com.fac |
        |                       |                       | ebook.buck.android"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `eq                   | ::: block             |
        |                       | uals​(Object another)` | This instance is      |
        |                       |                       | equal to all          |
        |                       |                       | instances of          |
        |                       |                       | `Android              |
        |                       |                       | BundleDescriptionArg` |
        |                       |                       | that have equal       |
        |                       |                       | attribute values.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.facebook.b       | `getAaptMode()`       |                       |
        | uck.android.AaptMode` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getAd                |                       |
        | ogle.common.collect.I | ditionalAaptParams()` |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common    | `getAllowedDupl       |                       |
        | .collect.ImmutableSet | icateResourceTypes()` |                       |
        | <RDotTxtEntry.RType>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getAndroidA          |                       |
        | Optional<SourcePath>` | ppModularityResult()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<co          | `getAndroi            |                       |
        | m.facebook.buck.andro | dSdkProguardConfig()` |                       |
        | id.ProGuardObfuscateS |                       |                       |
        | tep.SdkProguardType>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `O                    | `getApplicat          |                       |
        | ptional<List<Query>>` | ionModuleBlacklist()` |                       |
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
        | `com.g                | `getApplicationM      |                       |
        | oogle.common.collect. | odulesWithManifest()` |                       |
        | ImmutableSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.g                | `getApplicationMo     |                       |
        | oogle.common.collect. | dulesWithResources()` |                       |
        | ImmutableSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getApplic            |                       |
        | .common.collect.Immut | ationModuleTargets()` |                       |
        | ableSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<C           | `getAssetCo           |                       |
        | ompressionAlgorithm>` | mpressionAlgorithm()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common    | `getBannedDupl        |                       |
        | .collect.ImmutableSet | icateResourceTypes()` |                       |
        | <RDotTxtEntry.RType>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildConfigFields`   | `ge                   |                       |
        |                       | tBuildConfigValues()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getBui               |                       |
        | Optional<SourcePath>` | ldConfigValuesFile()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `g                    |                       |
        | Optional<SourcePath>` | etBundleConfigFile()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `co                   | `getCompatibleWith()` | ::: block             |
        | m.google.common.colle |                       | A list of             |
        | ct.ImmutableList<Unco |                       | `config_setting` a    |
        | nfiguredBuildTarget>` |                       | target is compatible  |
        |                       |                       | with.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `getCpuFilters()`     |                       |
        | ommon.collect.Immutab |                       |                       |
        | leSet<TargetCpuType>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Unco        | `getDef               | ::: block             |
        | nfiguredBuildTarget>` | aultTargetPlatform()` | The name of build     |
        |                       |                       | target default        |
        |                       |                       | \"new\" platform: it  |
        |                       |                       | is used when a        |
        |                       |                       | platform is not       |
        |                       |                       | specified either      |
        |                       |                       | globally or in a      |
        |                       |                       | target which used     |
        |                       |                       | this target as a      |
        |                       |                       | dependency.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getDeps()`           |                       |
        | n.collect.ImmutableSo |                       |                       |
        | rtedSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Opt                  | `getDexCompression()` |                       |
        | ional<com.facebook.bu |                       |                       |
        | ck.android.DexStore>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `g                    |                       |
        |                       | etDexGroupLibLimit()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getDexR              |                       |
        | Optional<SourcePath>` | eorderDataDumpFile()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `get                  |                       |
        | Optional<SourcePath>` | DexReorderToolFile()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getDexTool()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getDisablePreDex()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `HasDuplicateAndroi   | `getDuplica           |                       |
        | dResourceTypes.Duplic | teResourceBehavior()` |                       |
        | ateResourceBehaviour` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getDuplicat          |                       |
        | Optional<SourcePath>` | eResourceWhitelist()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `EnumSet              | `g                    |                       |
        | <RDotTxtEntry.RType>` | etEffectiveBannedDupl |                       |
        |                       | icateResourceTypes()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.co        | `                     |                       |
        | mmon.collect.Immutabl | getExopackageModes()` |                       |
        | eSet<ExopackageMode>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.g                | `getExtr              |                       |
        | oogle.common.collect. | aFilteredResources()` |                       |
        | ImmutableSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getIsCacheable()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getK                 |                       |
        |                       | eepResourcePattern()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildTarget`         | `getKeystore()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getLabels()`         |                       |
        | common.collect.Immuta |                       |                       |
        | bleSortedSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getLicenses()`       |                       |
        | e.common.collect.Immu |                       |                       |
        | tableSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `getLi                |                       |
        |                       | nearAllocHardLimit()` |                       |
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
        | `ManifestEntries`     | `                     |                       |
        |                       | getManifestEntries()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `g                    |                       |
        | Optional<SourcePath>` | etManifestSkeleton()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getMini              |                       |
        |                       | mizePrimaryDexSize()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getModu              |                       |
        | Optional<SourcePath>` | leManifestSkeleton()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getName()`           | ::: block             |
        |                       |                       | Each rule has a name  |
        |                       |                       | :::                   |
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
        | `com.google.common.c  | `getNat               |                       |
        | ollect.ImmutableMap<S | iveLibraryMergeMap()` |                       |
        | tring,​List<Pattern>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `O                    | `                     |                       |
        | ptional<BuildTarget>` | getNativeLibraryProgu |                       |
        |                       | ardConfigGenerator()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getNoDx()`           |                       |
        | .common.collect.Immut |                       |                       |
        | ableSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `get                  |                       |
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
        | `com.google.commo     | `getPreproc           |                       |
        | n.collect.ImmutableSo | essJavaClassesDeps()` |                       |
        | rtedSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getPri               |                       |
        | Optional<SourcePath>` | maryDexClassesFile()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `get                  |                       |
        | ogle.common.collect.I | PrimaryDexPatterns()` |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getPrim              |                       |
        | Optional<SourcePath>` | aryDexScenarioFile()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getProguardConfig()` |                       |
        | Optional<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `                     |                       |
        | ogle.common.collect.I | getProguardJvmArgs()` |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getRedex()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getRedexConfig()`    |                       |
        | Optional<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getRedexExtraArgs()` |                       |
        | n.collect.ImmutableLi |                       |                       |
        | st<StringWithMacros>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.goo              | `ge                   |                       |
        | gle.common.collect.Im | tRelinkerWhitelist()` |                       |
        | mutableList<Pattern>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `getR                 |                       |
        | .facebook.buck.androi | esourceCompression()` |                       |
        | d.ResourcesFilter.Res |                       |                       |
        | ourceCompressionMode` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getResourceFilter()` |                       |
        | ogle.common.collect.I |                       |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getRe                |                       |
        |                       | sourceUnionPackage()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getSecondary         |                       |
        | Optional<SourcePath>` | DexHeadClassesFile()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getSecondary         |                       |
        | Optional<SourcePath>` | DexTailClassesFile()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getTests()`          |                       |
        | n.collect.ImmutableSo |                       |                       |
        | rtedSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `ge                   |                       |
        |                       | tUseDynamicFeature()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getUseSplitDex()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `get                  |                       |
        |                       | XzCompressionLevel()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          | ::: block             |
        |                       |                       | Computes a hash code  |
        |                       |                       | from attributes:      |
        |                       |                       | `keystore`,           |
        |                       |                       | `useSplitDex`,        |
        |                       |                       | `min                  |
        |                       |                       | imizePrimaryDexSize`, |
        |                       |                       | `dexCompression`,     |
        |                       |                       | `primaryDexPatterns`, |
        |                       |                       | `pr                   |
        |                       |                       | imaryDexClassesFile`, |
        |                       |                       | `pri                  |
        |                       |                       | maryDexScenarioFile`, |
        |                       |                       | `primaryDexScen       |
        |                       |                       | arioOverflowAllowed`, |
        |                       |                       | `secondar             |
        |                       |                       | yDexHeadClassesFile`, |
        |                       |                       | `secondar             |
        |                       |                       | yDexTailClassesFile`, |
        |                       |                       | `bundleConfigFile`,   |
        |                       |                       | `android              |
        |                       |                       | AppModularityResult`, |
        |                       |                       | `l                    |
        |                       |                       | inearAllocHardLimit`, |
        |                       |                       | `dexGroupLibLimit`,   |
        |                       |                       | `resourceFilter`,     |
        |                       |                       | `prepro               |
        |                       |                       | cessJavaClassesDeps`, |
        |                       |                       | `xzCompressionLevel`, |
        |                       |                       | `pa                   |
        |                       |                       | ckageAssetLibraries`, |
        |                       |                       | `com                  |
        |                       |                       | pressAssetLibraries`, |
        |                       |                       | `assetC               |
        |                       |                       | ompressionAlgorithm`, |
        |                       |                       | `redex`,              |
        |                       |                       | `redexConfig`,        |
        |                       |                       | `redexExtraArgs`,     |
        |                       |                       | `aaptMode`,           |
        |                       |                       | `licenses`, `labels`, |
        |                       |                       | `de                   |
        |                       |                       | faultTargetPlatform`, |
        |                       |                       | `compatibleWith`,     |
        |                       |                       | `name`, `deps`,       |
        |                       |                       | `exopackage`,         |
        |                       |                       | `exopackageModes`,    |
        |                       |                       | `tests`, `manifest`,  |
        |                       |                       | `manifestSkeleton`,   |
        |                       |                       | `mod                  |
        |                       |                       | uleManifestSkeleton`, |
        |                       |                       | `packageType`,        |
        |                       |                       | `noDx`,               |
        |                       |                       | `disablePreDex`,      |
        |                       |                       | `andro                |
        |                       |                       | idSdkProguardConfig`, |
        |                       |                       | `optimizationPasses`, |
        |                       |                       | `proguardJvmArgs`,    |
        |                       |                       | `proguardConfig`,     |
        |                       |                       | `                     |
        |                       |                       | resourceCompression`, |
        |                       |                       | `skipCrunchPngs`,     |
        |                       |                       | `incl                 |
        |                       |                       | udesVectorDrawables`, |
        |                       |                       | `noA                  |
        |                       |                       | utoVersionResources`, |
        |                       |                       | `noVersionT           |
        |                       |                       | ransitionsResources`, |
        |                       |                       | `noAuto               |
        |                       |                       | AddOverlayResources`, |
        |                       |                       | `appli                |
        |                       |                       | cationModuleTargets`, |
        |                       |                       | `appli                |
        |                       |                       | cationModuleConfigs`, |
        |                       |                       | `applicationM         |
        |                       |                       | odulesWithResources`, |
        |                       |                       | `application          |
        |                       |                       | ModulesWithManifest`, |
        |                       |                       | `applicatio           |
        |                       |                       | nModuleDependencies`, |
        |                       |                       | `isCacheable`,        |
        |                       |                       | `a                    |
        |                       |                       | dditionalAaptParams`, |
        |                       |                       | `trimResourceIds`,    |
        |                       |                       | `allowRDo             |
        |                       |                       | tJavaInSecondaryDex`, |
        |                       |                       | `                     |
        |                       |                       | keepResourcePattern`, |
        |                       |                       | `r                    |
        |                       |                       | esourceUnionPackage`, |
        |                       |                       | `locales`,            |
        |                       |                       | `a                    |
        |                       |                       | apt2LocaleFiltering`, |
        |                       |                       | `loca                 |
        |                       |                       | lizedStringFileName`, |
        |                       |                       | `b                    |
        |                       |                       | uildStringSourceMap`, |
        |                       |                       | `ignor                |
        |                       |                       | eAaptProguardConfig`, |
        |                       |                       | `cpuFilters`,         |
        |                       |                       | `prepro               |
        |                       |                       | cessJavaClassesBash`, |
        |                       |                       | `reo                  |
        |                       |                       | rderClassesIntraDex`, |
        |                       |                       | `dexTool`,            |
        |                       |                       | `dexReorderToolFile`, |
        |                       |                       | `dex                  |
        |                       |                       | ReorderDataDumpFile`, |
        |                       |                       | `na                   |
        |                       |                       | tiveLibraryMergeMap`, |
        |                       |                       | `nat                  |
        |                       |                       | iveLibraryMergeGlue`, |
        |                       |                       | `nativeLibrar         |
        |                       |                       | yMergeCodeGenerator`, |
        |                       |                       | `nativeLibraryMe      |
        |                       |                       | rgeLocalizedSymbols`, |
        |                       |                       | `nativeLibraryProg    |
        |                       |                       | uardConfigGenerator`, |
        |                       |                       | `enableRelinker`,     |
        |                       |                       | `relinkerWhitelist`,  |
        |                       |                       | `manifestEntries`,    |
        |                       |                       | `buildConfigValues`,  |
        |                       |                       | `pos                  |
        |                       |                       | tFilterResourcesCmd`, |
        |                       |                       | `bu                   |
        |                       |                       | ildConfigValuesFile`, |
        |                       |                       | `skipProguard`,       |
        |                       |                       | `useDynamicFeature`,  |
        |                       |                       | `ext                  |
        |                       |                       | raFilteredResources`, |
        |                       |                       | `duplic               |
        |                       |                       | ateResourceBehavior`, |
        |                       |                       | `allowedDup           |
        |                       |                       | licateResourceTypes`, |
        |                       |                       | `bannedDup            |
        |                       |                       | licateResourceTypes`, |
        |                       |                       | `duplica              |
        |                       |                       | teResourceWhitelist`, |
        |                       |                       | `effectiveBannedDup   |
        |                       |                       | licateResourceTypes`, |
        |                       |                       | `applica              |
        |                       |                       | tionModuleBlacklist`. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isAa                 | ::: block             |
        |                       | pt2LocaleFiltering()` | Whether to filter     |
        |                       |                       | locales using aapt2.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isAllowRDot          |                       |
        |                       | JavaInSecondaryDex()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isBu                 |                       |
        |                       | ildStringSourceMap()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isComp               |                       |
        |                       | ressAssetLibraries()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isEnableRelinker()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `isExopackage()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isIgnore             |                       |
        |                       | AaptProguardConfig()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isInclu              |                       |
        |                       | desVectorDrawables()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isNoAutoA            |                       |
        |                       | ddOverlayResources()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isNoAu               |                       |
        |                       | toVersionResources()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isNoVersionTr        |                       |
        |                       | ansitionsResources()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isPac                |                       |
        |                       | kageAssetLibraries()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isPrimaryDexScena    |                       |
        |                       | rioOverflowAllowed()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isReor               |                       |
        |                       | derClassesIntraDex()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `isSkipCrunchPngs()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isSkipProguard()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isTrimResourceIds()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          | ::: block             |
        |                       |                       | Prints the immutable  |
        |                       |                       | value                 |
        |                       |                       | `Android              |
        |                       |                       | BundleDescriptionArg` |
        |                       |                       | with attribute        |
        |                       |                       | values.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `withApplic           |                       |
        | BundleDescriptionArg` | ationModuleBlacklist​( |                       |
        |                       | List<Query> queries)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.BuildRuleArg}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[BuildRuleArg](../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")

            `labelsContainsAnyOf`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getKeystore()}

        -   #### getKeystore

            ``` methodSignature
            public BuildTarget getKeystore()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `keystore` attribute

        []{#getUseSplitDex()}

        -   #### getUseSplitDex

            ``` methodSignature
            public boolean getUseSplitDex()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `useSplitDex` attribute

        []{#getMinimizePrimaryDexSize()}

        -   #### getMinimizePrimaryDexSize

            ``` methodSignature
            public boolean getMinimizePrimaryDexSize()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `minimizePrimaryDexSize` attribute

        []{#getDexCompression()}

        -   #### getDexCompression

            ``` methodSignature
            public Optional<com.facebook.buck.android.DexStore> getDexCompression()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `dexCompression` attribute

        []{#getPrimaryDexPatterns()}

        -   #### getPrimaryDexPatterns

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getPrimaryDexPatterns()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `primaryDexPatterns` attribute

        []{#getPrimaryDexClassesFile()}

        -   #### getPrimaryDexClassesFile

            ``` methodSignature
            public Optional<SourcePath> getPrimaryDexClassesFile()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `primaryDexClassesFile` attribute

        []{#getPrimaryDexScenarioFile()}

        -   #### getPrimaryDexScenarioFile

            ``` methodSignature
            public Optional<SourcePath> getPrimaryDexScenarioFile()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `primaryDexScenarioFile` attribute

        []{#isPrimaryDexScenarioOverflowAllowed()}

        -   #### isPrimaryDexScenarioOverflowAllowed

            ``` methodSignature
            public boolean isPrimaryDexScenarioOverflowAllowed()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `primaryDexScenarioOverflowAllowed`
                attribute

        []{#getSecondaryDexHeadClassesFile()}

        -   #### getSecondaryDexHeadClassesFile

            ``` methodSignature
            public Optional<SourcePath> getSecondaryDexHeadClassesFile()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `secondaryDexHeadClassesFile` attribute

        []{#getSecondaryDexTailClassesFile()}

        -   #### getSecondaryDexTailClassesFile

            ``` methodSignature
            public Optional<SourcePath> getSecondaryDexTailClassesFile()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `secondaryDexTailClassesFile` attribute

        []{#getBundleConfigFile()}

        -   #### getBundleConfigFile

            ``` methodSignature
            public Optional<SourcePath> getBundleConfigFile()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `bundleConfigFile` attribute

        []{#getAndroidAppModularityResult()}

        -   #### getAndroidAppModularityResult

            ``` methodSignature
            public Optional<SourcePath> getAndroidAppModularityResult()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `androidAppModularityResult` attribute

        []{#getLinearAllocHardLimit()}

        -   #### getLinearAllocHardLimit

            ``` methodSignature
            public long getLinearAllocHardLimit()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `linearAllocHardLimit` attribute

        []{#getDexGroupLibLimit()}

        -   #### getDexGroupLibLimit

            ``` methodSignature
            public int getDexGroupLibLimit()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `dexGroupLibLimit` attribute

        []{#getResourceFilter()}

        -   #### getResourceFilter

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getResourceFilter()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `resourceFilter` attribute

        []{#getPreprocessJavaClassesDeps()}

        -   #### getPreprocessJavaClassesDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildTarget> getPreprocessJavaClassesDeps()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `preprocessJavaClassesDeps` attribute

        []{#getXzCompressionLevel()}

        -   #### getXzCompressionLevel

            ``` methodSignature
            public int getXzCompressionLevel()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `xzCompressionLevel` attribute

        []{#isPackageAssetLibraries()}

        -   #### isPackageAssetLibraries

            ``` methodSignature
            public boolean isPackageAssetLibraries()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `packageAssetLibraries` attribute

        []{#isCompressAssetLibraries()}

        -   #### isCompressAssetLibraries

            ``` methodSignature
            public boolean isCompressAssetLibraries()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `compressAssetLibraries` attribute

        []{#getAssetCompressionAlgorithm()}

        -   #### getAssetCompressionAlgorithm

            ``` methodSignature
            public Optional<CompressionAlgorithm> getAssetCompressionAlgorithm()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `assetCompressionAlgorithm` attribute

        []{#getRedex()}

        -   #### getRedex

            ``` methodSignature
            public boolean getRedex()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `redex` attribute

        []{#getRedexConfig()}

        -   #### getRedexConfig

            ``` methodSignature
            public Optional<SourcePath> getRedexConfig()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `redexConfig` attribute

        []{#getRedexExtraArgs()}

        -   #### getRedexExtraArgs

            ``` methodSignature
            public com.google.common.collect.ImmutableList<StringWithMacros> getRedexExtraArgs()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `redexExtraArgs` attribute

        []{#getAaptMode()}

        -   #### getAaptMode

            ``` methodSignature
            public com.facebook.buck.android.AaptMode getAaptMode()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAaptMode` in interface `AndroidGraphEnhancerArgs`

            [Returns:]{.returnLabel}
            :   The value of the `aaptMode` attribute

        []{#getLicenses()}

        -   #### getLicenses

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<SourcePath> getLicenses()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `licenses` attribute

        []{#getLabels()}

        -   #### getLabels

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<String> getLabels()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `labels` attribute

        []{#getDefaultTargetPlatform()}

        -   #### getDefaultTargetPlatform

            ``` methodSignature
            public Optional<UnconfiguredBuildTarget> getDefaultTargetPlatform()
            ```

            ::: block
            The name of build target default \"new\" platform: it is
            used when a platform is not specified either globally or in
            a target which used this target as a dependency.
            The value is a build target, but we specify it as string,
            because this function is not actually called, but the attr
            is fetched by name from the raw (unconfigured) target node.
            :::

        []{#getCompatibleWith()}

        -   #### getCompatibleWith

            ``` methodSignature
            public com.google.common.collect.ImmutableList<UnconfiguredBuildTarget> getCompatibleWith()
            ```

            ::: block
            A list of `config_setting` a target is compatible with.
            :::

        []{#getName()}

        -   #### getName

            ``` methodSignature
            public String getName()
            ```

            ::: block
            Each rule has a name
            :::

        []{#getDeps()}

        -   #### getDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildTarget> getDeps()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `deps` attribute

        []{#isExopackage()}

        -   #### isExopackage

            ``` methodSignature
            public Optional<Boolean> isExopackage()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `exopackage` attribute

        []{#getExopackageModes()}

        -   #### getExopackageModes

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<ExopackageMode> getExopackageModes()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `exopackageModes` attribute

        []{#getTests()}

        -   #### getTests

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildTarget> getTests()
            ```

            [Returns:]{.returnLabel}
            :   A list of tests of this target.

        []{#getManifest()}

        -   #### getManifest

            ``` methodSignature
            public Optional<SourcePath> getManifest()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `manifest` attribute

        []{#getManifestSkeleton()}

        -   #### getManifestSkeleton

            ``` methodSignature
            public Optional<SourcePath> getManifestSkeleton()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `manifestSkeleton` attribute

        []{#getModuleManifestSkeleton()}

        -   #### getModuleManifestSkeleton

            ``` methodSignature
            public Optional<SourcePath> getModuleManifestSkeleton()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `moduleManifestSkeleton` attribute

        []{#getPackageType()}

        -   #### getPackageType

            ``` methodSignature
            public Optional<String> getPackageType()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `packageType` attribute

        []{#getNoDx()}

        -   #### getNoDx

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<BuildTarget> getNoDx()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `noDx` attribute

        []{#getDisablePreDex()}

        -   #### getDisablePreDex

            ``` methodSignature
            public boolean getDisablePreDex()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `disablePreDex` attribute

        []{#getAndroidSdkProguardConfig()}

        -   #### getAndroidSdkProguardConfig

            ``` methodSignature
            public Optional<com.facebook.buck.android.ProGuardObfuscateStep.SdkProguardType> getAndroidSdkProguardConfig()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `androidSdkProguardConfig` attribute

        []{#getOptimizationPasses()}

        -   #### getOptimizationPasses

            ``` methodSignature
            public int getOptimizationPasses()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `optimizationPasses` attribute

        []{#getProguardJvmArgs()}

        -   #### getProguardJvmArgs

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getProguardJvmArgs()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `proguardJvmArgs` attribute

        []{#getProguardConfig()}

        -   #### getProguardConfig

            ``` methodSignature
            public Optional<SourcePath> getProguardConfig()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `proguardConfig` attribute

        []{#getResourceCompression()}

        -   #### getResourceCompression

            ``` methodSignature
            public com.facebook.buck.android.ResourcesFilter.ResourceCompressionMode getResourceCompression()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `resourceCompression` attribute

        []{#isSkipCrunchPngs()}

        -   #### isSkipCrunchPngs

            ``` methodSignature
            public Optional<Boolean> isSkipCrunchPngs()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `skipCrunchPngs` attribute

        []{#isIncludesVectorDrawables()}

        -   #### isIncludesVectorDrawables

            ``` methodSignature
            public boolean isIncludesVectorDrawables()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `includesVectorDrawables` attribute

        []{#isNoAutoVersionResources()}

        -   #### isNoAutoVersionResources

            ``` methodSignature
            public boolean isNoAutoVersionResources()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `noAutoVersionResources` attribute

        []{#isNoVersionTransitionsResources()}

        -   #### isNoVersionTransitionsResources

            ``` methodSignature
            public boolean isNoVersionTransitionsResources()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `noVersionTransitionsResources`
                attribute

        []{#isNoAutoAddOverlayResources()}

        -   #### isNoAutoAddOverlayResources

            ``` methodSignature
            public boolean isNoAutoAddOverlayResources()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `noAutoAddOverlayResources` attribute

        []{#getApplicationModuleTargets()}

        -   #### getApplicationModuleTargets

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<BuildTarget> getApplicationModuleTargets()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `applicationModuleTargets` attribute

        []{#getApplicationModuleConfigs()}

        -   #### getApplicationModuleConfigs

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​com.google.common.collect.ImmutableList<BuildTarget>> getApplicationModuleConfigs()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `applicationModuleConfigs` attribute

        []{#getApplicationModulesWithResources()}

        -   #### getApplicationModulesWithResources

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<String> getApplicationModulesWithResources()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `applicationModulesWithResources`
                attribute

        []{#getApplicationModulesWithManifest()}

        -   #### getApplicationModulesWithManifest

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<String> getApplicationModulesWithManifest()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `applicationModulesWithManifest`
                attribute

        []{#getApplicationModuleDependencies()}

        -   #### getApplicationModuleDependencies

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableMap<String,​com.google.common.collect.ImmutableList<String>>> getApplicationModuleDependencies()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `applicationModuleDependencies`
                attribute

        []{#getIsCacheable()}

        -   #### getIsCacheable

            ``` methodSignature
            public boolean getIsCacheable()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `isCacheable` attribute

        []{#getAdditionalAaptParams()}

        -   #### getAdditionalAaptParams

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getAdditionalAaptParams()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `additionalAaptParams` attribute

        []{#isTrimResourceIds()}

        -   #### isTrimResourceIds

            ``` methodSignature
            public boolean isTrimResourceIds()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `trimResourceIds` attribute

        []{#isAllowRDotJavaInSecondaryDex()}

        -   #### isAllowRDotJavaInSecondaryDex

            ``` methodSignature
            public boolean isAllowRDotJavaInSecondaryDex()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `allowRDotJavaInSecondaryDex` attribute

        []{#getKeepResourcePattern()}

        -   #### getKeepResourcePattern

            ``` methodSignature
            public Optional<String> getKeepResourcePattern()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `keepResourcePattern` attribute

        []{#getResourceUnionPackage()}

        -   #### getResourceUnionPackage

            ``` methodSignature
            public Optional<String> getResourceUnionPackage()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `resourceUnionPackage` attribute

        []{#getLocales()}

        -   #### getLocales

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<String> getLocales()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `locales` attribute

        []{#isAapt2LocaleFiltering()}

        -   #### isAapt2LocaleFiltering

            ``` methodSignature
            public boolean isAapt2LocaleFiltering()
            ```

            ::: block
            Whether to filter locales using aapt2.
            :::

        []{#getLocalizedStringFileName()}

        -   #### getLocalizedStringFileName

            ``` methodSignature
            public Optional<String> getLocalizedStringFileName()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `localizedStringFileName` attribute

        []{#isBuildStringSourceMap()}

        -   #### isBuildStringSourceMap

            ``` methodSignature
            public boolean isBuildStringSourceMap()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `buildStringSourceMap` attribute

        []{#isIgnoreAaptProguardConfig()}

        -   #### isIgnoreAaptProguardConfig

            ``` methodSignature
            public boolean isIgnoreAaptProguardConfig()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `ignoreAaptProguardConfig` attribute

        []{#getCpuFilters()}

        -   #### getCpuFilters

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<TargetCpuType> getCpuFilters()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `cpuFilters` attribute

        []{#getPreprocessJavaClassesBash()}

        -   #### getPreprocessJavaClassesBash

            ``` methodSignature
            public Optional<StringWithMacros> getPreprocessJavaClassesBash()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `preprocessJavaClassesBash` attribute

        []{#isReorderClassesIntraDex()}

        -   #### isReorderClassesIntraDex

            ``` methodSignature
            public boolean isReorderClassesIntraDex()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `reorderClassesIntraDex` attribute

        []{#getDexTool()}

        -   #### getDexTool

            ``` methodSignature
            public String getDexTool()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `dexTool` attribute

        []{#getDexReorderToolFile()}

        -   #### getDexReorderToolFile

            ``` methodSignature
            public Optional<SourcePath> getDexReorderToolFile()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `dexReorderToolFile` attribute

        []{#getDexReorderDataDumpFile()}

        -   #### getDexReorderDataDumpFile

            ``` methodSignature
            public Optional<SourcePath> getDexReorderDataDumpFile()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `dexReorderDataDumpFile` attribute

        []{#getNativeLibraryMergeMap()}

        -   #### getNativeLibraryMergeMap

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​List<Pattern>> getNativeLibraryMergeMap()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `nativeLibraryMergeMap` attribute

        []{#getNativeLibraryMergeGlue()}

        -   #### getNativeLibraryMergeGlue

            ``` methodSignature
            public Optional<BuildTarget> getNativeLibraryMergeGlue()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `nativeLibraryMergeGlue` attribute

        []{#getNativeLibraryMergeCodeGenerator()}

        -   #### getNativeLibraryMergeCodeGenerator

            ``` methodSignature
            public Optional<BuildTarget> getNativeLibraryMergeCodeGenerator()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `nativeLibraryMergeCodeGenerator`
                attribute

        []{#getNativeLibraryMergeLocalizedSymbols()}

        -   #### getNativeLibraryMergeLocalizedSymbols

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableSortedSet<String>> getNativeLibraryMergeLocalizedSymbols()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `nativeLibraryMergeLocalizedSymbols`
                attribute

        []{#getNativeLibraryProguardConfigGenerator()}

        -   #### getNativeLibraryProguardConfigGenerator

            ``` methodSignature
            public Optional<BuildTarget> getNativeLibraryProguardConfigGenerator()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `nativeLibraryProguardConfigGenerator`
                attribute

        []{#isEnableRelinker()}

        -   #### isEnableRelinker

            ``` methodSignature
            public boolean isEnableRelinker()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `enableRelinker` attribute

        []{#getRelinkerWhitelist()}

        -   #### getRelinkerWhitelist

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Pattern> getRelinkerWhitelist()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `relinkerWhitelist` attribute

        []{#getManifestEntries()}

        -   #### getManifestEntries

            ``` methodSignature
            public ManifestEntries getManifestEntries()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `manifestEntries` attribute

        []{#getBuildConfigValues()}

        -   #### getBuildConfigValues

            ``` methodSignature
            public BuildConfigFields getBuildConfigValues()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `buildConfigValues` attribute

        []{#getPostFilterResourcesCmd()}

        -   #### getPostFilterResourcesCmd

            ``` methodSignature
            public Optional<StringWithMacros> getPostFilterResourcesCmd()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `postFilterResourcesCmd` attribute

        []{#getBuildConfigValuesFile()}

        -   #### getBuildConfigValuesFile

            ``` methodSignature
            public Optional<SourcePath> getBuildConfigValuesFile()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `buildConfigValuesFile` attribute

        []{#isSkipProguard()}

        -   #### isSkipProguard

            ``` methodSignature
            public boolean isSkipProguard()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `skipProguard` attribute

        []{#getUseDynamicFeature()}

        -   #### getUseDynamicFeature

            ``` methodSignature
            public boolean getUseDynamicFeature()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `useDynamicFeature` attribute

        []{#getExtraFilteredResources()}

        -   #### getExtraFilteredResources

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<String> getExtraFilteredResources()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `extraFilteredResources` attribute

        []{#getDuplicateResourceBehavior()}

        -   #### getDuplicateResourceBehavior

            ``` methodSignature
            public HasDuplicateAndroidResourceTypes.DuplicateResourceBehaviour getDuplicateResourceBehavior()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `duplicateResourceBehavior` attribute

        []{#getAllowedDuplicateResourceTypes()}

        -   #### getAllowedDuplicateResourceTypes

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<RDotTxtEntry.RType> getAllowedDuplicateResourceTypes()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `allowedDuplicateResourceTypes`
                attribute

        []{#getBannedDuplicateResourceTypes()}

        -   #### getBannedDuplicateResourceTypes

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<RDotTxtEntry.RType> getBannedDuplicateResourceTypes()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `bannedDuplicateResourceTypes`
                attribute

        []{#getDuplicateResourceWhitelist()}

        -   #### getDuplicateResourceWhitelist

            ``` methodSignature
            public Optional<SourcePath> getDuplicateResourceWhitelist()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `duplicateResourceWhitelist` attribute

        []{#getEffectiveBannedDuplicateResourceTypes()}

        -   #### getEffectiveBannedDuplicateResourceTypes

            ``` methodSignature
            public EnumSet<RDotTxtEntry.RType> getEffectiveBannedDuplicateResourceTypes()
            ```

            [Returns:]{.returnLabel}
            :   The computed-at-construction value of the
                `effectiveBannedDuplicateResourceTypes` attribute

        []{#getApplicationModuleBlacklist()}

        -   #### getApplicationModuleBlacklist

            ``` methodSignature
            public Optional<List<Query>> getApplicationModuleBlacklist()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `applicationModuleBlacklist` attribute

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(@Nullable
                                  Object another)
            ```

            ::: block
            This instance is equal to all instances of
            `AndroidBundleDescriptionArg` that have equal attribute
            values.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

            [Returns:]{.returnLabel}
            :   `true` if `this` is equal to `another` instance

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            ::: block
            Computes a hash code from attributes: `keystore`,
            `useSplitDex`, `minimizePrimaryDexSize`, `dexCompression`,
            `primaryDexPatterns`, `primaryDexClassesFile`,
            `primaryDexScenarioFile`,
            `primaryDexScenarioOverflowAllowed`,
            `secondaryDexHeadClassesFile`,
            `secondaryDexTailClassesFile`, `bundleConfigFile`,
            `androidAppModularityResult`, `linearAllocHardLimit`,
            `dexGroupLibLimit`, `resourceFilter`,
            `preprocessJavaClassesDeps`, `xzCompressionLevel`,
            `packageAssetLibraries`, `compressAssetLibraries`,
            `assetCompressionAlgorithm`, `redex`, `redexConfig`,
            `redexExtraArgs`, `aaptMode`, `licenses`, `labels`,
            `defaultTargetPlatform`, `compatibleWith`, `name`, `deps`,
            `exopackage`, `exopackageModes`, `tests`, `manifest`,
            `manifestSkeleton`, `moduleManifestSkeleton`, `packageType`,
            `noDx`, `disablePreDex`, `androidSdkProguardConfig`,
            `optimizationPasses`, `proguardJvmArgs`, `proguardConfig`,
            `resourceCompression`, `skipCrunchPngs`,
            `includesVectorDrawables`, `noAutoVersionResources`,
            `noVersionTransitionsResources`,
            `noAutoAddOverlayResources`, `applicationModuleTargets`,
            `applicationModuleConfigs`,
            `applicationModulesWithResources`,
            `applicationModulesWithManifest`,
            `applicationModuleDependencies`, `isCacheable`,
            `additionalAaptParams`, `trimResourceIds`,
            `allowRDotJavaInSecondaryDex`, `keepResourcePattern`,
            `resourceUnionPackage`, `locales`, `aapt2LocaleFiltering`,
            `localizedStringFileName`, `buildStringSourceMap`,
            `ignoreAaptProguardConfig`, `cpuFilters`,
            `preprocessJavaClassesBash`, `reorderClassesIntraDex`,
            `dexTool`, `dexReorderToolFile`, `dexReorderDataDumpFile`,
            `nativeLibraryMergeMap`, `nativeLibraryMergeGlue`,
            `nativeLibraryMergeCodeGenerator`,
            `nativeLibraryMergeLocalizedSymbols`,
            `nativeLibraryProguardConfigGenerator`, `enableRelinker`,
            `relinkerWhitelist`, `manifestEntries`, `buildConfigValues`,
            `postFilterResourcesCmd`, `buildConfigValuesFile`,
            `skipProguard`, `useDynamicFeature`,
            `extraFilteredResources`, `duplicateResourceBehavior`,
            `allowedDuplicateResourceTypes`,
            `bannedDuplicateResourceTypes`,
            `duplicateResourceWhitelist`,
            `effectiveBannedDuplicateResourceTypes`,
            `applicationModuleBlacklist`.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`

            [Returns:]{.returnLabel}
            :   hashCode value

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            ::: block
            Prints the immutable value `AndroidBundleDescriptionArg`
            with attribute values.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

            [Returns:]{.returnLabel}
            :   A string representation of the value

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static AndroidBundleDescriptionArg.Builder builder()
            ```

            ::: block
            Creates a builder for
            [`AndroidBundleDescriptionArg`](AndroidBundleDescriptionArg.html "class in com.facebook.buck.android").
            :::

            [Returns:]{.returnLabel}
            :   A new AndroidBundleDescriptionArg builder

        []{#withApplicationModuleBlacklist(java.util.List)}

        -   #### withApplicationModuleBlacklist

            ``` methodSignature
            public AndroidBundleDescriptionArg withApplicationModuleBlacklist​(List<Query> queries)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `withApplicationModuleBlacklist` in
                interface `HasApplicationModuleBlacklist`
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
