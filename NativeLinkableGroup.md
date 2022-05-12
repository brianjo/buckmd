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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain.nativelink](package-summary.html)
:::

## Interface NativeLinkableGroup {#interface-nativelinkablegroup .title title="Interface NativeLinkableGroup"}
:::

::: contentContainer
::: description
-   

    All Known Subinterfaces:
    :   `AbstractCxxLibraryGroup`, `HaskellOmnibusLinkable`,
        `LegacyNativeLinkableGroup`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `CxxLibraryGroup`, `CxxPrecompiledHeaderTemplate`,
        `CxxPrefixHeader`, `DLibrary`, `HalideLibrary`,
        `HaskellLibrary`, `PrebuiltAppleFramework`,
        `PrebuiltCxxLibrary`,
        `PrebuiltCxxLibraryGroupDescription.CustomPrebuiltCxxLibrary`,
        `PrebuiltHaskellLibrary`, `PreInclude`, `RustLibrary`,
        `SwiftRuntimeNativeLinkableGroup`, `SystemLuaCxxLibrary`

    ------------------------------------------------------------------------

        public interface NativeLinkableGroup

    ::: block
    Interface for
    [`BuildRule`](../../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
    objects (e.g. C++ libraries) which can contribute to the top-level
    link of a native binary (e.g. C++ binary). This represents the
    linkable object for all platforms.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Interface                       Description
          ------------------- ------------------------------- -------------
          `static class `     `NativeLinkableGroup.Linkage`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                           Description
          ------------------- ------------------------------------------------------------------------------------------------ -------------
          `BuildTarget`       `getBuildTarget()`                                                                                
          `NativeLinkable`    `getNativeLinkable​(CxxPlatform cxxPlatform,                  ActionGraphBuilder graphBuilder)`    

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

        []{#getNativeLinkable(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getNativeLinkable

            ``` methodSignature
            NativeLinkable getNativeLinkable​(CxxPlatform cxxPlatform,
                                             ActionGraphBuilder graphBuilder)
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
