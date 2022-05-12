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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.attr](package-summary.html)
:::

## Interface HasDeclaredAndExtraDeps {#interface-hasdeclaredandextradeps .title title="Interface HasDeclaredAndExtraDeps"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `AbstractBuildRuleWithDeclaredAndExtraDeps`, `AndroidAar`,
        `AndroidBinary`, `AndroidBuildConfig`, `AndroidBundle`,
        `AndroidInstrumentationApk`, `AndroidInstrumentationTest`,
        `AndroidResource`, `AndroidResourceIndex`,
        `AppleDebuggableBinary`, `AppleTest`,
        `AppleTestAggregatedDependencies`, `AppleTestX`,
        `BinaryWrapperRule`, `BuiltinApplePackage`, `CGoLibrary`,
        `CompareAbis`, `CoreDataModel`, `CsharpLibrary`, `CxxBinary`,
        `CxxGenrule`, `CxxLibraryGroup`, `CxxLuaExtension`,
        `CxxPrecompiledHeaderTemplate`, `CxxPrefixHeader`,
        `CxxPythonExtension`, `CxxTest`, `DBinary`, `DCompileBuildRule`,
        `DLibrary`, `DTest`, `GenAidl`, `GoBinary`, `GoCompile`,
        `GoLibrary`, `GoTest`, `GoTestMain`, `GoTestX`, `GwtBinary`,
        `GwtModule`, `HalideCompile`, `HalideLibrary`, `HaskellBinary`,
        `HaskellCompileRule`, `HaskellGhciRule`,
        `HaskellHaddockLibRule`, `HaskellHaddockRule`, `HaskellLibrary`,
        `HaskellLinkRule`, `HaskellPackageRule`, `HttpArchive`,
        `HttpFile`, `HttpFileBinary`, `JarFattener`,
        `JavaAnnotationProcessor`, `JavaBinary`, `Javadoc`,
        `JavaSourceJar`, `JavaTest`, `JavaTestRunner`, `JavaTestX`,
        `JsBundle`, `JsBundleAndroid`, `JsDependenciesFile`,
        `JsonConcatenate`, `Keystore`, `LuaBinary`, `LuaLibrary`,
        `LuaStandaloneBinary`, `MavenUberJar`, `MavenUberJar.SourceJar`,
        `MultiarchFile`, `NativeLibraryProguardGenerator`, `NdkLibrary`,
        `NoopBuildRuleWithDeclaredAndExtraDeps`, `OcamlBinary`,
        `OcamlBuild`, `OcamlCCompile`, `OcamlClean`,
        `OcamlDebugLauncher`, `OcamlLibrary`, `OcamlLink`,
        `OcamlMLCompile`, `PrebuiltAppleFramework`,
        `PrebuiltCxxLibrary`,
        `PrebuiltCxxLibraryGroupDescription.CustomPrebuiltCxxLibrary`,
        `PrebuiltDotnetLibrary`, `PrebuiltHaskellLibrary`,
        `PrebuiltJar`, `PrebuiltNativeLibrary`, `PrebuiltPythonLibrary`,
        `PreDexMerge`, `PreDexSingleDexMerge`, `PreDexSplitDexGroup`,
        `PreDexSplitDexMerge`, `PreInclude`, `PythonLibrary`,
        `PythonTest`, `PythonTestX`, `RemoteFile`, `RemoteFileBinary`,
        `RobolectricTest`, `RobolectricTestX`, `RustLibrary`,
        `RustTest`, `SceneKitAssets`, `ShBinary`, `ShTest`,
        `StandardJavacPlugin`, `TestSuite`, `UnstrippedNativeLibraries`,
        `UnzipAar`, `WriteStringTemplateRule`

    ------------------------------------------------------------------------

        public interface HasDeclaredAndExtraDeps

    ::: block
    Some rules have a legacy behavior of distinguishing between
    \"declared\" deps (i.e. the contents of the TargetNode\'s deps
    attribute) and \"extra\" deps (i.e. other deps which were detected
    somehow else).
    This class formalizes those concepts.

    Some rules have switched to have more custom handling of different
    kinds of deps. Other rules are currently very unclear as to what
    \"extra\" means, or when it should be used.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                           Method                       Description
          ----------------------------------------------------------- ---------------------------- -------------
          `SortedSet<BuildRule>`                                      `deprecatedGetExtraDeps()`    
          `SortedSet<BuildRule>`                                      `getDeclaredDeps()`           
          `com.google.common.collect.ImmutableSortedSet<BuildRule>`   `getTargetGraphOnlyDeps()`    

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

        []{#getDeclaredDeps()}

        -   #### getDeclaredDeps

            ``` methodSignature
            SortedSet<BuildRule> getDeclaredDeps()
            ```

        []{#deprecatedGetExtraDeps()}

        -   #### deprecatedGetExtraDeps

            ``` methodSignature
            SortedSet<BuildRule> deprecatedGetExtraDeps()
            ```

        []{#getTargetGraphOnlyDeps()}

        -   #### getTargetGraphOnlyDeps

            ``` methodSignature
            com.google.common.collect.ImmutableSortedSet<BuildRule> getTargetGraphOnlyDeps()
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
