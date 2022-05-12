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
[Package]{.packageLabelInType} [com.facebook.buck.core.description.attr](package-summary.html)
:::

## Interface ImplicitFlavorsInferringDescription {#interface-implicitflavorsinferringdescription .title title="Interface ImplicitFlavorsInferringDescription"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `AppleBinaryDescription`, `AppleLibraryDescription`,
        `CxxBinaryDescription`, `CxxLibraryDescription`

    ------------------------------------------------------------------------

        public interface ImplicitFlavorsInferringDescription

    ::: block
    While building up the target graph, we allow descriptions to apply
    default flavors (e.g., #iphonesimulator-x86_64 for C++ or
    Objective-C libraries built in an iPhone simulator environment) from
    the .buckconfig file.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                        Method                                                                                                                                                             Description
          -------------------------------------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `com.google.common.collect.ImmutableSortedSet<Flavor>`   `addImplicitFlavors​(com.google.common.collect.ImmutableSortedSet<Flavor> argDefaultFlavors,                   TargetConfiguration toolchainTargetConfiguration)`    

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

        []{#addImplicitFlavors(com.google.common.collect.ImmutableSortedSet,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### addImplicitFlavors

            ``` methodSignature
            com.google.common.collect.ImmutableSortedSet<Flavor> addImplicitFlavors​(com.google.common.collect.ImmutableSortedSet<Flavor> argDefaultFlavors,
                                                                                    TargetConfiguration toolchainTargetConfiguration)
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
