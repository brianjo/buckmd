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
[Package]{.packageLabelInType} [com.facebook.buck.skylark.function](package-summary.html)
:::

## Interface SkylarkProviderFunctionApi {#interface-skylarkproviderfunctionapi .title title="Interface SkylarkProviderFunctionApi"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `SkylarkProviderFunction`

    ------------------------------------------------------------------------

        public interface SkylarkProviderFunctionApi

    ::: block
    Interface for a global Skylark library containing the provider
    method.
    This is only separate from
    [`SkylarkRuleFunctionsApi`](SkylarkRuleFunctionsApi.html "interface in com.facebook.buck.skylark.function")
    at the moment so that new extensibility functionality can be
    disabled behind configuration until it has stabilized.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                             Method                                                                                                          Description
          ------------------------------------------------------------- --------------------------------------------------------------------------------------------------------------- -------------
          `com.google.devtools.build.lib.skylarkbuildapi.ProviderApi`   `provider​(String doc,         Object fields,         com.google.devtools.build.lib.events.Location location)`    

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

        []{#provider(java.lang.String,java.lang.Object,com.google.devtools.build.lib.events.Location)}

        -   #### provider

            ``` methodSignature
            com.google.devtools.build.lib.skylarkbuildapi.ProviderApi provider​(String doc,
                                                                               Object fields,
                                                                               com.google.devtools.build.lib.events.Location location)
                                                                        throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`
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
