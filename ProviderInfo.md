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

## Interface ProviderInfo\<U extends ProviderInfo\<U\>\> {#interface-providerinfou-extends-providerinfou .title title="Interface ProviderInfo"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable`,
        `SkylarkProviderInfo`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkValue`

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

        public interface ProviderInfo<U extends ProviderInfo<U>>
        extends SkylarkProviderInfo, com.google.devtools.build.lib.skylarkinterface.SkylarkValue

    ::: block
    The information, which is a struct-like object, passed between rules
    during rule analysis. This object is created via
    [`Provider`](Provider.html "interface in com.facebook.buck.core.rules.providers").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method            Description
          ------------------- ----------------- -------------
          `Provider<U>`       `getProvider()`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable}

            ### Methods inherited from interface com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable

            `debugPrint, repr, str`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.providers.SkylarkProviderInfo}

            ### Methods inherited from interface com.facebook.buck.core.rules.providers.[SkylarkProviderInfo](SkylarkProviderInfo.html "interface in com.facebook.buck.core.rules.providers")

            `getProviderInfo`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.google.devtools.build.lib.skylarkinterface.SkylarkValue}

            ### Methods inherited from interface com.google.devtools.build.lib.skylarkinterface.SkylarkValue

            `isHashable, isImmutable`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getProvider()}

        -   #### getProvider

            ``` methodSignature
            Provider<U> getProvider()
            ```

            [Returns:]{.returnLabel}
            :   the
                [`Provider`](Provider.html "interface in com.facebook.buck.core.rules.providers")
                instance that constructs instances of this info.
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
