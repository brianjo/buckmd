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
[Package]{.packageLabelInType} [com.facebook.buck.features.haskell](package-summary.html)
:::

## Interface HaskellCompileDep {#interface-haskellcompiledep .title title="Interface HaskellCompileDep"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `HaskellLibrary`, `PrebuiltHaskellLibrary`

    ------------------------------------------------------------------------

        public interface HaskellCompileDep

    ::: block
    An interface for rule which can provide interfaces files for a
    haskell compilation.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                          Method                                                                                                                                                            Description
          ---------------------------------------------------------- ----------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `Iterable<BuildRule>`                                      `getCompileDeps​(com.facebook.buck.features.haskell.HaskellPlatform platform)`                                                                                      
          `com.facebook.buck.features.haskell.HaskellCompileInput`   `getCompileInput​(com.facebook.buck.features.haskell.HaskellPlatform platform,                Linker.LinkableDepType depType,                boolean hsProfile)`    
          `com.facebook.buck.features.haskell.HaskellHaddockInput`   `getHaddockInput​(com.facebook.buck.features.haskell.HaskellPlatform platform)`                                                                                     

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

        []{#getCompileDeps(com.facebook.buck.features.haskell.HaskellPlatform)}

        -   #### getCompileDeps

            ``` methodSignature
            Iterable<BuildRule> getCompileDeps​(com.facebook.buck.features.haskell.HaskellPlatform platform)
            ```

            [Returns:]{.returnLabel}
            :   a list of deps needed to compile this rule.

        []{#getCompileInput(com.facebook.buck.features.haskell.HaskellPlatform,com.facebook.buck.cxx.toolchain.linker.Linker.LinkableDepType,boolean)}

        -   #### getCompileInput

            ``` methodSignature
            com.facebook.buck.features.haskell.HaskellCompileInput getCompileInput​(com.facebook.buck.features.haskell.HaskellPlatform platform,
                                                                                   Linker.LinkableDepType depType,
                                                                                   boolean hsProfile)
            ```

            [Returns:]{.returnLabel}
            :   the `HaskellCompileInput` object that contributes to
                compilation.

        []{#getHaddockInput(com.facebook.buck.features.haskell.HaskellPlatform)}

        -   #### getHaddockInput

            ``` methodSignature
            com.facebook.buck.features.haskell.HaskellHaddockInput getHaddockInput​(com.facebook.buck.features.haskell.HaskellPlatform platform)
            ```

            [Returns:]{.returnLabel}
            :   the {#link HaskellHaddockInput} object for compilation
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
