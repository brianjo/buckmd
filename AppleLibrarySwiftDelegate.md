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

## Interface AppleLibrarySwiftDelegate {#interface-applelibraryswiftdelegate .title title="Interface AppleLibrarySwiftDelegate"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `AppleTestDescription`

    ------------------------------------------------------------------------

        public interface AppleLibrarySwiftDelegate

    ::: block
    Provides an ability to inject
    [`CxxPreprocessorInput`](../cxx/CxxPreprocessorInput.html "class in com.facebook.buck.cxx")s
    for the Swift compilation process. This is useful if
    [`AppleLibraryDescription`](AppleLibraryDescription.html "class in com.facebook.buck.apple")
    is composed by another
    [`DescriptionWithTargetGraph`](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                Method                                                                                                                                                                                                                                        Description
          ---------------------------------------------------------------- --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `com.google.common.collect.ImmutableSet<CxxPreprocessorInput>`   `getPreprocessorInputForSwift​(BuildTarget buildTarget,                             ActionGraphBuilder graphBuilder,                             CxxPlatform cxxPlatform,                             CxxLibraryDescription.CommonArg args)`    

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

        []{#getPreprocessorInputForSwift(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.cxx.CxxLibraryDescription.CommonArg)}

        -   #### getPreprocessorInputForSwift

            ``` methodSignature
            com.google.common.collect.ImmutableSet<CxxPreprocessorInput> getPreprocessorInputForSwift​(BuildTarget buildTarget,
                                                                                                      ActionGraphBuilder graphBuilder,
                                                                                                      CxxPlatform cxxPlatform,
                                                                                                      CxxLibraryDescription.CommonArg args)
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
