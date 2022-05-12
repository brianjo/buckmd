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
[Package]{.packageLabelInType} [com.facebook.buck.core.description.attr](package-summary.html)
:::

## Interface ImplicitDepsInferringDescription\<T\> {#interface-implicitdepsinferringdescriptiont .title title="Interface ImplicitDepsInferringDescription"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `AbstractGenruleDescription`, `AndroidAarDescription`,
        `AndroidBinaryDescription`, `AndroidBuildConfigDescription`,
        `AndroidBundleDescription`,
        `AndroidInstrumentationApkDescription`,
        `AndroidInstrumentationTestDescription`,
        `AndroidLibraryDescription`, `AndroidPrebuiltAarDescription`,
        `AndroidResourceDescription`, `ApkGenruleDescription`,
        `AppleBinaryDescription`, `AppleBundleDescription`,
        `AppleLibraryDescription`, `ApplePackageDescription`,
        `AppleTestDescription`, `CgoLibraryDescription`,
        `CxxBinaryDescription`, `CxxGenruleDescription`,
        `CxxLibraryDescription`, `CxxLuaExtensionDescription`,
        `CxxPythonExtensionDescription`, `CxxTestDescription`,
        `DBinaryDescription`, `DLibraryDescription`, `DTestDescription`,
        `GenruleDescription`, `GoBinaryDescription`,
        `GoLibraryDescription`, `GoTestDescription`,
        `GroovyLibraryDescription`, `GroovyTestDescription`,
        `GwtBinaryDescription`, `HaskellBinaryDescription`,
        `HaskellGhciDescription`, `HaskellHaddockDescription`,
        `HaskellLibraryDescription`, `JarGenruleDescription`,
        `JavaBinaryDescription`, `JavaLibraryDescription`,
        `JavaTestDescription`, `JavaTestRunnerDescription`,
        `JsBundleDescription`, `JsBundleGenruleDescription`,
        `JsLibraryDescription`, `KotlinLibraryDescription`,
        `KotlinTestDescription`, `LegacyToolchainRuleDescription`,
        `LuaBinaryDescription`, `NdkLibraryDescription`,
        `OcamlBinaryDescription`, `OcamlLibraryDescription`,
        `PrebuiltCxxLibraryDescription`, `PythonBinaryDescription`,
        `PythonTestDescription`, `RobolectricTestDescription`,
        `RustBinaryDescription`, `RustLibraryDescription`,
        `RustTestDescription`, `ScalaLibraryDescription`,
        `ScalaTestDescription`, `SwiftLibraryDescription`

    ------------------------------------------------------------------------

        public interface ImplicitDepsInferringDescription<T>

    ::: block
    While building up the target graph, we infer the implicit
    dependencies of a rule by parsing all parameters with types
    [`SourcePath`](../../sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
    or
    [`BuildRule`](../../rules/BuildRule.html "interface in com.facebook.buck.core.rules").
    However, in some cases like
    [`GenruleDescription`](../../../shell/GenruleDescription.html "class in com.facebook.buck.shell"),
    the
    [`AbstractGenruleDescription.CommonArg.getCmd()`](../../../shell/AbstractGenruleDescription.CommonArg.html#getCmd())
    argument contains build targets in a specific format. Any
    [`Description`](../Description.html "interface in com.facebook.buck.core.description")
    that implements this interface can modify its implicit deps by
    poking at the raw build rule params.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                                                                                                                                                                                                                                                                                                                                                              Description
          ------------------- --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `void`              `findDepsForTargetFromConstructorArgs​(BuildTarget buildTarget,                                     CellNameResolver cellRoots,                                     T constructorArg,                                     com.google.common.collect.ImmutableCollection.Builder<BuildTarget> extraDepsBuilder,                                     com.google.common.collect.ImmutableCollection.Builder<BuildTarget> targetGraphOnlyDepsBuilder)`    

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

        []{#findDepsForTargetFromConstructorArgs(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.cell.nameresolver.CellNameResolver,java.lang.Object,com.google.common.collect.ImmutableCollection.Builder,com.google.common.collect.ImmutableCollection.Builder)}
        []{#findDepsForTargetFromConstructorArgs(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.cell.nameresolver.CellNameResolver,T,com.google.common.collect.ImmutableCollection.Builder,com.google.common.collect.ImmutableCollection.Builder)}

        -   #### findDepsForTargetFromConstructorArgs

            ``` methodSignature
            void findDepsForTargetFromConstructorArgs​(BuildTarget buildTarget,
                                                      CellNameResolver cellRoots,
                                                      T constructorArg,
                                                      com.google.common.collect.ImmutableCollection.Builder<BuildTarget> extraDepsBuilder,
                                                      com.google.common.collect.ImmutableCollection.Builder<BuildTarget> targetGraphOnlyDepsBuilder)
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
