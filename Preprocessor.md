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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain](package-summary.html)
:::

## Interface Preprocessor {#interface-preprocessor .title title="Interface Preprocessor"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AddsToRuleKey`, `Tool`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `ClangClPreprocessor`, `ClangPreprocessor`,
        `ClangWindowsPreprocessor`, `GccPreprocessor`,
        `WindowsPreprocessor`

    ------------------------------------------------------------------------

        public interface Preprocessor
        extends Tool

    ::: block
    Interface for a c/c++ preprocessor.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type            Method                                                             Description
          ---------------------------- ------------------------------------------------------------------ -------------
          `Iterable<String>`           `localIncludeArgs​(Iterable<String> includeRoots)`                   
          `Iterable<String>`           `precompiledHeaderArgs​(Path pchOutputPath)`                         
          `Iterable<String>`           `prefixHeaderArgs​(Path prefixHeader)`                               
          `default Iterable<String>`   `prefixOrPCHArgs​(boolean precompiled,                Path path)`    
          `boolean`                    `supportsHeaderMaps()`                                              
          `boolean`                    `supportsPrecompiledHeaders()`                                      
          `Iterable<String>`           `systemIncludeArgs​(Iterable<String> includeRoots)`                  

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
          .tableTab}[[Default
          Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.toolchain.tool.Tool}

            ### Methods inherited from interface com.facebook.buck.core.toolchain.tool.[Tool](../../core/toolchain/tool/Tool.html "interface in com.facebook.buck.core.toolchain.tool")

            `getCommandPrefix, getEnvironment`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#supportsHeaderMaps()}

        -   #### supportsHeaderMaps

            ``` methodSignature
            boolean supportsHeaderMaps()
            ```

        []{#supportsPrecompiledHeaders()}

        -   #### supportsPrecompiledHeaders

            ``` methodSignature
            boolean supportsPrecompiledHeaders()
            ```

        []{#localIncludeArgs(java.lang.Iterable)}

        -   #### localIncludeArgs

            ``` methodSignature
            Iterable<String> localIncludeArgs​(Iterable<String> includeRoots)
            ```

        []{#systemIncludeArgs(java.lang.Iterable)}

        -   #### systemIncludeArgs

            ``` methodSignature
            Iterable<String> systemIncludeArgs​(Iterable<String> includeRoots)
            ```

        []{#precompiledHeaderArgs(java.nio.file.Path)}

        -   #### precompiledHeaderArgs

            ``` methodSignature
            Iterable<String> precompiledHeaderArgs​(Path pchOutputPath)
            ```

        []{#prefixHeaderArgs(java.nio.file.Path)}

        -   #### prefixHeaderArgs

            ``` methodSignature
            Iterable<String> prefixHeaderArgs​(Path prefixHeader)
            ```

        []{#prefixOrPCHArgs(boolean,java.nio.file.Path)}

        -   #### prefixOrPCHArgs

            ``` methodSignature
            default Iterable<String> prefixOrPCHArgs​(boolean precompiled,
                                                     Path path)
            ```

            [Parameters:]{.paramLabel}
            :   `prefixHeader` - the `prefix_hedaer` param for the rule.
            :   `pchOutputPath` - either a `precompiled_header` path, or
                the result of precompiling `prefixHeader`. Not mutually
                exclusive with `prefixHeader`; if both are given, the
                precompiled version of it is preferred.
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
