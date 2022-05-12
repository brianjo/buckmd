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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain](package-summary.html)
:::

## Interface CxxPlatformsSupplier {#interface-cxxplatformssupplier .title title="Interface CxxPlatformsSupplier"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `Toolchain`, `ToolchainWithCapability`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AppleCxxPlatformsProvider`, `NdkCxxPlatformsProvider`

    ------------------------------------------------------------------------

        public interface CxxPlatformsSupplier
        extends ToolchainWithCapability

    ::: block
    A toolchain that provides CXX platforms.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                        Method                          Description
          ------------------------------------------------------------------------ ------------------------------- -------------
          `com.google.common.collect.ImmutableMap<Flavor,​UnresolvedCxxPlatform>`   `getUnresolvedCxxPlatforms()`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.toolchain.Toolchain}

            ### Methods inherited from interface com.facebook.buck.core.toolchain.[Toolchain](../../core/toolchain/Toolchain.html "interface in com.facebook.buck.core.toolchain")

            `getName`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getUnresolvedCxxPlatforms()}

        -   #### getUnresolvedCxxPlatforms

            ``` methodSignature
            com.google.common.collect.ImmutableMap<Flavor,​UnresolvedCxxPlatform> getUnresolvedCxxPlatforms()
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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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
