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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.providers](package-summary.html)
:::

## Interface SkylarkProviderInfo {#interface-skylarkproviderinfo .title title="Interface SkylarkProviderInfo"}
:::

::: contentContainer
::: description
-   

    All Known Subinterfaces:
    :   `ProviderInfo<U>`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `BuiltInProviderInfo`, `DefaultInfo`,
        `DotnetLegacyToolchainInfo`, `DotnetLibraryProviderInfo`,
        `ImmutableDefaultInfo`, `ImmutableDotnetLegacyToolchainInfo`,
        `ImmutableDotnetLibraryProviderInfo`, `ImmutableRunInfo`,
        `ImmutableTestInfo`, `RunInfo`, `TestInfo`,
        `UserDefinedProviderInfo`

    ------------------------------------------------------------------------

        public interface SkylarkProviderInfo

    ::: block
    An interface to
    [`ProviderInfo`](ProviderInfo.html "interface in com.facebook.buck.core.rules.providers")
    to use in skylark methods. This allows us to more easily validate
    user provided `SkylarkList` and `SkylarkDict` objects which have
    problems with generic subtypes. See
    `SkylarkList.getContents(Class, String)` for an example of a problem
    method
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                Description
          ------------------- --------------------- -------------
          `ProviderInfo<?>`   `getProviderInfo()`    

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

        []{#getProviderInfo()}

        -   #### getProviderInfo

            ``` methodSignature
            ProviderInfo<?> getProviderInfo()
            ```

            [Returns:]{.returnLabel}
            :   The original provider info
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
