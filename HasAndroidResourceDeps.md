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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Interface HasAndroidResourceDeps {#interface-hasandroidresourcedeps .title title="Interface HasAndroidResourceDeps"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `AndroidPrebuiltAar`, `AndroidResource`

    ------------------------------------------------------------------------

        public interface HasAndroidResourceDeps

    ::: block
    Indicates that this class may have android resources that should be
    packaged into an APK.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                             Description
          ------------------- ---------------------------------- -------------
          `SourcePath`        `getAssets()`                       
          `BuildTarget`       `getBuildTarget()`                  
          `SourcePath`        `getPathToRDotJavaPackageFile()`    
          `SourcePath`        `getPathToTextSymbolsFile()`        
          `String`            `getRDotJavaPackage()`              
          `SourcePath`        `getRes()`                          

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

        []{#getBuildTarget()}

        -   #### getBuildTarget

            ``` methodSignature
            BuildTarget getBuildTarget()
            ```

        []{#getRDotJavaPackage()}

        -   #### getRDotJavaPackage

            ``` methodSignature
            String getRDotJavaPackage()
            ```

            [Returns:]{.returnLabel}
            :   the package name in which to generate the R.java
                representing these resources.

        []{#getPathToTextSymbolsFile()}

        -   #### getPathToTextSymbolsFile

            ``` methodSignature
            SourcePath getPathToTextSymbolsFile()
            ```

            [Returns:]{.returnLabel}
            :   path to a temporary directory for storing text symbols.

        []{#getPathToRDotJavaPackageFile()}

        -   #### getPathToRDotJavaPackageFile

            ``` methodSignature
            SourcePath getPathToRDotJavaPackageFile()
            ```

            [Returns:]{.returnLabel}
            :   path to a file containing the package name for R.java.

        []{#getRes()}

        -   #### getRes

            ``` methodSignature
            @Nullable
            SourcePath getRes()
            ```

            [Returns:]{.returnLabel}
            :   path to a directory containing Android resources.

        []{#getAssets()}

        -   #### getAssets

            ``` methodSignature
            @Nullable
            SourcePath getAssets()
            ```

            [Returns:]{.returnLabel}
            :   path to a directory containing Android assets.
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
