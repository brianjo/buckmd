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
# Package com.facebook.buck.apple {#package-com.facebook.buck.apple .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [AbstractIdbFailureInfo](A        | ::: block                         |
    | bstractIdbFailureInfo.html "inter | Object that represents the        |
    | face in com.facebook.buck.apple") | failure information of a test     |
    |                                   | when using idb                    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AbstractIdbTestResult](          | ::: block                         |
    | AbstractIdbTestResult.html "inter | Object that represents the xctest |
    | face in com.facebook.buck.apple") | result when using idb             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleCustomLin                   | ::: block                         |
    | kingDepsDescription](AppleCustomL | This interface helps customizing  |
    | inkingDepsDescription.html "inter | linking dependencies.             |
    | face in com.facebook.buck.apple") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleLibrarySwiftDelegate](Appl  | ::: block                         |
    | eLibrarySwiftDelegate.html "inter | Provides an ability to inject     |
    | face in com.facebook.buck.apple") | [`CxxPreprocessorInput`](.        |
    |                                   | ./cxx/CxxPreprocessorInput.html " |
    |                                   | class in com.facebook.buck.cxx")s |
    |                                   | for the Swift compilation         |
    |                                   | process.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleNativ                       | ::: block                         |
    | eTargetDescriptionArg](AppleNativ | Arguments common to Apple         |
    | eTargetDescriptionArg.html "inter | targets.                          |
    | face in com.facebook.buck.apple") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildRuleWithBinary              | ::: block                         |
    | ](BuildRuleWithBinary.html "inter | Build rule that holds a binary    |
    | face in com.facebook.buck.apple") | build rule                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [GroupedSource.Visitor](          |                                   |
    | GroupedSource.Visitor.html "inter |                                   |
    | face in com.facebook.buck.apple") |                                   |
    +-----------------------------------+-----------------------------------+
    | [HasAppleBundleFields]            |                                   |
    | (HasAppleBundleFields.html "inter |                                   |
    | face in com.facebook.buck.apple") |                                   |
    +-----------------------------------+-----------------------------------+
    | [HasAppleBundleResou              | ::: block                         |
    | rcesDescription](HasAppleBundleRe | Rule description for rules which  |
    | sourcesDescription.html "interfac | have apple bundles                |
    | e in com.facebook.buck.apple")\<T | :::                               |
    | extends                           |                                   |
    | [BuildRuleArg]                    |                                   |
    | (../core/description/arg/BuildRul |                                   |
    | eArg.html "interface in com.faceb |                                   |
    | ook.buck.core.description.arg")\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [HasAppleCodesignFields](H        | ::: block                         |
    | asAppleCodesignFields.html "inter | Defines a set of codesign-related |
    | face in com.facebook.buck.apple") | fields that are applicable to     |
    |                                   | bundle-like rules.                |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HasEntitlementsFile              |                                   |
    | ](HasEntitlementsFile.html "inter |                                   |
    | face in com.facebook.buck.apple") |                                   |
    +-----------------------------------+-----------------------------------+
    | [IdbOutputParsing                 | ::: block                         |
    | .IdbResultCallback](IdbOutputPars | Callbacks invoked with events     |
    | ing.IdbResultCallback.html "inter | emitted by `idb`.                 |
    | face in com.facebook.buck.apple") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [IdbRunTestsStep.Stdout           | ::: block                         |
    | ReadingCallback](IdbRunTestsStep. | Interface for reading the stdout  |
    | StdoutReadingCallback.html "inter | of idb                            |
    | face in com.facebook.buck.apple") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [XCodeD                           |                                   |
    | escriptionClassSupplier](XCodeDes |                                   |
    | criptionClassSupplier.html "inter |                                   |
    | face in com.facebook.buck.apple") |                                   |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [AppleAssetC                      |                                   |
    | atalog](AppleAssetCatalog.html "c |                                   |
    | lass in com.facebook.buck.apple") |                                   |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | AppleAssetCatalogDescription](App | Description for an                |
    | leAssetCatalogDescription.html "c | apple_asset_catalog rule, which   |
    | lass in com.facebook.buck.apple") | identifies an asset catalog for   |
    |                                   | an iOS or Mac OS X library or     |
    |                                   | binary.                           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleA                           | ::: block                         |
    | ssetCatalogDescriptionArg](AppleA | Immutable implementation of       |
    | ssetCatalogDescriptionArg.html "c | `Appl                             |
    | lass in com.facebook.buck.apple") | eAssetCatalogDescription.Abstract |
    |                                   | AppleAssetCatalogDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleAssetCatalogDescr           | ::: block                         |
    | iptionArg.Builder](AppleAssetCata | Builds instances of type          |
    | logDescriptionArg.Builder.html "c | [`AppleAss                        |
    | lass in com.facebook.buck.apple") | etCatalogDescriptionArg`](AppleAs |
    |                                   | setCatalogDescriptionArg.html "cl |
    |                                   | ass in com.facebook.buck.apple"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleAssetCatalo                 | ::: block                         |
    | gsCompilationOptions](AppleAssetC | Argument type for                 |
    | atalogsCompilationOptions.html "c | a                                 |
    | lass in com.facebook.buck.apple") | sset_catalogs_compilation_options |
    |                                   | used in apple_bundle              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleAssetCatalogsCompilationOpt | ::: block                         |
    | ions.Builder](AppleAssetCatalogsC | Builds instances of type          |
    | ompilationOptions.Builder.html "c | [`AppleAssetCatalogs              |
    | lass in com.facebook.buck.apple") | CompilationOptions`](AppleAssetCa |
    |                                   | talogsCompilationOptions.html "cl |
    |                                   | ass in com.facebook.buck.apple"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleBinaryDescriptio            |                                   |
    | n](AppleBinaryDescription.html "c |                                   |
    | lass in com.facebook.buck.apple") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AppleBinaryDescriptionArg](      | ::: block                         |
    | AppleBinaryDescriptionArg.html "c | Immutable implementation of       |
    | lass in com.facebook.buck.apple") | `AppleBinaryDescription.Ab        |
    |                                   | stractAppleBinaryDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleBinar                       | ::: block                         |
    | yDescriptionArg.Builder](AppleBin | Builds instances of type          |
    | aryDescriptionArg.Builder.html "c | [`AppleBinaryDescriptionArg`](A   |
    | lass in com.facebook.buck.apple") | ppleBinaryDescriptionArg.html "cl |
    |                                   | ass in com.facebook.buck.apple"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleBu                          | ::: block                         |
    | ildRules](AppleBuildRules.html "c | Helpers for reading properties of |
    | lass in com.facebook.buck.apple") | Apple target build rules.         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleBundle](AppleBundle.html "c | ::: block                         |
    | lass in com.facebook.buck.apple") | Creates a bundle: a directory     |
    |                                   | containing files and              |
    |                                   | subdirectories, described by an   |
    |                                   | Info.plist.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleBundleDescriptio            |                                   |
    | n](AppleBundleDescription.html "c |                                   |
    | lass in com.facebook.buck.apple") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AppleBundleDescriptionArg](      | ::: block                         |
    | AppleBundleDescriptionArg.html "c | Immutable implementation of       |
    | lass in com.facebook.buck.apple") | `AppleBundleDescription.Ab        |
    |                                   | stractAppleBundleDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleBundl                       | ::: block                         |
    | eDescriptionArg.Builder](AppleBun | Builds instances of type          |
    | dleDescriptionArg.Builder.html "c | [`AppleBundleDescriptionArg`](A   |
    | lass in com.facebook.buck.apple") | ppleBundleDescriptionArg.html "cl |
    |                                   | ass in com.facebook.buck.apple"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleBundleResour                | ::: block                         |
    | ces](AppleBundleResources.html "c | Resources to be bundled into a    |
    | lass in com.facebook.buck.apple") | bundle.                           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 |                                   |
    | AppleBundleResources.Builder](App |                                   |
    | leBundleResources.Builder.html "c |                                   |
    | lass in com.facebook.buck.apple") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AppleConfig](AppleConfig.html "c |                                   |
    | lass in com.facebook.buck.apple") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AppleDebuggableBina              | ::: block                         |
    | ry](AppleDebuggableBinary.html "c | This build rule wraps the usual   |
    | lass in com.facebook.buck.apple") | build rule and should be treated  |
    |                                   | as top-level binary rule for      |
    |                                   | apple platform.                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleDependenciesCach            |                                   |
    | e](AppleDependenciesCache.html "c |                                   |
    | lass in com.facebook.buck.apple") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AppleDescriptionProvider]        |                                   |
    | (AppleDescriptionProvider.html "c |                                   |
    | lass in com.facebook.buck.apple") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AppleDescri                      | ::: block                         |
    | ptions](AppleDescriptions.html "c | Common logic for a                |
    | lass in com.facebook.buck.apple") | [`DescriptionWithTarge            |
    |                                   | tGraph`](../core/rules/Descriptio |
    |                                   | nWithTargetGraph.html "interface  |
    |                                   | in com.facebook.buck.core.rules") |
    |                                   | that creates Apple target rules.  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleDsym](AppleDsym.html "c     | ::: block                         |
    | lass in com.facebook.buck.apple") | Creates dSYM bundle for the given |
    |                                   | \_unstripped\_ binary.            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleHeaderVisibilities          | ::: block                         |
    | ](AppleHeaderVisibilities.html "c | Utility class with methods        |
    | lass in com.facebook.buck.apple") | working with                      |
    |                                   | [`H                               |
    |                                   | eaderVisibility`](../cxx/toolchai |
    |                                   | n/HeaderVisibility.html "enum in  |
    |                                   | com.facebook.buck.cxx.toolchain") |
    |                                   | in the context of Apple rules.    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleInfoPlistParsi              | ::: block                         |
    | ng](AppleInfoPlistParsing.html "c | Utility class to parse Info.plist |
    | lass in com.facebook.buck.apple") | from an Apple bundle.             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleLibraryDescription          |                                   |
    | ](AppleLibraryDescription.html "c |                                   |
    | lass in com.facebook.buck.apple") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AppleLibraryDescriptionArg](A    | ::: block                         |
    | ppleLibraryDescriptionArg.html "c | Immutable implementation of       |
    | lass in com.facebook.buck.apple") | `AppleLibraryDescription.Abs      |
    |                                   | tractAppleLibraryDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleLibrary                     | ::: block                         |
    | DescriptionArg.Builder](AppleLibr | Builds instances of type          |
    | aryDescriptionArg.Builder.html "c | [`AppleLibraryDescriptionArg`](Ap |
    | lass in com.facebook.buck.apple") | pleLibraryDescriptionArg.html "cl |
    |                                   | ass in com.facebook.buck.apple"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleLibraryDesc                 |                                   |
    | riptionSwiftEnhancer](AppleLibrar |                                   |
    | yDescriptionSwiftEnhancer.html "c |                                   |
    | lass in com.facebook.buck.apple") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AppleLibrarySwiftMetadata](      |                                   |
    | AppleLibrarySwiftMetadata.html "c |                                   |
    | lass in com.facebook.buck.apple") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ApplePackageDescription          |                                   |
    | ](ApplePackageDescription.html "c |                                   |
    | lass in com.facebook.buck.apple") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ApplePackageDescriptionArg](A    | ::: block                         |
    | pplePackageDescriptionArg.html "c | Immutable implementation of       |
    | lass in com.facebook.buck.apple") | `ApplePackageDescription.Abs      |
    |                                   | tractApplePackageDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ApplePackage                     | ::: block                         |
    | DescriptionArg.Builder](ApplePack | Builds instances of type          |
    | ageDescriptionArg.Builder.html "c | [`ApplePackageDescriptionArg`](Ap |
    | lass in com.facebook.buck.apple") | plePackageDescriptionArg.html "cl |
    |                                   | ass in com.facebook.buck.apple"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Apple                            |                                   |
    | Platforms](ApplePlatforms.html "c |                                   |
    | lass in com.facebook.buck.apple") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AppleResourceDescription]        | ::: block                         |
    | (AppleResourceDescription.html "c | Description for an apple_resource |
    | lass in com.facebook.buck.apple") | rule which copies resource files  |
    |                                   | to the built bundle.              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleResourceDescriptionArg](Ap  | ::: block                         |
    | pleResourceDescriptionArg.html "c | Immutable implementation of       |
    | lass in com.facebook.buck.apple") | `AppleResourceDescription.Abst    |
    |                                   | ractAppleResourceDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleResourceD                   | ::: block                         |
    | escriptionArg.Builder](AppleResou | Builds instances of type          |
    | rceDescriptionArg.Builder.html "c | [`                                |
    | lass in com.facebook.buck.apple") | AppleResourceDescriptionArg`](App |
    |                                   | leResourceDescriptionArg.html "cl |
    |                                   | ass in com.facebook.buck.apple"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleResourceProcessing          | ::: block                         |
    | ](AppleResourceProcessing.html "c | Contains shared logic for adding  |
    | lass in com.facebook.buck.apple") | resource processing steps to      |
    |                                   | apple build rules                 |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Apple                            |                                   |
    | Resources](AppleResources.html "c |                                   |
    | lass in com.facebook.buck.apple") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AppleTest](AppleTest.html "c     |                                   |
    | lass in com.facebook.buck.apple") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AppleT                           | ::: block                         |
    | estAggregatedDependencies](AppleT | Creates a directory containing    |
    | estAggregatedDependencies.html "c | the static resources along with a |
    | lass in com.facebook.buck.apple") | merged static library containing  |
    |                                   | all of the symbols that a test    |
    |                                   | target depends on.                |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleTestDescript                |                                   |
    | ion](AppleTestDescription.html "c |                                   |
    | lass in com.facebook.buck.apple") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AppleTestDescriptionArg          | ::: block                         |
    | ](AppleTestDescriptionArg.html "c | Immutable implementation of       |
    | lass in com.facebook.buck.apple") | `AppleTestDescription.            |
    |                                   | AbstractAppleTestDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleT                           | ::: block                         |
    | estDescriptionArg.Builder](AppleT | Builds instances of type          |
    | estDescriptionArg.Builder.html "c | [`AppleTestDescriptionArg`]       |
    | lass in com.facebook.buck.apple") | (AppleTestDescriptionArg.html "cl |
    |                                   | ass in com.facebook.buck.apple"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleTestX](AppleTestX.html "c   | ::: block                         |
    | lass in com.facebook.buck.apple") | Represents an apple_test rule     |
    |                                   | that implements the test protocol |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleToolchainBuildRule          | ::: block                         |
    | ](AppleToolchainBuildRule.html "c | This                              |
    | lass in com.facebook.buck.apple") | [`BuildRule`](../core             |
    |                                   | /rules/BuildRule.html "interface  |
    |                                   | in com.facebook.buck.core.rules") |
    |                                   | provides                          |
    |                                   | [`AppleCxxPlatform`](toolchain/A  |
    |                                   | ppleCxxPlatform.html "class in co |
    |                                   | m.facebook.buck.apple.toolchain") |
    |                                   | to use in                         |
    |                                   | [`AppleToolchainSetBuildRule`](Ap |
    |                                   | pleToolchainSetBuildRule.html "cl |
    |                                   | ass in com.facebook.buck.apple"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleToolchainDescription](      | ::: block                         |
    | AppleToolchainDescription.html "c | Defines an apple_toolchain rule   |
    | lass in com.facebook.buck.apple") | which provides                    |
    |                                   | [`AppleCxxPlatform`](toolchain/Ap |
    |                                   | pleCxxPlatform.html "class in com |
    |                                   | .facebook.buck.apple.toolchain"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | AppleToolchainDescriptionArg](App | apple_toolchain defines tools,    |
    | leToolchainDescriptionArg.html "c | cxx and swift toolchains and      |
    | lass in com.facebook.buck.apple") | other properties to define        |
    |                                   | AppleCxxPlatform.                 |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleToolchainDe                 | ::: block                         |
    | scriptionArg.Builder](AppleToolch | Builds instances of type          |
    | ainDescriptionArg.Builder.html "c | [`Ap                              |
    | lass in com.facebook.buck.apple") | pleToolchainDescriptionArg`](Appl |
    |                                   | eToolchainDescriptionArg.html "cl |
    |                                   | ass in com.facebook.buck.apple"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleToolchainSetBuildRule](A    | ::: block                         |
    | ppleToolchainSetBuildRule.html "c | This                              |
    | lass in com.facebook.buck.apple") | [`BuildRule`](../core             |
    |                                   | /rules/BuildRule.html "interface  |
    |                                   | in com.facebook.buck.core.rules") |
    |                                   | provides                          |
    |                                   | [`AppleCxxPlatform`](toolchain/A  |
    |                                   | ppleCxxPlatform.html "class in co |
    |                                   | m.facebook.buck.apple.toolchain") |
    |                                   | using                             |
    |                                   | [`AppleToolchainBuildRule`]       |
    |                                   | (AppleToolchainBuildRule.html "cl |
    |                                   | ass in com.facebook.buck.apple"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | AppleToolchainSetDescription](App | Defines an apple_toolchain_set    |
    | leToolchainSetDescription.html "c | rule that allows to list all      |
    | lass in com.facebook.buck.apple") | available apple_toolchain targets |
    |                                   | which will be used to create      |
    |                                   | [`AppleCxxPlatform`](toolchain/Ap |
    |                                   | pleCxxPlatform.html "class in com |
    |                                   | .facebook.buck.apple.toolchain"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleT                           | ::: block                         |
    | oolchainSetDescriptionArg](AppleT | An apple_toolchain_set is a list  |
    | oolchainSetDescriptionArg.html "c | of available apple_toolchain      |
    | lass in com.facebook.buck.apple") | targets.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleToolchainSetDescr           | ::: block                         |
    | iptionArg.Builder](AppleToolchain | Builds instances of type          |
    | SetDescriptionArg.Builder.html "c | [`AppleToo                        |
    | lass in com.facebook.buck.apple") | lchainSetDescriptionArg`](AppleTo |
    |                                   | olchainSetDescriptionArg.html "cl |
    |                                   | ass in com.facebook.buck.apple"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleWrapperResourceArg          | ::: block                         |
    | ](AppleWrapperResourceArg.html "c | A description for a resource      |
    | lass in com.facebook.buck.apple") | defined by a single path.         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleW                           | ::: block                         |
    | rapperResourceArg.Builder](AppleW | Builds instances of type          |
    | rapperResourceArg.Builder.html "c | [`AppleWrapperResourceArg`]       |
    | lass in com.facebook.buck.apple") | (AppleWrapperResourceArg.html "cl |
    |                                   | ass in com.facebook.buck.apple"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleXCodeDe                     |                                   |
    | scriptionClassSupplier](AppleXCod |                                   |
    | eDescriptionClassSupplier.html "c |                                   |
    | lass in com.facebook.buck.apple") |                                   |
    +-----------------------------------+-----------------------------------+
    | [BuiltinApplePac                  |                                   |
    | kage](BuiltinApplePackage.html "c |                                   |
    | lass in com.facebook.buck.apple") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Cor                              |                                   |
    | eDataModel](CoreDataModel.html "c |                                   |
    | lass in com.facebook.buck.apple") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CoreDataModelDescription]        | ::: block                         |
    | (CoreDataModelDescription.html "c | Description for a core_data_model |
    | lass in com.facebook.buck.apple") | rule, which identifies a model    |
    |                                   | file for use with Apple\'s Core   |
    |                                   | Data.                             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ExternallyBuiltApplePackage](Ex  | ::: block                         |
    | ternallyBuiltApplePackage.html "c | Rule for generating an apple      |
    | lass in com.facebook.buck.apple") | package via external script.      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Flavors](Flavors.html "c         |                                   |
    | lass in com.facebook.buck.apple") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Gro                              |                                   |
    | upedSource](GroupedSource.html "c |                                   |
    | lass in com.facebook.buck.apple") |                                   |
    +-----------------------------------+-----------------------------------+
    | [IdbOutput                        | ::: block                         |
    | Parsing](IdbOutputParsing.html "c | Utility class to parse the output |
    | lass in com.facebook.buck.apple") | from `idb`.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [IdbRunT                          | ::: block                         |
    | estsStep](IdbRunTestsStep.html "c | Runs `idb` on one or more logic,  |
    | lass in com.facebook.buck.apple") | ui or application tests           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [InfoPlistSubstituti              | ::: block                         |
    | on](InfoPlistSubstitution.html "c | Utility class to substitute Xcode |
    | lass in com.facebook.buck.apple") | Info.plist variables in the       |
    |                                   | forms:                            |
    |                                   | `  ${FOO}  $(FOO)  ${             |
    |                                   | FOO:modifier}  $(FOO:modifier)  ` |
    |                                   | with specified string values.     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [LibtoolStep](LibtoolStep.html "c | ::: block                         |
    | lass in com.facebook.buck.apple") | ShellStep for calling libtool.    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Mul                              | ::: block                         |
    | tiarchFile](MultiarchFile.html "c | Puts together multiple thin       |
    | lass in com.facebook.buck.apple") | library/binaries into a           |
    |                                   | multi-arch file.                  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [MultiarchFile                    |                                   |
    | Infos](MultiarchFileInfos.html "c |                                   |
    | lass in com.facebook.buck.apple") |                                   |
    +-----------------------------------+-----------------------------------+
    | [PrebuiltAppleFramewor            |                                   |
    | k](PrebuiltAppleFramework.html "c |                                   |
    | lass in com.facebook.buck.apple") |                                   |
    +-----------------------------------+-----------------------------------+
    | [PrebuiltAp                       |                                   |
    | pleFrameworkDescription](Prebuilt |                                   |
    | AppleFrameworkDescription.html "c |                                   |
    | lass in com.facebook.buck.apple") |                                   |
    +-----------------------------------+-----------------------------------+
    | [PrebuiltAppleFra                 | ::: block                         |
    | meworkDescriptionArg](PrebuiltApp | Immutable implementation of       |
    | leFrameworkDescriptionArg.html "c | `PrebuiltAppleF                   |
    | lass in com.facebook.buck.apple") | rameworkDescription.AbstractPrebu |
    |                                   | iltAppleFrameworkDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PrebuiltAppleFrameworkDescriptio | ::: block                         |
    | nArg.Builder](PrebuiltAppleFramew | Builds instances of type          |
    | orkDescriptionArg.Builder.html "c | [`PrebuiltAppleFrame              |
    | lass in com.facebook.buck.apple") | workDescriptionArg`](PrebuiltAppl |
    |                                   | eFrameworkDescriptionArg.html "cl |
    |                                   | ass in com.facebook.buck.apple"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RuleUtils](RuleUtils.html "c     | ::: block                         |
    | lass in com.facebook.buck.apple") | Common conversion functions from  |
    |                                   | raw Description Arg               |
    |                                   | specifications.                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Scene                            |                                   |
    | KitAssets](SceneKitAssets.html "c |                                   |
    | lass in com.facebook.buck.apple") |                                   |
    +-----------------------------------+-----------------------------------+
    | [SceneKitAssetsDescription](      | ::: block                         |
    | SceneKitAssetsDescription.html "c | Description for a scenekit_assets |
    | lass in com.facebook.buck.apple") | rule, which identifies a assets   |
    |                                   | directory for use with Apple\'s   |
    |                                   | SceneKit.                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [SourcePathWithAp                 | ::: block                         |
    | pleBundleDestination](SourcePathW | Simple type representing a        |
    | ithAppleBundleDestination.html "c | [`SourcePath`](../core/sourcepath |
    | lass in com.facebook.buck.apple") | /SourcePath.html "interface in co |
    |                                   | m.facebook.buck.core.sourcepath") |
    |                                   | and a destination                 |
    |                                   | [`AppleBundleDestinatio           |
    |                                   | n`](AppleBundleDestination.html " |
    |                                   | enum in com.facebook.buck.apple") |
    |                                   | in a resulting bundle where a     |
    |                                   | file or a directory with this     |
    |                                   | path should be copied.            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | TestCaseSummariesBuildingIdb](Tes | Implementation of                 |
    | tCaseSummariesBuildingIdb.html "c | [`IdbOutputParsing.               |
    | lass in com.facebook.buck.apple") | IdbResultCallback`](IdbOutputPars |
    |                                   | ing.IdbResultCallback.html "inter |
    |                                   | face in com.facebook.buck.apple") |
    |                                   | that collects `xctool` events and |
    |                                   | converts them to                  |
    |                                   | [`TestCaseSummary                 |
    |                                   | `](../test/TestCaseSummary.html " |
    |                                   | class in com.facebook.buck.test") |
    |                                   | objects, reporting progress to a  |
    |                                   | `                                 |
    |                                   |  TestRule.TestReportingCallback`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [XCodeDescri                      | ::: block                         |
    | ptions](XCodeDescriptions.html "c | Contains descriptions supported   |
    | lass in com.facebook.buck.apple") | by XCode.                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [XCodeDescriptionsFactory]        |                                   |
    | (XCodeDescriptionsFactory.html "c |                                   |
    | lass in com.facebook.buck.apple") |                                   |
    +-----------------------------------+-----------------------------------+
    | [XcodeP                           | ::: block                         |
    | ostbuildScriptDescription](XcodeP | Description for an                |
    | ostbuildScriptDescription.html "c | xcode_postbuild_script rule which |
    | lass in com.facebook.buck.apple") | runs a shell script after the     |
    |                                   | \'copy resources\' phase has run. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Xcod                             | ::: block                         |
    | ePrebuildScriptDescription](Xcode | Description for an                |
    | PrebuildScriptDescription.html "c | xcode_prebuild_script rule which  |
    | lass in com.facebook.buck.apple") | runs a shell script before the    |
    |                                   | Apple target that depends on it   |
    |                                   | is built.                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [XcodeScriptDescriptionArg](      | ::: block                         |
    | XcodeScriptDescriptionArg.html "c | Immutable implementation of       |
    | lass in com.facebook.buck.apple") | `Ab                               |
    |                                   | stractXcodeScriptDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [XcodeScrip                       | ::: block                         |
    | tDescriptionArg.Builder](XcodeScr | Builds instances of type          |
    | iptDescriptionArg.Builder.html "c | [`XcodeScriptDescriptionArg`](X   |
    | lass in com.facebook.buck.apple") | codeScriptDescriptionArg.html "cl |
    |                                   | ass in com.facebook.buck.apple"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Enum                              | Description                       |
    +===================================+===================================+
    | [AppleAs                          |                                   |
    | setCatalog.ValidationType](AppleA |                                   |
    | ssetCatalog.ValidationType.html " |                                   |
    | enum in com.facebook.buck.apple") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AppleBuildRules.Recursive        |                                   |
    | DependenciesMode](AppleBuildRules |                                   |
    | .RecursiveDependenciesMode.html " |                                   |
    | enum in com.facebook.buck.apple") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AppleBundleDestinati             | ::: block                         |
    | on](AppleBundleDestination.html " | Abstraction of a place in a       |
    | enum in com.facebook.buck.apple") | resulting bundle where resource   |
    |                                   | will be copied.                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleBundleExten                 | ::: block                         |
    | sion](AppleBundleExtension.html " | Known bundle extensions that have |
    | enum in com.facebook.buck.apple") | special handling.                 |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AppleDeb                         |                                   |
    | ugFormat](AppleDebugFormat.html " |                                   |
    | enum in com.facebook.buck.apple") |                                   |
    +-----------------------------------+-----------------------------------+
    | [AppleLibraryDescription.Type](Ap |                                   |
    | pleLibraryDescription.Type.html " |                                   |
    | enum in com.facebook.buck.apple") |                                   |
    +-----------------------------------+-----------------------------------+
    | [GroupedSourc                     | ::: block                         |
    | e.Type](GroupedSource.Type.html " | The type of grouped source entry  |
    | enum in com.facebook.buck.apple") | this object represents.           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [LibtoolSte                       | ::: block                         |
    | p.Style](LibtoolStep.Style.html " | Style of library to be created,   |
    | enum in com.facebook.buck.apple") | static or dynamic.                |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Enum Summary[ ]{.tabEnd}
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
