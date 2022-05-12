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

## Interface HasAppleCodesignFields {#interface-hasapplecodesignfields .title title="Interface HasAppleCodesignFields"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `AppleBundleDescriptionArg`, `AppleTestDescriptionArg`

    ------------------------------------------------------------------------

        public interface HasAppleCodesignFields

    ::: block
    Defines a set of codesign-related fields that are applicable to
    bundle-like rules.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                   Method                    Description
          --------------------------------------------------- ------------------------- -------------
          `com.google.common.collect.ImmutableList<String>`   `getCodesignFlags()`       
          `Optional<String>`                                  `getCodesignIdentity()`    

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

        []{#getCodesignFlags()}

        -   #### getCodesignFlags

            ``` methodSignature
            com.google.common.collect.ImmutableList<String> getCodesignFlags()
            ```

            [Returns:]{.returnLabel}
            :   Additional flags passed to the underlying codesign tool.
                For example, this can be used to sign deep macOS
                frameworks using \"\--deep\".

        []{#getCodesignIdentity()}

        -   #### getCodesignIdentity

            ``` methodSignature
            Optional<String> getCodesignIdentity()
            ```

            [Returns:]{.returnLabel}
            :   A codesign identity that will be used for adhoc signing
                (i.e., on platforms like macOS and simulators). This
                field can be used to sign with Developer ID on macOS.
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
