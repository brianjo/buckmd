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
[Package]{.packageLabelInType} [com.facebook.buck.android.toolchain.ndk](package-summary.html)
:::

## Interface NdkCxxPlatformCompiler {#interface-ndkcxxplatformcompiler .title title="Interface NdkCxxPlatformCompiler"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AddsToRuleKey`

    ------------------------------------------------------------------------

        public interface NdkCxxPlatformCompiler
        extends AddsToRuleKey
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                 Method                                                              Description
          --------------------------------- ------------------------------------------------------------------- -------------
          `String`                          `getGccVersion()`                                                    
          `NdkCompilerType`                 `getType()`                                                          
          `String`                          `getVersion()`                                                       
          `static NdkCxxPlatformCompiler`   `of​(NdkCompilerType type,   String version,   String gccVersion)`    

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

        []{#getType()}

        -   #### getType

            ``` methodSignature
            NdkCompilerType getType()
            ```

        []{#getVersion()}

        -   #### getVersion

            ``` methodSignature
            String getVersion()
            ```

            [Returns:]{.returnLabel}
            :   the compiler version, corresponding to either
                \`gcc_version\` or \`clang_version\` from the
                .buckconfig settings, depending on which compiler family
                was selected.

        []{#getGccVersion()}

        -   #### getGccVersion

            ``` methodSignature
            String getGccVersion()
            ```

            [Returns:]{.returnLabel}
            :   the GCC compiler version. Since even runtimes which are
                not GCC-based need to use GCC tools (e.g. ar, as,,
                ld.gold), we need to \*always\* have a version of GCC.

        []{#of(com.facebook.buck.android.toolchain.ndk.NdkCompilerType,java.lang.String,java.lang.String)}

        -   #### of

            ``` methodSignature
            static NdkCxxPlatformCompiler of​(NdkCompilerType type,
                                             String version,
                                             String gccVersion)
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
