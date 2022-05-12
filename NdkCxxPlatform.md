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
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.android.toolchain.ndk](package-summary.html)
:::

## Interface NdkCxxPlatform {#interface-ndkcxxplatform .title title="Interface NdkCxxPlatform"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface NdkCxxPlatform

    ::: block
    Adds Android-specific tools to
    [`CxxPlatform`](../../../cxx/toolchain/CxxPlatform.html "interface in com.facebook.buck.cxx.toolchain").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Interface                  Description
          ------------------- -------------------------- -------------
          `static class `     `NdkCxxPlatform.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                 Method                        Description
          --------------------------------- ----------------------------- -------------
          `static NdkCxxPlatform.Builder`   `builder()`                    
          `CxxPlatform`                     `getCxxPlatform()`             
          `NdkCxxRuntime`                   `getCxxRuntime()`              
          `Optional<SourcePath>`            `getCxxSharedRuntimePath()`    
          `Tool`                            `getObjdump()`                 

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getCxxPlatform()}

        -   #### getCxxPlatform

            ``` methodSignature
            CxxPlatform getCxxPlatform()
            ```

        []{#getCxxRuntime()}

        -   #### getCxxRuntime

            ``` methodSignature
            NdkCxxRuntime getCxxRuntime()
            ```

        []{#getObjdump()}

        -   #### getObjdump

            ``` methodSignature
            Tool getObjdump()
            ```

        []{#getCxxSharedRuntimePath()}

        -   #### getCxxSharedRuntimePath

            ``` methodSignature
            Optional<SourcePath> getCxxSharedRuntimePath()
            ```

            [Returns:]{.returnLabel}
            :   the
                [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
                to the C/C++ runtime library, if one is required.

        []{#builder()}

        -   #### builder

            ``` methodSignature
            static NdkCxxPlatform.Builder builder()
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
-   [Nested](#nested.class.summary) \| 
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
