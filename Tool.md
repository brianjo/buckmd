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
[Package]{.packageLabelInType} [com.facebook.buck.core.toolchain.tool](package-summary.html)
:::

## Interface Tool {#interface-tool .title title="Interface Tool"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AddsToRuleKey`

    ```{=html}
    <!-- -->
    ```

    All Known Subinterfaces:
    :   `Archiver`, `Compiler`, `Javac`, `Kotlinc`, `Linker`,
        `Preprocessor`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `BsdArchiver`, `ClangClCompiler`, `ClangClPreprocessor`,
        `ClangCompiler`, `ClangPreprocessor`, `ClangWindowsArchiver`,
        `ClangWindowsCompiler`, `ClangWindowsPreprocessor`,
        `CommandTool`, `DarwinLinker`, `DefaultCompiler`,
        `DelegatingTool`, `ExternalJavac`, `ExternalKotlinc`,
        `GccCompiler`, `GccPreprocessor`, `GnuArchiver`, `GnuLinker`,
        `Groovyc`, `HashedFileTool`, `InferDistTool`, `JarBackedJavac`,
        `JarBackedReflectedKotlinc`, `JdkProvidedInMemoryJavac`,
        `Jsr199Javac`, `PythonEnvironment`, `RunInfoLegacyTool`,
        `VersionedTool`, `WindowsArchiver`, `WindowsCompiler`,
        `WindowsLinker`, `WindowsMl64Compiler`, `WindowsPreprocessor`

    ------------------------------------------------------------------------

        public interface Tool
        extends AddsToRuleKey

    ::: block
    An abstraction for describing some tools used as part of the build.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                         Method                                                   Description
          --------------------------------------------------------- -------------------------------------------------------- -------------
          `com.google.common.collect.ImmutableList<String>`         `getCommandPrefix​(SourcePathResolverAdapter resolver)`    
          `com.google.common.collect.ImmutableMap<String,​String>`   `getEnvironment​(SourcePathResolverAdapter resolver)`      

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

        []{#getCommandPrefix(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### getCommandPrefix

            ``` methodSignature
            com.google.common.collect.ImmutableList<String> getCommandPrefix​(SourcePathResolverAdapter resolver)
            ```

            [Returns:]{.returnLabel}
            :   the prefix command use to run this tool.

        []{#getEnvironment(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### getEnvironment

            ``` methodSignature
            com.google.common.collect.ImmutableMap<String,​String> getEnvironment​(SourcePathResolverAdapter resolver)
            ```

            [Returns:]{.returnLabel}
            :   the list of environment variables to set when running
                the command.
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
