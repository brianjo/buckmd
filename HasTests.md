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

## Interface HasTests {#interface-hastests .title title="Interface HasTests"}
:::

::: contentContainer
::: description
-   

    All Known Subinterfaces:
    :   `AbstractGenruleDescription.CommonArg`, `AndroidKotlinCoreArg`,
        `AndroidLibraryDescription.CoreArg`,
        `AppleNativeTargetDescriptionArg`,
        `CxxBinaryDescription.CommonArg`, `CxxConstructorArg`,
        `CxxLibraryDescription.CommonArg`,
        `GroovyLibraryDescription.CoreArg`,
        `JavaLibraryDescription.CoreArg`, `JavaTestDescription.CoreArg`,
        `KotlinLibraryDescription.CoreArg`, `LinkableCxxConstructorArg`,
        `ScalaLibraryDescription.CoreArg`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AndroidAarDescriptionArg`, `AndroidBinaryDescriptionArg`,
        `AndroidBundleDescriptionArg`, `AndroidLibraryDescriptionArg`,
        `ApkGenruleDescriptionArg`, `AppleBinaryDescriptionArg`,
        `AppleBundleDescriptionArg`, `AppleLibraryDescriptionArg`,
        `AppleTestDescriptionArg`, `CgoLibraryDescriptionArg`,
        `CxxBinaryDescriptionArg`, `CxxGenruleDescriptionArg`,
        `CxxLibraryDescriptionArg`, `CxxLuaExtensionDescriptionArg`,
        `CxxPythonExtensionDescriptionArg`, `CxxTestDescriptionArg`,
        `GenruleDescriptionArg`, `GoLibraryDescriptionArg`,
        `GroovyLibraryDescriptionArg`, `GroovyTestDescriptionArg`,
        `HalideLibraryDescriptionArg`, `JarGenruleDescriptionArg`,
        `JavaBinaryDescriptionArg`, `JavaLibraryDescriptionArg`,
        `JavaTestDescriptionArg`, `JavaTestRunnerDescriptionArg`,
        `JsBundleGenruleDescriptionArg`, `JsLibraryDescriptionArg`,
        `KotlinLibraryDescriptionArg`, `KotlinTestDescriptionArg`,
        `PythonBinaryDescriptionArg`, `PythonLibraryDescriptionArg`,
        `PythonTestDescriptionArg`, `RobolectricTestDescriptionArg`,
        `RustBinaryDescriptionArg`, `RustLibraryDescriptionArg`,
        `ScalaLibraryDescriptionArg`, `ScalaTestDescriptionArg`,
        `ShBinaryDescriptionArg`

    ------------------------------------------------------------------------

        public interface HasTests

    ::: block
    A constructor arg of source rules with a list of their tests.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                             Method         Description
          ------------------------------------------------------------- -------------- -------------
          `com.google.common.collect.ImmutableSortedSet<BuildTarget>`   `getTests()`    

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

        []{#getTests()}

        -   #### getTests

            ``` methodSignature
            @NaturalOrder
            com.google.common.collect.ImmutableSortedSet<BuildTarget> getTests()
            ```

            [Returns:]{.returnLabel}
            :   A list of tests of this target.
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
