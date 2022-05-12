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

## Interface Compiler {#interface-compiler .title title="Interface Compiler"}
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
    :   `ClangClCompiler`, `ClangCompiler`, `ClangWindowsCompiler`,
        `DefaultCompiler`, `GccCompiler`, `WindowsCompiler`,
        `WindowsMl64Compiler`

    ------------------------------------------------------------------------

        public interface Compiler
        extends Tool

    ::: block
    Interface for a c/c++ compiler.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                             Method                                                                                                               Description
          ------------------------------------------------------------- -------------------------------------------------------------------------------------------------------------------- -------------
          `DependencyTrackingMode`                                      `getDependencyTrackingMode()`                                                                                         
          `Optional<com.google.common.collect.ImmutableList<String>>`   `getFlagsForColorDiagnostics()`                                                                                       
          `com.google.common.collect.ImmutableList<String>`             `getFlagsForReproducibleBuild​(String alternativeCompilationDir,                             Path currentCellPath)`    
          `com.google.common.collect.ImmutableList<String>`             `getPdcFlags()`                                                                                                       
          `com.google.common.collect.ImmutableList<String>`             `getPicFlags()`                                                                                                       
          `com.google.common.collect.ImmutableList<String>`             `getPreArgfileArgs()`                                                                                                 
          `Optional<String>`                                            `getStderr​(ProcessExecutor.Result result)`                                                                            
          `boolean`                                                     `getUseUnixPathSeparator()`                                                                                           
          `boolean`                                                     `isArgFileSupported()`                                                                                                
          `com.google.common.collect.ImmutableList<String>`             `languageArgs​(String language)`                                                                                       
          `boolean`                                                     `needsToRemoveCompiledFilenamesFromOutput()`                                                                          
          `com.google.common.collect.ImmutableList<String>`             `outputArgs​(String outputPath)`                                                                                       
          `com.google.common.collect.ImmutableList<String>`             `outputDependenciesArgs​(String outputPath)`                                                                           
          `boolean`                                                     `shouldSanitizeOutputBinary()`                                                                                        

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.toolchain.tool.Tool}

            ### Methods inherited from interface com.facebook.buck.core.toolchain.tool.[Tool](../../core/toolchain/tool/Tool.html "interface in com.facebook.buck.core.toolchain.tool")

            `getCommandPrefix, getEnvironment`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getFlagsForReproducibleBuild(java.lang.String,java.nio.file.Path)}

        -   #### getFlagsForReproducibleBuild

            ``` methodSignature
            com.google.common.collect.ImmutableList<String> getFlagsForReproducibleBuild​(String alternativeCompilationDir,
                                                                                         Path currentCellPath)
            ```

        []{#getFlagsForColorDiagnostics()}

        -   #### getFlagsForColorDiagnostics

            ``` methodSignature
            Optional<com.google.common.collect.ImmutableList<String>> getFlagsForColorDiagnostics()
            ```

        []{#languageArgs(java.lang.String)}

        -   #### languageArgs

            ``` methodSignature
            com.google.common.collect.ImmutableList<String> languageArgs​(String language)
            ```

        []{#isArgFileSupported()}

        -   #### isArgFileSupported

            ``` methodSignature
            boolean isArgFileSupported()
            ```

        []{#getPreArgfileArgs()}

        -   #### getPreArgfileArgs

            ``` methodSignature
            com.google.common.collect.ImmutableList<String> getPreArgfileArgs()
            ```

        []{#outputArgs(java.lang.String)}

        -   #### outputArgs

            ``` methodSignature
            com.google.common.collect.ImmutableList<String> outputArgs​(String outputPath)
            ```

        []{#outputDependenciesArgs(java.lang.String)}

        -   #### outputDependenciesArgs

            ``` methodSignature
            com.google.common.collect.ImmutableList<String> outputDependenciesArgs​(String outputPath)
            ```

        []{#getPicFlags()}

        -   #### getPicFlags

            ``` methodSignature
            com.google.common.collect.ImmutableList<String> getPicFlags()
            ```

        []{#getPdcFlags()}

        -   #### getPdcFlags

            ``` methodSignature
            com.google.common.collect.ImmutableList<String> getPdcFlags()
            ```

        []{#getDependencyTrackingMode()}

        -   #### getDependencyTrackingMode

            ``` methodSignature
            DependencyTrackingMode getDependencyTrackingMode()
            ```

        []{#shouldSanitizeOutputBinary()}

        -   #### shouldSanitizeOutputBinary

            ``` methodSignature
            boolean shouldSanitizeOutputBinary()
            ```

        []{#needsToRemoveCompiledFilenamesFromOutput()}

        -   #### needsToRemoveCompiledFilenamesFromOutput

            ``` methodSignature
            boolean needsToRemoveCompiledFilenamesFromOutput()
            ```

        []{#getStderr(com.facebook.buck.util.ProcessExecutor.Result)}

        -   #### getStderr

            ``` methodSignature
            Optional<String> getStderr​(ProcessExecutor.Result result)
            ```

        []{#getUseUnixPathSeparator()}

        -   #### getUseUnixPathSeparator

            ``` methodSignature
            boolean getUseUnixPathSeparator()
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
