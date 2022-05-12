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
[Package]{.packageLabelInType} [com.facebook.buck.features.go](package-summary.html)
:::

## Interface HasGoLinkable {#interface-hasgolinkable .title title="Interface HasGoLinkable"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `GoBinaryDescriptionArg`, `GoTestDescriptionArg`

    ------------------------------------------------------------------------

        public interface HasGoLinkable
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                               Method                       Description
          --------------------------------------------------------------- ---------------------------- -------------
          `com.google.common.collect.ImmutableList<String>`               `getAssemblerFlags()`         
          `com.google.common.collect.ImmutableList<String>`               `getCompilerFlags()`          
          `com.google.common.collect.ImmutableList<String>`               `getExternalLinkerFlags()`    
          `com.google.common.collect.ImmutableList<String>`               `getLinkerFlags()`            
          `Optional<com.facebook.buck.features.go.GoLinkStep.LinkMode>`   `getLinkMode()`               
          `Optional<Linker.LinkableDepType>`                              `getLinkStyle()`              
          `Optional<Flavor>`                                              `getPlatform()`               
          `com.google.common.collect.ImmutableSortedSet<SourcePath>`      `getResources()`              

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

        []{#getPlatform()}

        -   #### getPlatform

            ``` methodSignature
            Optional<Flavor> getPlatform()
            ```

        []{#getLinkStyle()}

        -   #### getLinkStyle

            ``` methodSignature
            Optional<Linker.LinkableDepType> getLinkStyle()
            ```

        []{#getLinkMode()}

        -   #### getLinkMode

            ``` methodSignature
            Optional<com.facebook.buck.features.go.GoLinkStep.LinkMode> getLinkMode()
            ```

        []{#getCompilerFlags()}

        -   #### getCompilerFlags

            ``` methodSignature
            com.google.common.collect.ImmutableList<String> getCompilerFlags()
            ```

        []{#getAssemblerFlags()}

        -   #### getAssemblerFlags

            ``` methodSignature
            com.google.common.collect.ImmutableList<String> getAssemblerFlags()
            ```

        []{#getLinkerFlags()}

        -   #### getLinkerFlags

            ``` methodSignature
            com.google.common.collect.ImmutableList<String> getLinkerFlags()
            ```

        []{#getExternalLinkerFlags()}

        -   #### getExternalLinkerFlags

            ``` methodSignature
            com.google.common.collect.ImmutableList<String> getExternalLinkerFlags()
            ```

        []{#getResources()}

        -   #### getResources

            ``` methodSignature
            @NaturalOrder
            com.google.common.collect.ImmutableSortedSet<SourcePath> getResources()
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
