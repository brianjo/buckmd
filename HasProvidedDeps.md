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

## Interface HasProvidedDeps {#interface-hasprovideddeps .title title="Interface HasProvidedDeps"}
:::

::: contentContainer
::: description
-   

    All Known Subinterfaces:
    :   `AndroidKotlinCoreArg`, `AndroidLibraryDescription.CoreArg`,
        `GroovyLibraryDescription.CoreArg`, `HasProvidedDepsQuery`,
        `JavaLibraryDescription.CoreArg`, `JavaTestDescription.CoreArg`,
        `KotlinLibraryDescription.CoreArg`,
        `ScalaLibraryDescription.CoreArg`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AndroidAarDescriptionArg`, `AndroidLibraryDescriptionArg`,
        `GroovyLibraryDescriptionArg`, `GroovyTestDescriptionArg`,
        `JavaLibraryDescriptionArg`, `JavaTestDescriptionArg`,
        `JavaTestRunnerDescriptionArg`, `KotlinLibraryDescriptionArg`,
        `KotlinTestDescriptionArg`, `RobolectricTestDescriptionArg`,
        `ScalaLibraryDescriptionArg`, `ScalaTestDescriptionArg`

    ------------------------------------------------------------------------

        public interface HasProvidedDeps
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                             Method                        Description
          ------------------------------------------------------------- ----------------------------- -------------
          `com.google.common.collect.ImmutableSortedSet<BuildTarget>`   `getExportedProvidedDeps()`    
          `com.google.common.collect.ImmutableSortedSet<BuildTarget>`   `getProvidedDeps()`            

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

        []{#getProvidedDeps()}

        -   #### getProvidedDeps

            ``` methodSignature
            @NaturalOrder
            com.google.common.collect.ImmutableSortedSet<BuildTarget> getProvidedDeps()
            ```

        []{#getExportedProvidedDeps()}

        -   #### getExportedProvidedDeps

            ``` methodSignature
            @NaturalOrder
            com.google.common.collect.ImmutableSortedSet<BuildTarget> getExportedProvidedDeps()
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
