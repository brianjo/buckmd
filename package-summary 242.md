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
-   Package
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Package com.facebook.buck.android {#package-com.facebook.buck.android .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [AndroidGraphEnhancerArgs](Andro  |                                   |
    | idGraphEnhancerArgs.html "interfa |                                   |
    | ce in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AndroidKotlinCoreArg](A          |                                   |
    | ndroidKotlinCoreArg.html "interfa |                                   |
    | ce in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AndroidL                         | ::: block                         |
    | ibraryCompilerFactory](AndroidLib | Factory providing implementations |
    | raryCompilerFactory.html "interfa | of                                |
    | ce in com.facebook.buck.android") | [`Configured                      |
    |                                   | CompilerFactory`](../jvm/java/Con |
    |                                   | figuredCompilerFactory.html "clas |
    |                                   | s in com.facebook.buck.jvm.java") |
    |                                   | for the specified `  language`.   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AndroidLibraryDe                 |                                   |
    | scription.CoreArg](AndroidLibrary |                                   |
    | Description.CoreArg.html "interfa |                                   |
    | ce in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AndroidLinkableMetadata](Andr    | ::: block                         |
    | oidLinkableMetadata.html "interfa | Information needed to determine   |
    | ce in com.facebook.buck.android") | the correct placement of native   |
    |                                   | linkables in an android apk       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AndroidManifestReader](An        | ::: block                         |
    | droidManifestReader.html "interfa | Allows querying an Android        |
    | ce in com.facebook.buck.android") | manifest file for various types   |
    |                                   | of information.                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AndroidNativeTargetConfigura     | ::: block                         |
    | tionMatcher](AndroidNativeTargetC | Encapsulates logic to check       |
    | onfigurationMatcher.html "interfa | whether platform in configuration |
    | ce in com.facebook.buck.android") | of a given target matches the CPU |
    |                                   | type.                             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DexWithClas                      | ::: block                         |
    | ses](DexWithClasses.html "interfa | Object that represents a          |
    | ce in com.facebook.buck.android") | `.dex.jar` file that knows what   |
    |                                   | `.class` files went into it, as   |
    |                                   | well as its estimated dex weight. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 |                                   |
    | FilteredResourcesProvider](Filter |                                   |
    | edResourcesProvider.html "interfa |                                   |
    | ce in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [FilterResourcesSteps             |                                   |
    | .DrawableFinder](FilterResourcesS |                                   |
    | teps.DrawableFinder.html "interfa |                                   |
    | ce in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [FilterResource                   |                                   |
    | sSteps.ImageScaler](FilterResourc |                                   |
    | esSteps.ImageScaler.html "interfa |                                   |
    | ce in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [HasAndroidResourceDeps](Has      | ::: block                         |
    | AndroidResourceDeps.html "interfa | Indicates that this class may     |
    | ce in com.facebook.buck.android") | have android resources that       |
    |                                   | should be packaged into an APK.   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HasDe                            |                                   |
    | xFiles](HasDexFiles.html "interfa |                                   |
    | ce in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [HasDuplicateAn                   |                                   |
    | droidResourceTypes](HasDuplicateA |                                   |
    | ndroidResourceTypes.html "interfa |                                   |
    | ce in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [HasExopackageArgs                |                                   |
    | ](HasExopackageArgs.html "interfa |                                   |
    | ce in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [HasInstallableApk                | ::: block                         |
    | ](HasInstallableApk.html "interfa | Build rule that generates an APK  |
    | ce in com.facebook.buck.android") | that can be installed with the    |
    |                                   | install command.                  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NativeLibraryBuildRule](Nat      | ::: block                         |
    | iveLibraryBuildRule.html "interfa | [`BuildRule`](../core             |
    | ce in com.facebook.buck.android") | /rules/BuildRule.html "interface  |
    |                                   | in com.facebook.buck.core.rules") |
    |                                   | that contains various `.so` files |
    |                                   | for Android, organized by target  |
    |                                   | CPU architecture.                 |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [SmartDexingStep.DexInputHa       |                                   |
    | shesProvider](SmartDexingStep.Dex |                                   |
    | InputHashesProvider.html "interfa |                                   |
    | ce in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [UnsortedAndroidResourc           |                                   |
    | eDeps.Callback](UnsortedAndroidRe |                                   |
    | sourceDeps.Callback.html "interfa |                                   |
    | ce in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [AabBuil                          | ::: block                         |
    | derStep](AabBuilderStep.html "cla | Merges resources into a final     |
    | ss in com.facebook.buck.android") | Android App Bundle using          |
    |                                   | bundletool.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Aap                              | ::: block                         |
    | t2Compile](Aapt2Compile.html "cla | Perform the \"aapt2 compile\"     |
    | ss in com.facebook.buck.android") | step of a single Android          |
    |                                   | resource.                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Aapt2Link](Aapt2Link.html "cla   | ::: block                         |
    | ss in com.facebook.buck.android") | Perform the \"aapt2 link\" step   |
    |                                   | of building an Android app.       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AaptPackageResource              | ::: block                         |
    | s](AaptPackageResources.html "cla | Packages the resources using      |
    | ss in com.facebook.buck.android") | `aapt`.                           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AaptStep](AaptStep.html "cla     | ::: block                         |
    | ss in com.facebook.buck.android") | Runs the Android Asset Packaging  |
    |                                   | Tool (`aapt`), which creates an   |
    |                                   | `.apk` file.                      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AdbHelper](AdbHelper.html "cla   | ::: block                         |
    | ss in com.facebook.buck.android") | Helper for executing commands     |
    |                                   | over ADB, especially for multiple |
    |                                   | devices.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AidlStep](AidlStep.html "cla     |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AndroidAar](AndroidAar.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AndroidAarDescription            | ::: block                         |
    | ](AndroidAarDescription.html "cla | Description for a                 |
    | ss in com.facebook.buck.android") | [`BuildRule`](../core             |
    |                                   | /rules/BuildRule.html "interface  |
    |                                   | in com.facebook.buck.core.rules") |
    |                                   | that generates an `.aar` file.    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AndroidAarDescriptionArg](A      | ::: block                         |
    | ndroidAarDescriptionArg.html "cla | Immutable implementation of       |
    | ss in com.facebook.buck.android") | `AndroidAarDescription.A          |
    |                                   | bstractAndroidAarDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AndroidAar                       | ::: block                         |
    | DescriptionArg.Builder](AndroidAa | Builds instances of type          |
    | rDescriptionArg.Builder.html "cla | [`AndroidAarDescriptionArg`](An   |
    | ss in com.facebook.buck.android") | droidAarDescriptionArg.html "clas |
    |                                   | s in com.facebook.buck.android"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AndroidApkBuildab                | ::: block                         |
    | le](AndroidApkBuildable.html "cla | The class is responsible to       |
    | ss in com.facebook.buck.android") | create unoptimized apk through    |
    |                                   | [`ApkBuilde                       |
    |                                   | rStep`](ApkBuilderStep.html "clas |
    |                                   | s in com.facebook.buck.android"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AndroidApkOptimiz                | ::: block                         |
    | er](AndroidApkOptimizer.html "cla | The class executes all binary     |
    | ss in com.facebook.buck.android") | steps responsible for optimizing  |
    |                                   | apk specific components.          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AndroidAppModularit              |                                   |
    | y](AndroidAppModularity.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AndroidA                         |                                   |
    | ppModularityDescription](AndroidA |                                   |
    | ppModularityDescription.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AndroidAppModu                   | ::: block                         |
    | larityDescriptionArg](AndroidAppM | Immutable implementation of       |
    | odularityDescriptionArg.html "cla | `AndroidApp                       |
    | ss in com.facebook.buck.android") | ModularityDescription.AbstractAnd |
    |                                   | roidAppModularityDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AndroidAppModularityDescriptio   | ::: block                         |
    | nArg.Builder](AndroidAppModularit | Builds instances of type          |
    | yDescriptionArg.Builder.html "cla | [`AndroidAppModula                |
    | ss in com.facebook.buck.android") | rityDescriptionArg`](AndroidAppMo |
    |                                   | dularityDescriptionArg.html "clas |
    |                                   | s in com.facebook.buck.android"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AndroidAppMo                     |                                   |
    | dularityGraphEnhancer](AndroidApp |                                   |
    | ModularityGraphEnhancer.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AndroidApp                       |                                   |
    | ModularityVerification](AndroidAp |                                   |
    | pModularityVerification.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Andro                            | ::: block                         |
    | idBinary](AndroidBinary.html "cla | android_binary( name =            |
    | ss in com.facebook.buck.android") | \'messenger\', manifest =         |
    |                                   | \'AndroidManifest.xml\', deps =   |
    |                                   | \[                                |
    |                                   | \'//src/com/facebo                |
    |                                   | ok/messenger:messenger_library\', |
    |                                   | \], )                             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AndroidBinaryDescription](A      |                                   |
    | ndroidBinaryDescription.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | AndroidBinaryDescriptionArg](Andr | Immutable implementation of       |
    | oidBinaryDescriptionArg.html "cla | `AndroidBinaryDescription.Abst    |
    | ss in com.facebook.buck.android") | ractAndroidBinaryDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AndroidBinaryDes                 | ::: block                         |
    | criptionArg.Builder](AndroidBinar | Builds instances of type          |
    | yDescriptionArg.Builder.html "cla | [`An                              |
    | ss in com.facebook.buck.android") | droidBinaryDescriptionArg`](Andro |
    |                                   | idBinaryDescriptionArg.html "clas |
    |                                   | s in com.facebook.buck.android"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AndroidBinaryE                   | ::: block                         |
    | xopackageSymlinkTree](AndroidBina | Create an exopackage symlink tree |
    | ryExopackageSymlinkTree.html "cla | for Android binaries rules        |
    | ss in com.facebook.buck.android") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AndroidBinaryFactor              |                                   |
    | y](AndroidBinaryFactory.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AndroidBinaryFilesInfo]          |                                   |
    | (AndroidBinaryFilesInfo.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AndroidBinaryGraphEnhancer](And  |                                   |
    | roidBinaryGraphEnhancer.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AndroidBinar                     |                                   |
    | yGraphEnhancerFactory](AndroidBin |                                   |
    | aryGraphEnhancerFactory.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [An                               | ::: block                         |
    | droidBinaryNonExoInstaller](Andro | Installs a non-exopackage apk.    |
    | idBinaryNonExoInstaller.html "cla | :::                               |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AndroidBinaryOptimizer]          | ::: block                         |
    | (AndroidBinaryOptimizer.html "cla | The class executes all common     |
    | ss in com.facebook.buck.android") | binary steps responsible for      |
    |                                   | optimizing aab/apk.               |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AndroidBinaryPathUtility](A      | ::: block                         |
    | ndroidBinaryPathUtility.html "cla | Utility class to resolve path     |
    | ss in com.facebook.buck.android") | conflicts in aab/apk.             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AndroidBuckCo                    |                                   |
    | nfig](AndroidBuckConfig.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AndroidBuildCon                  | ::: block                         |
    | fig](AndroidBuildConfig.html "cla | [`BuildRule`](../core             |
    | ss in com.facebook.buck.android") | /rules/BuildRule.html "interface  |
    |                                   | in com.facebook.buck.core.rules") |
    |                                   | that can generate a               |
    |                                   | `BuildConfig.java` file and       |
    |                                   | compile it so it can be used as a |
    |                                   | Java library.                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Andr                             |                                   |
    | oidBuildConfigDescription](Androi |                                   |
    | dBuildConfigDescription.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AndroidBui                       | ::: block                         |
    | ldConfigDescriptionArg](AndroidBu | Immutable implementation of       |
    | ildConfigDescriptionArg.html "cla | `Androi                           |
    | ss in com.facebook.buck.android") | dBuildConfigDescription.AbstractA |
    |                                   | ndroidBuildConfigDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AndroidBuildConfigDescript       | ::: block                         |
    | ionArg.Builder](AndroidBuildConfi | Builds instances of type          |
    | gDescriptionArg.Builder.html "cla | [`AndroidBuild                    |
    | ss in com.facebook.buck.android") | ConfigDescriptionArg`](AndroidBui |
    |                                   | ldConfigDescriptionArg.html "clas |
    |                                   | s in com.facebook.buck.android"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Andro                            | ::: block                         |
    | idBundle](AndroidBundle.html "cla | android_bundle( name =            |
    | ss in com.facebook.buck.android") | \'messenger\', manifest =         |
    |                                   | \'AndroidManifest.xml\', deps =   |
    |                                   | \[                                |
    |                                   | \'//src/com/facebo                |
    |                                   | ok/messenger:messenger_library\', |
    |                                   | \], )                             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AndroidBundleBuildable]          | ::: block                         |
    | (AndroidBundleBuildable.html "cla | The class is responsible to       |
    | ss in com.facebook.buck.android") | create final bundle by taking     |
    |                                   | individual module information and |
    |                                   | passing to `Config.Bundletool`    |
    |                                   | through                           |
    |                                   | [`AabBuilde                       |
    |                                   | rStep`](AabBuilderStep.html "clas |
    |                                   | s in com.facebook.buck.android"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AndroidBundleDescription](A      |                                   |
    | ndroidBundleDescription.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | AndroidBundleDescriptionArg](Andr | Immutable implementation of       |
    | oidBundleDescriptionArg.html "cla | `AndroidBundleDescription.Abst    |
    | ss in com.facebook.buck.android") | ractAndroidBundleDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AndroidBundleDes                 | ::: block                         |
    | criptionArg.Builder](AndroidBundl | Builds instances of type          |
    | eDescriptionArg.Builder.html "cla | [`An                              |
    | ss in com.facebook.buck.android") | droidBundleDescriptionArg`](Andro |
    |                                   | idBundleDescriptionArg.html "clas |
    |                                   | s in com.facebook.buck.android"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AndroidBundleFactor              |                                   |
    | y](AndroidBundleFactory.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AndroidBundleOptimizer]          | ::: block                         |
    | (AndroidBundleOptimizer.html "cla | The class executes all binary     |
    | ss in com.facebook.buck.android") | steps responsible for optimizing  |
    |                                   | aab specific components.          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AndroidClasspathProvider](A      |                                   |
    | ndroidClasspathProvider.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [                                 |                                   |
    | AndroidDescriptionsProvider](Andr |                                   |
    | oidDescriptionsProvider.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AndroidInstallConfi              |                                   |
    | g](AndroidInstallConfig.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AndroidInstrumentationApk](An    | ::: block                         |
    | droidInstrumentationApk.html "cla | Apk that functions as a test      |
    | ss in com.facebook.buck.android") | package in Android.               |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AndroidInstrumenta               |                                   |
    | tionApkDescription](AndroidInstru |                                   |
    | mentationApkDescription.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AndroidInstrumentationAp         | ::: block                         |
    | kDescriptionArg](AndroidInstrumen | Immutable implementation of       |
    | tationApkDescriptionArg.html "cla | `AndroidInstrumentati             |
    | ss in com.facebook.buck.android") | onApkDescription.AbstractAndroidI |
    |                                   | nstrumentationApkDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Android                          | ::: block                         |
    | InstrumentationApkDescriptionArg. | Builds instances of type          |
    | Builder](AndroidInstrumentationAp | [`AndroidInstrumentationApkD      |
    | kDescriptionArg.Builder.html "cla | escriptionArg`](AndroidInstrument |
    | ss in com.facebook.buck.android") | ationApkDescriptionArg.html "clas |
    |                                   | s in com.facebook.buck.android"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AndroidInstrumentationTest](And  |                                   |
    | roidInstrumentationTest.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AndroidInstrumentati             |                                   |
    | onTestDescription](AndroidInstrum |                                   |
    | entationTestDescription.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AndroidInstrumentationTest       | ::: block                         |
    | DescriptionArg](AndroidInstrument | Immutable implementation of       |
    | ationTestDescriptionArg.html "cla | `AndroidInstrumentation           |
    | ss in com.facebook.buck.android") | TestDescription.AbstractAndroidIn |
    |                                   | strumentationTestDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AndroidIn                        | ::: block                         |
    | strumentationTestDescriptionArg.B | Builds instances of type          |
    | uilder](AndroidInstrumentationTes | [`AndroidInstrumentationTestDe    |
    | tDescriptionArg.Builder.html "cla | scriptionArg`](AndroidInstrumenta |
    | ss in com.facebook.buck.android") | tionTestDescriptionArg.html "clas |
    |                                   | s in com.facebook.buck.android"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Android                          |                                   |
    | Library](AndroidLibrary.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AndroidLibrary.Builder]          |                                   |
    | (AndroidLibrary.Builder.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AndroidLibraryDescription](An    |                                   |
    | droidLibraryDescription.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [An                               | ::: block                         |
    | droidLibraryDescriptionArg](Andro | Immutable implementation of       |
    | idLibraryDescriptionArg.html "cla | `AndroidLibraryDescription.Abstr  |
    | ss in com.facebook.buck.android") | actAndroidLibraryDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AndroidLibraryDesc               | ::: block                         |
    | riptionArg.Builder](AndroidLibrar | Builds instances of type          |
    | yDescriptionArg.Builder.html "cla | [`Andr                            |
    | ss in com.facebook.buck.android") | oidLibraryDescriptionArg`](Androi |
    |                                   | dLibraryDescriptionArg.html "clas |
    |                                   | s in com.facebook.buck.android"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 |                                   |
    | AndroidLibraryGraphEnhancer](Andr |                                   |
    | oidLibraryGraphEnhancer.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AndroidMa                        | ::: block                         |
    | nifest](AndroidManifest.html "cla | [`AndroidMan                      |
    | ss in com.facebook.buck.android") | ifest`](AndroidManifest.html "cla |
    |                                   | ss in com.facebook.buck.android") |
    |                                   | is a                              |
    |                                   | [`BuildRule`](../core             |
    |                                   | /rules/BuildRule.html "interface  |
    |                                   | in com.facebook.buck.core.rules") |
    |                                   | that can generate an Android      |
    |                                   | manifest from a skeleton manifest |
    |                                   | and the library manifests from    |
    |                                   | its dependencies.                 |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AndroidManifestDescription](And  |                                   |
    | roidManifestDescription.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Andr                             | ::: block                         |
    | oidManifestDescriptionArg](Androi | Immutable implementation of       |
    | dManifestDescriptionArg.html "cla | `                                 |
    | ss in com.facebook.buck.android") | AndroidManifestDescription.Abstra |
    |                                   | ctAndroidManifestDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AndroidManifestDescr             | ::: block                         |
    | iptionArg.Builder](AndroidManifes | Builds instances of type          |
    | tDescriptionArg.Builder.html "cla | [`Androi                          |
    | ss in com.facebook.buck.android") | dManifestDescriptionArg`](Android |
    |                                   | ManifestDescriptionArg.html "clas |
    |                                   | s in com.facebook.buck.android"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AndroidManifestFactory]          |                                   |
    | (AndroidManifestFactory.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [An                               |                                   |
    | droidModuleConsistencyStep](Andro |                                   |
    | idModuleConsistencyStep.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AndroidNativeLibsPackageable     |                                   |
    | GraphEnhancer](AndroidNativeLibsP |                                   |
    | ackageableGraphEnhancer.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AndroidPrebuilt                  |                                   |
    | Aar](AndroidPrebuiltAar.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Andr                             | ::: block                         |
    | oidPrebuiltAarDescription](Androi | Description for a                 |
    | dPrebuiltAarDescription.html "cla | [`BuildRule`](../core             |
    | ss in com.facebook.buck.android") | /rules/BuildRule.html "interface  |
    |                                   | in com.facebook.buck.core.rules") |
    |                                   | that wraps an `.aar` file as an   |
    |                                   | Android dependency.               |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AndroidPre                       | ::: block                         |
    | builtAarDescriptionArg](AndroidPr | Immutable implementation of       |
    | ebuiltAarDescriptionArg.html "cla | `Androi                           |
    | ss in com.facebook.buck.android") | dPrebuiltAarDescription.AbstractA |
    |                                   | ndroidPrebuiltAarDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AndroidPrebuiltAarDescript       | ::: block                         |
    | ionArg.Builder](AndroidPrebuiltAa | Builds instances of type          |
    | rDescriptionArg.Builder.html "cla | [`AndroidPrebu                    |
    | ss in com.facebook.buck.android") | iltAarDescriptionArg`](AndroidPre |
    |                                   | builtAarDescriptionArg.html "clas |
    |                                   | s in com.facebook.buck.android"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AndroidRe                        | ::: block                         |
    | source](AndroidResource.html "cla | An object that represents the     |
    | ss in com.facebook.buck.android") | resources of an android library.  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AndroidResourceDescription](And  |                                   |
    | roidResourceDescription.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Andr                             | ::: block                         |
    | oidResourceDescriptionArg](Androi | Immutable implementation of       |
    | dResourceDescriptionArg.html "cla | `                                 |
    | ss in com.facebook.buck.android") | AndroidResourceDescription.Abstra |
    |                                   | ctAndroidResourceDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AndroidResourceDescr             | ::: block                         |
    | iptionArg.Builder](AndroidResourc | Builds instances of type          |
    | eDescriptionArg.Builder.html "cla | [`Androi                          |
    | ss in com.facebook.buck.android") | dResourceDescriptionArg`](Android |
    |                                   | ResourceDescriptionArg.html "clas |
    |                                   | s in com.facebook.buck.android"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AndroidResourceHelper            |                                   |
    | ](AndroidResourceHelper.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AndroidResourceInde              |                                   |
    | x](AndroidResourceIndex.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AndroidTra                       |                                   |
    | nsitiveDependencyGraph](AndroidTr |                                   |
    | ansitiveDependencyGraph.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ApkBuil                          | ::: block                         |
    | derStep](ApkBuilderStep.html "cla | Merges resources into a final     |
    | ss in com.facebook.buck.android") | APK.                              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ApkGenrule](ApkGenrule.html "cla | ::: block                         |
    | ss in com.facebook.buck.android") | A specialization of a genrule     |
    |                                   | that specifically allows the      |
    |                                   | modification of apks.             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ApkGenruleDescription            |                                   |
    | ](ApkGenruleDescription.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ApkGenruleDescriptionArg](A      | ::: block                         |
    | pkGenruleDescriptionArg.html "cla | Immutable implementation of       |
    | ss in com.facebook.buck.android") | `ApkGenruleDescription.A          |
    |                                   | bstractApkGenruleDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ApkGenrule                       | ::: block                         |
    | DescriptionArg.Builder](ApkGenrul | Builds instances of type          |
    | eDescriptionArg.Builder.html "cla | [`ApkGenruleDescriptionArg`](Ap   |
    | ss in com.facebook.buck.android") | kGenruleDescriptionArg.html "clas |
    |                                   | s in com.facebook.buck.android"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ApkInst                          |                                   |
    | allStep](ApkInstallStep.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AppBuil                          | ::: block                         |
    | derBase](AppBuilderBase.html "cla | A class that provides information |
    | ss in com.facebook.buck.android") | that are shared across AabBuilder |
    |                                   | and ApkBuilder, currently only    |
    |                                   | private key and certificate are   |
    |                                   | needed                            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppBuilderBase.PrivateKe         |                                   |
    | yAndCertificate](AppBuilderBase.P |                                   |
    | rivateKeyAndCertificate.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AppModularityMetadataUtil](Ap    |                                   |
    | pModularityMetadataUtil.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AssembleDirectori                |                                   |
    | es](AssembleDirectories.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [BuckEventAndroidLogger]          | ::: block                         |
    | (BuckEventAndroidLogger.html "cla | Implementation of `ILogger` which |
    | ss in com.facebook.buck.android") | posts to an                       |
    |                                   | [`BuckEventBus`](                 |
    |                                   | ../event/BuckEventBus.html "inter |
    |                                   | face in com.facebook.buck.event") |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Bui                              | ::: block                         |
    | ldConfigs](BuildConfigs.html "cla | Utilities for generating a        |
    | ss in com.facebook.buck.android") | `BuildConfig.java` file for       |
    |                                   | Android.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ClassName                        | ::: block                         |
    | Filter](ClassNameFilter.html "cla | Filter for internal class names.  |
    | ss in com.facebook.buck.android") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CompileStringsS                  | ::: block                         |
    | tep](CompileStringsStep.html "cla | This                              |
    | ss in com.facebook.buck.android") | [`Step`](../step/Step.html "inte  |
    |                                   | rface in com.facebook.buck.step") |
    |                                   | takes a list of string resource   |
    |                                   | files (strings.xml), groups them  |
    |                                   | by locales, and for each locale   |
    |                                   | generates a file with all the     |
    |                                   | string resources for that locale. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ConcatStep](ConcatStep.html "cla | ::: block                         |
    | ss in com.facebook.buck.android") | Takes in a list of files and      |
    |                                   | outputs a concatenation of them   |
    |                                   | in the same directory.            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ConstraintBasedAndroi            | ::: block                         |
    | dNativeTargetConfigurationMatcher | Matcher that uses constraints to  |
    | ](ConstraintBasedAndroidNativeTar | figure out whether platform in    |
    | getConfigurationMatcher.html "cla | target configuration matches the  |
    | ss in com.facebook.buck.android") | CPU type.                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CopyNativeLibrari                | ::: block                         |
    | es](CopyNativeLibraries.html "cla | A                                 |
    | ss in com.facebook.buck.android") | [`BuildRule`](../core             |
    |                                   | /rules/BuildRule.html "interface  |
    |                                   | in com.facebook.buck.core.rules") |
    |                                   | that gathers shared objects       |
    |                                   | generated by `ndk_library` and    |
    |                                   | `  prebuilt_native_library` rules |
    |                                   | into a directory.                 |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Cop                              |                                   |
    | yNativeLibraries.StrippedObjectDe |                                   |
    | scription](CopyNativeLibraries.St |                                   |
    | rippedObjectDescription.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [DefaultAndroidLibr               |                                   |
    | aryCompilerFactory](DefaultAndroi |                                   |
    | dLibraryCompilerFactory.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [De                               |                                   |
    | faultAndroidManifestReader](Defau |                                   |
    | ltAndroidManifestReader.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [DexProducedFromJavaLibrary](Dex  | ::: block                         |
    | ProducedFromJavaLibrary.html "cla | [                                 |
    | ss in com.facebook.buck.android") | `DexProducedFromJavaLibrary`](Dex |
    |                                   | ProducedFromJavaLibrary.html "cla |
    |                                   | ss in com.facebook.buck.android") |
    |                                   | is a                              |
    |                                   | [`BuildRule`](../core             |
    |                                   | /rules/BuildRule.html "interface  |
    |                                   | in com.facebook.buck.core.rules") |
    |                                   | that serves a very specific       |
    |                                   | purpose: it takes a               |
    |                                   | [`JavaLibrary`](../jv             |
    |                                   | m/core/JavaLibrary.html "interfac |
    |                                   | e in com.facebook.buck.jvm.core") |
    |                                   | and dexes the output of the       |
    |                                   | [`JavaLibrary`](../jv             |
    |                                   | m/core/JavaLibrary.html "interfac |
    |                                   | e in com.facebook.buck.jvm.core") |
    |                                   | if its list of classes is         |
    |                                   | non-empty.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Dummy                            | ::: block                         |
    | RDotJava](DummyRDotJava.html "cla | Buildable that takes in a list of |
    | ss in com.facebook.buck.android") | [`HasAndroidResourceDeps`](Has    |
    |                                   | AndroidResourceDeps.html "interfa |
    |                                   | ce in com.facebook.buck.android") |
    |                                   | and for each of these rules,      |
    |                                   | first creates an `R.java` file    |
    |                                   | using                             |
    |                                   | [`MergeAndroidResourcesStep`](Me  |
    |                                   | rgeAndroidResourcesStep.html "cla |
    |                                   | ss in com.facebook.buck.android") |
    |                                   | and compiles it to generate a     |
    |                                   | corresponding `R.class` file.     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DxConfig](DxConfig.html "cla     |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [DxStep](DxStep.html "cla         |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ExopackageArgsHelpe              |                                   |
    | r](ExopackageArgsHelper.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Exopacka                         | ::: block                         |
    | geDeviceDirectoryLister](Exopacka | This lists the entire contents of |
    | geDeviceDirectoryLister.html "cla | the exopackage installation       |
    | ss in com.facebook.buck.android") | directory on the requested        |
    |                                   | devices.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ExopackageFilesInstaller](E      | ::: block                         |
    | xopackageFilesInstaller.html "cla | Installs exopackage files to the  |
    | ss in com.facebook.buck.android") | device/devices.                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ExopackageInstallFinisher](Ex    | ::: block                         |
    | opackageInstallFinisher.html "cla | Finishes exopackage installation  |
    | ss in com.facebook.buck.android") | by: updating the metadata.txt     |
    |                                   | files for the different           |
    |                                   | exopackage types deleting         |
    |                                   | unwanted files (.so/.dex/.apk     |
    |                                   | from previous installs)           |
    |                                   | installing the apk killing the    |
    |                                   | app/process                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Ex                               | ::: block                         |
    | opackageResourcesInstaller](Exopa | Installs exopackage resource      |
    | ckageResourcesInstaller.html "cla | files to the device/devices.      |
    | ss in com.facebook.buck.android") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Extrac                           |                                   |
    | tFromAndroidManifestStep](Extract |                                   |
    | FromAndroidManifestStep.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [FilterResourcesStep              | ::: block                         |
    | s](FilterResourcesSteps.html "cla | This                              |
    | ss in com.facebook.buck.android") | [`Step`](../step/Step.html "inte  |
    |                                   | rface in com.facebook.buck.step") |
    |                                   | copies `res` directories to a     |
    |                                   | different location, while         |
    |                                   | filtering out certain resources.  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Fi                               |                                   |
    | lterResourcesSteps.Builder](Filte |                                   |
    | rResourcesSteps.Builder.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [FilterResourcesSteps.DefaultDr   |                                   |
    | awableFinder](FilterResourcesStep |                                   |
    | s.DefaultDrawableFinder.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [FilterResourcesS                 | ::: block                         |
    | teps.ResourceFilter](FilterResour | Helper class for interpreting the |
    | cesSteps.ResourceFilter.html "cla | resource_filter argument to       |
    | ss in com.facebook.buck.android") | android_binary().                 |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [GenAidl](GenAidl.html "cla       | ::: block                         |
    | ss in com.facebook.buck.android") | Buildable for generating a .java  |
    |                                   | file from an .aidl file.          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [GenAidlDescript                  |                                   |
    | ion](GenAidlDescription.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [GenAidlDescriptionArg            | ::: block                         |
    | ](GenAidlDescriptionArg.html "cla | Immutable implementation of       |
    | ss in com.facebook.buck.android") | `GenAidlDescriptio                |
    |                                   | n.AbstractGenAidlDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [GenA                             | ::: block                         |
    | idlDescriptionArg.Builder](GenAid | Builds instances of type          |
    | lDescriptionArg.Builder.html "cla | [`GenAidlDescriptionArg`]         |
    | ss in com.facebook.buck.android") | (GenAidlDescriptionArg.html "clas |
    |                                   | s in com.facebook.buck.android"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [GenerateBuildConfigStep](        |                                   |
    | GenerateBuildConfigStep.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [GenerateManifestSte              |                                   |
    | p](GenerateManifestStep.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [GenerateRDo                      |                                   |
    | tJava](GenerateRDotJava.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [GenerateStringResources](        | ::: block                         |
    | GenerateStringResources.html "cla | Copy filtered string resources    |
    | ss in com.facebook.buck.android") | (values/strings.xml) files to     |
    |                                   | output directory.                 |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [GetStringsFilesSt                | ::: block                         |
    | ep](GetStringsFilesStep.html "cla | Generates a list of strings.xml   |
    | ss in com.facebook.buck.android") | files                             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HashInputJarsToDexStep]          | ::: block                         |
    | (HashInputJarsToDexStep.html "cla | Step responsible for hashing dex  |
    | ss in com.facebook.buck.android") | inputs to be passed to            |
    |                                   | [`SmartDexing                     |
    |                                   | Step`](SmartDexingStep.html "clas |
    |                                   | s in com.facebook.buck.android"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HasInstallableApk.ApkInfo](Ha    |                                   |
    | sInstallableApk.ApkInfo.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [IdentityResourcesProvider](Id    |                                   |
    | entityResourcesProvider.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [InstrumentationSt                |                                   |
    | ep](InstrumentationStep.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [IntraDexReorderSt                | ::: block                         |
    | ep](IntraDexReorderStep.html "cla | Runs a user supplied reordering   |
    | ss in com.facebook.buck.android") | tool on all dexes.                |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [KeystorePropert                  |                                   |
    | ies](KeystoreProperties.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [MergeAndroidResourcesStep](Me    |                                   |
    | rgeAndroidResourcesStep.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [M                                | ::: block                         |
    | ergeAssets](MergeAssets.html "cla | MergeAssets adds the assets for   |
    | ss in com.facebook.buck.android") | an APK into the output of aapt.   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | MergeThirdPartyJarResources](Merg | Merges resources from third party |
    | eThirdPartyJarResources.html "cla | jars for exo-for-resources.       |
    | ss in com.facebook.buck.android") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ModuleInfo](ModuleInfo.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [NativeFil                        |                                   |
    | esInfo](NativeFilesInfo.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Native                           | ::: block                         |
    | LibraryProguardGenerator](NativeL | This provides a way for           |
    | ibraryProguardGenerator.html "cla | android_binary rules to generate  |
    | ss in com.facebook.buck.android") | proguard config based on the      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Ndk                              |                                   |
    | BuildStep](NdkBuildStep.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [NdkLibrary](NdkLibrary.html "cla | ::: block                         |
    | ss in com.facebook.buck.android") | An object that represents a       |
    |                                   | collection of Android NDK source  |
    |                                   | code.                             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NdkLibraryDescription            | Deprecated.                       |
    | ](NdkLibraryDescription.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [NdkLibraryDescriptionArg](N      | ::: block                         |
    | dkLibraryDescriptionArg.html "cla | Immutable implementation of       |
    | ss in com.facebook.buck.android") | `NdkLibraryDescription.A          |
    |                                   | bstractNdkLibraryDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NdkLibrary                       | ::: block                         |
    | DescriptionArg.Builder](NdkLibrar | Builds instances of type          |
    | yDescriptionArg.Builder.html "cla | [`NdkLibraryDescriptionArg`](Nd   |
    | ss in com.facebook.buck.android") | kLibraryDescriptionArg.html "clas |
    |                                   | s in com.facebook.buck.android"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NdkToolchainBuildRule            | ::: block                         |
    | ](NdkToolchainBuildRule.html "cla | This                              |
    | ss in com.facebook.buck.android") | [`BuildRule`](../core             |
    |                                   | /rules/BuildRule.html "interface  |
    |                                   | in com.facebook.buck.core.rules") |
    |                                   | is just a placeholder to hold the |
    |                                   | created                           |
    |                                   | [`NdkCxxPl                        |
    |                                   | atform`](toolchain/ndk/NdkCxxPlat |
    |                                   | form.html "interface in com.faceb |
    |                                   | ook.buck.android.toolchain.ndk"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NdkToolchainDescription](        | ::: block                         |
    | NdkToolchainDescription.html "cla | Defines an ndk_toolchain rule     |
    | ss in com.facebook.buck.android") | that allows a                     |
    |                                   | [`NdkCxxP                         |
    |                                   | latform`](toolchain/ndk/NdkCxxPla |
    |                                   | tform.html "interface in com.face |
    |                                   | book.buck.android.toolchain.ndk") |
    |                                   | to be configured as a build       |
    |                                   | target.                           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NdkToolchainDescriptionArg](Ndk  | ::: block                         |
    | ToolchainDescriptionArg.html "cla | An ndk_toolchain is mostly just a |
    | ss in com.facebook.buck.android") | cxx_toolchain and a few other     |
    |                                   | fields.                           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NdkToolchainDe                   | ::: block                         |
    | scriptionArg.Builder](NdkToolchai | Builds instances of type          |
    | nDescriptionArg.Builder.html "cla | [`                                |
    | ss in com.facebook.buck.android") | NdkToolchainDescriptionArg`](NdkT |
    |                                   | oolchainDescriptionArg.html "clas |
    |                                   | s in com.facebook.buck.android"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NoDxArg                          |                                   |
    | sHelper](NoDxArgsHelper.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [NoopAndroidNativeTargetConfigura | ::: block                         |
    | tionMatcher](NoopAndroidNativeTar | An implementation that doesn\'t   |
    | getConfigurationMatcher.html "cla | perform any calculations and      |
    | ss in com.facebook.buck.android") | always matches targets.           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PackagedRes                      | ::: block                         |
    | ource](PackagedResource.html "cla | Represents a zip that has been    |
    | ss in com.facebook.buck.android") | packaged as a resource with Buck, |
    |                                   | but which should be expanded at   |
    |                                   | most once during Buck\'s          |
    |                                   | execution (not per-build).        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PackageStringAsse                | ::: block                         |
    | ts](PackageStringAssets.html "cla | Buildable responsible for         |
    | ss in com.facebook.buck.android") | compiling non-english string      |
    |                                   | resources to `.fbstr` files       |
    |                                   | stored as assets.                 |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PrebuiltNativeLibrary            | ::: block                         |
    | ](PrebuiltNativeLibrary.html "cla | An object that represents the     |
    | ss in com.facebook.buck.android") | resources prebuilt native         |
    |                                   | library.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PrebuiltNa                       |                                   |
    | tiveLibraryDescription](PrebuiltN |                                   |
    | ativeLibraryDescription.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [PrebuiltNativeLi                 | ::: block                         |
    | braryDescriptionArg](PrebuiltNati | Immutable implementation of       |
    | veLibraryDescriptionArg.html "cla | `PrebuiltNati                     |
    | ss in com.facebook.buck.android") | veLibraryDescription.AbstractPreb |
    |                                   | uiltNativeLibraryDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PrebuiltNativeLibraryDescription | ::: block                         |
    | Arg.Builder](PrebuiltNativeLibrar | Builds instances of type          |
    | yDescriptionArg.Builder.html "cla | [`PrebuiltNativeLibr              |
    | ss in com.facebook.buck.android") | aryDescriptionArg`](PrebuiltNativ |
    |                                   | eLibraryDescriptionArg.html "clas |
    |                                   | s in com.facebook.buck.android"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PreDexedFilesSort                | ::: block                         |
    | er](PreDexedFilesSorter.html "cla | Responsible for bucketing         |
    | ss in com.facebook.buck.android") | pre-dexed objects into primary    |
    |                                   | and secondary dex files.          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PreDexedFilesSorter.Result](Pre  |                                   |
    | DexedFilesSorter.Result.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [P                                | ::: block                         |
    | reDexMerge](PreDexMerge.html "cla | Buildable that is responsible     |
    | ss in com.facebook.buck.android") | for: Bucketing pre-dexed jars     |
    |                                   | into lists for primary and        |
    |                                   | secondary dex files (if the app   |
    |                                   | is split-dex).                    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PreDexSingleDexMerg              | ::: block                         |
    | e](PreDexSingleDexMerge.html "cla | Constructs a single merged dex    |
    | ss in com.facebook.buck.android") | file from pre-dexed inputs        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PreDexSplitDexGro                | ::: block                         |
    | up](PreDexSplitDexGroup.html "cla | Takes a subset of the predexed    |
    | ss in com.facebook.buck.android") | libraries (for a single           |
    |                                   | APKModule) and produces copies of |
    |                                   | the predexed libraries to be      |
    |                                   | merged into the primary dex, and  |
    |                                   | a set of secondary dexes, capped  |
    |                                   | at the dex weight limit.          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PreDexSplitDexMer                | ::: block                         |
    | ge](PreDexSplitDexMerge.html "cla | This is the top level rule        |
    | ss in com.facebook.buck.android") | responsible for producing         |
    |                                   | multiple dexes for an apk from    |
    |                                   | predexed library rules.           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ProGuar                          |                                   |
    | dConfig](ProGuardConfig.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ProguardM                        | ::: block                         |
    | apping](ProguardMapping.html "cla | Parser for ProGuard-generated     |
    | ss in com.facebook.buck.android") | mapping files.                    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ProGuardObfuscateStep            |                                   |
    | ](ProGuardObfuscateStep.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [RedexArgs                        |                                   |
    | Helper](RedexArgsHelper.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ReplaceM                         | ::: block                         |
    | anifestPlaceholdersStep](ReplaceM | Replaces placeholders in the      |
    | anifestPlaceholdersStep.html "cla | android manifest.                 |
    | ss in com.facebook.buck.android") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ResourceFiles                    |                                   |
    | Info](ResourceFilesInfo.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ResourceF                        |                                   |
    | ilters](ResourceFilters.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ResourceFilters.Qualifiers](Res  |                                   |
    | ourceFilters.Qualifiers.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Resources                        | ::: block                         |
    | Filter](ResourcesFilter.html "cla | Buildable that is responsible for |
    | ss in com.facebook.buck.android") | taking a set of res/ directories  |
    |                                   | and applying an optional resource |
    |                                   | filter to them, ultimately        |
    |                                   | generating the final set of res/  |
    |                                   | directories whose contents should |
    |                                   | be included in an APK.            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 |                                   |
    | ResourcesFilter.BuildOutput](Reso |                                   |
    | urcesFilter.BuildOutput.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Robolectr                        |                                   |
    | icTest](RobolectricTest.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [RobolectricTestDescription](Rob  |                                   |
    | olectricTestDescription.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Robo                             | ::: block                         |
    | lectricTestDescriptionArg](Robole | Immutable implementation of       |
    | ctricTestDescriptionArg.html "cla | `                                 |
    | ss in com.facebook.buck.android") | RobolectricTestDescription.Abstra |
    |                                   | ctRobolectricTestDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RobolectricTestDescr             | ::: block                         |
    | iptionArg.Builder](RobolectricTes | Builds instances of type          |
    | tDescriptionArg.Builder.html "cla | [`Robole                          |
    | ss in com.facebook.buck.android") | ctricTestDescriptionArg`](Robolec |
    |                                   | tricTestDescriptionArg.html "clas |
    |                                   | s in com.facebook.buck.android"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Robolectric                      | ::: block                         |
    | TestX](RobolectricTestX.html "cla | The new Robolectric Test rule     |
    | ss in com.facebook.buck.android") | that uses the test protocol to    |
    |                                   | run.                              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [SmartDexi                        | ::: block                         |
    | ngStep](SmartDexingStep.html "cla | Optimized dx command runner which |
    | ss in com.facebook.buck.android") | can invoke multiple dx commands   |
    |                                   | in parallel and also avoid doing  |
    |                                   | unnecessary dx invocations in the |
    |                                   | first place.                      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [SplitRe                          |                                   |
    | sources](SplitResources.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [SplitUberRDotJavaJa              | ::: block                         |
    | r](SplitUberRDotJavaJar.html "cla | Split a jar generated by          |
    | ss in com.facebook.buck.android") | compiling uber-R.java files into  |
    |                                   | subset jars.                      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Spl                              | ::: block                         |
    | itZipStep](SplitZipStep.html "cla | Split zipping tool designed to    |
    | ss in com.facebook.buck.android") | divide input code blobs into a    |
    |                                   | set of output jar files such that |
    |                                   | none will exceed the DexOpt       |
    |                                   | LinearAlloc limit or the dx       |
    |                                   | method limit when passed through  |
    |                                   | dx \--dex.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [StringRes                        | ::: block                         |
    | ources](StringResources.html "cla | Represents string resources of    |
    | ss in com.facebook.buck.android") | types string, plural and array    |
    |                                   | for a locale.                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Strip                            | ::: block                         |
    | Linkable](StripLinkable.html "cla | A BuildRule for stripping         |
    | ss in com.facebook.buck.android") | (removing inessential information |
    |                                   | from executable binary programs   |
    |                                   | and object files) binaries.       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [StripStep](StripStep.html "cla   | ::: block                         |
    | ss in com.facebook.buck.android") | Run strip on a binary.            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [UnitTestO                        | ::: block                         |
    | ptions](UnitTestOptions.html "cla | Creates a                         |
    | ss in com.facebook.buck.android") | \"test_config.properties\" file   |
    |                                   | to be included for additional     |
    |                                   | configuration during Android unit |
    |                                   | tests                             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 |                                   |
    | UnsortedAndroidResourceDeps](Unso |                                   |
    | rtedAndroidResourceDeps.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [UnstrippedNativeLibraries](Un    |                                   |
    | strippedNativeLibraries.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [UnzipAar](UnzipAar.html "cla     |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [WriteAppModuleMetadataStep](Wri  |                                   |
    | teAppModuleMetadataStep.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [WriteFileHash                    | ::: block                         |
    | Code](WriteFileHashCode.html "cla | Computes the hash of a file and   |
    | ss in com.facebook.buck.android") | writes it as the output.          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Zip                              |                                   |
    | alignStep](ZipalignStep.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Enum                              | Description                       |
    +===================================+===================================+
    | [AndroidBuckConfig.N              | ::: block                         |
    | dkSearchOrderEntry](AndroidBuckCo | Values acceptable for             |
    | nfig.NdkSearchOrderEntry.html "en | ndk.ndk_search_order.             |
    | um in com.facebook.buck.android") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AndroidInstallConfig.            |                                   |
    | ConcurrentInstall](AndroidInstall |                                   |
    | Config.ConcurrentInstall.html "en |                                   |
    | um in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AndroidLibraryDescr              |                                   |
    | iption.JvmLanguage](AndroidLibrar |                                   |
    | yDescription.JvmLanguage.html "en |                                   |
    | um in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [BinaryType](BinaryType.html "en  | ::: block                         |
    | um in com.facebook.buck.android") | Supported android binary types    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CompressionAlgorit               | ::: block                         |
    | hm](CompressionAlgorithm.html "en | Assets in the apks (e.g.          |
    | um in com.facebook.buck.android") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DxSt                             | ::: block                         |
    | ep.Option](DxStep.Option.html "en | Options to pass to `dx`.          |
    | um in com.facebook.buck.android") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HasDuplicateAndroidResourceTyp   |                                   |
    | es.DuplicateResourceBehaviour](Ha |                                   |
    | sDuplicateAndroidResourceTypes.Du |                                   |
    | plicateResourceBehaviour.html "en |                                   |
    | um in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ResourceFilters.Density]         | ::: block                         |
    | (ResourceFilters.Density.html "en | Represents the names and values   |
    | um in com.facebook.buck.android") | of valid densities for resources  |
    |                                   | as defined in                     |
    |                                   | http://developer.android.co       |
    |                                   | m/guide/topics/resources/providin |
    |                                   | g-resources.html#DensityQualifier |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Enum Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Exception                         | Description                       |
    +===================================+===================================+
    | [AdbHelper.                       | ::: block                         |
    | CommandFailedException](AdbHelper | An exception that indicates that  |
    | .CommandFailedException.html "cla | an executed command returned an   |
    | ss in com.facebook.buck.android") | unsuccessful exit code.           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [MergeAndroidResou                |                                   |
    | rcesStep.DuplicateResourceExcepti |                                   |
    | on](MergeAndroidResourcesStep.Dup |                                   |
    | licateResourceException.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+

    : Exception Summary[ ]{.tabEnd}
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../index.html)
-   Package
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

[]{#skip.navbar.bottom}
:::
