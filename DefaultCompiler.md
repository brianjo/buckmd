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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
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

## Class DefaultCompiler {#class-defaultcompiler .title title="Class DefaultCompiler"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.toolchain.tool.DelegatingTool](../../core/toolchain/tool/DelegatingTool.html "class in com.facebook.buck.core.toolchain.tool")

    -   -   com.facebook.buck.cxx.toolchain.DefaultCompiler

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`, `Tool`, `Compiler`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `ClangCompiler`, `GccCompiler`, `WindowsCompiler`,
        `WindowsMl64Compiler`

    ------------------------------------------------------------------------

        public abstract class DefaultCompiler
        extends DelegatingTool
        implements Compiler

    ::: block
    Default implementation of the Compiler interface.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                 Description
          --------------------------------------------------------------------------- -------------
          `DefaultCompiler​(Tool tool,                boolean useUnixPathSeparator)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                             Method                                                                                                       Description
          ------------------------------------------------------------- ------------------------------------------------------------------------------------------------------------ -------------
          `DependencyTrackingMode`                                      `getDependencyTrackingMode()`                                                                                 
          `Optional<com.google.common.collect.ImmutableList<String>>`   `getFlagsForColorDiagnostics()`                                                                               
          `com.google.common.collect.ImmutableList<String>`             `getFlagsForReproducibleBuild​(String altCompilationDir,                             Path currentCellPath)`    
          `com.google.common.collect.ImmutableList<String>`             `getPdcFlags()`                                                                                               
          `com.google.common.collect.ImmutableList<String>`             `getPicFlags()`                                                                                               
          `com.google.common.collect.ImmutableList<String>`             `getPreArgfileArgs()`                                                                                         
          `Optional<String>`                                            `getStderr​(ProcessExecutor.Result result)`                                                                    
          `boolean`                                                     `getUseUnixPathSeparator()`                                                                                   
          `boolean`                                                     `isArgFileSupported()`                                                                                        
          `com.google.common.collect.ImmutableList<String>`             `languageArgs​(String inputLanguage)`                                                                          
          `boolean`                                                     `needsToRemoveCompiledFilenamesFromOutput()`                                                                  
          `com.google.common.collect.ImmutableList<String>`             `outputArgs​(String outputPath)`                                                                               
          `com.google.common.collect.ImmutableList<String>`             `outputDependenciesArgs​(String outputPath)`                                                                   
          `boolean`                                                     `shouldSanitizeOutputBinary()`                                                                                

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.toolchain.tool.DelegatingTool}

            ### Methods inherited from class com.facebook.buck.core.toolchain.tool.[DelegatingTool](../../core/toolchain/tool/DelegatingTool.html "class in com.facebook.buck.core.toolchain.tool")

            `getCommandPrefix, getEnvironment`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.toolchain.tool.Tool}

            ### Methods inherited from interface com.facebook.buck.core.toolchain.tool.[Tool](../../core/toolchain/tool/Tool.html "interface in com.facebook.buck.core.toolchain.tool")

            `getCommandPrefix, getEnvironment`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.toolchain.tool.Tool,boolean)}

        -   #### DefaultCompiler

                public DefaultCompiler​(Tool tool,
                                       boolean useUnixPathSeparator)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getFlagsForReproducibleBuild(java.lang.String,java.nio.file.Path)}

        -   #### getFlagsForReproducibleBuild

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getFlagsForReproducibleBuild​(String altCompilationDir,
                                                                                                Path currentCellPath)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFlagsForReproducibleBuild` in interface `Compiler`

        []{#getFlagsForColorDiagnostics()}

        -   #### getFlagsForColorDiagnostics

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableList<String>> getFlagsForColorDiagnostics()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFlagsForColorDiagnostics` in interface `Compiler`

        []{#isArgFileSupported()}

        -   #### isArgFileSupported

            ``` methodSignature
            public boolean isArgFileSupported()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isArgFileSupported` in interface `Compiler`

        []{#getPreArgfileArgs()}

        -   #### getPreArgfileArgs

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getPreArgfileArgs()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPreArgfileArgs` in interface `Compiler`

        []{#outputArgs(java.lang.String)}

        -   #### outputArgs

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> outputArgs​(String outputPath)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `outputArgs` in interface `Compiler`

        []{#outputDependenciesArgs(java.lang.String)}

        -   #### outputDependenciesArgs

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> outputDependenciesArgs​(String outputPath)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `outputDependenciesArgs` in interface `Compiler`

        []{#languageArgs(java.lang.String)}

        -   #### languageArgs

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> languageArgs​(String inputLanguage)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `languageArgs` in interface `Compiler`

        []{#getPdcFlags()}

        -   #### getPdcFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getPdcFlags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPdcFlags` in interface `Compiler`

        []{#getPicFlags()}

        -   #### getPicFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getPicFlags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPicFlags` in interface `Compiler`

        []{#getDependencyTrackingMode()}

        -   #### getDependencyTrackingMode

            ``` methodSignature
            public DependencyTrackingMode getDependencyTrackingMode()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDependencyTrackingMode` in interface `Compiler`

        []{#shouldSanitizeOutputBinary()}

        -   #### shouldSanitizeOutputBinary

            ``` methodSignature
            public boolean shouldSanitizeOutputBinary()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `shouldSanitizeOutputBinary` in interface `Compiler`

        []{#needsToRemoveCompiledFilenamesFromOutput()}

        -   #### needsToRemoveCompiledFilenamesFromOutput

            ``` methodSignature
            public boolean needsToRemoveCompiledFilenamesFromOutput()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `needsToRemoveCompiledFilenamesFromOutput` in
                interface `Compiler`

        []{#getStderr(com.facebook.buck.util.ProcessExecutor.Result)}

        -   #### getStderr

            ``` methodSignature
            public Optional<String> getStderr​(ProcessExecutor.Result result)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getStderr` in interface `Compiler`

        []{#getUseUnixPathSeparator()}

        -   #### getUseUnixPathSeparator

            ``` methodSignature
            public boolean getUseUnixPathSeparator()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getUseUnixPathSeparator` in interface `Compiler`
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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::