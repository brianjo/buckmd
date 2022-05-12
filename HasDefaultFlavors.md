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
[Package]{.packageLabelInType} [com.facebook.buck.core.model](package-summary.html)
:::

## Interface HasDefaultFlavors {#interface-hasdefaultflavors .title title="Interface HasDefaultFlavors"}
:::

::: contentContainer
::: description
-   

    All Known Subinterfaces:
    :   `AppleNativeTargetDescriptionArg`,
        `CxxBinaryDescription.CommonArg`, `CxxConstructorArg`,
        `CxxLibraryDescription.CommonArg`, `LinkableCxxConstructorArg`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AppleBinaryDescriptionArg`, `AppleLibraryDescriptionArg`,
        `AppleTestDescriptionArg`, `CgoLibraryDescriptionArg`,
        `CxxBinaryDescriptionArg`, `CxxLibraryDescriptionArg`,
        `CxxLuaExtensionDescriptionArg`,
        `CxxPythonExtensionDescriptionArg`, `CxxTestDescriptionArg`,
        `HalideLibraryDescriptionArg`

    ------------------------------------------------------------------------

        public interface HasDefaultFlavors

    ::: block
    A constructor arg of rules which have default flavors.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                        Method                  Description
          -------------------------------------------------------- ----------------------- -------------
          `com.google.common.collect.ImmutableSortedSet<Flavor>`   `getDefaultFlavors()`    

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

        []{#getDefaultFlavors()}

        -   #### getDefaultFlavors

            ``` methodSignature
            @NaturalOrder
            com.google.common.collect.ImmutableSortedSet<Flavor> getDefaultFlavors()
            ```

            [Returns:]{.returnLabel}
            :   If present, the default flavors with which to build this
                target if none are provided on the command line.
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
