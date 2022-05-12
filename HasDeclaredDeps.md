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
[Package]{.packageLabelInType} [com.facebook.buck.core.description.arg](package-summary.html)
:::

## Interface HasDeclaredDeps {#interface-hasdeclareddeps .title title="Interface HasDeclaredDeps"}
:::

::: contentContainer
::: description
-   

    All Known Subinterfaces:
    :   `AndroidKotlinCoreArg`, `AndroidLibraryDescription.CoreArg`,
        `AppleNativeTargetDescriptionArg`,
        `CxxBinaryDescription.CommonArg`, `CxxConstructorArg`,
        `CxxLibraryDescription.CommonArg`,
        `GroovyLibraryDescription.CoreArg`, `HasDepsQuery`,
        `HasNamedDeclaredDeps`, `JavacPluginArgs`,
        `JavaLibraryDescription.CoreArg`, `JavaTestDescription.CoreArg`,
        `KotlinLibraryDescription.CoreArg`, `LinkableCxxConstructorArg`,
        `RustCommonArgs`, `ScalaLibraryDescription.CoreArg`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AndroidAarDescriptionArg`,
        `AndroidAppModularityDescriptionArg`,
        `AndroidBinaryDescriptionArg`, `AndroidBundleDescriptionArg`,
        `AndroidInstrumentationApkDescriptionArg`,
        `AndroidLibraryDescriptionArg`, `AndroidManifestDescriptionArg`,
        `AndroidPrebuiltAarDescriptionArg`,
        `AndroidResourceDescriptionArg`, `AppleBinaryDescriptionArg`,
        `AppleBundleDescriptionArg`, `AppleLibraryDescriptionArg`,
        `AppleTestDescriptionArg`, `CgoLibraryDescriptionArg`,
        `CxxBinaryDescriptionArg`, `CxxLibraryDescriptionArg`,
        `CxxLuaExtensionDescriptionArg`,
        `CxxPrecompiledHeaderDescriptionArg`,
        `CxxPythonExtensionDescriptionArg`, `CxxTestDescriptionArg`,
        `DBinaryDescriptionArg`, `DLibraryDescriptionArg`,
        `DTestDescriptionArg`, `GenAidlDescriptionArg`,
        `GoBinaryDescriptionArg`, `GoLibraryDescriptionArg`,
        `GoTestDescriptionArg`, `GroovyLibraryDescriptionArg`,
        `GroovyTestDescriptionArg`, `GwtBinaryDescriptionArg`,
        `HalideLibraryDescriptionArg`, `HaskellBinaryDescriptionArg`,
        `HaskellGhciDescriptionArg`, `HaskellHaddockDescriptionArg`,
        `HaskellLibraryDescriptionArg`,
        `HaskellPrebuiltLibraryDescriptionArg`,
        `JavaAnnotationProcessorDescriptionArg`,
        `JavaBinaryDescriptionArg`, `JavaLibraryDescriptionArg`,
        `JavaPluginDescriptionArg`, `JavaTestDescriptionArg`,
        `JavaTestRunnerDescriptionArg`, `JsBundleDescriptionArg`,
        `JsLibraryDescriptionArg`, `KeystoreDescriptionArg`,
        `KotlinLibraryDescriptionArg`, `KotlinTestDescriptionArg`,
        `LuaBinaryDescriptionArg`, `LuaLibraryDescriptionArg`,
        `NdkLibraryDescriptionArg`, `OcamlBinaryDescriptionArg`,
        `OcamlLibraryDescriptionArg`,
        `PrebuiltAppleFrameworkDescriptionArg`,
        `PrebuiltCxxLibraryDescriptionArg`,
        `PrebuiltCxxLibraryGroupDescriptionArg`,
        `PrebuiltGoLibraryDescriptionArg`, `PrebuiltJarDescriptionArg`,
        `PrebuiltNativeLibraryDescriptionArg`,
        `PrebuiltOcamlLibraryDescriptionArg`,
        `PrebuiltPythonLibraryDescriptionArg`,
        `PrebuiltRustLibraryDescriptionArg`,
        `PythonBinaryDescriptionArg`, `PythonLibraryDescriptionArg`,
        `PythonTestDescriptionArg`, `RobolectricTestDescriptionArg`,
        `RustBinaryDescriptionArg`, `RustLibraryDescriptionArg`,
        `RustTestDescriptionArg`, `ScalaLibraryDescriptionArg`,
        `ScalaTestDescriptionArg`, `ShBinaryDescriptionArg`,
        `ShTestDescriptionArg`, `SwiftLibraryDescriptionArg`

    ------------------------------------------------------------------------

        public interface HasDeclaredDeps
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                             Method        Description
          ------------------------------------------------------------- ------------- -------------
          `com.google.common.collect.ImmutableSortedSet<BuildTarget>`   `getDeps()`    

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

        []{#getDeps()}

        -   #### getDeps

            ``` methodSignature
            @NaturalOrder
            com.google.common.collect.ImmutableSortedSet<BuildTarget> getDeps()
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
