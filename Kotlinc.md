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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.kotlin](package-summary.html)
:::

## Interface Kotlinc {#interface-kotlinc .title title="Interface Kotlinc"}
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
    :   `ExternalKotlinc`, `JarBackedReflectedKotlinc`

    ------------------------------------------------------------------------

        public interface Kotlinc
        extends Tool

    ::: block
    Interface for a kotlin compiler.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                         Method                                                                                                                                                                                                                                                                                                                                                                                                        Description
          --------------------------------------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `int`                                                     `buildWithClasspath​(ExecutionContext context,                   BuildTarget invokingRule,                   com.google.common.collect.ImmutableList<String> options,                   com.google.common.collect.ImmutableSortedSet<Path> kotlinSourceFilePaths,                   Path pathToSrcsList,                   Optional<Path> workingDirectory,                   ProjectFilesystem fileSystem)`    
          `com.google.common.collect.ImmutableList<Path>`           `getAdditionalClasspathEntries​(SourcePathResolverAdapter sourcePathResolverAdapter)`                                                                                                                                                                                                                                                                                                                           
          `Path`                                                    `getAnnotationProcessorPath​(SourcePathResolverAdapter sourcePathResolverAdapter)`                                                                                                                                                                                                                                                                                                                              
          `String`                                                  `getDescription​(com.google.common.collect.ImmutableList<String> options,               com.google.common.collect.ImmutableSortedSet<Path> kotlinSourceFilePaths,               Path pathToSrcsList)`                                                                                                                                                                                                           
          `default com.google.common.collect.ImmutableList<Path>`   `getExpandedSourcePaths​(ProjectFilesystem projectFilesystem,                       ProjectFilesystemFactory projectFilesystemFactory,                       com.google.common.collect.ImmutableSet<Path> kotlinSourceFilePaths,                       Optional<Path> workingDirectory)`                                                                                                                        
          `String`                                                  `getShortName()`                                                                                                                                                                                                                                                                                                                                                                                               
          `Path`                                                    `getStdlibPath​(SourcePathResolverAdapter sourcePathResolverAdapter)`                                                                                                                                                                                                                                                                                                                                           
          `com.facebook.buck.jvm.kotlin.KotlincVersion`             `getVersion()`                                                                                                                                                                                                                                                                                                                                                                                                 

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

        []{#getVersion()}

        -   #### getVersion

            ``` methodSignature
            com.facebook.buck.jvm.kotlin.KotlincVersion getVersion()
            ```

        []{#buildWithClasspath(com.facebook.buck.core.build.execution.context.ExecutionContext,com.facebook.buck.core.model.BuildTarget,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableSortedSet,java.nio.file.Path,java.util.Optional,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### buildWithClasspath

            ``` methodSignature
            int buildWithClasspath​(ExecutionContext context,
                                   BuildTarget invokingRule,
                                   com.google.common.collect.ImmutableList<String> options,
                                   com.google.common.collect.ImmutableSortedSet<Path> kotlinSourceFilePaths,
                                   Path pathToSrcsList,
                                   Optional<Path> workingDirectory,
                                   ProjectFilesystem fileSystem)
                            throws InterruptedException
            ```

            [Throws:]{.throwsLabel}
            :   `InterruptedException`

        []{#getDescription(com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableSortedSet,java.nio.file.Path)}

        -   #### getDescription

            ``` methodSignature
            String getDescription​(com.google.common.collect.ImmutableList<String> options,
                                  com.google.common.collect.ImmutableSortedSet<Path> kotlinSourceFilePaths,
                                  Path pathToSrcsList)
            ```

        []{#getShortName()}

        -   #### getShortName

            ``` methodSignature
            String getShortName()
            ```

        []{#getAnnotationProcessorPath(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### getAnnotationProcessorPath

            ``` methodSignature
            Path getAnnotationProcessorPath​(SourcePathResolverAdapter sourcePathResolverAdapter)
            ```

        []{#getStdlibPath(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### getStdlibPath

            ``` methodSignature
            Path getStdlibPath​(SourcePathResolverAdapter sourcePathResolverAdapter)
            ```

        []{#getAdditionalClasspathEntries(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### getAdditionalClasspathEntries

            ``` methodSignature
            com.google.common.collect.ImmutableList<Path> getAdditionalClasspathEntries​(SourcePathResolverAdapter sourcePathResolverAdapter)
            ```

        []{#getExpandedSourcePaths(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.io.filesystem.ProjectFilesystemFactory,com.google.common.collect.ImmutableSet,java.util.Optional)}

        -   #### getExpandedSourcePaths

            ``` methodSignature
            default com.google.common.collect.ImmutableList<Path> getExpandedSourcePaths​(ProjectFilesystem projectFilesystem,
                                                                                         ProjectFilesystemFactory projectFilesystemFactory,
                                                                                         com.google.common.collect.ImmutableSet<Path> kotlinSourceFilePaths,
                                                                                         Optional<Path> workingDirectory)
                                                                                  throws InterruptedException,
                                                                                         IOException
            ```

            [Throws:]{.throwsLabel}
            :   `InterruptedException`
            :   `IOException`
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
