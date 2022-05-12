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

## Interface AndroidNativeTargetConfigurationMatcher {#interface-androidnativetargetconfigurationmatcher .title title="Interface AndroidNativeTargetConfigurationMatcher"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `ConstraintBasedAndroidNativeTargetConfigurationMatcher`,
        `NoopAndroidNativeTargetConfigurationMatcher`

    ------------------------------------------------------------------------

        public interface AndroidNativeTargetConfigurationMatcher

    ::: block
    Encapsulates logic to check whether platform in configuration of a
    given target matches the CPU type.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                                                   Description
          ------------------- ---------------------------------------------------------------------------------------------------------------------------------------- -------------
          `boolean`           `nativeTargetConfigurationMatchesCpuType​(BuildTarget buildTarget,                                        TargetCpuType targetCpuType)`    

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

        []{#nativeTargetConfigurationMatchesCpuType(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.android.toolchain.ndk.TargetCpuType)}

        -   #### nativeTargetConfigurationMatchesCpuType

            ``` methodSignature
            boolean nativeTargetConfigurationMatchesCpuType​(BuildTarget buildTarget,
                                                            TargetCpuType targetCpuType)
            ```

            [Returns:]{.returnLabel}
            :   `true` when platform in configuration of the target
                matches the given CPU type.
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
