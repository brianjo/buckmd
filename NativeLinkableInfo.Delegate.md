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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain.nativelink](package-summary.html)
:::

## Interface NativeLinkableInfo.Delegate {#interface-nativelinkableinfo.delegate .title title="Interface NativeLinkableInfo.Delegate"}
:::

::: contentContainer
::: description
-   

    Enclosing class:
    :   [NativeLinkableInfo](NativeLinkableInfo.html "class in com.facebook.buck.cxx.toolchain.nativelink")

    ------------------------------------------------------------------------

        public static interface NativeLinkableInfo.Delegate

    ::: block
    The Delegate allows instances to create
    [`NativeLinkableInput`](NativeLinkableInput.html "class in com.facebook.buck.cxx.toolchain.nativelink")
    when requested. The returned values will be cached.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                             Method                                                                                                                                                                              Description
          ------------------------------------------------------------- ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `NativeLinkableInput`                                         `computeInput​(ActionGraphBuilder graphBuilder,             Linker.LinkableDepType type,             boolean forceLinkWhole,             TargetConfiguration targetConfiguration)`    
          `com.google.common.collect.ImmutableMap<String,​SourcePath>`   `getSharedLibraries​(ActionGraphBuilder graphBuilder)`                                                                                                                                
          `default boolean`                                             `isPrebuiltSOForHaskellOmnibus​(ActionGraphBuilder graphBuilder)`                                                                                                                     

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
          .tableTab}[[Default
          Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#computeInput(com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.cxx.toolchain.linker.Linker.LinkableDepType,boolean,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### computeInput

            ``` methodSignature
            NativeLinkableInput computeInput​(ActionGraphBuilder graphBuilder,
                                             Linker.LinkableDepType type,
                                             boolean forceLinkWhole,
                                             TargetConfiguration targetConfiguration)
            ```

        []{#getSharedLibraries(com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getSharedLibraries

            ``` methodSignature
            com.google.common.collect.ImmutableMap<String,​SourcePath> getSharedLibraries​(ActionGraphBuilder graphBuilder)
            ```

        []{#isPrebuiltSOForHaskellOmnibus(com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### isPrebuiltSOForHaskellOmnibus

            ``` methodSignature
            default boolean isPrebuiltSOForHaskellOmnibus​(ActionGraphBuilder graphBuilder)
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
