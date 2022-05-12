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
[Package]{.packageLabelInType} [com.facebook.buck.apple](package-summary.html)
:::

## Interface HasAppleBundleFields {#interface-hasapplebundlefields .title title="Interface HasAppleBundleFields"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `AppleBundleDescriptionArg`, `AppleTestDescriptionArg`

    ------------------------------------------------------------------------

        public interface HasAppleBundleFields
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                         Method                                   Description
          --------------------------------------------------------- ---------------------------------------- -------------
          `default AppleAssetCatalogsCompilationOptions`            `getAssetCatalogsCompilationOptions()`    
          `Either<AppleBundleExtension,​String>`                     `getExtension()`                          
          `SourcePath`                                              `getInfoPlist()`                          
          `com.google.common.collect.ImmutableMap<String,​String>`   `getInfoPlistSubstitutions()`             
          `Optional<Boolean>`                                       `getIsAppClip()`                          
          `Optional<String>`                                        `getProductName()`                        
          `Optional<String>`                                        `getXcodeProductType()`                   

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
          .tableTab}[[Default
          Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getExtension()}

        -   #### getExtension

            ``` methodSignature
            Either<AppleBundleExtension,​String> getExtension()
            ```

        []{#getInfoPlist()}

        -   #### getInfoPlist

            ``` methodSignature
            SourcePath getInfoPlist()
            ```

        []{#getProductName()}

        -   #### getProductName

            ``` methodSignature
            Optional<String> getProductName()
            ```

        []{#getXcodeProductType()}

        -   #### getXcodeProductType

            ``` methodSignature
            Optional<String> getXcodeProductType()
            ```

        []{#getIsAppClip()}

        -   #### getIsAppClip

            ``` methodSignature
            Optional<Boolean> getIsAppClip()
            ```

        []{#getInfoPlistSubstitutions()}

        -   #### getInfoPlistSubstitutions

            ``` methodSignature
            com.google.common.collect.ImmutableMap<String,​String> getInfoPlistSubstitutions()
            ```

        []{#getAssetCatalogsCompilationOptions()}

        -   #### getAssetCatalogsCompilationOptions

            ``` methodSignature
            @Default
            default AppleAssetCatalogsCompilationOptions getAssetCatalogsCompilationOptions()
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
