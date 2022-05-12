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

## Class ClangWindowsCompiler {#class-clangwindowscompiler .title title="Class ClangWindowsCompiler"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.toolchain.tool.DelegatingTool](../../core/toolchain/tool/DelegatingTool.html "class in com.facebook.buck.core.toolchain.tool")

    -   -   [com.facebook.buck.cxx.toolchain.DefaultCompiler](DefaultCompiler.html "class in com.facebook.buck.cxx.toolchain")

        -   -   [com.facebook.buck.cxx.toolchain.ClangCompiler](ClangCompiler.html "class in com.facebook.buck.cxx.toolchain")

            -   -   com.facebook.buck.cxx.toolchain.ClangWindowsCompiler

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`, `Tool`, `Compiler`

    ------------------------------------------------------------------------

        public class ClangWindowsCompiler
        extends ClangCompiler

    ::: block
    Compiler implementation for the Clang for Windows toolchain.
    This uses clang.exe directly, not simply clang-cl which is a
    CL-compatible front end for clang. This implementation exists
    basically only because of argfile differences.
    \--rsp-quoting=windows should be added to use argfile on Windows.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                               Description
          ------------------------------------------------------------------------------------------------------------------------- -------------
          `ClangWindowsCompiler​(Tool tool,                     ToolType toolType,                     boolean useDependencyTree)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                   Method                                                                                                       Description
          --------------------------------------------------- ------------------------------------------------------------------------------------------------------------ -------------
          `com.google.common.collect.ImmutableList<String>`   `getFlagsForReproducibleBuild​(String altCompilationDir,                             Path currentCellPath)`    
          `com.google.common.collect.ImmutableList<String>`   `getPreArgfileArgs()`                                                                                         

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.toolchain.ClangCompiler}

            ### Methods inherited from class com.facebook.buck.cxx.toolchain.[ClangCompiler](ClangCompiler.html "class in com.facebook.buck.cxx.toolchain")

            `getDependencyTrackingMode, getFlagsForColorDiagnostics, isArgFileSupported, outputDependenciesArgs`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.toolchain.DefaultCompiler}

            ### Methods inherited from class com.facebook.buck.cxx.toolchain.[DefaultCompiler](DefaultCompiler.html "class in com.facebook.buck.cxx.toolchain")

            `getPdcFlags, getPicFlags, getStderr, getUseUnixPathSeparator, languageArgs, needsToRemoveCompiledFilenamesFromOutput, outputArgs, shouldSanitizeOutputBinary`

        ```{=html}
        <!-- -->
        ```
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

        []{#<init>(com.facebook.buck.core.toolchain.tool.Tool,com.facebook.buck.cxx.toolchain.ToolType,boolean)}

        -   #### ClangWindowsCompiler

                public ClangWindowsCompiler​(Tool tool,
                                            ToolType toolType,
                                            boolean useDependencyTree)
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

            [Overrides:]{.overrideSpecifyLabel}
            :   `getFlagsForReproducibleBuild` in class `ClangCompiler`

        []{#getPreArgfileArgs()}

        -   #### getPreArgfileArgs

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getPreArgfileArgs()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPreArgfileArgs` in interface `Compiler`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getPreArgfileArgs` in class `DefaultCompiler`
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
