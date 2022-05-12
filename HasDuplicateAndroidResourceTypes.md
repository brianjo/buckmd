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

## Interface HasDuplicateAndroidResourceTypes {#interface-hasduplicateandroidresourcetypes .title title="Interface HasDuplicateAndroidResourceTypes"}
:::

::: contentContainer
::: description
-   

    All Known Subinterfaces:
    :   `AndroidGraphEnhancerArgs`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AndroidBinaryDescriptionArg`, `AndroidBundleDescriptionArg`

    ------------------------------------------------------------------------

        public interface HasDuplicateAndroidResourceTypes
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Interface                                                       Description
          ------------------- --------------------------------------------------------------- -------------
          `static class `     `HasDuplicateAndroidResourceTypes.DuplicateResourceBehaviour`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                       Method                                         Description
          ----------------------------------------------------------------------- ---------------------------------------------- -------------
          `Set<RDotTxtEntry.RType>`                                               `getAllowedDuplicateResourceTypes()`            
          `Set<RDotTxtEntry.RType>`                                               `getBannedDuplicateResourceTypes()`             
          `default HasDuplicateAndroidResourceTypes.DuplicateResourceBehaviour`   `getDuplicateResourceBehavior()`                
          `Optional<SourcePath>`                                                  `getDuplicateResourceWhitelist()`               
          `default EnumSet<RDotTxtEntry.RType>`                                   `getEffectiveBannedDuplicateResourceTypes()`    

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

        []{#getDuplicateResourceBehavior()}

        -   #### getDuplicateResourceBehavior

            ``` methodSignature
            @Default
            default HasDuplicateAndroidResourceTypes.DuplicateResourceBehaviour getDuplicateResourceBehavior()
            ```

        []{#getAllowedDuplicateResourceTypes()}

        -   #### getAllowedDuplicateResourceTypes

            ``` methodSignature
            Set<RDotTxtEntry.RType> getAllowedDuplicateResourceTypes()
            ```

        []{#getBannedDuplicateResourceTypes()}

        -   #### getBannedDuplicateResourceTypes

            ``` methodSignature
            Set<RDotTxtEntry.RType> getBannedDuplicateResourceTypes()
            ```

        []{#getDuplicateResourceWhitelist()}

        -   #### getDuplicateResourceWhitelist

            ``` methodSignature
            Optional<SourcePath> getDuplicateResourceWhitelist()
            ```

        []{#getEffectiveBannedDuplicateResourceTypes()}

        -   #### getEffectiveBannedDuplicateResourceTypes

            ``` methodSignature
            @Derived
            default EnumSet<RDotTxtEntry.RType> getEffectiveBannedDuplicateResourceTypes()
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
-   [Nested](#nested.class.summary) \| 
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
